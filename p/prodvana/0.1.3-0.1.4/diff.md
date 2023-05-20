# Comparing `tmp/prodvana-0.1.3.tar.gz` & `tmp/prodvana-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodvana-0.1.3.tar", max compression
+gzip compressed data, was "prodvana-0.1.4.tar", max compression
```

## Comparing `prodvana-0.1.3.tar` & `prodvana-0.1.4.tar`

### file list

```diff
@@ -1,336 +1,336 @@
--rw-r--r--   0        0        0       81 2023-05-19 19:00:48.877495 prodvana-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.877495 prodvana-0.1.3/prodvana/__init__.py
--rw-r--r--   0        0        0     2708 2023-05-19 19:00:48.877495 prodvana-0.1.3/prodvana/client.py
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/agent/__init__.py
--rw-r--r--   0        0        0    19183 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/agent/agent_interaction_pb2.py
--rw-r--r--   0        0        0    18983 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi
--rw-r--r--   0        0        0    22573 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py
--rw-r--r--   0        0        0     6760 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/application/__init__.py
--rw-r--r--   0        0        0     4200 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/application/application_config_pb2.py
--rw-r--r--   0        0        0     4693 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/application/application_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/application/application_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/application/application_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    24873 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/application/application_manager_pb2.py
--rw-r--r--   0        0        0    16394 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/application/application_manager_pb2.pyi
--rw-r--r--   0        0        0    22241 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py
--rw-r--r--   0        0        0     6755 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2801 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/application/object_pb2.py
--rw-r--r--   0        0        0     2184 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/application/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/application/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/application/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     2294 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/application/user_metadata_pb2.py
--rw-r--r--   0        0        0     1670 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/application/user_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/auth/__init__.py
--rw-r--r--   0        0        0    13908 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/auth/auth_manager_pb2.py
--rw-r--r--   0        0        0    10206 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi
--rw-r--r--   0        0        0    18631 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py
--rw-r--r--   0        0        0     6767 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     5071 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/auth/auth_pb2.py
--rw-r--r--   0        0        0     5515 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/auth/auth_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/auth/auth_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/auth/auth_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/blobs/__init__.py
--rw-r--r--   0        0        0     2876 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py
--rw-r--r--   0        0        0     1129 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi
--rw-r--r--   0        0        0     2704 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py
--rw-r--r--   0        0        0      895 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/capability/__init__.py
--rw-r--r--   0        0        0     6823 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/capability/capability_pb2.py
--rw-r--r--   0        0        0     5455 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/capability/capability_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/capability/capability_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/capability/capability_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/__init__.py
--rw-r--r--   0        0        0     1595 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py
--rw-r--r--   0        0        0      869 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.pyi
--rw-r--r--   0        0        0     2659 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/env_pb2.py
--rw-r--r--   0        0        0     2017 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/env_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/env_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/env_pb2_grpc.pyi
--rw-r--r--   0        0        0     3634 2023-05-19 19:00:48.881495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/external_config_pb2.py
--rw-r--r--   0        0        0     4163 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/external_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/external_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/external_config_pb2_grpc.pyi
--rw-r--r--   0        0        0     5630 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/helm_pb2.py
--rw-r--r--   0        0        0     5448 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/helm_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/helm_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/helm_pb2_grpc.pyi
--rw-r--r--   0        0        0     1890 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/links_pb2.py
--rw-r--r--   0        0        0      846 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/links_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/links_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/links_pb2_grpc.pyi
--rw-r--r--   0        0        0     1384 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/maturity_pb2.py
--rw-r--r--   0        0        0     1103 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/maturity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.pyi
--rw-r--r--   0        0        0     2541 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/meta_pb2.py
--rw-r--r--   0        0        0     2531 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/meta_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/meta_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/meta_pb2_grpc.pyi
--rw-r--r--   0        0        0     2516 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/notification_pb2.py
--rw-r--r--   0        0        0     1337 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/notification_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/notification_pb2_grpc.pyi
--rw-r--r--   0        0        0    10776 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/parameters_pb2.py
--rw-r--r--   0        0        0     8692 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/parameters_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.pyi
--rw-r--r--   0        0        0    13928 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/program_pb2.py
--rw-r--r--   0        0        0    15915 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/program_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/program_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/program_pb2_grpc.pyi
--rw-r--r--   0        0        0     1837 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/ref_pb2.py
--rw-r--r--   0        0        0      743 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/ref_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/ref_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/ref_pb2_grpc.pyi
--rw-r--r--   0        0        0     3229 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/retry_pb2.py
--rw-r--r--   0        0        0     2757 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/retry_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/retry_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/retry_pb2_grpc.pyi
--rw-r--r--   0        0        0     2192 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/task_pb2.py
--rw-r--r--   0        0        0     1490 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/task_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/task_pb2_grpc.pyi
--rw-r--r--   0        0        0     1929 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/version_push_pb2.py
--rw-r--r--   0        0        0     1782 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/version_push_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/version_push_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/common_config/version_push_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/config_file/__init__.py
--rw-r--r--   0        0        0     3576 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/config_file/config_pb2.py
--rw-r--r--   0        0        0     4132 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/config_file/config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/config_file/config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/config_file/config_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/config_writeback/__init__.py
--rw-r--r--   0        0        0     1648 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/config_writeback/writeback_pb2.py
--rw-r--r--   0        0        0     1131 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/delivery/__init__.py
--rw-r--r--   0        0        0     2652 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/delivery/delivery_config_pb2.py
--rw-r--r--   0        0        0     2294 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/delivery_module/__init__.py
--rw-r--r--   0        0        0     6840 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/delivery_module/config_pb2.py
--rw-r--r--   0        0        0     6043 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/delivery_module/config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/delivery_module/config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/delivery_module/config_pb2_grpc.pyi
--rw-r--r--   0        0        0    11266 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/delivery_module/manager_pb2.py
--rw-r--r--   0        0        0     7072 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/delivery_module/manager_pb2.pyi
--rw-r--r--   0        0        0    10633 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/delivery_module/manager_pb2_grpc.py
--rw-r--r--   0        0        0     3123 2023-05-19 19:00:48.885495 prodvana-0.1.3/prodvana/proto/prodvana/delivery_module/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2566 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/delivery_module/object_pb2.py
--rw-r--r--   0        0        0     1823 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/delivery_module/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/delivery_module/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/delivery_module/object_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/desired_state/__init__.py
--rw-r--r--   0        0        0    33432 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/desired_state/manager_pb2.py
--rw-r--r--   0        0        0    28076 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/desired_state/manager_pb2.pyi
--rw-r--r--   0        0        0    18226 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py
--rw-r--r--   0        0        0     5259 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/desired_state/model/__init__.py
--rw-r--r--   0        0        0    36449 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py
--rw-r--r--   0        0        0    61730 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.pyi
--rw-r--r--   0        0        0     3895 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/desired_state/model/entity_pb2.py
--rw-r--r--   0        0        0     7903 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/environment/__init__.py
--rw-r--r--   0        0        0    17651 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/environment/clusters_pb2.py
--rw-r--r--   0        0        0    23424 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/environment/clusters_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/environment/clusters_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/environment/clusters_pb2_grpc.pyi
--rw-r--r--   0        0        0    18211 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/environment/environment_manager_pb2.py
--rw-r--r--   0        0        0    14932 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi
--rw-r--r--   0        0        0    17792 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py
--rw-r--r--   0        0        0     5195 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/events/__init__.py
--rw-r--r--   0        0        0     6416 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/events/events_manager_pb2.py
--rw-r--r--   0        0        0     5547 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/events/events_manager_pb2.pyi
--rw-r--r--   0        0        0     2714 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py
--rw-r--r--   0        0        0      853 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     3627 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/events/events_pb2.py
--rw-r--r--   0        0        0     4131 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/events/events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/events/events_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/events/events_pb2_grpc.pyi
--rw-r--r--   0        0        0    15940 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/events/types_pb2.py
--rw-r--r--   0        0        0    30800 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/events/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/events/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/events/types_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/insights/__init__.py
--rw-r--r--   0        0        0     3041 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/insights/insights_pb2.py
--rw-r--r--   0        0        0     3508 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/insights/insights_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/insights/insights_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/insights/insights_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/managed_resource/__init__.py
--rw-r--r--   0        0        0    14774 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/managed_resource/manager_pb2.py
--rw-r--r--   0        0        0    13338 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi
--rw-r--r--   0        0        0    12065 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py
--rw-r--r--   0        0        0     3657 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/metrics/__init__.py
--rw-r--r--   0        0        0     5507 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/metrics/metrics_pb2.py
--rw-r--r--   0        0        0     8746 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/metrics/metrics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/object/__init__.py
--rw-r--r--   0        0        0     1844 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/object/meta_pb2.py
--rw-r--r--   0        0        0     1957 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/object/meta_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/object/meta_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.889495 prodvana-0.1.3/prodvana/proto/prodvana/object/meta_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/organization/__init__.py
--rw-r--r--   0        0        0    16162 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/organization/organization_manager_pb2.py
--rw-r--r--   0        0        0     9762 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi
--rw-r--r--   0        0        0    14668 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py
--rw-r--r--   0        0        0     4779 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2859 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/organization/user_metadata_pb2.py
--rw-r--r--   0        0        0     1972 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/pipelines/__init__.py
--rw-r--r--   0        0        0     7494 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/pipelines/object_pb2.py
--rw-r--r--   0        0        0    10914 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/pipelines/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/pipelines/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/pipelines/object_pb2_grpc.pyi
--rw-r--r--   0        0        0    10003 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/pipelines/pipelines_pb2.py
--rw-r--r--   0        0        0    11698 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/protection/__init__.py
--rw-r--r--   0        0        0     3412 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/protection/attachments_pb2.py
--rw-r--r--   0        0        0     2828 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/protection/attachments_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/protection/attachments_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/protection/attachments_pb2_grpc.pyi
--rw-r--r--   0        0        0     1859 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/protection/object_pb2.py
--rw-r--r--   0        0        0     1425 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/protection/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/protection/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/protection/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     8400 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/protection/protection_config_pb2.py
--rw-r--r--   0        0        0     8865 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/protection/protection_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    10471 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/protection/protection_manager_pb2.py
--rw-r--r--   0        0        0     6767 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi
--rw-r--r--   0        0        0    10450 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py
--rw-r--r--   0        0        0     3113 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     6255 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/protection/protection_reference_pb2.py
--rw-r--r--   0        0        0     4847 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/release_channel/__init__.py
--rw-r--r--   0        0        0     3574 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/release_channel/object_pb2.py
--rw-r--r--   0        0        0     3325 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/release_channel/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/release_channel/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/release_channel/object_pb2_grpc.pyi
--rw-r--r--   0        0        0    12153 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py
--rw-r--r--   0        0        0    12710 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    11989 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py
--rw-r--r--   0        0        0     7509 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi
--rw-r--r--   0        0        0    13099 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py
--rw-r--r--   0        0        0     4150 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/repo/__init__.py
--rw-r--r--   0        0        0     2441 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/repo/repo_pb2.py
--rw-r--r--   0        0        0     2315 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/repo/repo_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/repo/repo_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/repo/repo_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/runtimes/__init__.py
--rw-r--r--   0        0        0     1559 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/runtimes/extensions_pb2.py
--rw-r--r--   0        0        0     1360 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/runtimes/extensions_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/runtimes/extensions_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/runtimes/extensions_pb2_grpc.pyi
--rw-r--r--   0        0        0     7542 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py
--rw-r--r--   0        0        0     6671 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.893495 prodvana-0.1.3/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/scm/__init__.py
--rw-r--r--   0        0        0     1265 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/scm/types_pb2.py
--rw-r--r--   0        0        0      914 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/scm/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/scm/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/scm/types_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/secrets/__init__.py
--rw-r--r--   0        0        0    10074 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py
--rw-r--r--   0        0        0     4586 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi
--rw-r--r--   0        0        0     9936 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py
--rw-r--r--   0        0        0     2847 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/service/__init__.py
--rw-r--r--   0        0        0     5498 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/service/object_pb2.py
--rw-r--r--   0        0        0     5760 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/service/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/service/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/service/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     2655 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/service/parameters_pb2.py
--rw-r--r--   0        0        0     2424 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/service/parameters_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/service/parameters_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/service/parameters_pb2_grpc.pyi
--rw-r--r--   0        0        0    30923 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/service/service_config_pb2.py
--rw-r--r--   0        0        0    42140 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/service/service_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/service/service_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/service/service_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    48527 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/service/service_manager_pb2.py
--rw-r--r--   0        0        0    38025 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/service/service_manager_pb2.pyi
--rw-r--r--   0        0        0    41143 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py
--rw-r--r--   0        0        0    12424 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2934 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/service/user_metadata_pb2.py
--rw-r--r--   0        0        0     2106 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/service/user_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/settings/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/settings/organization/__init__.py
--rw-r--r--   0        0        0     8509 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/settings/organization/users_pb2.py
--rw-r--r--   0        0        0     5677 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/settings/organization/users_pb2.pyi
--rw-r--r--   0        0        0     8214 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py
--rw-r--r--   0        0        0     2318 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/stat/__init__.py
--rw-r--r--   0        0        0     1530 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/stat/efficiency_pb2.py
--rw-r--r--   0        0        0     1156 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/stat/efficiency_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/template/__init__.py
--rw-r--r--   0        0        0     2429 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/template/service_pb2.py
--rw-r--r--   0        0        0     1768 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/template/service_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/template/service_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/template/service_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/users/__init__.py
--rw-r--r--   0        0        0     1505 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/users/users_pb2.py
--rw-r--r--   0        0        0     1451 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/users/users_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/users/users_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/users/users_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/version/__init__.py
--rw-r--r--   0        0        0     2099 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/version/source_metadata_pb2.py
--rw-r--r--   0        0        0     2255 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/version/source_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/volumes/__init__.py
--rw-r--r--   0        0        0     4805 2023-05-19 19:00:48.897495 prodvana-0.1.3/prodvana/proto/prodvana/volumes/volumes_pb2.py
--rw-r--r--   0        0        0     4793 2023-05-19 19:00:48.901495 prodvana-0.1.3/prodvana/proto/prodvana/volumes/volumes_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.901495 prodvana-0.1.3/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.901495 prodvana-0.1.3/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.901495 prodvana-0.1.3/prodvana/proto/prodvana/workflow/__init__.py
--rw-r--r--   0        0        0     5412 2023-05-19 19:00:48.901495 prodvana-0.1.3/prodvana/proto/prodvana/workflow/integration_config_pb2.py
--rw-r--r--   0        0        0     4328 2023-05-19 19:00:48.901495 prodvana-0.1.3/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.901495 prodvana-0.1.3/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.901495 prodvana-0.1.3/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    69010 2023-05-19 19:00:48.901495 prodvana-0.1.3/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py
--rw-r--r--   0        0        0    50096 2023-05-19 19:00:48.901495 prodvana-0.1.3/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi
--rw-r--r--   0        0        0    55859 2023-05-19 19:00:48.901495 prodvana-0.1.3/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py
--rw-r--r--   0        0        0    16155 2023-05-19 19:00:48.901495 prodvana-0.1.3/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.901495 prodvana-0.1.3/prodvana/proto/validate/__init__.py
--rw-r--r--   0        0        0    21204 2023-05-19 19:00:48.901495 prodvana-0.1.3/prodvana/proto/validate/validate_pb2.py
--rw-r--r--   0        0        0    64630 2023-05-19 19:00:48.901495 prodvana-0.1.3/prodvana/proto/validate/validate_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-19 19:00:48.901495 prodvana-0.1.3/prodvana/proto/validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-19 19:00:48.901495 prodvana-0.1.3/prodvana/proto/validate/validate_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.901495 prodvana-0.1.3/prodvana/py.typed
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.901495 prodvana-0.1.3/prodvana/utils/__init__.py
--rw-r--r--   0        0        0      538 2023-05-19 19:00:48.901495 prodvana-0.1.3/prodvana/utils/desired_states.py
--rw-r--r--   0        0        0     4095 2023-05-19 19:00:48.901495 prodvana-0.1.3/prodvana/utils/service_config.py
--rw-r--r--   0        0        0     7188 2023-05-19 19:00:48.901495 prodvana-0.1.3/prodvana/utils/tests/test_service_config.py
--rw-r--r--   0        0        0      718 2023-05-19 19:03:26.434463 prodvana-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      817 1970-01-01 00:00:00.000000 prodvana-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       81 2023-05-19 19:00:48.877495 prodvana-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-19 19:00:48.877495 prodvana-0.1.4/prodvana/__init__.py
+-rw-r--r--   0        0        0     3529 2023-05-19 23:43:46.670463 prodvana-0.1.4/prodvana/client.py
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.480946 prodvana-0.1.4/prodvana/proto/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.480946 prodvana-0.1.4/prodvana/proto/prodvana/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.504946 prodvana-0.1.4/prodvana/proto/prodvana/agent/__init__.py
+-rw-r--r--   0        0        0    19183 2023-05-20 13:57:37.164948 prodvana-0.1.4/prodvana/proto/prodvana/agent/agent_interaction_pb2.py
+-rw-r--r--   0        0        0    18983 2023-05-20 13:57:37.364947 prodvana-0.1.4/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi
+-rw-r--r--   0        0        0    22573 2023-05-20 13:57:37.164948 prodvana-0.1.4/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py
+-rw-r--r--   0        0        0     6760 2023-05-20 13:57:37.364947 prodvana-0.1.4/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.516946 prodvana-0.1.4/prodvana/proto/prodvana/application/__init__.py
+-rw-r--r--   0        0        0     4200 2023-05-20 13:57:37.204948 prodvana-0.1.4/prodvana/proto/prodvana/application/application_config_pb2.py
+-rw-r--r--   0        0        0     4693 2023-05-20 13:57:37.404946 prodvana-0.1.4/prodvana/proto/prodvana/application/application_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.208948 prodvana-0.1.4/prodvana/proto/prodvana/application/application_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.404946 prodvana-0.1.4/prodvana/proto/prodvana/application/application_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    24873 2023-05-20 13:57:37.208948 prodvana-0.1.4/prodvana/proto/prodvana/application/application_manager_pb2.py
+-rw-r--r--   0        0        0    16394 2023-05-20 13:57:37.396947 prodvana-0.1.4/prodvana/proto/prodvana/application/application_manager_pb2.pyi
+-rw-r--r--   0        0        0    22241 2023-05-20 13:57:37.204948 prodvana-0.1.4/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     6755 2023-05-20 13:57:37.400946 prodvana-0.1.4/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2801 2023-05-20 13:57:37.208948 prodvana-0.1.4/prodvana/proto/prodvana/application/object_pb2.py
+-rw-r--r--   0        0        0     2184 2023-05-20 13:57:37.400946 prodvana-0.1.4/prodvana/proto/prodvana/application/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.204948 prodvana-0.1.4/prodvana/proto/prodvana/application/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.400946 prodvana-0.1.4/prodvana/proto/prodvana/application/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2294 2023-05-20 13:57:37.212948 prodvana-0.1.4/prodvana/proto/prodvana/application/user_metadata_pb2.py
+-rw-r--r--   0        0        0     1670 2023-05-20 13:57:37.396947 prodvana-0.1.4/prodvana/proto/prodvana/application/user_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.200948 prodvana-0.1.4/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.404946 prodvana-0.1.4/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.516946 prodvana-0.1.4/prodvana/proto/prodvana/auth/__init__.py
+-rw-r--r--   0        0        0    13908 2023-05-20 13:57:37.196948 prodvana-0.1.4/prodvana/proto/prodvana/auth/auth_manager_pb2.py
+-rw-r--r--   0        0        0    10206 2023-05-20 13:57:37.392947 prodvana-0.1.4/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi
+-rw-r--r--   0        0        0    18631 2023-05-20 13:57:37.200948 prodvana-0.1.4/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     6767 2023-05-20 13:57:37.396947 prodvana-0.1.4/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5071 2023-05-20 13:57:37.196948 prodvana-0.1.4/prodvana/proto/prodvana/auth/auth_pb2.py
+-rw-r--r--   0        0        0     5515 2023-05-20 13:57:37.392947 prodvana-0.1.4/prodvana/proto/prodvana/auth/auth_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.196948 prodvana-0.1.4/prodvana/proto/prodvana/auth/auth_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.392947 prodvana-0.1.4/prodvana/proto/prodvana/auth/auth_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.484946 prodvana-0.1.4/prodvana/proto/prodvana/blobs/__init__.py
+-rw-r--r--   0        0        0     2876 2023-05-20 13:57:37.092949 prodvana-0.1.4/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py
+-rw-r--r--   0        0        0     1129 2023-05-20 13:57:37.304947 prodvana-0.1.4/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi
+-rw-r--r--   0        0        0     2704 2023-05-20 13:57:37.092949 prodvana-0.1.4/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py
+-rw-r--r--   0        0        0      895 2023-05-20 13:57:37.308947 prodvana-0.1.4/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.504946 prodvana-0.1.4/prodvana/proto/prodvana/capability/__init__.py
+-rw-r--r--   0        0        0     6823 2023-05-20 13:57:37.160948 prodvana-0.1.4/prodvana/proto/prodvana/capability/capability_pb2.py
+-rw-r--r--   0        0        0     5455 2023-05-20 13:57:37.360947 prodvana-0.1.4/prodvana/proto/prodvana/capability/capability_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.160948 prodvana-0.1.4/prodvana/proto/prodvana/capability/capability_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.364947 prodvana-0.1.4/prodvana/proto/prodvana/capability/capability_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.520946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/__init__.py
+-rw-r--r--   0        0        0     1595 2023-05-20 13:57:37.236948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py
+-rw-r--r--   0        0        0      869 2023-05-20 13:57:37.436946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.252947 prodvana-0.1.4/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.428946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2659 2023-05-20 13:57:37.232948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/env_pb2.py
+-rw-r--r--   0        0        0     2017 2023-05-20 13:57:37.436946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/env_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.252947 prodvana-0.1.4/prodvana/proto/prodvana/common_config/env_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.456946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/env_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3634 2023-05-20 13:57:37.240948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/external_config_pb2.py
+-rw-r--r--   0        0        0     4163 2023-05-20 13:57:37.440946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/external_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.260948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/external_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.456946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/external_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5630 2023-05-20 13:57:37.252947 prodvana-0.1.4/prodvana/proto/prodvana/common_config/helm_pb2.py
+-rw-r--r--   0        0        0     5448 2023-05-20 13:57:37.440946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/helm_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.256947 prodvana-0.1.4/prodvana/proto/prodvana/common_config/helm_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.448946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/helm_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1890 2023-05-20 13:57:37.268947 prodvana-0.1.4/prodvana/proto/prodvana/common_config/links_pb2.py
+-rw-r--r--   0        0        0      846 2023-05-20 13:57:37.432946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/links_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.248947 prodvana-0.1.4/prodvana/proto/prodvana/common_config/links_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.444946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/links_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1384 2023-05-20 13:57:37.240948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/maturity_pb2.py
+-rw-r--r--   0        0        0     1103 2023-05-20 13:57:37.424946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/maturity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.236948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.440946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2541 2023-05-20 13:57:37.244948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/meta_pb2.py
+-rw-r--r--   0        0        0     2531 2023-05-20 13:57:37.424946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/meta_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.232948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/meta_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.432946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/meta_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2516 2023-05-20 13:57:37.256947 prodvana-0.1.4/prodvana/proto/prodvana/common_config/notification_pb2.py
+-rw-r--r--   0        0        0     1337 2023-05-20 13:57:37.428946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.228948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/notification_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.448946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/notification_pb2_grpc.pyi
+-rw-r--r--   0        0        0    10776 2023-05-20 13:57:37.248947 prodvana-0.1.4/prodvana/proto/prodvana/common_config/parameters_pb2.py
+-rw-r--r--   0        0        0     8692 2023-05-20 13:57:37.448946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/parameters_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.260948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.456946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.pyi
+-rw-r--r--   0        0        0    13928 2023-05-20 13:57:37.264948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/program_pb2.py
+-rw-r--r--   0        0        0    15915 2023-05-20 13:57:37.452946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/program_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.264948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/program_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.428946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/program_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1837 2023-05-20 13:57:37.260948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/ref_pb2.py
+-rw-r--r--   0        0        0      743 2023-05-20 13:57:37.432946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/ref_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.236948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/ref_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.436946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/ref_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3229 2023-05-20 13:57:37.240948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/retry_pb2.py
+-rw-r--r--   0        0        0     2757 2023-05-20 13:57:37.444946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/retry_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.244948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/retry_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.444946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/retry_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2192 2023-05-20 13:57:37.248947 prodvana-0.1.4/prodvana/proto/prodvana/common_config/task_pb2.py
+-rw-r--r--   0        0        0     1490 2023-05-20 13:57:37.424946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.244948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.452946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1929 2023-05-20 13:57:37.264948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/version_push_pb2.py
+-rw-r--r--   0        0        0     1782 2023-05-20 13:57:37.452946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/version_push_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.256947 prodvana-0.1.4/prodvana/proto/prodvana/common_config/version_push_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.436946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/version_push_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.492946 prodvana-0.1.4/prodvana/proto/prodvana/config_file/__init__.py
+-rw-r--r--   0        0        0     3576 2023-05-20 14:21:41.769423 prodvana-0.1.4/prodvana/proto/prodvana/config_file/config_pb2.py
+-rw-r--r--   0        0        0     4132 2023-05-20 14:21:41.769423 prodvana-0.1.4/prodvana/proto/prodvana/config_file/config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.104948 prodvana-0.1.4/prodvana/proto/prodvana/config_file/config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.320947 prodvana-0.1.4/prodvana/proto/prodvana/config_file/config_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.488946 prodvana-0.1.4/prodvana/proto/prodvana/config_writeback/__init__.py
+-rw-r--r--   0        0        0     1648 2023-05-20 13:57:37.100948 prodvana-0.1.4/prodvana/proto/prodvana/config_writeback/writeback_pb2.py
+-rw-r--r--   0        0        0     1131 2023-05-20 13:57:37.312947 prodvana-0.1.4/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.100948 prodvana-0.1.4/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.316947 prodvana-0.1.4/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.524946 prodvana-0.1.4/prodvana/proto/prodvana/delivery/__init__.py
+-rw-r--r--   0        0        0     2652 2023-05-20 13:57:37.272947 prodvana-0.1.4/prodvana/proto/prodvana/delivery/delivery_config_pb2.py
+-rw-r--r--   0        0        0     2294 2023-05-20 13:57:37.464946 prodvana-0.1.4/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.272947 prodvana-0.1.4/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.464946 prodvana-0.1.4/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 14:21:41.769423 prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/__init__.py
+-rw-r--r--   0        0        0     6840 2023-05-20 14:21:41.769423 prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/config_pb2.py
+-rw-r--r--   0        0        0     6043 2023-05-20 14:21:41.769423 prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 14:21:41.769423 prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 14:21:41.769423 prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    11266 2023-05-20 14:21:41.769423 prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/manager_pb2.py
+-rw-r--r--   0        0        0     7072 2023-05-20 14:21:41.769423 prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/manager_pb2.pyi
+-rw-r--r--   0        0        0    10633 2023-05-20 14:21:41.769423 prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     3123 2023-05-20 14:21:41.769423 prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2566 2023-05-20 14:21:41.769423 prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/object_pb2.py
+-rw-r--r--   0        0        0     1823 2023-05-20 14:21:41.769423 prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 14:21:41.769423 prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 14:21:41.769423 prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.508946 prodvana-0.1.4/prodvana/proto/prodvana/desired_state/__init__.py
+-rw-r--r--   0        0        0    33432 2023-05-20 13:57:37.172948 prodvana-0.1.4/prodvana/proto/prodvana/desired_state/manager_pb2.py
+-rw-r--r--   0        0        0    28076 2023-05-20 13:57:37.372947 prodvana-0.1.4/prodvana/proto/prodvana/desired_state/manager_pb2.pyi
+-rw-r--r--   0        0        0    18226 2023-05-20 13:57:37.176948 prodvana-0.1.4/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     5259 2023-05-20 13:57:37.372947 prodvana-0.1.4/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.512946 prodvana-0.1.4/prodvana/proto/prodvana/desired_state/model/__init__.py
+-rw-r--r--   0        0        0    36441 2023-05-20 13:57:37.176948 prodvana-0.1.4/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py
+-rw-r--r--   0        0        0    61690 2023-05-20 13:57:37.376947 prodvana-0.1.4/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.180948 prodvana-0.1.4/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.380947 prodvana-0.1.4/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3895 2023-05-20 13:57:37.180948 prodvana-0.1.4/prodvana/proto/prodvana/desired_state/model/entity_pb2.py
+-rw-r--r--   0        0        0     7903 2023-05-20 13:57:37.376947 prodvana-0.1.4/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.180948 prodvana-0.1.4/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.376947 prodvana-0.1.4/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.504946 prodvana-0.1.4/prodvana/proto/prodvana/environment/__init__.py
+-rw-r--r--   0        0        0    17651 2023-05-20 13:57:37.168948 prodvana-0.1.4/prodvana/proto/prodvana/environment/clusters_pb2.py
+-rw-r--r--   0        0        0    23424 2023-05-20 13:57:37.372947 prodvana-0.1.4/prodvana/proto/prodvana/environment/clusters_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.168948 prodvana-0.1.4/prodvana/proto/prodvana/environment/clusters_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.368947 prodvana-0.1.4/prodvana/proto/prodvana/environment/clusters_pb2_grpc.pyi
+-rw-r--r--   0        0        0    18211 2023-05-20 13:57:37.172948 prodvana-0.1.4/prodvana/proto/prodvana/environment/environment_manager_pb2.py
+-rw-r--r--   0        0        0    14932 2023-05-20 13:57:37.368947 prodvana-0.1.4/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi
+-rw-r--r--   0        0        0    17792 2023-05-20 13:57:37.168948 prodvana-0.1.4/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     5195 2023-05-20 13:57:37.368947 prodvana-0.1.4/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.496946 prodvana-0.1.4/prodvana/proto/prodvana/events/__init__.py
+-rw-r--r--   0        0        0     6416 2023-05-20 13:57:37.116948 prodvana-0.1.4/prodvana/proto/prodvana/events/events_manager_pb2.py
+-rw-r--r--   0        0        0     5547 2023-05-20 13:57:37.332947 prodvana-0.1.4/prodvana/proto/prodvana/events/events_manager_pb2.pyi
+-rw-r--r--   0        0        0     2714 2023-05-20 13:57:37.120948 prodvana-0.1.4/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py
+-rw-r--r--   0        0        0      853 2023-05-20 13:57:37.332947 prodvana-0.1.4/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3627 2023-05-20 13:57:37.120948 prodvana-0.1.4/prodvana/proto/prodvana/events/events_pb2.py
+-rw-r--r--   0        0        0     4131 2023-05-20 13:57:37.328947 prodvana-0.1.4/prodvana/proto/prodvana/events/events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.116948 prodvana-0.1.4/prodvana/proto/prodvana/events/events_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.332947 prodvana-0.1.4/prodvana/proto/prodvana/events/events_pb2_grpc.pyi
+-rw-r--r--   0        0        0    15940 2023-05-20 13:57:37.116948 prodvana-0.1.4/prodvana/proto/prodvana/events/types_pb2.py
+-rw-r--r--   0        0        0    30800 2023-05-20 13:57:37.328947 prodvana-0.1.4/prodvana/proto/prodvana/events/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.124948 prodvana-0.1.4/prodvana/proto/prodvana/events/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.328947 prodvana-0.1.4/prodvana/proto/prodvana/events/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.512946 prodvana-0.1.4/prodvana/proto/prodvana/insights/__init__.py
+-rw-r--r--   0        0        0     3041 2023-05-20 13:57:37.188948 prodvana-0.1.4/prodvana/proto/prodvana/insights/insights_pb2.py
+-rw-r--r--   0        0        0     3508 2023-05-20 13:57:37.384947 prodvana-0.1.4/prodvana/proto/prodvana/insights/insights_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.188948 prodvana-0.1.4/prodvana/proto/prodvana/insights/insights_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.388947 prodvana-0.1.4/prodvana/proto/prodvana/insights/insights_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.520946 prodvana-0.1.4/prodvana/proto/prodvana/managed_resource/__init__.py
+-rw-r--r--   0        0        0    14774 2023-05-20 13:57:37.228948 prodvana-0.1.4/prodvana/proto/prodvana/managed_resource/manager_pb2.py
+-rw-r--r--   0        0        0    13338 2023-05-20 13:57:37.420946 prodvana-0.1.4/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi
+-rw-r--r--   0        0        0    12065 2023-05-20 13:57:37.228948 prodvana-0.1.4/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     3657 2023-05-20 13:57:37.420946 prodvana-0.1.4/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.504946 prodvana-0.1.4/prodvana/proto/prodvana/metrics/__init__.py
+-rw-r--r--   0        0        0     5507 2023-05-20 13:57:37.156948 prodvana-0.1.4/prodvana/proto/prodvana/metrics/metrics_pb2.py
+-rw-r--r--   0        0        0     8746 2023-05-20 13:57:37.360947 prodvana-0.1.4/prodvana/proto/prodvana/metrics/metrics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.160948 prodvana-0.1.4/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.360947 prodvana-0.1.4/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.496946 prodvana-0.1.4/prodvana/proto/prodvana/object/__init__.py
+-rw-r--r--   0        0        0     1844 2023-05-20 13:57:37.128948 prodvana-0.1.4/prodvana/proto/prodvana/object/meta_pb2.py
+-rw-r--r--   0        0        0     1957 2023-05-20 13:57:37.336947 prodvana-0.1.4/prodvana/proto/prodvana/object/meta_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.128948 prodvana-0.1.4/prodvana/proto/prodvana/object/meta_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.340947 prodvana-0.1.4/prodvana/proto/prodvana/object/meta_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.512946 prodvana-0.1.4/prodvana/proto/prodvana/organization/__init__.py
+-rw-r--r--   0        0        0    16162 2023-05-20 13:57:37.184948 prodvana-0.1.4/prodvana/proto/prodvana/organization/organization_manager_pb2.py
+-rw-r--r--   0        0        0     9762 2023-05-20 13:57:37.384947 prodvana-0.1.4/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi
+-rw-r--r--   0        0        0    14668 2023-05-20 13:57:37.184948 prodvana-0.1.4/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     4779 2023-05-20 13:57:37.380947 prodvana-0.1.4/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2859 2023-05-20 13:57:37.188948 prodvana-0.1.4/prodvana/proto/prodvana/organization/user_metadata_pb2.py
+-rw-r--r--   0        0        0     1972 2023-05-20 13:57:37.380947 prodvana-0.1.4/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.184948 prodvana-0.1.4/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.384947 prodvana-0.1.4/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.500946 prodvana-0.1.4/prodvana/proto/prodvana/pipelines/__init__.py
+-rw-r--r--   0        0        0     7494 2023-05-20 13:57:37.144948 prodvana-0.1.4/prodvana/proto/prodvana/pipelines/object_pb2.py
+-rw-r--r--   0        0        0    10914 2023-05-20 13:57:37.348947 prodvana-0.1.4/prodvana/proto/prodvana/pipelines/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.140948 prodvana-0.1.4/prodvana/proto/prodvana/pipelines/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.344947 prodvana-0.1.4/prodvana/proto/prodvana/pipelines/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0    10003 2023-05-20 13:57:37.144948 prodvana-0.1.4/prodvana/proto/prodvana/pipelines/pipelines_pb2.py
+-rw-r--r--   0        0        0    11698 2023-05-20 13:57:37.348947 prodvana-0.1.4/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.136948 prodvana-0.1.4/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.348947 prodvana-0.1.4/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.484946 prodvana-0.1.4/prodvana/proto/prodvana/protection/__init__.py
+-rw-r--r--   0        0        0     3412 2023-05-20 13:57:37.080949 prodvana-0.1.4/prodvana/proto/prodvana/protection/attachments_pb2.py
+-rw-r--r--   0        0        0     2828 2023-05-20 13:57:37.292947 prodvana-0.1.4/prodvana/proto/prodvana/protection/attachments_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.068949 prodvana-0.1.4/prodvana/proto/prodvana/protection/attachments_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.296947 prodvana-0.1.4/prodvana/proto/prodvana/protection/attachments_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1859 2023-05-20 13:57:37.076949 prodvana-0.1.4/prodvana/proto/prodvana/protection/object_pb2.py
+-rw-r--r--   0        0        0     1425 2023-05-20 13:57:37.296947 prodvana-0.1.4/prodvana/proto/prodvana/protection/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.072949 prodvana-0.1.4/prodvana/proto/prodvana/protection/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.288947 prodvana-0.1.4/prodvana/proto/prodvana/protection/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     8400 2023-05-20 13:57:37.068949 prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_config_pb2.py
+-rw-r--r--   0        0        0     8865 2023-05-20 13:57:37.300947 prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.076949 prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.296947 prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    10471 2023-05-20 13:57:37.084949 prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_manager_pb2.py
+-rw-r--r--   0        0        0     6767 2023-05-20 13:57:37.292947 prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi
+-rw-r--r--   0        0        0    10450 2023-05-20 13:57:37.072949 prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     3113 2023-05-20 13:57:37.296947 prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6255 2023-05-20 13:57:37.080949 prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_reference_pb2.py
+-rw-r--r--   0        0        0     4847 2023-05-20 13:57:37.292947 prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.076949 prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.288947 prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.500946 prodvana-0.1.4/prodvana/proto/prodvana/release_channel/__init__.py
+-rw-r--r--   0        0        0     3574 2023-05-20 13:57:37.152948 prodvana-0.1.4/prodvana/proto/prodvana/release_channel/object_pb2.py
+-rw-r--r--   0        0        0     3325 2023-05-20 13:57:37.356947 prodvana-0.1.4/prodvana/proto/prodvana/release_channel/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.148948 prodvana-0.1.4/prodvana/proto/prodvana/release_channel/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.352947 prodvana-0.1.4/prodvana/proto/prodvana/release_channel/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0    12153 2023-05-20 13:57:37.156948 prodvana-0.1.4/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py
+-rw-r--r--   0        0        0    12710 2023-05-20 13:57:37.356947 prodvana-0.1.4/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.148948 prodvana-0.1.4/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.352947 prodvana-0.1.4/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    11989 2023-05-20 13:57:37.152948 prodvana-0.1.4/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py
+-rw-r--r--   0        0        0     7509 2023-05-20 13:57:37.352947 prodvana-0.1.4/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi
+-rw-r--r--   0        0        0    13099 2023-05-20 13:57:37.148948 prodvana-0.1.4/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     4150 2023-05-20 13:57:37.356947 prodvana-0.1.4/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.516946 prodvana-0.1.4/prodvana/proto/prodvana/repo/__init__.py
+-rw-r--r--   0        0        0     2441 2023-05-20 13:57:37.192948 prodvana-0.1.4/prodvana/proto/prodvana/repo/repo_pb2.py
+-rw-r--r--   0        0        0     2315 2023-05-20 13:57:37.388947 prodvana-0.1.4/prodvana/proto/prodvana/repo/repo_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.192948 prodvana-0.1.4/prodvana/proto/prodvana/repo/repo_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.388947 prodvana-0.1.4/prodvana/proto/prodvana/repo/repo_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.484946 prodvana-0.1.4/prodvana/proto/prodvana/runtimes/__init__.py
+-rw-r--r--   0        0        0     1559 2023-05-20 13:57:37.084949 prodvana-0.1.4/prodvana/proto/prodvana/runtimes/extensions_pb2.py
+-rw-r--r--   0        0        0     1360 2023-05-20 13:57:37.300947 prodvana-0.1.4/prodvana/proto/prodvana/runtimes/extensions_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.088949 prodvana-0.1.4/prodvana/proto/prodvana/runtimes/extensions_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.304947 prodvana-0.1.4/prodvana/proto/prodvana/runtimes/extensions_pb2_grpc.pyi
+-rw-r--r--   0        0        0     7542 2023-05-20 13:57:37.088949 prodvana-0.1.4/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py
+-rw-r--r--   0        0        0     6671 2023-05-20 13:57:37.300947 prodvana-0.1.4/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.084949 prodvana-0.1.4/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.304947 prodvana-0.1.4/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.492946 prodvana-0.1.4/prodvana/proto/prodvana/scm/__init__.py
+-rw-r--r--   0        0        0     1265 2023-05-20 13:57:37.108949 prodvana-0.1.4/prodvana/proto/prodvana/scm/types_pb2.py
+-rw-r--r--   0        0        0      914 2023-05-20 13:57:37.324947 prodvana-0.1.4/prodvana/proto/prodvana/scm/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.108949 prodvana-0.1.4/prodvana/proto/prodvana/scm/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.320947 prodvana-0.1.4/prodvana/proto/prodvana/scm/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.488946 prodvana-0.1.4/prodvana/proto/prodvana/secrets/__init__.py
+-rw-r--r--   0        0        0    10074 2023-05-20 13:57:37.100948 prodvana-0.1.4/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py
+-rw-r--r--   0        0        0     4586 2023-05-20 13:57:37.312947 prodvana-0.1.4/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi
+-rw-r--r--   0        0        0     9936 2023-05-20 13:57:37.096948 prodvana-0.1.4/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     2847 2023-05-20 13:57:37.312947 prodvana-0.1.4/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.520946 prodvana-0.1.4/prodvana/proto/prodvana/service/__init__.py
+-rw-r--r--   0        0        0     5498 2023-05-20 13:57:37.216948 prodvana-0.1.4/prodvana/proto/prodvana/service/object_pb2.py
+-rw-r--r--   0        0        0     5760 2023-05-20 13:57:37.412947 prodvana-0.1.4/prodvana/proto/prodvana/service/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.216948 prodvana-0.1.4/prodvana/proto/prodvana/service/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.408946 prodvana-0.1.4/prodvana/proto/prodvana/service/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2655 2023-05-20 13:57:37.220948 prodvana-0.1.4/prodvana/proto/prodvana/service/parameters_pb2.py
+-rw-r--r--   0        0        0     2424 2023-05-20 13:57:37.416947 prodvana-0.1.4/prodvana/proto/prodvana/service/parameters_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.224948 prodvana-0.1.4/prodvana/proto/prodvana/service/parameters_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.420946 prodvana-0.1.4/prodvana/proto/prodvana/service/parameters_pb2_grpc.pyi
+-rw-r--r--   0        0        0    30923 2023-05-20 13:57:37.220948 prodvana-0.1.4/prodvana/proto/prodvana/service/service_config_pb2.py
+-rw-r--r--   0        0        0    42140 2023-05-20 13:57:37.412947 prodvana-0.1.4/prodvana/proto/prodvana/service/service_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.220948 prodvana-0.1.4/prodvana/proto/prodvana/service/service_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.416947 prodvana-0.1.4/prodvana/proto/prodvana/service/service_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    47994 2023-05-20 13:57:37.216948 prodvana-0.1.4/prodvana/proto/prodvana/service/service_manager_pb2.py
+-rw-r--r--   0        0        0    38013 2023-05-20 13:57:37.412947 prodvana-0.1.4/prodvana/proto/prodvana/service/service_manager_pb2.pyi
+-rw-r--r--   0        0        0    33828 2023-05-20 13:57:37.224948 prodvana-0.1.4/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     9674 2023-05-20 13:57:37.408946 prodvana-0.1.4/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2934 2023-05-20 13:57:37.224948 prodvana-0.1.4/prodvana/proto/prodvana/service/user_metadata_pb2.py
+-rw-r--r--   0        0        0     2106 2023-05-20 13:57:37.408946 prodvana-0.1.4/prodvana/proto/prodvana/service/user_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.212948 prodvana-0.1.4/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.416947 prodvana-0.1.4/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.492946 prodvana-0.1.4/prodvana/proto/prodvana/settings/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.492946 prodvana-0.1.4/prodvana/proto/prodvana/settings/organization/__init__.py
+-rw-r--r--   0        0        0     8509 2023-05-20 13:57:37.104948 prodvana-0.1.4/prodvana/proto/prodvana/settings/organization/users_pb2.py
+-rw-r--r--   0        0        0     5677 2023-05-20 13:57:37.316947 prodvana-0.1.4/prodvana/proto/prodvana/settings/organization/users_pb2.pyi
+-rw-r--r--   0        0        0     8214 2023-05-20 13:57:37.104948 prodvana-0.1.4/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py
+-rw-r--r--   0        0        0     2318 2023-05-20 13:57:37.316947 prodvana-0.1.4/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.496946 prodvana-0.1.4/prodvana/proto/prodvana/stat/__init__.py
+-rw-r--r--   0        0        0     1530 2023-05-20 13:57:37.112949 prodvana-0.1.4/prodvana/proto/prodvana/stat/efficiency_pb2.py
+-rw-r--r--   0        0        0     1156 2023-05-20 13:57:37.324947 prodvana-0.1.4/prodvana/proto/prodvana/stat/efficiency_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.112949 prodvana-0.1.4/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.324947 prodvana-0.1.4/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.520946 prodvana-0.1.4/prodvana/proto/prodvana/template/__init__.py
+-rw-r--r--   0        0        0     2429 2023-05-20 13:57:37.268947 prodvana-0.1.4/prodvana/proto/prodvana/template/service_pb2.py
+-rw-r--r--   0        0        0     1768 2023-05-20 13:57:37.460946 prodvana-0.1.4/prodvana/proto/prodvana/template/service_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.268947 prodvana-0.1.4/prodvana/proto/prodvana/template/service_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.460946 prodvana-0.1.4/prodvana/proto/prodvana/template/service_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.484946 prodvana-0.1.4/prodvana/proto/prodvana/users/__init__.py
+-rw-r--r--   0        0        0     1505 2023-05-20 13:57:37.068949 prodvana-0.1.4/prodvana/proto/prodvana/users/users_pb2.py
+-rw-r--r--   0        0        0     1451 2023-05-20 13:57:37.284947 prodvana-0.1.4/prodvana/proto/prodvana/users/users_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.064949 prodvana-0.1.4/prodvana/proto/prodvana/users/users_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.288947 prodvana-0.1.4/prodvana/proto/prodvana/users/users_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.496946 prodvana-0.1.4/prodvana/proto/prodvana/version/__init__.py
+-rw-r--r--   0        0        0     2099 2023-05-20 13:57:37.124948 prodvana-0.1.4/prodvana/proto/prodvana/version/source_metadata_pb2.py
+-rw-r--r--   0        0        0     2255 2023-05-20 13:57:37.336947 prodvana-0.1.4/prodvana/proto/prodvana/version/source_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.124948 prodvana-0.1.4/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.336947 prodvana-0.1.4/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.488946 prodvana-0.1.4/prodvana/proto/prodvana/volumes/__init__.py
+-rw-r--r--   0        0        0     4805 2023-05-20 13:57:37.092949 prodvana-0.1.4/prodvana/proto/prodvana/volumes/volumes_pb2.py
+-rw-r--r--   0        0        0     4793 2023-05-20 13:57:37.308947 prodvana-0.1.4/prodvana/proto/prodvana/volumes/volumes_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.096948 prodvana-0.1.4/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.308947 prodvana-0.1.4/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.500946 prodvana-0.1.4/prodvana/proto/prodvana/workflow/__init__.py
+-rw-r--r--   0        0        0     5412 2023-05-20 13:57:37.132948 prodvana-0.1.4/prodvana/proto/prodvana/workflow/integration_config_pb2.py
+-rw-r--r--   0        0        0     4328 2023-05-20 13:57:37.340947 prodvana-0.1.4/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.132948 prodvana-0.1.4/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.340947 prodvana-0.1.4/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    69010 2023-05-20 13:57:37.132948 prodvana-0.1.4/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py
+-rw-r--r--   0        0        0    50096 2023-05-20 13:57:37.344947 prodvana-0.1.4/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi
+-rw-r--r--   0        0        0    55859 2023-05-20 13:57:37.136948 prodvana-0.1.4/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py
+-rw-r--r--   0        0        0    16155 2023-05-20 13:57:37.344947 prodvana-0.1.4/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-20 13:57:37.524946 prodvana-0.1.4/prodvana/proto/validate/__init__.py
+-rw-r--r--   0        0        0    21204 2023-05-20 13:57:37.284947 prodvana-0.1.4/prodvana/proto/validate/validate_pb2.py
+-rw-r--r--   0        0        0    64630 2023-05-20 13:57:37.476946 prodvana-0.1.4/prodvana/proto/validate/validate_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-20 13:57:37.280947 prodvana-0.1.4/prodvana/proto/validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-20 13:57:37.476946 prodvana-0.1.4/prodvana/proto/validate/validate_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 19:00:48.901495 prodvana-0.1.4/prodvana/py.typed
+-rw-r--r--   0        0        0        0 2023-05-19 19:00:48.901495 prodvana-0.1.4/prodvana/utils/__init__.py
+-rw-r--r--   0        0        0      538 2023-05-19 19:00:48.901495 prodvana-0.1.4/prodvana/utils/desired_states.py
+-rw-r--r--   0        0        0     4079 2023-05-20 03:23:03.669262 prodvana-0.1.4/prodvana/utils/service_config.py
+-rw-r--r--   0        0        0     7140 2023-05-20 03:23:03.669262 prodvana-0.1.4/prodvana/utils/tests/test_service_config.py
+-rw-r--r--   0        0        0      741 2023-05-20 03:23:03.669262 prodvana-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      817 1970-01-01 00:00:00.000000 prodvana-0.1.4/PKG-INFO
```

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/agent/agent_interaction_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/agent/agent_interaction_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py` & `prodvana-0.1.4/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/application/application_config_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/application/application_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/application/application_config_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/application/application_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/application/application_manager_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/application/application_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/application/application_manager_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/application/application_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py` & `prodvana-0.1.4/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/application/object_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/application/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/application/object_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/application/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/application/user_metadata_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/application/user_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/application/user_metadata_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/application/user_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/auth/auth_manager_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/auth/auth_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py` & `prodvana-0.1.4/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/auth/auth_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/auth/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/auth/auth_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/auth/auth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py` & `prodvana-0.1.4/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/capability/capability_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/capability/capability_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/capability/capability_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/capability/capability_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/common_config/env_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/common_config/env_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/common_config/env_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/common_config/env_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/common_config/external_config_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/common_config/external_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/common_config/external_config_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/common_config/external_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/common_config/helm_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/common_config/helm_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/common_config/helm_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/common_config/helm_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/common_config/links_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/common_config/links_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/common_config/links_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/common_config/links_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/common_config/maturity_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/common_config/maturity_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/common_config/maturity_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/common_config/maturity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/common_config/meta_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/common_config/meta_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/common_config/meta_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/common_config/meta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/common_config/notification_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/common_config/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/common_config/notification_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/common_config/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/common_config/parameters_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/common_config/parameters_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/common_config/parameters_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/common_config/parameters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/common_config/program_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/common_config/program_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/common_config/program_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/common_config/program_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/common_config/ref_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/common_config/ref_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/common_config/ref_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/common_config/ref_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/common_config/retry_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/common_config/retry_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/common_config/retry_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/common_config/retry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/common_config/task_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/common_config/task_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/common_config/task_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/common_config/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/common_config/version_push_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/common_config/version_push_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/common_config/version_push_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/common_config/version_push_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/config_file/config_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/config_file/config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/config_file/config_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/config_file/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/config_writeback/writeback_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/config_writeback/writeback_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/delivery/delivery_config_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/delivery/delivery_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/delivery_module/config_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/delivery_module/config_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/delivery_module/manager_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/delivery_module/manager_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/delivery_module/manager_pb2_grpc.py` & `prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/delivery_module/manager_pb2_grpc.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/delivery_module/object_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/delivery_module/object_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/desired_state/manager_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/desired_state/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/desired_state/manager_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/desired_state/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py` & `prodvana-0.1.4/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 from prodvana.proto.prodvana.common_config import program_pb2 as prodvana_dot_common__config_dot_program__pb2
 from prodvana.proto.prodvana.common_config import retry_pb2 as prodvana_dot_common__config_dot_retry__pb2
 from prodvana.proto.prodvana.protection import protection_reference_pb2 as prodvana_dot_protection_dot_protection__reference__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0prodvana/desired_state/model/desired_state.proto\x12\x1cprodvana.desired_state.model\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17validate/validate.proto\x1a$prodvana/common_config/program.proto\x1a\"prodvana/common_config/retry.proto\x1a.prodvana/protection/protection_reference.proto\"p\n\x0eProtectionLink\x12;\n\tlifecycle\x18\x03 \x01(\x0b\x32(.prodvana.protection.ProtectionLifecycle\x12\x15\n\rattachment_id\x18\x04 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\x93\x06\n\tCondition\x12X\n\x07rc_cond\x18\x01 \x01(\x0b\x32\x45.prodvana.desired_state.model.Condition.ReleaseChannelStableConditionH\x00\x12Q\n\x0fmanual_approval\x18\x02 \x01(\x0b\x32\x36.prodvana.desired_state.model.Condition.ManualApprovalH\x00\x12\\\n\x0b\x63ustom_task\x18\x03 \x01(\x0b\x32\x45.prodvana.desired_state.model.Condition.CustomTaskSuccessfulConditionH\x00\x12\x18\n\x10\x64\x65sired_state_id\x18\x04 \x01(\t\x1a\xa7\x01\n\x1dReleaseChannelStableCondition\x12\x13\n\x0b\x61pplication\x18\x01 \x01(\t\x12\x0f\n\x07service\x18\x02 \x01(\t\x12\x12\n\nservice_id\x18\x03 \x01(\t\x12\x17\n\x0frelease_channel\x18\x04 \x01(\t\x12\x1a\n\x12release_channel_id\x18\x05 \x01(\t\x12\x17\n\x0fservice_version\x18\x06 \x01(\t\x1a\x1f\n\x0eManualApproval\x12\r\n\x05topic\x18\x01 \x01(\t\x1a\x88\x02\n\x1d\x43ustomTaskSuccessfulCondition\x12\x18\n\x10\x63ustom_task_name\x18\x01 \x01(\t\x12\x66\n\nprotection\x18\x02 \x01(\x0b\x32P.prodvana.desired_state.model.Condition.CustomTaskSuccessfulCondition.ProtectionH\x00\x1a[\n\nProtection\x12\x0c\n\x04name\x18\x01 \x01(\t\x12?\n\ttask_type\x18\x03 \x01(\x0e\x32,.prodvana.desired_state.model.CustomTaskTypeB\x08\n\x06sourceB\x0b\n\tcondition\"L\n\nIdentifier\x12\x30\n\x04type\x18\x01 \x01(\x0e\x32\".prodvana.desired_state.model.Type\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x89\x03\n\x08Metadata\x12>\n\rpreconditions\x18\x01 \x03(\x0b\x32\'.prodvana.desired_state.model.Condition\x12;\n\ninvariants\x18\x02 \x03(\x0b\x32\'.prodvana.desired_state.model.Condition\x12\x36\n\x04self\x18\x03 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12\x18\n\x10\x64\x65sired_state_id\x18\x04 \x01(\t\x12\x1d\n\x15root_desired_state_id\x18\x05 \x01(\t\x12\x46\n\x10protection_links\x18\x06 \x03(\x0b\x32,.prodvana.desired_state.model.ProtectionLink\x12G\n\x0bprotections\x18\x07 \x03(\x0b\x32\x32.prodvana.desired_state.model.ProtectionAttachment\"\xad\x01\n\x11StatusExplanation\x12\x39\n\x07subject\x18\x01 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12:\n\x06reason\x18\x02 \x01(\x0e\x32*.prodvana.desired_state.model.StatusReason\x12\x0f\n\x07message\x18\x03 \x01(\t\x12\x10\n\x08messages\x18\x04 \x03(\t\"\x8b\x01\n\x11\x41\x63tionExplanation\x12&\n\x02ts\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12=\n\x0b\x61\x63tion_type\x18\x02 \x01(\x0e\x32(.prodvana.desired_state.model.ActionType\x12\x0f\n\x07message\x18\x03 \x01(\t\"\xd7\x01\n\x07Version\x12\x17\n\x0fservice_version\x18\x01 \x01(\t\x12\x10\n\x08replicas\x18\x02 \x01(\x05\x12\x1a\n\x12\x61vailable_replicas\x18\x08 \x01(\x05\x12\x32\n\x0epush_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x61\x63tive\x18\x05 \x01(\x08\x12\x17\n\x0ftarget_replicas\x18\x06 \x01(\x05J\x04\x08\x03\x10\x04J\x04\x08\x07\x10\x08R\tunhealthyR\x11unhealthy_reasons\"\x86\x03\n\x14ServiceInstanceState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0b\x61pplication\x18\x02 \x01(\t\x12\x0f\n\x07service\x18\x03 \x01(\t\x12\x17\n\x0frelease_channel\x18\x04 \x01(\t\x12\x12\n\nservice_id\x18\x08 \x01(\t\x12\x1a\n\x12release_channel_id\x18\t \x01(\t\x12\x37\n\x08versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12?\n\x10rollback_version\x18\x06 \x01(\x0b\x32%.prodvana.desired_state.model.Version\x12\x10\n\x08rollback\x18\x07 \x01(\x08\x12=\n\x08\x64\x65livery\x18\n \x01(\x0b\x32+.prodvana.desired_state.model.DeliveryState\"\x9d\x02\n\x0cServiceState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0b\x61pplication\x18\x02 \x01(\t\x12\x0f\n\x07service\x18\x03 \x01(\t\x12\x12\n\nservice_id\x18\x05 \x01(\t\x12L\n\x10release_channels\x18\x06 \x03(\x0b\x32\x32.prodvana.desired_state.model.ServiceInstanceState\x12\x43\n\x0c\x63ustom_tasks\x18\x07 \x03(\x0b\x32-.prodvana.desired_state.model.CustomTaskStateJ\x04\x08\x04\x10\x05J\x04\x08\x08\x10\t\"\xd2\x01\n\x11ServiceGroupState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12<\n\x08services\x18\x02 \x03(\x0b\x32*.prodvana.desired_state.model.ServiceState\x12\x43\n\x0c\x63ustom_tasks\x18\x03 \x03(\x0b\x32-.prodvana.desired_state.model.CustomTaskStateJ\x04\x08\x04\x10\x05\"\xa8\x02\n\x13\x43\x61naryProgressState\x12H\n\x06status\x18\x01 \x01(\x0e\x32\x38.prodvana.desired_state.model.CanaryProgressState.Status\x12 \n\rcanary_weight\x18\x02 \x01(\x05\x42\t\xfa\x42\x06\x1a\x04\x18\x64(\x00\x12+\n\x08\x64uration\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x39\n\x15pause_start_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"=\n\x06Status\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07PENDING\x10\x01\x12\n\n\x06PAUSED\x10\x02\x12\r\n\tCOMPLETED\x10\x03\"\x94\x03\n\rDeliveryState\x12\x18\n\x10\x64\x65sired_state_id\x18\x0c \x01(\t\x12\x42\n\x06status\x18\x08 \x01(\x0e\x32\x32.prodvana.desired_state.model.DeliveryState.Status\x12\x0f\n\x07message\x18\x06 \x01(\t\x12J\n\x0f\x63\x61nary_progress\x18\x0b \x03(\x0b\x32\x31.prodvana.desired_state.model.CanaryProgressState\x12\x11\n\tfirst_run\x18\r \x01(\x08\x12\x12\n\ngeneration\x18\x0e \x01(\t\"q\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x16\n\x12STATUS_PROGRESSING\x10\x01\x12\x11\n\rSTATUS_PAUSED\x10\x02\x12\x12\n\x0eSTATUS_HEALTHY\x10\x03\x12\x14\n\x10STATUS_UNHEALTHY\x10\x04J\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x07\x10\x08J\x04\x08\t\x10\nJ\x04\x08\n\x10\x0b\"\xff\x03\n\rRuntimeObject\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0bobject_type\x18\x02 \x01(\t\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x37\n\x08versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x42\n\x06status\x18\x06 \x01(\x0e\x32\x32.prodvana.desired_state.model.RuntimeObject.Status\x12?\n\x10rollback_version\x18\x07 \x01(\x0b\x32%.prodvana.desired_state.model.Version\x12=\n\x08\x64\x65livery\x18\x08 \x01(\x0b\x32+.prodvana.desired_state.model.DeliveryState\x12\x18\n\x10version_agnostic\x18\n \x01(\x08\x12\x12\n\nstate_hash\x18\x0b \x01(\x0c\x12\x0f\n\x07message\x18\x0c \x01(\t\"0\n\x06Status\x12\x0b\n\x07PENDING\x10\x00\x12\r\n\tSUCCEEDED\x10\x01\x12\n\n\x06\x46\x41ILED\x10\x02J\x04\x08\t\x10\nR\x0eunhealthy_pods\"O\n\x0e\x43onditionState\x12=\n\x06status\x18\x01 \x01(\x0e\x32-.prodvana.desired_state.model.ConditionStatus\"\xde\x02\n\x0c\x43ontrolState\x12\x10\n\x08rollback\x18\x01 \x01(\x08\x12I\n\x13precondition_states\x18\x02 \x03(\x0b\x32,.prodvana.desired_state.model.ConditionState\x12\x46\n\x10invariant_states\x18\x03 \x03(\x0b\x32,.prodvana.desired_state.model.ConditionState\x12\x0e\n\x06paused\x18\x04 \x01(\x08\x12L\n\x13status_explanations\x18\x05 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12K\n\x12\x61\x63tion_explanation\x18\x06 \x01(\x0b\x32/.prodvana.desired_state.model.ActionExplanation\"\x9e\x01\n\x13ManualApprovalState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x42\n\x06status\x18\x02 \x01(\x0e\x32\x32.prodvana.desired_state.model.ManualApprovalStatus\x12\r\n\x05topic\x18\x03 \x01(\t\"\xed\x04\n\x05State\x12=\n\x07service\x18\x01 \x01(\x0b\x32*.prodvana.desired_state.model.ServiceStateH\x00\x12N\n\x10service_instance\x18\x02 \x01(\x0b\x32\x32.prodvana.desired_state.model.ServiceInstanceStateH\x00\x12H\n\rservice_group\x18\x03 \x01(\x0b\x32/.prodvana.desired_state.model.ServiceGroupStateH\x00\x12\x45\n\x0eruntime_object\x18\x04 \x01(\x0b\x32+.prodvana.desired_state.model.RuntimeObjectH\x00\x12L\n\x0fmanual_approval\x18\x05 \x01(\x0b\x32\x31.prodvana.desired_state.model.ManualApprovalStateH\x00\x12\x44\n\x0b\x63ustom_task\x18\x06 \x01(\x0b\x32-.prodvana.desired_state.model.CustomTaskStateH\x00\x12S\n\x15protection_attachment\x18\x07 \x01(\x0b\x32\x32.prodvana.desired_state.model.ProtectionAttachmentH\x00\x12L\n\x0fprotection_link\x18\x08 \x01(\x0b\x32\x31.prodvana.desired_state.model.ProtectionLinkStateH\x00\x42\r\n\x0bstate_oneof\"\x82\x01\n\x0b\x41nnotations\x12I\n\x0b\x61nnotations\x18\x01 \x03(\x0b\x32\x34.prodvana.desired_state.model.Annotations.Annotation\x1a(\n\nAnnotation\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\xae\x01\n\x18\x43ustomTaskExecutionState\x12>\n\x06status\x18\x01 \x01(\x0e\x32..prodvana.desired_state.model.CustomTaskStatus\x12\x10\n\x08\x61ttempts\x18\x02 \x01(\x03\x12@\n\x1clatest_attempt_end_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xce\x03\n\x0f\x43ustomTaskState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x15\n\x04name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x1c\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x13\n\x0b\x61pplication\x18\x04 \x01(\t\x12\x16\n\x0e\x61pplication_id\x18\x05 \x01(\t\x12\x17\n\x0frelease_channel\x18\x06 \x01(\t\x12\x1a\n\x12release_channel_id\x18\x07 \x01(\t\x12@\n\x07program\x18\t \x01(\x0b\x32%.prodvana.common_config.ProgramConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12J\n\ntask_state\x18\x0c \x01(\x0b\x32\x36.prodvana.desired_state.model.CustomTaskExecutionState\x12\x39\n\x0cretry_config\x18\r \x01(\x0b\x32#.prodvana.common_config.RetryConfig\x12\x13\n\x0bservice_ids\x18\x0e \x03(\tJ\x04\x08\x08\x10\tJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0c\"\xd4\x04\n\x13ProtectionLinkState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12=\n\x06status\x18\x02 \x01(\x0e\x32-.prodvana.desired_state.model.ConditionStatus\x12:\n\x04link\x18\x03 \x01(\x0b\x32,.prodvana.desired_state.model.ProtectionLink\x12\x35\n\x11started_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x11stopped_timestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12T\n\x0estopped_reason\x18\x06 \x01(\x0e\x32<.prodvana.desired_state.model.ProtectionLinkState.StopReason\x12;\n\x17\x66irst_success_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x8a\x01\n\nStopReason\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x17\n\x13LIFECYCLE_COMPLETED\x10\x01\x12\x12\n\x0eSUCCEEDED_ONCE\x10\x02\x12\x1a\n\x16SUCCEEDED_FOR_DURATION\x10\x03\x12\r\n\tTIMED_OUT\x10\x04\x12\n\n\x06\x46\x41ILED\x10\x05\x12\x0b\n\x07\x44\x45LETED\x10\x06\"\x89\x04\n\x14ProtectionAttachment\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x37\n\x08versions\x18\x02 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x46\n\x17last_completed_versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12<\n\x18last_completed_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\x15last_completed_status\x18\x07 \x01(\x0e\x32*.prodvana.desired_state.model.SimpleStatus\x12[\n\"last_completed_status_explanations\x18\x08 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12&\n\x1elast_completed_applied_version\x18\t \x01(\t\x12\x15\n\rprotection_id\x18\x03 \x01(\t\x12\x15\n\rattachment_id\x18\x04 \x01(\t\"\xde\x01\n\x06Signal\x12\x36\n\x04type\x18\x01 \x01(\x0e\x32(.prodvana.desired_state.model.SignalType\x12Z\n\x12\x64\x65livery_promotion\x18\x02 \x01(\x0b\x32<.prodvana.desired_state.model.Signal.DeliveryPromotionConfigH\x00\x1a\x36\n\x17\x44\x65liveryPromotionConfig\x12\r\n\x05stage\x18\x01 \x01(\x03\x12\x0c\n\x04\x66ull\x18\x02 \x01(\x08\x42\x08\n\x06\x63onfig\"?\n\x08\x44\x65\x62ugLog\x12&\n\x02ts\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0b\n\x03log\x18\x02 \x01(\t*\xb3\x01\n\x04Type\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07SERVICE\x10\x01\x12\x14\n\x10SERVICE_INSTANCE\x10\x02\x12\x11\n\rSERVICE_GROUP\x10\x03\x12\x12\n\x0eRUNTIME_OBJECT\x10\x04\x12\x13\n\x0fMANUAL_APPROVAL\x10\x05\x12\x0f\n\x0b\x43USTOM_TASK\x10\x06\x12\x19\n\x15PROTECTION_ATTACHMENT\x10\x07\x12\x13\n\x0fPROTECTION_LINK\x10\x08*w\n\tLifecycle\x12\x15\n\x11UNKNOWN_LIFECYCLE\x10\x00\x12\x15\n\x11\x43ONVERGENCE_START\x10\x01\x12\x10\n\x0cPRE_APPROVAL\x10\x02\x12\x11\n\rPOST_APPROVAL\x10\x03\x12\x08\n\x04PUSH\x10\x04\x12\r\n\tPOST_PUSH\x10\x05*\x8e\x01\n\x0e\x43ustomTaskType\x12\x1c\n\x18\x43USTOM_TASK_TYPE_UNKNOWN\x10\x00\x12\x15\n\x11PRE_APPROVAL_TASK\x10\x01\x12\x0c\n\x08\x41PPROVAL\x10\x02\x12\x16\n\x12POST_APPROVAL_TASK\x10\x03\x12\r\n\tPUSH_TASK\x10\x04\x12\x12\n\x0ePOST_PUSH_TASK\x10\x05*\xf0\x01\n\x06Status\x12\x12\n\x0eUNKNOWN_STATUS\x10\x00\x12\x0e\n\nCONVERGING\x10\x01\x12\r\n\tCONVERGED\x10\x02\x12\n\n\x06\x46\x41ILED\x10\x03\x12\x10\n\x0cROLLING_BACK\x10\x04\x12\x0f\n\x0bROLLED_BACK\x10\x05\x12\x13\n\x0f\x46\x41ILED_ROLLBACK\x10\x0c\x12\n\n\x06PAUSED\x10\x06\x12\x10\n\x0c\x43HILD_PAUSED\x10\x07\x12\x19\n\x15WAITING_PRECONDITIONS\x10\x08\x12\x0c\n\x08REPLACED\x10\t\x12\x1b\n\x17WAITING_MANUAL_APPROVAL\x10\n\x12\x0b\n\x07\x44\x45LETED\x10\x0b*R\n\x0cSimpleStatus\x12\x0e\n\nSS_UNKNOWN\x10\x00\x12\x11\n\rSS_CONVERGING\x10\x01\x12\x10\n\x0cSS_CONVERGED\x10\x02\x12\r\n\tSS_FAILED\x10\x03*\xec\x01\n\x0cStatusReason\x12\x12\n\x0eREASON_UNKNOWN\x10\x00\x12\x14\n\x10NO_CURRENT_STATE\x10\x01\x12\x10\n\x0c\x41PPLY_FAILED\x10\x02\x12\x12\n\x0eUNHEALTHY_PODS\x10\x03\x12\x11\n\rUPDATING_PODS\x10\x04\x12\x14\n\x10VERSION_MISMATCH\x10\x05\x12\x19\n\x15RUNTIME_OBJECT_FAILED\x10\x06\x12\x18\n\x14PRECONDITIONS_FAILED\x10\x07\x12\x1c\n\x18MANUAL_APPROVAL_REJECTED\x10\x08\x12\x10\n\x0cSTUCK_ENTITY\x10\t*r\n\nActionType\x12\x17\n\x13\x41\x43TION_TYPE_UNKNOWN\x10\x00\x12\x18\n\x14\x41\x43TION_TYPE_APPLYING\x10\x01\x12\x17\n\x13\x41\x43TION_TYPE_APPLIED\x10\x02\x12\x18\n\x14\x41\x43TION_TYPE_COMPLETE\x10\x03*\x96\x01\n\x0f\x43onditionStatus\x12\x1c\n\x18\x43ONDITION_UNKNOWN_STATUS\x10\x00\x12\x15\n\x11\x43ONDITION_PENDING\x10\x01\x12\x17\n\x13\x43ONDITION_SATISFIED\x10\x02\x12\x1f\n\x1b\x43ONDITION_MANUALLY_BYPASSED\x10\x03\x12\x14\n\x10\x43ONDITION_FAILED\x10\x04*?\n\x14ManualApprovalStatus\x12\x0b\n\x07PENDING\x10\x00\x12\x0c\n\x08\x41PPROVED\x10\x01\x12\x0c\n\x08REJECTED\x10\x02*\x85\x01\n\x10\x43ustomTaskStatus\x12\x17\n\x13\x43USTOM_TASK_PENDING\x10\x00\x12\x1a\n\x16\x43USTOM_TASK_SUCCESSFUL\x10\x01\x12!\n\x1d\x43USTOM_TASK_RETRIES_EXHAUSTED\x10\x02\x12\x19\n\x15\x43USTOM_TASK_TIMED_OUT\x10\x03*8\n\nSignalType\x12\x12\n\x0eSIGNAL_UNKNOWN\x10\x00\x12\x16\n\x12\x44\x45LIVERY_PROMOTION\x10\x01\x42XZVgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/desired_state/modelb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0prodvana/desired_state/model/desired_state.proto\x12\x1cprodvana.desired_state.model\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17validate/validate.proto\x1a$prodvana/common_config/program.proto\x1a\"prodvana/common_config/retry.proto\x1a.prodvana/protection/protection_reference.proto\"p\n\x0eProtectionLink\x12;\n\tlifecycle\x18\x03 \x01(\x0b\x32(.prodvana.protection.ProtectionLifecycle\x12\x15\n\rattachment_id\x18\x04 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\x93\x06\n\tCondition\x12X\n\x07rc_cond\x18\x01 \x01(\x0b\x32\x45.prodvana.desired_state.model.Condition.ReleaseChannelStableConditionH\x00\x12Q\n\x0fmanual_approval\x18\x02 \x01(\x0b\x32\x36.prodvana.desired_state.model.Condition.ManualApprovalH\x00\x12\\\n\x0b\x63ustom_task\x18\x03 \x01(\x0b\x32\x45.prodvana.desired_state.model.Condition.CustomTaskSuccessfulConditionH\x00\x12\x18\n\x10\x64\x65sired_state_id\x18\x04 \x01(\t\x1a\xa7\x01\n\x1dReleaseChannelStableCondition\x12\x13\n\x0b\x61pplication\x18\x01 \x01(\t\x12\x0f\n\x07service\x18\x02 \x01(\t\x12\x12\n\nservice_id\x18\x03 \x01(\t\x12\x17\n\x0frelease_channel\x18\x04 \x01(\t\x12\x1a\n\x12release_channel_id\x18\x05 \x01(\t\x12\x17\n\x0fservice_version\x18\x06 \x01(\t\x1a\x1f\n\x0eManualApproval\x12\r\n\x05topic\x18\x01 \x01(\t\x1a\x88\x02\n\x1d\x43ustomTaskSuccessfulCondition\x12\x18\n\x10\x63ustom_task_name\x18\x01 \x01(\t\x12\x66\n\nprotection\x18\x02 \x01(\x0b\x32P.prodvana.desired_state.model.Condition.CustomTaskSuccessfulCondition.ProtectionH\x00\x1a[\n\nProtection\x12\x0c\n\x04name\x18\x01 \x01(\t\x12?\n\ttask_type\x18\x03 \x01(\x0e\x32,.prodvana.desired_state.model.CustomTaskTypeB\x08\n\x06sourceB\x0b\n\tcondition\"L\n\nIdentifier\x12\x30\n\x04type\x18\x01 \x01(\x0e\x32\".prodvana.desired_state.model.Type\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x89\x03\n\x08Metadata\x12>\n\rpreconditions\x18\x01 \x03(\x0b\x32\'.prodvana.desired_state.model.Condition\x12;\n\ninvariants\x18\x02 \x03(\x0b\x32\'.prodvana.desired_state.model.Condition\x12\x36\n\x04self\x18\x03 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12\x18\n\x10\x64\x65sired_state_id\x18\x04 \x01(\t\x12\x1d\n\x15root_desired_state_id\x18\x05 \x01(\t\x12\x46\n\x10protection_links\x18\x06 \x03(\x0b\x32,.prodvana.desired_state.model.ProtectionLink\x12G\n\x0bprotections\x18\x07 \x03(\x0b\x32\x32.prodvana.desired_state.model.ProtectionAttachment\"\xad\x01\n\x11StatusExplanation\x12\x39\n\x07subject\x18\x01 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12:\n\x06reason\x18\x02 \x01(\x0e\x32*.prodvana.desired_state.model.StatusReason\x12\x0f\n\x07message\x18\x03 \x01(\t\x12\x10\n\x08messages\x18\x04 \x03(\t\"\x8b\x01\n\x11\x41\x63tionExplanation\x12&\n\x02ts\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12=\n\x0b\x61\x63tion_type\x18\x02 \x01(\x0e\x32(.prodvana.desired_state.model.ActionType\x12\x0f\n\x07message\x18\x03 \x01(\t\"\xcf\x01\n\x07Version\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x10\n\x08replicas\x18\x02 \x01(\x05\x12\x1a\n\x12\x61vailable_replicas\x18\x08 \x01(\x05\x12\x32\n\x0epush_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x61\x63tive\x18\x05 \x01(\x08\x12\x17\n\x0ftarget_replicas\x18\x06 \x01(\x05J\x04\x08\x03\x10\x04J\x04\x08\x07\x10\x08R\tunhealthyR\x11unhealthy_reasons\"\x86\x03\n\x14ServiceInstanceState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0b\x61pplication\x18\x02 \x01(\t\x12\x0f\n\x07service\x18\x03 \x01(\t\x12\x17\n\x0frelease_channel\x18\x04 \x01(\t\x12\x12\n\nservice_id\x18\x08 \x01(\t\x12\x1a\n\x12release_channel_id\x18\t \x01(\t\x12\x37\n\x08versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12?\n\x10rollback_version\x18\x06 \x01(\x0b\x32%.prodvana.desired_state.model.Version\x12\x10\n\x08rollback\x18\x07 \x01(\x08\x12=\n\x08\x64\x65livery\x18\n \x01(\x0b\x32+.prodvana.desired_state.model.DeliveryState\"\x9d\x02\n\x0cServiceState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0b\x61pplication\x18\x02 \x01(\t\x12\x0f\n\x07service\x18\x03 \x01(\t\x12\x12\n\nservice_id\x18\x05 \x01(\t\x12L\n\x10release_channels\x18\x06 \x03(\x0b\x32\x32.prodvana.desired_state.model.ServiceInstanceState\x12\x43\n\x0c\x63ustom_tasks\x18\x07 \x03(\x0b\x32-.prodvana.desired_state.model.CustomTaskStateJ\x04\x08\x04\x10\x05J\x04\x08\x08\x10\t\"\xd2\x01\n\x11ServiceGroupState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12<\n\x08services\x18\x02 \x03(\x0b\x32*.prodvana.desired_state.model.ServiceState\x12\x43\n\x0c\x63ustom_tasks\x18\x03 \x03(\x0b\x32-.prodvana.desired_state.model.CustomTaskStateJ\x04\x08\x04\x10\x05\"\xa8\x02\n\x13\x43\x61naryProgressState\x12H\n\x06status\x18\x01 \x01(\x0e\x32\x38.prodvana.desired_state.model.CanaryProgressState.Status\x12 \n\rcanary_weight\x18\x02 \x01(\x05\x42\t\xfa\x42\x06\x1a\x04\x18\x64(\x00\x12+\n\x08\x64uration\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x39\n\x15pause_start_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"=\n\x06Status\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07PENDING\x10\x01\x12\n\n\x06PAUSED\x10\x02\x12\r\n\tCOMPLETED\x10\x03\"\x94\x03\n\rDeliveryState\x12\x18\n\x10\x64\x65sired_state_id\x18\x0c \x01(\t\x12\x42\n\x06status\x18\x08 \x01(\x0e\x32\x32.prodvana.desired_state.model.DeliveryState.Status\x12\x0f\n\x07message\x18\x06 \x01(\t\x12J\n\x0f\x63\x61nary_progress\x18\x0b \x03(\x0b\x32\x31.prodvana.desired_state.model.CanaryProgressState\x12\x11\n\tfirst_run\x18\r \x01(\x08\x12\x12\n\ngeneration\x18\x0e \x01(\t\"q\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x16\n\x12STATUS_PROGRESSING\x10\x01\x12\x11\n\rSTATUS_PAUSED\x10\x02\x12\x12\n\x0eSTATUS_HEALTHY\x10\x03\x12\x14\n\x10STATUS_UNHEALTHY\x10\x04J\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x07\x10\x08J\x04\x08\t\x10\nJ\x04\x08\n\x10\x0b\"\xff\x03\n\rRuntimeObject\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0bobject_type\x18\x02 \x01(\t\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x37\n\x08versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x42\n\x06status\x18\x06 \x01(\x0e\x32\x32.prodvana.desired_state.model.RuntimeObject.Status\x12?\n\x10rollback_version\x18\x07 \x01(\x0b\x32%.prodvana.desired_state.model.Version\x12=\n\x08\x64\x65livery\x18\x08 \x01(\x0b\x32+.prodvana.desired_state.model.DeliveryState\x12\x18\n\x10version_agnostic\x18\n \x01(\x08\x12\x12\n\nstate_hash\x18\x0b \x01(\x0c\x12\x0f\n\x07message\x18\x0c \x01(\t\"0\n\x06Status\x12\x0b\n\x07PENDING\x10\x00\x12\r\n\tSUCCEEDED\x10\x01\x12\n\n\x06\x46\x41ILED\x10\x02J\x04\x08\t\x10\nR\x0eunhealthy_pods\"O\n\x0e\x43onditionState\x12=\n\x06status\x18\x01 \x01(\x0e\x32-.prodvana.desired_state.model.ConditionStatus\"\xde\x02\n\x0c\x43ontrolState\x12\x10\n\x08rollback\x18\x01 \x01(\x08\x12I\n\x13precondition_states\x18\x02 \x03(\x0b\x32,.prodvana.desired_state.model.ConditionState\x12\x46\n\x10invariant_states\x18\x03 \x03(\x0b\x32,.prodvana.desired_state.model.ConditionState\x12\x0e\n\x06paused\x18\x04 \x01(\x08\x12L\n\x13status_explanations\x18\x05 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12K\n\x12\x61\x63tion_explanation\x18\x06 \x01(\x0b\x32/.prodvana.desired_state.model.ActionExplanation\"\x9e\x01\n\x13ManualApprovalState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x42\n\x06status\x18\x02 \x01(\x0e\x32\x32.prodvana.desired_state.model.ManualApprovalStatus\x12\r\n\x05topic\x18\x03 \x01(\t\"\xed\x04\n\x05State\x12=\n\x07service\x18\x01 \x01(\x0b\x32*.prodvana.desired_state.model.ServiceStateH\x00\x12N\n\x10service_instance\x18\x02 \x01(\x0b\x32\x32.prodvana.desired_state.model.ServiceInstanceStateH\x00\x12H\n\rservice_group\x18\x03 \x01(\x0b\x32/.prodvana.desired_state.model.ServiceGroupStateH\x00\x12\x45\n\x0eruntime_object\x18\x04 \x01(\x0b\x32+.prodvana.desired_state.model.RuntimeObjectH\x00\x12L\n\x0fmanual_approval\x18\x05 \x01(\x0b\x32\x31.prodvana.desired_state.model.ManualApprovalStateH\x00\x12\x44\n\x0b\x63ustom_task\x18\x06 \x01(\x0b\x32-.prodvana.desired_state.model.CustomTaskStateH\x00\x12S\n\x15protection_attachment\x18\x07 \x01(\x0b\x32\x32.prodvana.desired_state.model.ProtectionAttachmentH\x00\x12L\n\x0fprotection_link\x18\x08 \x01(\x0b\x32\x31.prodvana.desired_state.model.ProtectionLinkStateH\x00\x42\r\n\x0bstate_oneof\"\x82\x01\n\x0b\x41nnotations\x12I\n\x0b\x61nnotations\x18\x01 \x03(\x0b\x32\x34.prodvana.desired_state.model.Annotations.Annotation\x1a(\n\nAnnotation\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\xae\x01\n\x18\x43ustomTaskExecutionState\x12>\n\x06status\x18\x01 \x01(\x0e\x32..prodvana.desired_state.model.CustomTaskStatus\x12\x10\n\x08\x61ttempts\x18\x02 \x01(\x03\x12@\n\x1clatest_attempt_end_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xce\x03\n\x0f\x43ustomTaskState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x15\n\x04name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x1c\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x13\n\x0b\x61pplication\x18\x04 \x01(\t\x12\x16\n\x0e\x61pplication_id\x18\x05 \x01(\t\x12\x17\n\x0frelease_channel\x18\x06 \x01(\t\x12\x1a\n\x12release_channel_id\x18\x07 \x01(\t\x12@\n\x07program\x18\t \x01(\x0b\x32%.prodvana.common_config.ProgramConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12J\n\ntask_state\x18\x0c \x01(\x0b\x32\x36.prodvana.desired_state.model.CustomTaskExecutionState\x12\x39\n\x0cretry_config\x18\r \x01(\x0b\x32#.prodvana.common_config.RetryConfig\x12\x13\n\x0bservice_ids\x18\x0e \x03(\tJ\x04\x08\x08\x10\tJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0c\"\xd4\x04\n\x13ProtectionLinkState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12=\n\x06status\x18\x02 \x01(\x0e\x32-.prodvana.desired_state.model.ConditionStatus\x12:\n\x04link\x18\x03 \x01(\x0b\x32,.prodvana.desired_state.model.ProtectionLink\x12\x35\n\x11started_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x11stopped_timestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12T\n\x0estopped_reason\x18\x06 \x01(\x0e\x32<.prodvana.desired_state.model.ProtectionLinkState.StopReason\x12;\n\x17\x66irst_success_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x8a\x01\n\nStopReason\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x17\n\x13LIFECYCLE_COMPLETED\x10\x01\x12\x12\n\x0eSUCCEEDED_ONCE\x10\x02\x12\x1a\n\x16SUCCEEDED_FOR_DURATION\x10\x03\x12\r\n\tTIMED_OUT\x10\x04\x12\n\n\x06\x46\x41ILED\x10\x05\x12\x0b\n\x07\x44\x45LETED\x10\x06\"\x89\x04\n\x14ProtectionAttachment\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x37\n\x08versions\x18\x02 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x46\n\x17last_completed_versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12<\n\x18last_completed_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\x15last_completed_status\x18\x07 \x01(\x0e\x32*.prodvana.desired_state.model.SimpleStatus\x12[\n\"last_completed_status_explanations\x18\x08 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12&\n\x1elast_completed_applied_version\x18\t \x01(\t\x12\x15\n\rprotection_id\x18\x03 \x01(\t\x12\x15\n\rattachment_id\x18\x04 \x01(\t\"\xde\x01\n\x06Signal\x12\x36\n\x04type\x18\x01 \x01(\x0e\x32(.prodvana.desired_state.model.SignalType\x12Z\n\x12\x64\x65livery_promotion\x18\x02 \x01(\x0b\x32<.prodvana.desired_state.model.Signal.DeliveryPromotionConfigH\x00\x1a\x36\n\x17\x44\x65liveryPromotionConfig\x12\r\n\x05stage\x18\x01 \x01(\x03\x12\x0c\n\x04\x66ull\x18\x02 \x01(\x08\x42\x08\n\x06\x63onfig\"?\n\x08\x44\x65\x62ugLog\x12&\n\x02ts\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0b\n\x03log\x18\x02 \x01(\t*\xb3\x01\n\x04Type\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07SERVICE\x10\x01\x12\x14\n\x10SERVICE_INSTANCE\x10\x02\x12\x11\n\rSERVICE_GROUP\x10\x03\x12\x12\n\x0eRUNTIME_OBJECT\x10\x04\x12\x13\n\x0fMANUAL_APPROVAL\x10\x05\x12\x0f\n\x0b\x43USTOM_TASK\x10\x06\x12\x19\n\x15PROTECTION_ATTACHMENT\x10\x07\x12\x13\n\x0fPROTECTION_LINK\x10\x08*w\n\tLifecycle\x12\x15\n\x11UNKNOWN_LIFECYCLE\x10\x00\x12\x15\n\x11\x43ONVERGENCE_START\x10\x01\x12\x10\n\x0cPRE_APPROVAL\x10\x02\x12\x11\n\rPOST_APPROVAL\x10\x03\x12\x08\n\x04PUSH\x10\x04\x12\r\n\tPOST_PUSH\x10\x05*\x8e\x01\n\x0e\x43ustomTaskType\x12\x1c\n\x18\x43USTOM_TASK_TYPE_UNKNOWN\x10\x00\x12\x15\n\x11PRE_APPROVAL_TASK\x10\x01\x12\x0c\n\x08\x41PPROVAL\x10\x02\x12\x16\n\x12POST_APPROVAL_TASK\x10\x03\x12\r\n\tPUSH_TASK\x10\x04\x12\x12\n\x0ePOST_PUSH_TASK\x10\x05*\xf0\x01\n\x06Status\x12\x12\n\x0eUNKNOWN_STATUS\x10\x00\x12\x0e\n\nCONVERGING\x10\x01\x12\r\n\tCONVERGED\x10\x02\x12\n\n\x06\x46\x41ILED\x10\x03\x12\x10\n\x0cROLLING_BACK\x10\x04\x12\x0f\n\x0bROLLED_BACK\x10\x05\x12\x13\n\x0f\x46\x41ILED_ROLLBACK\x10\x0c\x12\n\n\x06PAUSED\x10\x06\x12\x10\n\x0c\x43HILD_PAUSED\x10\x07\x12\x19\n\x15WAITING_PRECONDITIONS\x10\x08\x12\x0c\n\x08REPLACED\x10\t\x12\x1b\n\x17WAITING_MANUAL_APPROVAL\x10\n\x12\x0b\n\x07\x44\x45LETED\x10\x0b*R\n\x0cSimpleStatus\x12\x0e\n\nSS_UNKNOWN\x10\x00\x12\x11\n\rSS_CONVERGING\x10\x01\x12\x10\n\x0cSS_CONVERGED\x10\x02\x12\r\n\tSS_FAILED\x10\x03*\xec\x01\n\x0cStatusReason\x12\x12\n\x0eREASON_UNKNOWN\x10\x00\x12\x14\n\x10NO_CURRENT_STATE\x10\x01\x12\x10\n\x0c\x41PPLY_FAILED\x10\x02\x12\x12\n\x0eUNHEALTHY_PODS\x10\x03\x12\x11\n\rUPDATING_PODS\x10\x04\x12\x14\n\x10VERSION_MISMATCH\x10\x05\x12\x19\n\x15RUNTIME_OBJECT_FAILED\x10\x06\x12\x18\n\x14PRECONDITIONS_FAILED\x10\x07\x12\x1c\n\x18MANUAL_APPROVAL_REJECTED\x10\x08\x12\x10\n\x0cSTUCK_ENTITY\x10\t*r\n\nActionType\x12\x17\n\x13\x41\x43TION_TYPE_UNKNOWN\x10\x00\x12\x18\n\x14\x41\x43TION_TYPE_APPLYING\x10\x01\x12\x17\n\x13\x41\x43TION_TYPE_APPLIED\x10\x02\x12\x18\n\x14\x41\x43TION_TYPE_COMPLETE\x10\x03*\x96\x01\n\x0f\x43onditionStatus\x12\x1c\n\x18\x43ONDITION_UNKNOWN_STATUS\x10\x00\x12\x15\n\x11\x43ONDITION_PENDING\x10\x01\x12\x17\n\x13\x43ONDITION_SATISFIED\x10\x02\x12\x1f\n\x1b\x43ONDITION_MANUALLY_BYPASSED\x10\x03\x12\x14\n\x10\x43ONDITION_FAILED\x10\x04*?\n\x14ManualApprovalStatus\x12\x0b\n\x07PENDING\x10\x00\x12\x0c\n\x08\x41PPROVED\x10\x01\x12\x0c\n\x08REJECTED\x10\x02*\x85\x01\n\x10\x43ustomTaskStatus\x12\x17\n\x13\x43USTOM_TASK_PENDING\x10\x00\x12\x1a\n\x16\x43USTOM_TASK_SUCCESSFUL\x10\x01\x12!\n\x1d\x43USTOM_TASK_RETRIES_EXHAUSTED\x10\x02\x12\x19\n\x15\x43USTOM_TASK_TIMED_OUT\x10\x03*8\n\nSignalType\x12\x12\n\x0eSIGNAL_UNKNOWN\x10\x00\x12\x16\n\x12\x44\x45LIVERY_PROMOTION\x10\x01\x42XZVgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/desired_state/modelb\x06proto3')
 
 _TYPE = DESCRIPTOR.enum_types_by_name['Type']
 Type = enum_type_wrapper.EnumTypeWrapper(_TYPE)
 _LIFECYCLE = DESCRIPTOR.enum_types_by_name['Lifecycle']
 Lifecycle = enum_type_wrapper.EnumTypeWrapper(_LIFECYCLE)
 _CUSTOMTASKTYPE = DESCRIPTOR.enum_types_by_name['CustomTaskType']
 CustomTaskType = enum_type_wrapper.EnumTypeWrapper(_CUSTOMTASKTYPE)
@@ -371,36 +371,36 @@
   _CANARYPROGRESSSTATE.fields_by_name['canary_weight']._serialized_options = b'\372B\006\032\004\030d(\000'
   _CUSTOMTASKSTATE.fields_by_name['name']._options = None
   _CUSTOMTASKSTATE.fields_by_name['name']._serialized_options = b'\372B\004r\002\020\001'
   _CUSTOMTASKSTATE.fields_by_name['description']._options = None
   _CUSTOMTASKSTATE.fields_by_name['description']._serialized_options = b'\372B\004r\002\020\001'
   _CUSTOMTASKSTATE.fields_by_name['program']._options = None
   _CUSTOMTASKSTATE.fields_by_name['program']._serialized_options = b'\372B\005\212\001\002\020\001'
-  _TYPE._serialized_start=7730
-  _TYPE._serialized_end=7909
-  _LIFECYCLE._serialized_start=7911
-  _LIFECYCLE._serialized_end=8030
-  _CUSTOMTASKTYPE._serialized_start=8033
-  _CUSTOMTASKTYPE._serialized_end=8175
-  _STATUS._serialized_start=8178
-  _STATUS._serialized_end=8418
-  _SIMPLESTATUS._serialized_start=8420
-  _SIMPLESTATUS._serialized_end=8502
-  _STATUSREASON._serialized_start=8505
-  _STATUSREASON._serialized_end=8741
-  _ACTIONTYPE._serialized_start=8743
-  _ACTIONTYPE._serialized_end=8857
-  _CONDITIONSTATUS._serialized_start=8860
-  _CONDITIONSTATUS._serialized_end=9010
-  _MANUALAPPROVALSTATUS._serialized_start=9012
-  _MANUALAPPROVALSTATUS._serialized_end=9075
-  _CUSTOMTASKSTATUS._serialized_start=9078
-  _CUSTOMTASKSTATUS._serialized_end=9211
-  _SIGNALTYPE._serialized_start=9213
-  _SIGNALTYPE._serialized_end=9269
+  _TYPE._serialized_start=7722
+  _TYPE._serialized_end=7901
+  _LIFECYCLE._serialized_start=7903
+  _LIFECYCLE._serialized_end=8022
+  _CUSTOMTASKTYPE._serialized_start=8025
+  _CUSTOMTASKTYPE._serialized_end=8167
+  _STATUS._serialized_start=8170
+  _STATUS._serialized_end=8410
+  _SIMPLESTATUS._serialized_start=8412
+  _SIMPLESTATUS._serialized_end=8494
+  _STATUSREASON._serialized_start=8497
+  _STATUSREASON._serialized_end=8733
+  _ACTIONTYPE._serialized_start=8735
+  _ACTIONTYPE._serialized_end=8849
+  _CONDITIONSTATUS._serialized_start=8852
+  _CONDITIONSTATUS._serialized_end=9002
+  _MANUALAPPROVALSTATUS._serialized_start=9004
+  _MANUALAPPROVALSTATUS._serialized_end=9067
+  _CUSTOMTASKSTATUS._serialized_start=9070
+  _CUSTOMTASKSTATUS._serialized_end=9203
+  _SIGNALTYPE._serialized_start=9205
+  _SIGNALTYPE._serialized_end=9261
   _PROTECTIONLINK._serialized_start=294
   _PROTECTIONLINK._serialized_end=406
   _CONDITION._serialized_start=409
   _CONDITION._serialized_end=1196
   _CONDITION_RELEASECHANNELSTABLECONDITION._serialized_start=716
   _CONDITION_RELEASECHANNELSTABLECONDITION._serialized_end=883
   _CONDITION_MANUALAPPROVAL._serialized_start=885
@@ -414,55 +414,55 @@
   _METADATA._serialized_start=1277
   _METADATA._serialized_end=1670
   _STATUSEXPLANATION._serialized_start=1673
   _STATUSEXPLANATION._serialized_end=1846
   _ACTIONEXPLANATION._serialized_start=1849
   _ACTIONEXPLANATION._serialized_end=1988
   _VERSION._serialized_start=1991
-  _VERSION._serialized_end=2206
-  _SERVICEINSTANCESTATE._serialized_start=2209
-  _SERVICEINSTANCESTATE._serialized_end=2599
-  _SERVICESTATE._serialized_start=2602
-  _SERVICESTATE._serialized_end=2887
-  _SERVICEGROUPSTATE._serialized_start=2890
-  _SERVICEGROUPSTATE._serialized_end=3100
-  _CANARYPROGRESSSTATE._serialized_start=3103
-  _CANARYPROGRESSSTATE._serialized_end=3399
-  _CANARYPROGRESSSTATE_STATUS._serialized_start=3338
-  _CANARYPROGRESSSTATE_STATUS._serialized_end=3399
-  _DELIVERYSTATE._serialized_start=3402
-  _DELIVERYSTATE._serialized_end=3806
-  _DELIVERYSTATE_STATUS._serialized_start=3645
-  _DELIVERYSTATE_STATUS._serialized_end=3758
-  _RUNTIMEOBJECT._serialized_start=3809
-  _RUNTIMEOBJECT._serialized_end=4320
-  _RUNTIMEOBJECT_STATUS._serialized_start=4250
-  _RUNTIMEOBJECT_STATUS._serialized_end=4298
-  _CONDITIONSTATE._serialized_start=4322
-  _CONDITIONSTATE._serialized_end=4401
-  _CONTROLSTATE._serialized_start=4404
-  _CONTROLSTATE._serialized_end=4754
-  _MANUALAPPROVALSTATE._serialized_start=4757
-  _MANUALAPPROVALSTATE._serialized_end=4915
-  _STATE._serialized_start=4918
-  _STATE._serialized_end=5539
-  _ANNOTATIONS._serialized_start=5542
-  _ANNOTATIONS._serialized_end=5672
-  _ANNOTATIONS_ANNOTATION._serialized_start=5632
-  _ANNOTATIONS_ANNOTATION._serialized_end=5672
-  _CUSTOMTASKEXECUTIONSTATE._serialized_start=5675
-  _CUSTOMTASKEXECUTIONSTATE._serialized_end=5849
-  _CUSTOMTASKSTATE._serialized_start=5852
-  _CUSTOMTASKSTATE._serialized_end=6314
-  _PROTECTIONLINKSTATE._serialized_start=6317
-  _PROTECTIONLINKSTATE._serialized_end=6913
-  _PROTECTIONLINKSTATE_STOPREASON._serialized_start=6775
-  _PROTECTIONLINKSTATE_STOPREASON._serialized_end=6913
-  _PROTECTIONATTACHMENT._serialized_start=6916
-  _PROTECTIONATTACHMENT._serialized_end=7437
-  _SIGNAL._serialized_start=7440
-  _SIGNAL._serialized_end=7662
-  _SIGNAL_DELIVERYPROMOTIONCONFIG._serialized_start=7598
-  _SIGNAL_DELIVERYPROMOTIONCONFIG._serialized_end=7652
-  _DEBUGLOG._serialized_start=7664
-  _DEBUGLOG._serialized_end=7727
+  _VERSION._serialized_end=2198
+  _SERVICEINSTANCESTATE._serialized_start=2201
+  _SERVICEINSTANCESTATE._serialized_end=2591
+  _SERVICESTATE._serialized_start=2594
+  _SERVICESTATE._serialized_end=2879
+  _SERVICEGROUPSTATE._serialized_start=2882
+  _SERVICEGROUPSTATE._serialized_end=3092
+  _CANARYPROGRESSSTATE._serialized_start=3095
+  _CANARYPROGRESSSTATE._serialized_end=3391
+  _CANARYPROGRESSSTATE_STATUS._serialized_start=3330
+  _CANARYPROGRESSSTATE_STATUS._serialized_end=3391
+  _DELIVERYSTATE._serialized_start=3394
+  _DELIVERYSTATE._serialized_end=3798
+  _DELIVERYSTATE_STATUS._serialized_start=3637
+  _DELIVERYSTATE_STATUS._serialized_end=3750
+  _RUNTIMEOBJECT._serialized_start=3801
+  _RUNTIMEOBJECT._serialized_end=4312
+  _RUNTIMEOBJECT_STATUS._serialized_start=4242
+  _RUNTIMEOBJECT_STATUS._serialized_end=4290
+  _CONDITIONSTATE._serialized_start=4314
+  _CONDITIONSTATE._serialized_end=4393
+  _CONTROLSTATE._serialized_start=4396
+  _CONTROLSTATE._serialized_end=4746
+  _MANUALAPPROVALSTATE._serialized_start=4749
+  _MANUALAPPROVALSTATE._serialized_end=4907
+  _STATE._serialized_start=4910
+  _STATE._serialized_end=5531
+  _ANNOTATIONS._serialized_start=5534
+  _ANNOTATIONS._serialized_end=5664
+  _ANNOTATIONS_ANNOTATION._serialized_start=5624
+  _ANNOTATIONS_ANNOTATION._serialized_end=5664
+  _CUSTOMTASKEXECUTIONSTATE._serialized_start=5667
+  _CUSTOMTASKEXECUTIONSTATE._serialized_end=5841
+  _CUSTOMTASKSTATE._serialized_start=5844
+  _CUSTOMTASKSTATE._serialized_end=6306
+  _PROTECTIONLINKSTATE._serialized_start=6309
+  _PROTECTIONLINKSTATE._serialized_end=6905
+  _PROTECTIONLINKSTATE_STOPREASON._serialized_start=6767
+  _PROTECTIONLINKSTATE_STOPREASON._serialized_end=6905
+  _PROTECTIONATTACHMENT._serialized_start=6908
+  _PROTECTIONATTACHMENT._serialized_end=7429
+  _SIGNAL._serialized_start=7432
+  _SIGNAL._serialized_end=7654
+  _SIGNAL_DELIVERYPROMOTIONCONFIG._serialized_start=7590
+  _SIGNAL_DELIVERYPROMOTIONCONFIG._serialized_end=7644
+  _DEBUGLOG._serialized_start=7656
+  _DEBUGLOG._serialized_end=7719
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -554,21 +554,21 @@
     def ClearField(self, field_name: typing_extensions.Literal["action_type", b"action_type", "message", b"message", "ts", b"ts"]) -> None: ...
 
 global___ActionExplanation = ActionExplanation
 
 class Version(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    SERVICE_VERSION_FIELD_NUMBER: builtins.int
+    VERSION_FIELD_NUMBER: builtins.int
     REPLICAS_FIELD_NUMBER: builtins.int
     AVAILABLE_REPLICAS_FIELD_NUMBER: builtins.int
     PUSH_TIMESTAMP_FIELD_NUMBER: builtins.int
     ACTIVE_FIELD_NUMBER: builtins.int
     TARGET_REPLICAS_FIELD_NUMBER: builtins.int
-    service_version: builtins.str
+    version: builtins.str
     replicas: builtins.int
     """Created/running replicas, can be in any state"""
     available_replicas: builtins.int
     """Replicas which have passed healthchecks for required duration."""
     @property
     def push_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
     active: builtins.bool
@@ -576,23 +576,23 @@
     A runtime object will have exactly one active version, while a service instance may have one or more
     depending on if it maps to more than one runtime object.
     """
     target_replicas: builtins.int
     def __init__(
         self,
         *,
-        service_version: builtins.str = ...,
+        version: builtins.str = ...,
         replicas: builtins.int = ...,
         available_replicas: builtins.int = ...,
         push_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         active: builtins.bool = ...,
         target_replicas: builtins.int = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["push_timestamp", b"push_timestamp"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["active", b"active", "available_replicas", b"available_replicas", "push_timestamp", b"push_timestamp", "replicas", b"replicas", "service_version", b"service_version", "target_replicas", b"target_replicas"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["active", b"active", "available_replicas", b"available_replicas", "push_timestamp", b"push_timestamp", "replicas", b"replicas", "target_replicas", b"target_replicas", "version", b"version"]) -> None: ...
 
 global___Version = Version
 
 class ServiceInstanceState(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     META_FIELD_NUMBER: builtins.int
```

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/desired_state/model/entity_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/desired_state/model/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/environment/clusters_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/environment/clusters_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/environment/clusters_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/environment/clusters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/environment/environment_manager_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/environment/environment_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py` & `prodvana-0.1.4/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/events/events_manager_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/events/events_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/events/events_manager_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/events/events_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py` & `prodvana-0.1.4/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/events/events_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/events/events_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/events/events_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/events/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/events/types_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/events/types_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/events/types_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/events/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/insights/insights_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/insights/insights_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/insights/insights_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/insights/insights_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/managed_resource/manager_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/managed_resource/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py` & `prodvana-0.1.4/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/metrics/metrics_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/metrics/metrics_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/metrics/metrics_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/metrics/metrics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/object/meta_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/object/meta_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/object/meta_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/object/meta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/organization/organization_manager_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/organization/organization_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py` & `prodvana-0.1.4/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/organization/user_metadata_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/organization/user_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/pipelines/object_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/pipelines/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/pipelines/object_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/pipelines/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/pipelines/pipelines_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/pipelines/pipelines_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/protection/attachments_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/protection/attachments_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/protection/attachments_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/protection/attachments_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/protection/object_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/protection/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/protection/object_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/protection/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/protection/protection_config_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/protection/protection_config_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/protection/protection_manager_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py` & `prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/protection/protection_reference_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_reference_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/release_channel/object_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/release_channel/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/release_channel/object_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/release_channel/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py` & `prodvana-0.1.4/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/repo/repo_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/repo/repo_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/repo/repo_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/repo/repo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/runtimes/extensions_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/runtimes/extensions_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/runtimes/extensions_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/runtimes/extensions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/scm/types_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/scm/types_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/scm/types_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/scm/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py` & `prodvana-0.1.4/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/service/object_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/service/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/service/object_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/service/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/service/parameters_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/service/parameters_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/service/parameters_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/service/parameters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/service/service_config_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/service/service_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/service/service_config_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/service/service_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/service/service_manager_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/service/service_manager_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from prodvana.proto.prodvana.metrics import metrics_pb2 as prodvana_dot_metrics_dot_metrics__pb2
 from prodvana.proto.prodvana.insights import insights_pb2 as prodvana_dot_insights_dot_insights__pb2
 from prodvana.proto.prodvana.repo import repo_pb2 as prodvana_dot_repo_dot_repo__pb2
 from prodvana.proto.prodvana.version import source_metadata_pb2 as prodvana_dot_version_dot_source__metadata__pb2
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&prodvana/service/service_manager.proto\x12\x10prodvana.service\x1a\x1cgoogle/api/annotations.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\'prodvana/common_config/parameters.proto\x1a!prodvana/service/parameters.proto\x1a%prodvana/service/service_config.proto\x1a$prodvana/service/user_metadata.proto\x1a\x1dprodvana/service/object.proto\x1a\x1eprodvana/stat/efficiency.proto\x1a\x1eprodvana/metrics/metrics.proto\x1a prodvana/insights/insights.proto\x1a\x18prodvana/repo/repo.proto\x1a&prodvana/version/source_metadata.proto\x1a\x17validate/validate.proto\"w\n\x1dServiceConfigVersionReference\x12\x13\n\x0b\x61pplication\x18\x01 \x01(\t\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\'\n\x16service_config_version\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"\xb5\x05\n\x12\x41pplyParametersReq\x12\x39\n\x0eservice_config\x18\x01 \x01(\x0b\x32\x1f.prodvana.service.ServiceConfigH\x00\x12Q\n\x16service_config_version\x18\x08 \x01(\x0b\x32/.prodvana.service.ServiceConfigVersionReferenceH\x00\x12I\n\nparameters\x18\t \x03(\x0b\x32&.prodvana.common_config.ParameterValueB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x62\n\x13per_release_channel\x18\n \x03(\x0b\x32\x36.prodvana.service.ApplyParametersReq.PerReleaseChannelB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12%\n\x1dtest_only_skip_registry_check\x18\x04 \x01(\x08\x12\x13\n\x0b\x61pplication\x18\x05 \x01(\t\x12(\n\x06source\x18\x06 \x01(\x0e\x32\x18.prodvana.version.Source\x12\x39\n\x0fsource_metadata\x18\x07 \x01(\x0b\x32 .prodvana.version.SourceMetadata\x1a\x80\x01\n\x11PerReleaseChannel\x12 \n\x0frelease_channel\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12I\n\nparameters\x18\x02 \x03(\x0b\x32&.prodvana.common_config.ParameterValueB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x42\x0c\n\x05oneof\x12\x03\xf8\x42\x01J\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04R\x10release_channelsR\x12\x63ompute_efficiency\"r\n\x13\x41pplyParametersResp\x12\x12\n\nservice_id\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x36\n\x0f\x65\x66\x66iciency_stat\x18\x03 \x01(\x0b\x32\x1d.prodvana.stat.EfficiencyStat\"\xf9\x01\n\x1bValidateApplyParametersResp\x12/\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1f.prodvana.service.ServiceConfig\x12\x38\n\x0f\x63ompiled_config\x18\x02 \x01(\x0b\x32\x1f.prodvana.service.ServiceConfig\x12\x13\n\x0b\x61pp_version\x18\x03 \x01(\t\x12Z\n!compiled_service_instance_configs\x18\x04 \x03(\x0b\x32/.prodvana.service.CompiledServiceInstanceConfig\"Z\n\x18GetMaterializedConfigReq\x12\x18\n\x07service\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x13\n\x0b\x61pplication\x18\x03 \x01(\t\"\xd3\x02\n\x19GetMaterializedConfigResp\x12/\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1f.prodvana.service.ServiceConfig\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x38\n\x0f\x63ompiled_config\x18\x03 \x01(\x0b\x32\x1f.prodvana.service.ServiceConfig\x12Z\n!compiled_service_instance_configs\x18\x04 \x03(\x0b\x32/.prodvana.service.CompiledServiceInstanceConfig\x12^\n\x10version_metadata\x18\x05 \x01(\x0b\x32\x44.prodvana.service.ListMaterializedConfigVersionsResp.VersionMetadata\"A\n\x10\x44\x65leteServiceReq\x12\x18\n\x07service\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x13\n\x0b\x61pplication\x18\x02 \x01(\t\"\x13\n\x11\x44\x65leteServiceResp\"A\n\x0fListServicesReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x10\n\x08\x64\x65tailed\x18\x02 \x01(\x08\"?\n\x10ListServicesResp\x12+\n\x08services\x18\x01 \x03(\x0b\x32\x19.prodvana.service.Service\"G\n\rGetServiceReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"<\n\x0eGetServiceResp\x12*\n\x07service\x18\x01 \x01(\x0b\x32\x19.prodvana.service.Service\"Q\n\x17ListServiceInstancesReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"X\n\x18ListServiceInstancesResp\x12<\n\x11service_instances\x18\x01 \x03(\x0b\x32!.prodvana.service.ServiceInstance\"q\n\x15GetServiceInstanceReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12 \n\x0frelease_channel\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"U\n\x16GetServiceInstanceResp\x12;\n\x10service_instance\x18\x01 \x01(\x0b\x32!.prodvana.service.ServiceInstance\"\xcc\x01\n\x14GetServiceMetricsReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x33\n\x0fstart_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x0cinclude_cost\x18\x05 \x01(\x08\"~\n\x15GetServiceMetricsResp\x12?\n\x12\x64\x65ployment_metrics\x18\x01 \x01(\x0b\x32#.prodvana.metrics.DeploymentMetrics\x12$\n\x04\x63ost\x18\x02 \x01(\x0b\x32\x16.prodvana.metrics.Cost\"O\n\x15GetServiceInsightsReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"o\n\x0eListCommitsReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x12\n\npage_token\x18\x03 \x01(\t\x12\x11\n\tpage_size\x18\x04 \x01(\x05\"R\n\x0fListCommitsResp\x12&\n\x07\x63ommits\x18\x01 \x03(\x0b\x32\x15.prodvana.repo.Commit\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"F\n\x16GetServiceInsightsResp\x12,\n\x08insights\x18\x01 \x03(\x0b\x32\x1a.prodvana.insights.Insight\"\xbd\x01\n\x17SnoozeServiceInsightReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x31\n\x05\x63lass\x18\x03 \x01(\x0e\x32\x18.prodvana.insights.ClassB\x08\xfa\x42\x05\x82\x01\x02\x10\x01\x12\x37\n\x08\x64uration\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationB\n\xfa\x42\x07\xaa\x01\x04\x08\x01*\x00\"\x1a\n\x18SnoozeServiceInsightResp\"O\n\x15GetServiceMetadataReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"Q\n\x16GetServiceMetadataResp\x12\x37\n\x08metadata\x18\x01 \x01(\x0b\x32%.prodvana.service.ServiceUserMetadata\"\x92\x01\n\x15SetServiceMetadataReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x41\n\x08metadata\x18\x03 \x01(\x0b\x32%.prodvana.service.ServiceUserMetadataB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\"\x18\n\x16SetServiceMetadataResp\"\x82\x01\n!ListMaterializedConfigVersionsReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x12\n\npage_token\x18\x03 \x01(\t\x12\x11\n\tpage_size\x18\x04 \x01(\x05\"\xad\x03\n\"ListMaterializedConfigVersionsResp\x12V\n\x08versions\x18\x01 \x03(\x0b\x32\x44.prodvana.service.ListMaterializedConfigVersionsResp.VersionMetadata\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\x1a\x95\x02\n\x0fVersionMetadata\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x36\n\x12\x63reation_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0e\x63onfig_version\x18\x03 \x01(\t\x12<\n\nparameters\x18\x04 \x01(\x0b\x32(.prodvana.service.ServiceParameterValues\x12(\n\x06source\x18\x05 \x01(\x0e\x32\x18.prodvana.version.Source\x12\x39\n\x0fsource_metadata\x18\x06 \x01(\x0b\x32 .prodvana.version.SourceMetadata\"\xdc\x01\n\x14\x43onfigureService2Req\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x41\n\x0eservice_config\x18\x02 \x01(\x0b\x32\x1f.prodvana.service.ServiceConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12(\n\x06source\x18\x03 \x01(\x0e\x32\x18.prodvana.version.Source\x12\x39\n\x0fsource_metadata\x18\x04 \x01(\x0b\x32 .prodvana.version.SourceMetadata\"C\n\x15\x43onfigureService2Resp\x12\x12\n\nservice_id\x18\x01 \x01(\t\x12\x16\n\x0e\x63onfig_version\x18\x02 \x01(\t\"}\n\x1cListServiceConfigVersionsReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x12\n\npage_token\x18\x03 \x01(\t\x12\x11\n\tpage_size\x18\x04 \x01(\x05\"\xcd\x02\n\x1dListServiceConfigVersionsResp\x12Q\n\x08versions\x18\x01 \x03(\x0b\x32?.prodvana.service.ListServiceConfigVersionsResp.VersionMetadata\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\x1a\xbf\x01\n\x0fVersionMetadata\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x36\n\x12\x63reation_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12(\n\x06source\x18\x03 \x01(\x0e\x32\x18.prodvana.version.Source\x12\x39\n\x0fsource_metadata\x18\x04 \x01(\x0b\x32 .prodvana.version.SourceMetadata\"f\n\x14GetServiceConfig2Req\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x16\n\x0e\x63onfig_version\x18\x03 \x01(\t\"\xc2\x01\n\x15GetServiceConfig2Resp\x12/\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1f.prodvana.service.ServiceConfig\x12\x16\n\x0e\x63onfig_version\x18\x02 \x01(\t\x12`\n\x17\x63onfig_version_metadata\x18\x03 \x01(\x0b\x32?.prodvana.service.ListServiceConfigVersionsResp.VersionMetadata2\xe1\x1b\n\x0eServiceManager\x12\x98\x01\n\x11\x43onfigureService2\x12&.prodvana.service.ConfigureService2Req\x1a\'.prodvana.service.ConfigureService2Resp\"2\x82\xd3\xe4\x93\x02,\"\'/v1/{application=*}/services/configure2:\x01*\x12\xbe\x01\n\x19ListServiceConfigVersions\x12..prodvana.service.ListServiceConfigVersionsReq\x1a/.prodvana.service.ListServiceConfigVersionsResp\"@\x82\xd3\xe4\x93\x02:\x12\x38/v1/{application=*}/services/{service=*}/config/versions\x12\x9d\x01\n\x11GetServiceConfig2\x12&.prodvana.service.GetServiceConfig2Req\x1a\'.prodvana.service.GetServiceConfig2Resp\"7\x82\xd3\xe4\x93\x02\x31\x12//v1/{application=*}/services/{service=*}/config\x12\x98\x01\n\x0f\x41pplyParameters\x12$.prodvana.service.ApplyParametersReq\x1a%.prodvana.service.ApplyParametersResp\"8\x82\xd3\xe4\x93\x02\x32\"-/v1/{application=*}/services/apply-parameters:\x01*\x12\xb1\x01\n\x17ValidateApplyParameters\x12$.prodvana.service.ApplyParametersReq\x1a-.prodvana.service.ValidateApplyParametersResp\"A\x82\xd3\xe4\x93\x02;\"6/v1/{application=*}/services/apply-parameters/validate:\x01*\x12\xb6\x01\n\x15GetMaterializedConfig\x12*.prodvana.service.GetMaterializedConfigReq\x1a+.prodvana.service.GetMaterializedConfigResp\"D\x82\xd3\xe4\x93\x02>\x12</v1/{application=*}/services/{service=*}/materialized/config\x12\xda\x01\n\x1eListMaterializedConfigVersions\x12\x33.prodvana.service.ListMaterializedConfigVersionsReq\x1a\x34.prodvana.service.ListMaterializedConfigVersionsResp\"M\x82\xd3\xe4\x93\x02G\x12\x45/v1/{application=*}/services/{service=*}/materialized/config/versions\x12\x91\x01\n\rDeleteService\x12\".prodvana.service.DeleteServiceReq\x1a#.prodvana.service.DeleteServiceResp\"7\x82\xd3\xe4\x93\x02\x31*//v1/{application=*}/services/{service=*}/delete\x12\x88\x01\n\x0cListServices\x12!.prodvana.service.ListServicesReq\x1a\".prodvana.service.ListServicesResp\"1\x82\xd3\xe4\x93\x02+\x12)/v1/applications/{application=*}/services\x12Y\n\x0eListServicesV2\x12!.prodvana.service.ListServicesReq\x1a\".prodvana.service.ListServicesResp\"\x00\x12\x99\x01\n\x0bListCommits\x12 .prodvana.service.ListCommitsReq\x1a!.prodvana.service.ListCommitsResp\"E\x82\xd3\xe4\x93\x02?\x12=/v1/applications/{application=*}/services/{service=*}/commits\x12\x8e\x01\n\nGetService\x12\x1f.prodvana.service.GetServiceReq\x1a .prodvana.service.GetServiceResp\"=\x82\xd3\xe4\x93\x02\x37\x12\x35/v1/applications/{application=*}/services/{service=*}\x12S\n\x0cGetServiceV2\x12\x1f.prodvana.service.GetServiceReq\x1a .prodvana.service.GetServiceResp\"\x00\x12\xbd\x01\n\x14ListServiceInstances\x12).prodvana.service.ListServiceInstancesReq\x1a*.prodvana.service.ListServiceInstancesResp\"N\x82\xd3\xe4\x93\x02H\x12\x46/v1/applications/{application=*}/services/{service=*}/release-channels\x12q\n\x16ListServiceInstancesV2\x12).prodvana.service.ListServiceInstancesReq\x1a*.prodvana.service.ListServiceInstancesResp\"\x00\x12\xcb\x01\n\x12GetServiceInstance\x12\'.prodvana.service.GetServiceInstanceReq\x1a(.prodvana.service.GetServiceInstanceResp\"b\x82\xd3\xe4\x93\x02\\\x12Z/v1/applications/{application=*}/services/{service=*}/release-channels/{release_channel=*}\x12k\n\x14GetServiceInstanceV2\x12\'.prodvana.service.GetServiceInstanceReq\x1a(.prodvana.service.GetServiceInstanceResp\"\x00\x12\xab\x01\n\x11GetServiceMetrics\x12&.prodvana.service.GetServiceMetricsReq\x1a\'.prodvana.service.GetServiceMetricsResp\"E\x82\xd3\xe4\x93\x02?\x12=/v1/applications/{application=*}/services/{service=*}/metrics\x12\xaf\x01\n\x12GetServiceInsights\x12\'.prodvana.service.GetServiceInsightsReq\x1a(.prodvana.service.GetServiceInsightsResp\"F\x82\xd3\xe4\x93\x02@\x12>/v1/applications/{application=*}/services/{service=*}/insights\x12\xbc\x01\n\x14SnoozeServiceInsight\x12).prodvana.service.SnoozeServiceInsightReq\x1a*.prodvana.service.SnoozeServiceInsightResp\"M\x82\xd3\xe4\x93\x02G\x1a\x45/v1/applications/{application=*}/services/{service=*}/insights/snooze\x12\xaf\x01\n\x12GetServiceMetadata\x12\'.prodvana.service.GetServiceMetadataReq\x1a(.prodvana.service.GetServiceMetadataResp\"F\x82\xd3\xe4\x93\x02@\x12>/v1/applications/{application=*}/services/{service=*}/metadata\x12\xb2\x01\n\x12SetServiceMetadata\x12\'.prodvana.service.SetServiceMetadataReq\x1a(.prodvana.service.SetServiceMetadataResp\"I\x82\xd3\xe4\x93\x02\x43\">/v1/applications/{application=*}/services/{service=*}/metadata:\x01*BLZJgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/serviceb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&prodvana/service/service_manager.proto\x12\x10prodvana.service\x1a\x1cgoogle/api/annotations.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\'prodvana/common_config/parameters.proto\x1a!prodvana/service/parameters.proto\x1a%prodvana/service/service_config.proto\x1a$prodvana/service/user_metadata.proto\x1a\x1dprodvana/service/object.proto\x1a\x1eprodvana/stat/efficiency.proto\x1a\x1eprodvana/metrics/metrics.proto\x1a prodvana/insights/insights.proto\x1a\x18prodvana/repo/repo.proto\x1a&prodvana/version/source_metadata.proto\x1a\x17validate/validate.proto\"w\n\x1dServiceConfigVersionReference\x12\x13\n\x0b\x61pplication\x18\x01 \x01(\t\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\'\n\x16service_config_version\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"\xb5\x05\n\x12\x41pplyParametersReq\x12\x39\n\x0eservice_config\x18\x01 \x01(\x0b\x32\x1f.prodvana.service.ServiceConfigH\x00\x12Q\n\x16service_config_version\x18\x08 \x01(\x0b\x32/.prodvana.service.ServiceConfigVersionReferenceH\x00\x12I\n\nparameters\x18\t \x03(\x0b\x32&.prodvana.common_config.ParameterValueB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x62\n\x13per_release_channel\x18\n \x03(\x0b\x32\x36.prodvana.service.ApplyParametersReq.PerReleaseChannelB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12%\n\x1dtest_only_skip_registry_check\x18\x04 \x01(\x08\x12\x13\n\x0b\x61pplication\x18\x05 \x01(\t\x12(\n\x06source\x18\x06 \x01(\x0e\x32\x18.prodvana.version.Source\x12\x39\n\x0fsource_metadata\x18\x07 \x01(\x0b\x32 .prodvana.version.SourceMetadata\x1a\x80\x01\n\x11PerReleaseChannel\x12 \n\x0frelease_channel\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12I\n\nparameters\x18\x02 \x03(\x0b\x32&.prodvana.common_config.ParameterValueB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x42\x0c\n\x05oneof\x12\x03\xf8\x42\x01J\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04R\x10release_channelsR\x12\x63ompute_efficiency\"r\n\x13\x41pplyParametersResp\x12\x12\n\nservice_id\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x36\n\x0f\x65\x66\x66iciency_stat\x18\x03 \x01(\x0b\x32\x1d.prodvana.stat.EfficiencyStat\"\xf9\x01\n\x1bValidateApplyParametersResp\x12/\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1f.prodvana.service.ServiceConfig\x12\x38\n\x0f\x63ompiled_config\x18\x02 \x01(\x0b\x32\x1f.prodvana.service.ServiceConfig\x12\x13\n\x0b\x61pp_version\x18\x03 \x01(\t\x12Z\n!compiled_service_instance_configs\x18\x04 \x03(\x0b\x32/.prodvana.service.CompiledServiceInstanceConfig\"Z\n\x18GetMaterializedConfigReq\x12\x18\n\x07service\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x13\n\x0b\x61pplication\x18\x03 \x01(\t\"\xd3\x02\n\x19GetMaterializedConfigResp\x12/\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1f.prodvana.service.ServiceConfig\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x38\n\x0f\x63ompiled_config\x18\x03 \x01(\x0b\x32\x1f.prodvana.service.ServiceConfig\x12Z\n!compiled_service_instance_configs\x18\x04 \x03(\x0b\x32/.prodvana.service.CompiledServiceInstanceConfig\x12^\n\x10version_metadata\x18\x05 \x01(\x0b\x32\x44.prodvana.service.ListMaterializedConfigVersionsResp.VersionMetadata\"A\n\x10\x44\x65leteServiceReq\x12\x18\n\x07service\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x13\n\x0b\x61pplication\x18\x02 \x01(\t\"\x13\n\x11\x44\x65leteServiceResp\"A\n\x0fListServicesReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x10\n\x08\x64\x65tailed\x18\x02 \x01(\x08\"?\n\x10ListServicesResp\x12+\n\x08services\x18\x01 \x03(\x0b\x32\x19.prodvana.service.Service\"G\n\rGetServiceReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"<\n\x0eGetServiceResp\x12*\n\x07service\x18\x01 \x01(\x0b\x32\x19.prodvana.service.Service\"Q\n\x17ListServiceInstancesReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"X\n\x18ListServiceInstancesResp\x12<\n\x11service_instances\x18\x01 \x03(\x0b\x32!.prodvana.service.ServiceInstance\"q\n\x15GetServiceInstanceReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12 \n\x0frelease_channel\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"U\n\x16GetServiceInstanceResp\x12;\n\x10service_instance\x18\x01 \x01(\x0b\x32!.prodvana.service.ServiceInstance\"\xcc\x01\n\x14GetServiceMetricsReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x33\n\x0fstart_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x0cinclude_cost\x18\x05 \x01(\x08\"~\n\x15GetServiceMetricsResp\x12?\n\x12\x64\x65ployment_metrics\x18\x01 \x01(\x0b\x32#.prodvana.metrics.DeploymentMetrics\x12$\n\x04\x63ost\x18\x02 \x01(\x0b\x32\x16.prodvana.metrics.Cost\"O\n\x15GetServiceInsightsReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"o\n\x0eListCommitsReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x12\n\npage_token\x18\x03 \x01(\t\x12\x11\n\tpage_size\x18\x04 \x01(\x05\"R\n\x0fListCommitsResp\x12&\n\x07\x63ommits\x18\x01 \x03(\x0b\x32\x15.prodvana.repo.Commit\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"F\n\x16GetServiceInsightsResp\x12,\n\x08insights\x18\x01 \x03(\x0b\x32\x1a.prodvana.insights.Insight\"\xbd\x01\n\x17SnoozeServiceInsightReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x31\n\x05\x63lass\x18\x03 \x01(\x0e\x32\x18.prodvana.insights.ClassB\x08\xfa\x42\x05\x82\x01\x02\x10\x01\x12\x37\n\x08\x64uration\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationB\n\xfa\x42\x07\xaa\x01\x04\x08\x01*\x00\"\x1a\n\x18SnoozeServiceInsightResp\"O\n\x15GetServiceMetadataReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"Q\n\x16GetServiceMetadataResp\x12\x37\n\x08metadata\x18\x01 \x01(\x0b\x32%.prodvana.service.ServiceUserMetadata\"\x92\x01\n\x15SetServiceMetadataReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x41\n\x08metadata\x18\x03 \x01(\x0b\x32%.prodvana.service.ServiceUserMetadataB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\"\x18\n\x16SetServiceMetadataResp\"\x82\x01\n!ListMaterializedConfigVersionsReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x12\n\npage_token\x18\x03 \x01(\t\x12\x11\n\tpage_size\x18\x04 \x01(\x05\"\xad\x03\n\"ListMaterializedConfigVersionsResp\x12V\n\x08versions\x18\x01 \x03(\x0b\x32\x44.prodvana.service.ListMaterializedConfigVersionsResp.VersionMetadata\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\x1a\x95\x02\n\x0fVersionMetadata\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x36\n\x12\x63reation_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0e\x63onfig_version\x18\x03 \x01(\t\x12<\n\nparameters\x18\x04 \x01(\x0b\x32(.prodvana.service.ServiceParameterValues\x12(\n\x06source\x18\x05 \x01(\x0e\x32\x18.prodvana.version.Source\x12\x39\n\x0fsource_metadata\x18\x06 \x01(\x0b\x32 .prodvana.version.SourceMetadata\"\xdb\x01\n\x13\x43onfigureServiceReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x41\n\x0eservice_config\x18\x02 \x01(\x0b\x32\x1f.prodvana.service.ServiceConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12(\n\x06source\x18\x03 \x01(\x0e\x32\x18.prodvana.version.Source\x12\x39\n\x0fsource_metadata\x18\x04 \x01(\x0b\x32 .prodvana.version.SourceMetadata\"B\n\x14\x43onfigureServiceResp\x12\x12\n\nservice_id\x18\x01 \x01(\t\x12\x16\n\x0e\x63onfig_version\x18\x02 \x01(\t\"}\n\x1cListServiceConfigVersionsReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x12\n\npage_token\x18\x03 \x01(\t\x12\x11\n\tpage_size\x18\x04 \x01(\x05\"\xcd\x02\n\x1dListServiceConfigVersionsResp\x12Q\n\x08versions\x18\x01 \x03(\x0b\x32?.prodvana.service.ListServiceConfigVersionsResp.VersionMetadata\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\x1a\xbf\x01\n\x0fVersionMetadata\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x36\n\x12\x63reation_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12(\n\x06source\x18\x03 \x01(\x0e\x32\x18.prodvana.version.Source\x12\x39\n\x0fsource_metadata\x18\x04 \x01(\x0b\x32 .prodvana.version.SourceMetadata\"e\n\x13GetServiceConfigReq\x12\x1c\n\x0b\x61pplication\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x18\n\x07service\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x16\n\x0e\x63onfig_version\x18\x03 \x01(\t\"\xc1\x01\n\x14GetServiceConfigResp\x12/\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1f.prodvana.service.ServiceConfig\x12\x16\n\x0e\x63onfig_version\x18\x02 \x01(\t\x12`\n\x17\x63onfig_version_metadata\x18\x03 \x01(\x0b\x32?.prodvana.service.ListServiceConfigVersionsResp.VersionMetadata2\xcb\x18\n\x0eServiceManager\x12\x95\x01\n\x10\x43onfigureService\x12%.prodvana.service.ConfigureServiceReq\x1a&.prodvana.service.ConfigureServiceResp\"2\x82\xd3\xe4\x93\x02,\"\'/v1/{application=*}/services/configure2:\x01*\x12\xbe\x01\n\x19ListServiceConfigVersions\x12..prodvana.service.ListServiceConfigVersionsReq\x1a/.prodvana.service.ListServiceConfigVersionsResp\"@\x82\xd3\xe4\x93\x02:\x12\x38/v1/{application=*}/services/{service=*}/config/versions\x12\x9a\x01\n\x10GetServiceConfig\x12%.prodvana.service.GetServiceConfigReq\x1a&.prodvana.service.GetServiceConfigResp\"7\x82\xd3\xe4\x93\x02\x31\x12//v1/{application=*}/services/{service=*}/config\x12\x98\x01\n\x0f\x41pplyParameters\x12$.prodvana.service.ApplyParametersReq\x1a%.prodvana.service.ApplyParametersResp\"8\x82\xd3\xe4\x93\x02\x32\"-/v1/{application=*}/services/apply-parameters:\x01*\x12\xb1\x01\n\x17ValidateApplyParameters\x12$.prodvana.service.ApplyParametersReq\x1a-.prodvana.service.ValidateApplyParametersResp\"A\x82\xd3\xe4\x93\x02;\"6/v1/{application=*}/services/apply-parameters/validate:\x01*\x12\xb6\x01\n\x15GetMaterializedConfig\x12*.prodvana.service.GetMaterializedConfigReq\x1a+.prodvana.service.GetMaterializedConfigResp\"D\x82\xd3\xe4\x93\x02>\x12</v1/{application=*}/services/{service=*}/materialized/config\x12\xda\x01\n\x1eListMaterializedConfigVersions\x12\x33.prodvana.service.ListMaterializedConfigVersionsReq\x1a\x34.prodvana.service.ListMaterializedConfigVersionsResp\"M\x82\xd3\xe4\x93\x02G\x12\x45/v1/{application=*}/services/{service=*}/materialized/config/versions\x12\x91\x01\n\rDeleteService\x12\".prodvana.service.DeleteServiceReq\x1a#.prodvana.service.DeleteServiceResp\"7\x82\xd3\xe4\x93\x02\x31*//v1/{application=*}/services/{service=*}/delete\x12\x88\x01\n\x0cListServices\x12!.prodvana.service.ListServicesReq\x1a\".prodvana.service.ListServicesResp\"1\x82\xd3\xe4\x93\x02+\x12)/v1/applications/{application=*}/services\x12\x99\x01\n\x0bListCommits\x12 .prodvana.service.ListCommitsReq\x1a!.prodvana.service.ListCommitsResp\"E\x82\xd3\xe4\x93\x02?\x12=/v1/applications/{application=*}/services/{service=*}/commits\x12\x8e\x01\n\nGetService\x12\x1f.prodvana.service.GetServiceReq\x1a .prodvana.service.GetServiceResp\"=\x82\xd3\xe4\x93\x02\x37\x12\x35/v1/applications/{application=*}/services/{service=*}\x12\xbd\x01\n\x14ListServiceInstances\x12).prodvana.service.ListServiceInstancesReq\x1a*.prodvana.service.ListServiceInstancesResp\"N\x82\xd3\xe4\x93\x02H\x12\x46/v1/applications/{application=*}/services/{service=*}/release-channels\x12\xcb\x01\n\x12GetServiceInstance\x12\'.prodvana.service.GetServiceInstanceReq\x1a(.prodvana.service.GetServiceInstanceResp\"b\x82\xd3\xe4\x93\x02\\\x12Z/v1/applications/{application=*}/services/{service=*}/release-channels/{release_channel=*}\x12\xab\x01\n\x11GetServiceMetrics\x12&.prodvana.service.GetServiceMetricsReq\x1a\'.prodvana.service.GetServiceMetricsResp\"E\x82\xd3\xe4\x93\x02?\x12=/v1/applications/{application=*}/services/{service=*}/metrics\x12\xaf\x01\n\x12GetServiceInsights\x12\'.prodvana.service.GetServiceInsightsReq\x1a(.prodvana.service.GetServiceInsightsResp\"F\x82\xd3\xe4\x93\x02@\x12>/v1/applications/{application=*}/services/{service=*}/insights\x12\xbc\x01\n\x14SnoozeServiceInsight\x12).prodvana.service.SnoozeServiceInsightReq\x1a*.prodvana.service.SnoozeServiceInsightResp\"M\x82\xd3\xe4\x93\x02G\x1a\x45/v1/applications/{application=*}/services/{service=*}/insights/snooze\x12\xaf\x01\n\x12GetServiceMetadata\x12\'.prodvana.service.GetServiceMetadataReq\x1a(.prodvana.service.GetServiceMetadataResp\"F\x82\xd3\xe4\x93\x02@\x12>/v1/applications/{application=*}/services/{service=*}/metadata\x12\xb2\x01\n\x12SetServiceMetadata\x12\'.prodvana.service.SetServiceMetadataReq\x1a(.prodvana.service.SetServiceMetadataResp\"I\x82\xd3\xe4\x93\x02\x43\">/v1/applications/{application=*}/services/{service=*}/metadata:\x01*BLZJgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/serviceb\x06proto3')
 
 
 
 _SERVICECONFIGVERSIONREFERENCE = DESCRIPTOR.message_types_by_name['ServiceConfigVersionReference']
 _APPLYPARAMETERSREQ = DESCRIPTOR.message_types_by_name['ApplyParametersReq']
 _APPLYPARAMETERSREQ_PERRELEASECHANNEL = _APPLYPARAMETERSREQ.nested_types_by_name['PerReleaseChannel']
 _APPLYPARAMETERSRESP = DESCRIPTOR.message_types_by_name['ApplyParametersResp']
@@ -60,21 +60,21 @@
 _GETSERVICEMETADATAREQ = DESCRIPTOR.message_types_by_name['GetServiceMetadataReq']
 _GETSERVICEMETADATARESP = DESCRIPTOR.message_types_by_name['GetServiceMetadataResp']
 _SETSERVICEMETADATAREQ = DESCRIPTOR.message_types_by_name['SetServiceMetadataReq']
 _SETSERVICEMETADATARESP = DESCRIPTOR.message_types_by_name['SetServiceMetadataResp']
 _LISTMATERIALIZEDCONFIGVERSIONSREQ = DESCRIPTOR.message_types_by_name['ListMaterializedConfigVersionsReq']
 _LISTMATERIALIZEDCONFIGVERSIONSRESP = DESCRIPTOR.message_types_by_name['ListMaterializedConfigVersionsResp']
 _LISTMATERIALIZEDCONFIGVERSIONSRESP_VERSIONMETADATA = _LISTMATERIALIZEDCONFIGVERSIONSRESP.nested_types_by_name['VersionMetadata']
-_CONFIGURESERVICE2REQ = DESCRIPTOR.message_types_by_name['ConfigureService2Req']
-_CONFIGURESERVICE2RESP = DESCRIPTOR.message_types_by_name['ConfigureService2Resp']
+_CONFIGURESERVICEREQ = DESCRIPTOR.message_types_by_name['ConfigureServiceReq']
+_CONFIGURESERVICERESP = DESCRIPTOR.message_types_by_name['ConfigureServiceResp']
 _LISTSERVICECONFIGVERSIONSREQ = DESCRIPTOR.message_types_by_name['ListServiceConfigVersionsReq']
 _LISTSERVICECONFIGVERSIONSRESP = DESCRIPTOR.message_types_by_name['ListServiceConfigVersionsResp']
 _LISTSERVICECONFIGVERSIONSRESP_VERSIONMETADATA = _LISTSERVICECONFIGVERSIONSRESP.nested_types_by_name['VersionMetadata']
-_GETSERVICECONFIG2REQ = DESCRIPTOR.message_types_by_name['GetServiceConfig2Req']
-_GETSERVICECONFIG2RESP = DESCRIPTOR.message_types_by_name['GetServiceConfig2Resp']
+_GETSERVICECONFIGREQ = DESCRIPTOR.message_types_by_name['GetServiceConfigReq']
+_GETSERVICECONFIGRESP = DESCRIPTOR.message_types_by_name['GetServiceConfigResp']
 ServiceConfigVersionReference = _reflection.GeneratedProtocolMessageType('ServiceConfigVersionReference', (_message.Message,), {
   'DESCRIPTOR' : _SERVICECONFIGVERSIONREFERENCE,
   '__module__' : 'prodvana.service.service_manager_pb2'
   # @@protoc_insertion_point(class_scope:prodvana.service.ServiceConfigVersionReference)
   })
 _sym_db.RegisterMessage(ServiceConfigVersionReference)
 
@@ -293,27 +293,27 @@
   'DESCRIPTOR' : _LISTMATERIALIZEDCONFIGVERSIONSRESP,
   '__module__' : 'prodvana.service.service_manager_pb2'
   # @@protoc_insertion_point(class_scope:prodvana.service.ListMaterializedConfigVersionsResp)
   })
 _sym_db.RegisterMessage(ListMaterializedConfigVersionsResp)
 _sym_db.RegisterMessage(ListMaterializedConfigVersionsResp.VersionMetadata)
 
-ConfigureService2Req = _reflection.GeneratedProtocolMessageType('ConfigureService2Req', (_message.Message,), {
-  'DESCRIPTOR' : _CONFIGURESERVICE2REQ,
+ConfigureServiceReq = _reflection.GeneratedProtocolMessageType('ConfigureServiceReq', (_message.Message,), {
+  'DESCRIPTOR' : _CONFIGURESERVICEREQ,
   '__module__' : 'prodvana.service.service_manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.service.ConfigureService2Req)
+  # @@protoc_insertion_point(class_scope:prodvana.service.ConfigureServiceReq)
   })
-_sym_db.RegisterMessage(ConfigureService2Req)
+_sym_db.RegisterMessage(ConfigureServiceReq)
 
-ConfigureService2Resp = _reflection.GeneratedProtocolMessageType('ConfigureService2Resp', (_message.Message,), {
-  'DESCRIPTOR' : _CONFIGURESERVICE2RESP,
+ConfigureServiceResp = _reflection.GeneratedProtocolMessageType('ConfigureServiceResp', (_message.Message,), {
+  'DESCRIPTOR' : _CONFIGURESERVICERESP,
   '__module__' : 'prodvana.service.service_manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.service.ConfigureService2Resp)
+  # @@protoc_insertion_point(class_scope:prodvana.service.ConfigureServiceResp)
   })
-_sym_db.RegisterMessage(ConfigureService2Resp)
+_sym_db.RegisterMessage(ConfigureServiceResp)
 
 ListServiceConfigVersionsReq = _reflection.GeneratedProtocolMessageType('ListServiceConfigVersionsReq', (_message.Message,), {
   'DESCRIPTOR' : _LISTSERVICECONFIGVERSIONSREQ,
   '__module__' : 'prodvana.service.service_manager_pb2'
   # @@protoc_insertion_point(class_scope:prodvana.service.ListServiceConfigVersionsReq)
   })
 _sym_db.RegisterMessage(ListServiceConfigVersionsReq)
@@ -329,27 +329,27 @@
   'DESCRIPTOR' : _LISTSERVICECONFIGVERSIONSRESP,
   '__module__' : 'prodvana.service.service_manager_pb2'
   # @@protoc_insertion_point(class_scope:prodvana.service.ListServiceConfigVersionsResp)
   })
 _sym_db.RegisterMessage(ListServiceConfigVersionsResp)
 _sym_db.RegisterMessage(ListServiceConfigVersionsResp.VersionMetadata)
 
-GetServiceConfig2Req = _reflection.GeneratedProtocolMessageType('GetServiceConfig2Req', (_message.Message,), {
-  'DESCRIPTOR' : _GETSERVICECONFIG2REQ,
+GetServiceConfigReq = _reflection.GeneratedProtocolMessageType('GetServiceConfigReq', (_message.Message,), {
+  'DESCRIPTOR' : _GETSERVICECONFIGREQ,
   '__module__' : 'prodvana.service.service_manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.service.GetServiceConfig2Req)
+  # @@protoc_insertion_point(class_scope:prodvana.service.GetServiceConfigReq)
   })
-_sym_db.RegisterMessage(GetServiceConfig2Req)
+_sym_db.RegisterMessage(GetServiceConfigReq)
 
-GetServiceConfig2Resp = _reflection.GeneratedProtocolMessageType('GetServiceConfig2Resp', (_message.Message,), {
-  'DESCRIPTOR' : _GETSERVICECONFIG2RESP,
+GetServiceConfigResp = _reflection.GeneratedProtocolMessageType('GetServiceConfigResp', (_message.Message,), {
+  'DESCRIPTOR' : _GETSERVICECONFIGRESP,
   '__module__' : 'prodvana.service.service_manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.service.GetServiceConfig2Resp)
+  # @@protoc_insertion_point(class_scope:prodvana.service.GetServiceConfigResp)
   })
-_sym_db.RegisterMessage(GetServiceConfig2Resp)
+_sym_db.RegisterMessage(GetServiceConfigResp)
 
 _SERVICEMANAGER = DESCRIPTOR.services_by_name['ServiceManager']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZJgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/service'
   _SERVICECONFIGVERSIONREFERENCE.fields_by_name['service']._options = None
@@ -416,32 +416,32 @@
   _SETSERVICEMETADATAREQ.fields_by_name['service']._serialized_options = b'\372B\004r\002\020\001'
   _SETSERVICEMETADATAREQ.fields_by_name['metadata']._options = None
   _SETSERVICEMETADATAREQ.fields_by_name['metadata']._serialized_options = b'\372B\005\212\001\002\020\001'
   _LISTMATERIALIZEDCONFIGVERSIONSREQ.fields_by_name['application']._options = None
   _LISTMATERIALIZEDCONFIGVERSIONSREQ.fields_by_name['application']._serialized_options = b'\372B\004r\002\020\001'
   _LISTMATERIALIZEDCONFIGVERSIONSREQ.fields_by_name['service']._options = None
   _LISTMATERIALIZEDCONFIGVERSIONSREQ.fields_by_name['service']._serialized_options = b'\372B\004r\002\020\001'
-  _CONFIGURESERVICE2REQ.fields_by_name['application']._options = None
-  _CONFIGURESERVICE2REQ.fields_by_name['application']._serialized_options = b'\372B\004r\002\020\001'
-  _CONFIGURESERVICE2REQ.fields_by_name['service_config']._options = None
-  _CONFIGURESERVICE2REQ.fields_by_name['service_config']._serialized_options = b'\372B\005\212\001\002\020\001'
+  _CONFIGURESERVICEREQ.fields_by_name['application']._options = None
+  _CONFIGURESERVICEREQ.fields_by_name['application']._serialized_options = b'\372B\004r\002\020\001'
+  _CONFIGURESERVICEREQ.fields_by_name['service_config']._options = None
+  _CONFIGURESERVICEREQ.fields_by_name['service_config']._serialized_options = b'\372B\005\212\001\002\020\001'
   _LISTSERVICECONFIGVERSIONSREQ.fields_by_name['application']._options = None
   _LISTSERVICECONFIGVERSIONSREQ.fields_by_name['application']._serialized_options = b'\372B\004r\002\020\001'
   _LISTSERVICECONFIGVERSIONSREQ.fields_by_name['service']._options = None
   _LISTSERVICECONFIGVERSIONSREQ.fields_by_name['service']._serialized_options = b'\372B\004r\002\020\001'
-  _GETSERVICECONFIG2REQ.fields_by_name['application']._options = None
-  _GETSERVICECONFIG2REQ.fields_by_name['application']._serialized_options = b'\372B\004r\002\020\001'
-  _GETSERVICECONFIG2REQ.fields_by_name['service']._options = None
-  _GETSERVICECONFIG2REQ.fields_by_name['service']._serialized_options = b'\372B\004r\002\020\001'
-  _SERVICEMANAGER.methods_by_name['ConfigureService2']._options = None
-  _SERVICEMANAGER.methods_by_name['ConfigureService2']._serialized_options = b'\202\323\344\223\002,\"\'/v1/{application=*}/services/configure2:\001*'
+  _GETSERVICECONFIGREQ.fields_by_name['application']._options = None
+  _GETSERVICECONFIGREQ.fields_by_name['application']._serialized_options = b'\372B\004r\002\020\001'
+  _GETSERVICECONFIGREQ.fields_by_name['service']._options = None
+  _GETSERVICECONFIGREQ.fields_by_name['service']._serialized_options = b'\372B\004r\002\020\001'
+  _SERVICEMANAGER.methods_by_name['ConfigureService']._options = None
+  _SERVICEMANAGER.methods_by_name['ConfigureService']._serialized_options = b'\202\323\344\223\002,\"\'/v1/{application=*}/services/configure2:\001*'
   _SERVICEMANAGER.methods_by_name['ListServiceConfigVersions']._options = None
   _SERVICEMANAGER.methods_by_name['ListServiceConfigVersions']._serialized_options = b'\202\323\344\223\002:\0228/v1/{application=*}/services/{service=*}/config/versions'
-  _SERVICEMANAGER.methods_by_name['GetServiceConfig2']._options = None
-  _SERVICEMANAGER.methods_by_name['GetServiceConfig2']._serialized_options = b'\202\323\344\223\0021\022//v1/{application=*}/services/{service=*}/config'
+  _SERVICEMANAGER.methods_by_name['GetServiceConfig']._options = None
+  _SERVICEMANAGER.methods_by_name['GetServiceConfig']._serialized_options = b'\202\323\344\223\0021\022//v1/{application=*}/services/{service=*}/config'
   _SERVICEMANAGER.methods_by_name['ApplyParameters']._options = None
   _SERVICEMANAGER.methods_by_name['ApplyParameters']._serialized_options = b'\202\323\344\223\0022\"-/v1/{application=*}/services/apply-parameters:\001*'
   _SERVICEMANAGER.methods_by_name['ValidateApplyParameters']._options = None
   _SERVICEMANAGER.methods_by_name['ValidateApplyParameters']._serialized_options = b'\202\323\344\223\002;\"6/v1/{application=*}/services/apply-parameters/validate:\001*'
   _SERVICEMANAGER.methods_by_name['GetMaterializedConfig']._options = None
   _SERVICEMANAGER.methods_by_name['GetMaterializedConfig']._serialized_options = b'\202\323\344\223\002>\022</v1/{application=*}/services/{service=*}/materialized/config'
   _SERVICEMANAGER.methods_by_name['ListMaterializedConfigVersions']._options = None
@@ -528,24 +528,24 @@
   _SETSERVICEMETADATARESP._serialized_end=4119
   _LISTMATERIALIZEDCONFIGVERSIONSREQ._serialized_start=4122
   _LISTMATERIALIZEDCONFIGVERSIONSREQ._serialized_end=4252
   _LISTMATERIALIZEDCONFIGVERSIONSRESP._serialized_start=4255
   _LISTMATERIALIZEDCONFIGVERSIONSRESP._serialized_end=4684
   _LISTMATERIALIZEDCONFIGVERSIONSRESP_VERSIONMETADATA._serialized_start=4407
   _LISTMATERIALIZEDCONFIGVERSIONSRESP_VERSIONMETADATA._serialized_end=4684
-  _CONFIGURESERVICE2REQ._serialized_start=4687
-  _CONFIGURESERVICE2REQ._serialized_end=4907
-  _CONFIGURESERVICE2RESP._serialized_start=4909
-  _CONFIGURESERVICE2RESP._serialized_end=4976
-  _LISTSERVICECONFIGVERSIONSREQ._serialized_start=4978
-  _LISTSERVICECONFIGVERSIONSREQ._serialized_end=5103
-  _LISTSERVICECONFIGVERSIONSRESP._serialized_start=5106
-  _LISTSERVICECONFIGVERSIONSRESP._serialized_end=5439
-  _LISTSERVICECONFIGVERSIONSRESP_VERSIONMETADATA._serialized_start=5248
-  _LISTSERVICECONFIGVERSIONSRESP_VERSIONMETADATA._serialized_end=5439
-  _GETSERVICECONFIG2REQ._serialized_start=5441
-  _GETSERVICECONFIG2REQ._serialized_end=5543
-  _GETSERVICECONFIG2RESP._serialized_start=5546
-  _GETSERVICECONFIG2RESP._serialized_end=5740
-  _SERVICEMANAGER._serialized_start=5743
-  _SERVICEMANAGER._serialized_end=9296
+  _CONFIGURESERVICEREQ._serialized_start=4687
+  _CONFIGURESERVICEREQ._serialized_end=4906
+  _CONFIGURESERVICERESP._serialized_start=4908
+  _CONFIGURESERVICERESP._serialized_end=4974
+  _LISTSERVICECONFIGVERSIONSREQ._serialized_start=4976
+  _LISTSERVICECONFIGVERSIONSREQ._serialized_end=5101
+  _LISTSERVICECONFIGVERSIONSRESP._serialized_start=5104
+  _LISTSERVICECONFIGVERSIONSRESP._serialized_end=5437
+  _LISTSERVICECONFIGVERSIONSRESP_VERSIONMETADATA._serialized_start=5246
+  _LISTSERVICECONFIGVERSIONSRESP_VERSIONMETADATA._serialized_end=5437
+  _GETSERVICECONFIGREQ._serialized_start=5439
+  _GETSERVICECONFIGREQ._serialized_end=5540
+  _GETSERVICECONFIGRESP._serialized_start=5543
+  _GETSERVICECONFIGRESP._serialized_end=5736
+  _SERVICEMANAGER._serialized_start=5739
+  _SERVICEMANAGER._serialized_end=8886
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/service/service_manager_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/service/service_manager_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -666,15 +666,15 @@
         versions: collections.abc.Iterable[global___ListMaterializedConfigVersionsResp.VersionMetadata] | None = ...,
         next_page_token: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["next_page_token", b"next_page_token", "versions", b"versions"]) -> None: ...
 
 global___ListMaterializedConfigVersionsResp = ListMaterializedConfigVersionsResp
 
-class ConfigureService2Req(google.protobuf.message.Message):
+class ConfigureServiceReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     APPLICATION_FIELD_NUMBER: builtins.int
     SERVICE_CONFIG_FIELD_NUMBER: builtins.int
     SOURCE_FIELD_NUMBER: builtins.int
     SOURCE_METADATA_FIELD_NUMBER: builtins.int
     application: builtins.str
@@ -690,32 +690,32 @@
         service_config: prodvana.proto.prodvana.service.service_config_pb2.ServiceConfig | None = ...,
         source: prodvana.proto.prodvana.version.source_metadata_pb2.Source.ValueType = ...,
         source_metadata: prodvana.proto.prodvana.version.source_metadata_pb2.SourceMetadata | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["service_config", b"service_config", "source_metadata", b"source_metadata"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "service_config", b"service_config", "source", b"source", "source_metadata", b"source_metadata"]) -> None: ...
 
-global___ConfigureService2Req = ConfigureService2Req
+global___ConfigureServiceReq = ConfigureServiceReq
 
-class ConfigureService2Resp(google.protobuf.message.Message):
+class ConfigureServiceResp(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SERVICE_ID_FIELD_NUMBER: builtins.int
     CONFIG_VERSION_FIELD_NUMBER: builtins.int
     service_id: builtins.str
     config_version: builtins.str
     def __init__(
         self,
         *,
         service_id: builtins.str = ...,
         config_version: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["config_version", b"config_version", "service_id", b"service_id"]) -> None: ...
 
-global___ConfigureService2Resp = ConfigureService2Resp
+global___ConfigureServiceResp = ConfigureServiceResp
 
 class ListServiceConfigVersionsReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     APPLICATION_FIELD_NUMBER: builtins.int
     SERVICE_FIELD_NUMBER: builtins.int
     PAGE_TOKEN_FIELD_NUMBER: builtins.int
@@ -774,15 +774,15 @@
         versions: collections.abc.Iterable[global___ListServiceConfigVersionsResp.VersionMetadata] | None = ...,
         next_page_token: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["next_page_token", b"next_page_token", "versions", b"versions"]) -> None: ...
 
 global___ListServiceConfigVersionsResp = ListServiceConfigVersionsResp
 
-class GetServiceConfig2Req(google.protobuf.message.Message):
+class GetServiceConfigReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     APPLICATION_FIELD_NUMBER: builtins.int
     SERVICE_FIELD_NUMBER: builtins.int
     CONFIG_VERSION_FIELD_NUMBER: builtins.int
     application: builtins.str
     service: builtins.str
@@ -793,17 +793,17 @@
         *,
         application: builtins.str = ...,
         service: builtins.str = ...,
         config_version: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "config_version", b"config_version", "service", b"service"]) -> None: ...
 
-global___GetServiceConfig2Req = GetServiceConfig2Req
+global___GetServiceConfigReq = GetServiceConfigReq
 
-class GetServiceConfig2Resp(google.protobuf.message.Message):
+class GetServiceConfigResp(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CONFIG_FIELD_NUMBER: builtins.int
     CONFIG_VERSION_FIELD_NUMBER: builtins.int
     CONFIG_VERSION_METADATA_FIELD_NUMBER: builtins.int
     @property
     def config(self) -> prodvana.proto.prodvana.service.service_config_pb2.ServiceConfig: ...
@@ -817,8 +817,8 @@
         config: prodvana.proto.prodvana.service.service_config_pb2.ServiceConfig | None = ...,
         config_version: builtins.str = ...,
         config_version_metadata: global___ListServiceConfigVersionsResp.VersionMetadata | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["config", b"config", "config_version_metadata", b"config_version_metadata"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["config", b"config", "config_version", b"config_version", "config_version_metadata", b"config_version_metadata"]) -> None: ...
 
-global___GetServiceConfig2Resp = GetServiceConfig2Resp
+global___GetServiceConfigResp = GetServiceConfigResp
```

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py` & `prodvana-0.1.4/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.ConfigureService2 = channel.unary_unary(
-                '/prodvana.service.ServiceManager/ConfigureService2',
-                request_serializer=prodvana_dot_service_dot_service__manager__pb2.ConfigureService2Req.SerializeToString,
-                response_deserializer=prodvana_dot_service_dot_service__manager__pb2.ConfigureService2Resp.FromString,
+        self.ConfigureService = channel.unary_unary(
+                '/prodvana.service.ServiceManager/ConfigureService',
+                request_serializer=prodvana_dot_service_dot_service__manager__pb2.ConfigureServiceReq.SerializeToString,
+                response_deserializer=prodvana_dot_service_dot_service__manager__pb2.ConfigureServiceResp.FromString,
                 )
         self.ListServiceConfigVersions = channel.unary_unary(
                 '/prodvana.service.ServiceManager/ListServiceConfigVersions',
                 request_serializer=prodvana_dot_service_dot_service__manager__pb2.ListServiceConfigVersionsReq.SerializeToString,
                 response_deserializer=prodvana_dot_service_dot_service__manager__pb2.ListServiceConfigVersionsResp.FromString,
                 )
-        self.GetServiceConfig2 = channel.unary_unary(
-                '/prodvana.service.ServiceManager/GetServiceConfig2',
-                request_serializer=prodvana_dot_service_dot_service__manager__pb2.GetServiceConfig2Req.SerializeToString,
-                response_deserializer=prodvana_dot_service_dot_service__manager__pb2.GetServiceConfig2Resp.FromString,
+        self.GetServiceConfig = channel.unary_unary(
+                '/prodvana.service.ServiceManager/GetServiceConfig',
+                request_serializer=prodvana_dot_service_dot_service__manager__pb2.GetServiceConfigReq.SerializeToString,
+                response_deserializer=prodvana_dot_service_dot_service__manager__pb2.GetServiceConfigResp.FromString,
                 )
         self.ApplyParameters = channel.unary_unary(
                 '/prodvana.service.ServiceManager/ApplyParameters',
                 request_serializer=prodvana_dot_service_dot_service__manager__pb2.ApplyParametersReq.SerializeToString,
                 response_deserializer=prodvana_dot_service_dot_service__manager__pb2.ApplyParametersResp.FromString,
                 )
         self.ValidateApplyParameters = channel.unary_unary(
@@ -55,54 +55,34 @@
                 response_deserializer=prodvana_dot_service_dot_service__manager__pb2.DeleteServiceResp.FromString,
                 )
         self.ListServices = channel.unary_unary(
                 '/prodvana.service.ServiceManager/ListServices',
                 request_serializer=prodvana_dot_service_dot_service__manager__pb2.ListServicesReq.SerializeToString,
                 response_deserializer=prodvana_dot_service_dot_service__manager__pb2.ListServicesResp.FromString,
                 )
-        self.ListServicesV2 = channel.unary_unary(
-                '/prodvana.service.ServiceManager/ListServicesV2',
-                request_serializer=prodvana_dot_service_dot_service__manager__pb2.ListServicesReq.SerializeToString,
-                response_deserializer=prodvana_dot_service_dot_service__manager__pb2.ListServicesResp.FromString,
-                )
         self.ListCommits = channel.unary_unary(
                 '/prodvana.service.ServiceManager/ListCommits',
                 request_serializer=prodvana_dot_service_dot_service__manager__pb2.ListCommitsReq.SerializeToString,
                 response_deserializer=prodvana_dot_service_dot_service__manager__pb2.ListCommitsResp.FromString,
                 )
         self.GetService = channel.unary_unary(
                 '/prodvana.service.ServiceManager/GetService',
                 request_serializer=prodvana_dot_service_dot_service__manager__pb2.GetServiceReq.SerializeToString,
                 response_deserializer=prodvana_dot_service_dot_service__manager__pb2.GetServiceResp.FromString,
                 )
-        self.GetServiceV2 = channel.unary_unary(
-                '/prodvana.service.ServiceManager/GetServiceV2',
-                request_serializer=prodvana_dot_service_dot_service__manager__pb2.GetServiceReq.SerializeToString,
-                response_deserializer=prodvana_dot_service_dot_service__manager__pb2.GetServiceResp.FromString,
-                )
         self.ListServiceInstances = channel.unary_unary(
                 '/prodvana.service.ServiceManager/ListServiceInstances',
                 request_serializer=prodvana_dot_service_dot_service__manager__pb2.ListServiceInstancesReq.SerializeToString,
                 response_deserializer=prodvana_dot_service_dot_service__manager__pb2.ListServiceInstancesResp.FromString,
                 )
-        self.ListServiceInstancesV2 = channel.unary_unary(
-                '/prodvana.service.ServiceManager/ListServiceInstancesV2',
-                request_serializer=prodvana_dot_service_dot_service__manager__pb2.ListServiceInstancesReq.SerializeToString,
-                response_deserializer=prodvana_dot_service_dot_service__manager__pb2.ListServiceInstancesResp.FromString,
-                )
         self.GetServiceInstance = channel.unary_unary(
                 '/prodvana.service.ServiceManager/GetServiceInstance',
                 request_serializer=prodvana_dot_service_dot_service__manager__pb2.GetServiceInstanceReq.SerializeToString,
                 response_deserializer=prodvana_dot_service_dot_service__manager__pb2.GetServiceInstanceResp.FromString,
                 )
-        self.GetServiceInstanceV2 = channel.unary_unary(
-                '/prodvana.service.ServiceManager/GetServiceInstanceV2',
-                request_serializer=prodvana_dot_service_dot_service__manager__pb2.GetServiceInstanceReq.SerializeToString,
-                response_deserializer=prodvana_dot_service_dot_service__manager__pb2.GetServiceInstanceResp.FromString,
-                )
         self.GetServiceMetrics = channel.unary_unary(
                 '/prodvana.service.ServiceManager/GetServiceMetrics',
                 request_serializer=prodvana_dot_service_dot_service__manager__pb2.GetServiceMetricsReq.SerializeToString,
                 response_deserializer=prodvana_dot_service_dot_service__manager__pb2.GetServiceMetricsResp.FromString,
                 )
         self.GetServiceInsights = channel.unary_unary(
                 '/prodvana.service.ServiceManager/GetServiceInsights',
@@ -125,28 +105,27 @@
                 response_deserializer=prodvana_dot_service_dot_service__manager__pb2.SetServiceMetadataResp.FromString,
                 )
 
 
 class ServiceManagerServicer(object):
     """Missing associated documentation comment in .proto file."""
 
-    def ConfigureService2(self, request, context):
-        """TODO(naphat) rename this to ConfigureService
-        """
+    def ConfigureService(self, request, context):
+        """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def ListServiceConfigVersions(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetServiceConfig2(self, request, context):
+    def GetServiceConfig(self, request, context):
         """unparametrized configs
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def ApplyParameters(self, request, context):
@@ -181,66 +160,38 @@
 
     def ListServices(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ListServicesV2(self, request, context):
-        """identical to ListServices, kept around for compatibility purposes
-        """
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
     def ListCommits(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetService(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetServiceV2(self, request, context):
-        """identical to GetService, kept around for compatibility purposes
-        """
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
     def ListServiceInstances(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ListServiceInstancesV2(self, request, context):
-        """identical to ListServiceInstances, kept around for compatibility purposes
-        """
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
     def GetServiceInstance(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetServiceInstanceV2(self, request, context):
-        """identical to GetServiceInstance, kept around for compatibility purposes
-        """
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
     def GetServiceMetrics(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetServiceInsights(self, request, context):
@@ -266,28 +217,28 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_ServiceManagerServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'ConfigureService2': grpc.unary_unary_rpc_method_handler(
-                    servicer.ConfigureService2,
-                    request_deserializer=prodvana_dot_service_dot_service__manager__pb2.ConfigureService2Req.FromString,
-                    response_serializer=prodvana_dot_service_dot_service__manager__pb2.ConfigureService2Resp.SerializeToString,
+            'ConfigureService': grpc.unary_unary_rpc_method_handler(
+                    servicer.ConfigureService,
+                    request_deserializer=prodvana_dot_service_dot_service__manager__pb2.ConfigureServiceReq.FromString,
+                    response_serializer=prodvana_dot_service_dot_service__manager__pb2.ConfigureServiceResp.SerializeToString,
             ),
             'ListServiceConfigVersions': grpc.unary_unary_rpc_method_handler(
                     servicer.ListServiceConfigVersions,
                     request_deserializer=prodvana_dot_service_dot_service__manager__pb2.ListServiceConfigVersionsReq.FromString,
                     response_serializer=prodvana_dot_service_dot_service__manager__pb2.ListServiceConfigVersionsResp.SerializeToString,
             ),
-            'GetServiceConfig2': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetServiceConfig2,
-                    request_deserializer=prodvana_dot_service_dot_service__manager__pb2.GetServiceConfig2Req.FromString,
-                    response_serializer=prodvana_dot_service_dot_service__manager__pb2.GetServiceConfig2Resp.SerializeToString,
+            'GetServiceConfig': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetServiceConfig,
+                    request_deserializer=prodvana_dot_service_dot_service__manager__pb2.GetServiceConfigReq.FromString,
+                    response_serializer=prodvana_dot_service_dot_service__manager__pb2.GetServiceConfigResp.SerializeToString,
             ),
             'ApplyParameters': grpc.unary_unary_rpc_method_handler(
                     servicer.ApplyParameters,
                     request_deserializer=prodvana_dot_service_dot_service__manager__pb2.ApplyParametersReq.FromString,
                     response_serializer=prodvana_dot_service_dot_service__manager__pb2.ApplyParametersResp.SerializeToString,
             ),
             'ValidateApplyParameters': grpc.unary_unary_rpc_method_handler(
@@ -311,54 +262,34 @@
                     response_serializer=prodvana_dot_service_dot_service__manager__pb2.DeleteServiceResp.SerializeToString,
             ),
             'ListServices': grpc.unary_unary_rpc_method_handler(
                     servicer.ListServices,
                     request_deserializer=prodvana_dot_service_dot_service__manager__pb2.ListServicesReq.FromString,
                     response_serializer=prodvana_dot_service_dot_service__manager__pb2.ListServicesResp.SerializeToString,
             ),
-            'ListServicesV2': grpc.unary_unary_rpc_method_handler(
-                    servicer.ListServicesV2,
-                    request_deserializer=prodvana_dot_service_dot_service__manager__pb2.ListServicesReq.FromString,
-                    response_serializer=prodvana_dot_service_dot_service__manager__pb2.ListServicesResp.SerializeToString,
-            ),
             'ListCommits': grpc.unary_unary_rpc_method_handler(
                     servicer.ListCommits,
                     request_deserializer=prodvana_dot_service_dot_service__manager__pb2.ListCommitsReq.FromString,
                     response_serializer=prodvana_dot_service_dot_service__manager__pb2.ListCommitsResp.SerializeToString,
             ),
             'GetService': grpc.unary_unary_rpc_method_handler(
                     servicer.GetService,
                     request_deserializer=prodvana_dot_service_dot_service__manager__pb2.GetServiceReq.FromString,
                     response_serializer=prodvana_dot_service_dot_service__manager__pb2.GetServiceResp.SerializeToString,
             ),
-            'GetServiceV2': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetServiceV2,
-                    request_deserializer=prodvana_dot_service_dot_service__manager__pb2.GetServiceReq.FromString,
-                    response_serializer=prodvana_dot_service_dot_service__manager__pb2.GetServiceResp.SerializeToString,
-            ),
             'ListServiceInstances': grpc.unary_unary_rpc_method_handler(
                     servicer.ListServiceInstances,
                     request_deserializer=prodvana_dot_service_dot_service__manager__pb2.ListServiceInstancesReq.FromString,
                     response_serializer=prodvana_dot_service_dot_service__manager__pb2.ListServiceInstancesResp.SerializeToString,
             ),
-            'ListServiceInstancesV2': grpc.unary_unary_rpc_method_handler(
-                    servicer.ListServiceInstancesV2,
-                    request_deserializer=prodvana_dot_service_dot_service__manager__pb2.ListServiceInstancesReq.FromString,
-                    response_serializer=prodvana_dot_service_dot_service__manager__pb2.ListServiceInstancesResp.SerializeToString,
-            ),
             'GetServiceInstance': grpc.unary_unary_rpc_method_handler(
                     servicer.GetServiceInstance,
                     request_deserializer=prodvana_dot_service_dot_service__manager__pb2.GetServiceInstanceReq.FromString,
                     response_serializer=prodvana_dot_service_dot_service__manager__pb2.GetServiceInstanceResp.SerializeToString,
             ),
-            'GetServiceInstanceV2': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetServiceInstanceV2,
-                    request_deserializer=prodvana_dot_service_dot_service__manager__pb2.GetServiceInstanceReq.FromString,
-                    response_serializer=prodvana_dot_service_dot_service__manager__pb2.GetServiceInstanceResp.SerializeToString,
-            ),
             'GetServiceMetrics': grpc.unary_unary_rpc_method_handler(
                     servicer.GetServiceMetrics,
                     request_deserializer=prodvana_dot_service_dot_service__manager__pb2.GetServiceMetricsReq.FromString,
                     response_serializer=prodvana_dot_service_dot_service__manager__pb2.GetServiceMetricsResp.SerializeToString,
             ),
             'GetServiceInsights': grpc.unary_unary_rpc_method_handler(
                     servicer.GetServiceInsights,
@@ -387,27 +318,27 @@
 
 
  # This class is part of an EXPERIMENTAL API.
 class ServiceManager(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def ConfigureService2(request,
+    def ConfigureService(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/prodvana.service.ServiceManager/ConfigureService2',
-            prodvana_dot_service_dot_service__manager__pb2.ConfigureService2Req.SerializeToString,
-            prodvana_dot_service_dot_service__manager__pb2.ConfigureService2Resp.FromString,
+        return grpc.experimental.unary_unary(request, target, '/prodvana.service.ServiceManager/ConfigureService',
+            prodvana_dot_service_dot_service__manager__pb2.ConfigureServiceReq.SerializeToString,
+            prodvana_dot_service_dot_service__manager__pb2.ConfigureServiceResp.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def ListServiceConfigVersions(request,
             target,
             options=(),
@@ -421,27 +352,27 @@
         return grpc.experimental.unary_unary(request, target, '/prodvana.service.ServiceManager/ListServiceConfigVersions',
             prodvana_dot_service_dot_service__manager__pb2.ListServiceConfigVersionsReq.SerializeToString,
             prodvana_dot_service_dot_service__manager__pb2.ListServiceConfigVersionsResp.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetServiceConfig2(request,
+    def GetServiceConfig(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/prodvana.service.ServiceManager/GetServiceConfig2',
-            prodvana_dot_service_dot_service__manager__pb2.GetServiceConfig2Req.SerializeToString,
-            prodvana_dot_service_dot_service__manager__pb2.GetServiceConfig2Resp.FromString,
+        return grpc.experimental.unary_unary(request, target, '/prodvana.service.ServiceManager/GetServiceConfig',
+            prodvana_dot_service_dot_service__manager__pb2.GetServiceConfigReq.SerializeToString,
+            prodvana_dot_service_dot_service__manager__pb2.GetServiceConfigResp.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def ApplyParameters(request,
             target,
             options=(),
@@ -540,31 +471,14 @@
         return grpc.experimental.unary_unary(request, target, '/prodvana.service.ServiceManager/ListServices',
             prodvana_dot_service_dot_service__manager__pb2.ListServicesReq.SerializeToString,
             prodvana_dot_service_dot_service__manager__pb2.ListServicesResp.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ListServicesV2(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/prodvana.service.ServiceManager/ListServicesV2',
-            prodvana_dot_service_dot_service__manager__pb2.ListServicesReq.SerializeToString,
-            prodvana_dot_service_dot_service__manager__pb2.ListServicesResp.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
     def ListCommits(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -591,31 +505,14 @@
         return grpc.experimental.unary_unary(request, target, '/prodvana.service.ServiceManager/GetService',
             prodvana_dot_service_dot_service__manager__pb2.GetServiceReq.SerializeToString,
             prodvana_dot_service_dot_service__manager__pb2.GetServiceResp.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetServiceV2(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/prodvana.service.ServiceManager/GetServiceV2',
-            prodvana_dot_service_dot_service__manager__pb2.GetServiceReq.SerializeToString,
-            prodvana_dot_service_dot_service__manager__pb2.GetServiceResp.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
     def ListServiceInstances(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -625,31 +522,14 @@
         return grpc.experimental.unary_unary(request, target, '/prodvana.service.ServiceManager/ListServiceInstances',
             prodvana_dot_service_dot_service__manager__pb2.ListServiceInstancesReq.SerializeToString,
             prodvana_dot_service_dot_service__manager__pb2.ListServiceInstancesResp.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ListServiceInstancesV2(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/prodvana.service.ServiceManager/ListServiceInstancesV2',
-            prodvana_dot_service_dot_service__manager__pb2.ListServiceInstancesReq.SerializeToString,
-            prodvana_dot_service_dot_service__manager__pb2.ListServiceInstancesResp.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
     def GetServiceInstance(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -659,31 +539,14 @@
         return grpc.experimental.unary_unary(request, target, '/prodvana.service.ServiceManager/GetServiceInstance',
             prodvana_dot_service_dot_service__manager__pb2.GetServiceInstanceReq.SerializeToString,
             prodvana_dot_service_dot_service__manager__pb2.GetServiceInstanceResp.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetServiceInstanceV2(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/prodvana.service.ServiceManager/GetServiceInstanceV2',
-            prodvana_dot_service_dot_service__manager__pb2.GetServiceInstanceReq.SerializeToString,
-            prodvana_dot_service_dot_service__manager__pb2.GetServiceInstanceResp.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
     def GetServiceMetrics(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -4,26 +4,25 @@
 """
 import abc
 import grpc
 import prodvana.proto.prodvana.service.service_manager_pb2
 
 class ServiceManagerStub:
     def __init__(self, channel: grpc.Channel) -> None: ...
-    ConfigureService2: grpc.UnaryUnaryMultiCallable[
-        prodvana.proto.prodvana.service.service_manager_pb2.ConfigureService2Req,
-        prodvana.proto.prodvana.service.service_manager_pb2.ConfigureService2Resp,
+    ConfigureService: grpc.UnaryUnaryMultiCallable[
+        prodvana.proto.prodvana.service.service_manager_pb2.ConfigureServiceReq,
+        prodvana.proto.prodvana.service.service_manager_pb2.ConfigureServiceResp,
     ]
-    """TODO(naphat) rename this to ConfigureService"""
     ListServiceConfigVersions: grpc.UnaryUnaryMultiCallable[
         prodvana.proto.prodvana.service.service_manager_pb2.ListServiceConfigVersionsReq,
         prodvana.proto.prodvana.service.service_manager_pb2.ListServiceConfigVersionsResp,
     ]
-    GetServiceConfig2: grpc.UnaryUnaryMultiCallable[
-        prodvana.proto.prodvana.service.service_manager_pb2.GetServiceConfig2Req,
-        prodvana.proto.prodvana.service.service_manager_pb2.GetServiceConfig2Resp,
+    GetServiceConfig: grpc.UnaryUnaryMultiCallable[
+        prodvana.proto.prodvana.service.service_manager_pb2.GetServiceConfigReq,
+        prodvana.proto.prodvana.service.service_manager_pb2.GetServiceConfigResp,
     ]
     """unparametrized configs"""
     ApplyParameters: grpc.UnaryUnaryMultiCallable[
         prodvana.proto.prodvana.service.service_manager_pb2.ApplyParametersReq,
         prodvana.proto.prodvana.service.service_manager_pb2.ApplyParametersResp,
     ]
     ValidateApplyParameters: grpc.UnaryUnaryMultiCallable[
@@ -42,50 +41,30 @@
         prodvana.proto.prodvana.service.service_manager_pb2.DeleteServiceReq,
         prodvana.proto.prodvana.service.service_manager_pb2.DeleteServiceResp,
     ]
     ListServices: grpc.UnaryUnaryMultiCallable[
         prodvana.proto.prodvana.service.service_manager_pb2.ListServicesReq,
         prodvana.proto.prodvana.service.service_manager_pb2.ListServicesResp,
     ]
-    ListServicesV2: grpc.UnaryUnaryMultiCallable[
-        prodvana.proto.prodvana.service.service_manager_pb2.ListServicesReq,
-        prodvana.proto.prodvana.service.service_manager_pb2.ListServicesResp,
-    ]
-    """identical to ListServices, kept around for compatibility purposes"""
     ListCommits: grpc.UnaryUnaryMultiCallable[
         prodvana.proto.prodvana.service.service_manager_pb2.ListCommitsReq,
         prodvana.proto.prodvana.service.service_manager_pb2.ListCommitsResp,
     ]
     GetService: grpc.UnaryUnaryMultiCallable[
         prodvana.proto.prodvana.service.service_manager_pb2.GetServiceReq,
         prodvana.proto.prodvana.service.service_manager_pb2.GetServiceResp,
     ]
-    GetServiceV2: grpc.UnaryUnaryMultiCallable[
-        prodvana.proto.prodvana.service.service_manager_pb2.GetServiceReq,
-        prodvana.proto.prodvana.service.service_manager_pb2.GetServiceResp,
-    ]
-    """identical to GetService, kept around for compatibility purposes"""
     ListServiceInstances: grpc.UnaryUnaryMultiCallable[
         prodvana.proto.prodvana.service.service_manager_pb2.ListServiceInstancesReq,
         prodvana.proto.prodvana.service.service_manager_pb2.ListServiceInstancesResp,
     ]
-    ListServiceInstancesV2: grpc.UnaryUnaryMultiCallable[
-        prodvana.proto.prodvana.service.service_manager_pb2.ListServiceInstancesReq,
-        prodvana.proto.prodvana.service.service_manager_pb2.ListServiceInstancesResp,
-    ]
-    """identical to ListServiceInstances, kept around for compatibility purposes"""
     GetServiceInstance: grpc.UnaryUnaryMultiCallable[
         prodvana.proto.prodvana.service.service_manager_pb2.GetServiceInstanceReq,
         prodvana.proto.prodvana.service.service_manager_pb2.GetServiceInstanceResp,
     ]
-    GetServiceInstanceV2: grpc.UnaryUnaryMultiCallable[
-        prodvana.proto.prodvana.service.service_manager_pb2.GetServiceInstanceReq,
-        prodvana.proto.prodvana.service.service_manager_pb2.GetServiceInstanceResp,
-    ]
-    """identical to GetServiceInstance, kept around for compatibility purposes"""
     GetServiceMetrics: grpc.UnaryUnaryMultiCallable[
         prodvana.proto.prodvana.service.service_manager_pb2.GetServiceMetricsReq,
         prodvana.proto.prodvana.service.service_manager_pb2.GetServiceMetricsResp,
     ]
     GetServiceInsights: grpc.UnaryUnaryMultiCallable[
         prodvana.proto.prodvana.service.service_manager_pb2.GetServiceInsightsReq,
         prodvana.proto.prodvana.service.service_manager_pb2.GetServiceInsightsResp,
@@ -101,32 +80,31 @@
     SetServiceMetadata: grpc.UnaryUnaryMultiCallable[
         prodvana.proto.prodvana.service.service_manager_pb2.SetServiceMetadataReq,
         prodvana.proto.prodvana.service.service_manager_pb2.SetServiceMetadataResp,
     ]
 
 class ServiceManagerServicer(metaclass=abc.ABCMeta):
     @abc.abstractmethod
-    def ConfigureService2(
+    def ConfigureService(
         self,
-        request: prodvana.proto.prodvana.service.service_manager_pb2.ConfigureService2Req,
+        request: prodvana.proto.prodvana.service.service_manager_pb2.ConfigureServiceReq,
         context: grpc.ServicerContext,
-    ) -> prodvana.proto.prodvana.service.service_manager_pb2.ConfigureService2Resp:
-        """TODO(naphat) rename this to ConfigureService"""
+    ) -> prodvana.proto.prodvana.service.service_manager_pb2.ConfigureServiceResp: ...
     @abc.abstractmethod
     def ListServiceConfigVersions(
         self,
         request: prodvana.proto.prodvana.service.service_manager_pb2.ListServiceConfigVersionsReq,
         context: grpc.ServicerContext,
     ) -> prodvana.proto.prodvana.service.service_manager_pb2.ListServiceConfigVersionsResp: ...
     @abc.abstractmethod
-    def GetServiceConfig2(
+    def GetServiceConfig(
         self,
-        request: prodvana.proto.prodvana.service.service_manager_pb2.GetServiceConfig2Req,
+        request: prodvana.proto.prodvana.service.service_manager_pb2.GetServiceConfigReq,
         context: grpc.ServicerContext,
-    ) -> prodvana.proto.prodvana.service.service_manager_pb2.GetServiceConfig2Resp:
+    ) -> prodvana.proto.prodvana.service.service_manager_pb2.GetServiceConfigResp:
         """unparametrized configs"""
     @abc.abstractmethod
     def ApplyParameters(
         self,
         request: prodvana.proto.prodvana.service.service_manager_pb2.ApplyParametersReq,
         context: grpc.ServicerContext,
     ) -> prodvana.proto.prodvana.service.service_manager_pb2.ApplyParametersResp: ...
@@ -157,66 +135,38 @@
     @abc.abstractmethod
     def ListServices(
         self,
         request: prodvana.proto.prodvana.service.service_manager_pb2.ListServicesReq,
         context: grpc.ServicerContext,
     ) -> prodvana.proto.prodvana.service.service_manager_pb2.ListServicesResp: ...
     @abc.abstractmethod
-    def ListServicesV2(
-        self,
-        request: prodvana.proto.prodvana.service.service_manager_pb2.ListServicesReq,
-        context: grpc.ServicerContext,
-    ) -> prodvana.proto.prodvana.service.service_manager_pb2.ListServicesResp:
-        """identical to ListServices, kept around for compatibility purposes"""
-    @abc.abstractmethod
     def ListCommits(
         self,
         request: prodvana.proto.prodvana.service.service_manager_pb2.ListCommitsReq,
         context: grpc.ServicerContext,
     ) -> prodvana.proto.prodvana.service.service_manager_pb2.ListCommitsResp: ...
     @abc.abstractmethod
     def GetService(
         self,
         request: prodvana.proto.prodvana.service.service_manager_pb2.GetServiceReq,
         context: grpc.ServicerContext,
     ) -> prodvana.proto.prodvana.service.service_manager_pb2.GetServiceResp: ...
     @abc.abstractmethod
-    def GetServiceV2(
-        self,
-        request: prodvana.proto.prodvana.service.service_manager_pb2.GetServiceReq,
-        context: grpc.ServicerContext,
-    ) -> prodvana.proto.prodvana.service.service_manager_pb2.GetServiceResp:
-        """identical to GetService, kept around for compatibility purposes"""
-    @abc.abstractmethod
     def ListServiceInstances(
         self,
         request: prodvana.proto.prodvana.service.service_manager_pb2.ListServiceInstancesReq,
         context: grpc.ServicerContext,
     ) -> prodvana.proto.prodvana.service.service_manager_pb2.ListServiceInstancesResp: ...
     @abc.abstractmethod
-    def ListServiceInstancesV2(
-        self,
-        request: prodvana.proto.prodvana.service.service_manager_pb2.ListServiceInstancesReq,
-        context: grpc.ServicerContext,
-    ) -> prodvana.proto.prodvana.service.service_manager_pb2.ListServiceInstancesResp:
-        """identical to ListServiceInstances, kept around for compatibility purposes"""
-    @abc.abstractmethod
     def GetServiceInstance(
         self,
         request: prodvana.proto.prodvana.service.service_manager_pb2.GetServiceInstanceReq,
         context: grpc.ServicerContext,
     ) -> prodvana.proto.prodvana.service.service_manager_pb2.GetServiceInstanceResp: ...
     @abc.abstractmethod
-    def GetServiceInstanceV2(
-        self,
-        request: prodvana.proto.prodvana.service.service_manager_pb2.GetServiceInstanceReq,
-        context: grpc.ServicerContext,
-    ) -> prodvana.proto.prodvana.service.service_manager_pb2.GetServiceInstanceResp:
-        """identical to GetServiceInstance, kept around for compatibility purposes"""
-    @abc.abstractmethod
     def GetServiceMetrics(
         self,
         request: prodvana.proto.prodvana.service.service_manager_pb2.GetServiceMetricsReq,
         context: grpc.ServicerContext,
     ) -> prodvana.proto.prodvana.service.service_manager_pb2.GetServiceMetricsResp: ...
     @abc.abstractmethod
     def GetServiceInsights(
```

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/service/user_metadata_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/service/user_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/service/user_metadata_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/service/user_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/settings/organization/users_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/settings/organization/users_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/settings/organization/users_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/settings/organization/users_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py` & `prodvana-0.1.4/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/stat/efficiency_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/stat/efficiency_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/stat/efficiency_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/stat/efficiency_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/template/service_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/template/service_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/template/service_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/template/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/users/users_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/users/users_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/users/users_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/users/users_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/version/source_metadata_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/version/source_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/version/source_metadata_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/version/source_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/volumes/volumes_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/volumes/volumes_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/volumes/volumes_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/volumes/volumes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/workflow/integration_config_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/workflow/integration_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py` & `prodvana-0.1.4/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py` & `prodvana-0.1.4/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi` & `prodvana-0.1.4/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/validate/validate_pb2.py` & `prodvana-0.1.4/prodvana/proto/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/proto/validate/validate_pb2.pyi` & `prodvana-0.1.4/prodvana/proto/validate/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/utils/desired_states.py` & `prodvana-0.1.4/prodvana/utils/desired_states.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.3/prodvana/utils/service_config.py` & `prodvana-0.1.4/prodvana/utils/service_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,27 +30,27 @@
     if summary.desired_state.HasField("service"):
         service = summary.desired_state.service
         for rc in service.release_channels:
             target_versions.add(
                 ServiceVersion(
                     application=service.application,
                     service=service.service,
-                    version=rc.versions[0].service_version,
+                    version=rc.versions[0].version,
                 )
             )
 
     if summary.desired_state.HasField("service_group"):
         service_group = summary.desired_state.service_group
         for service in service_group.services:
             for rc in service.release_channels:
                 target_versions.add(
                     ServiceVersion(
                         application=service.application,
                         service=service.service,
-                        version=rc.versions[0].service_version,
+                        version=rc.versions[0].version,
                     )
                 )
 
     images = set[ImageDetails]()
     for version in target_versions:
         this_images = get_images_from_service_version(
             client,
```

### Comparing `prodvana-0.1.3/prodvana/utils/tests/test_service_config.py` & `prodvana-0.1.4/prodvana/utils/tests/test_service_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         manager_pb2.DesiredStateSummary(
             desired_state=desired_state_pb2.State(
                 service=desired_state_pb2.ServiceState(
                     release_channels=[
                         desired_state_pb2.ServiceInstanceState(
                             versions=[
                                 desired_state_pb2.Version(
-                                    service_version="pvn-service-1",
+                                    version="pvn-service-1",
                                 ),
                             ],
                         ),
                     ],
                 ),
             ),
         ),
@@ -64,23 +64,23 @@
             desired_state=desired_state_pb2.State(
                 service=desired_state_pb2.ServiceState(
                     release_channels=[
                         desired_state_pb2.ServiceInstanceState(
                             release_channel="staging",
                             versions=[
                                 desired_state_pb2.Version(
-                                    service_version="pvn-service-2",
+                                    version="pvn-service-2",
                                 ),
                             ],
                         ),
                         desired_state_pb2.ServiceInstanceState(
                             release_channel="production",
                             versions=[
                                 desired_state_pb2.Version(
-                                    service_version="pvn-service-1",
+                                    version="pvn-service-1",
                                 ),
                             ],
                         ),
                     ],
                 ),
             ),
         ),
@@ -124,15 +124,15 @@
         manager_pb2.DesiredStateSummary(
             desired_state=desired_state_pb2.State(
                 service=desired_state_pb2.ServiceState(
                     release_channels=[
                         desired_state_pb2.ServiceInstanceState(
                             versions=[
                                 desired_state_pb2.Version(
-                                    service_version="pvn-service-1",
+                                    version="pvn-service-1",
                                 ),
                             ],
                         ),
                     ],
                 ),
             ),
         ),
@@ -156,23 +156,23 @@
             desired_state=desired_state_pb2.State(
                 service=desired_state_pb2.ServiceState(
                     release_channels=[
                         desired_state_pb2.ServiceInstanceState(
                             release_channel="staging",
                             versions=[
                                 desired_state_pb2.Version(
-                                    service_version="pvn-service-2",
+                                    version="pvn-service-2",
                                 ),
                             ],
                         ),
                         desired_state_pb2.ServiceInstanceState(
                             release_channel="production",
                             versions=[
                                 desired_state_pb2.Version(
-                                    service_version="pvn-service-1",
+                                    version="pvn-service-1",
                                 ),
                             ],
                         ),
                     ],
                 ),
             ),
         ),
```

### Comparing `prodvana-0.1.3/pyproject.toml` & `prodvana-0.1.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [tool.poetry]
 name = "prodvana"
-version = "0.1.3"
+version = "0.1.4"
 description = "Prodvana's client libraries"
 readme = "README.md"
 authors = []
 homepage = "https://prodvana.io"
 documentation = "https://docs.prodvana.io"
 repository = "https://github.com/prodvana/prodvana-public"
+exclude = ["examples"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 protobuf = ">=4.21.0,<5.0"
 types-protobuf = ">=3.20.0,<5.0"
 grpcio = ">=1.48.0,<2.0"
 grpc-stubs = ">=1.24.0,<2.0"
```

### Comparing `prodvana-0.1.3/PKG-INFO` & `prodvana-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodvana
-Version: 0.1.3
+Version: 0.1.4
 Summary: Prodvana's client libraries
 Home-page: https://prodvana.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: google-api-python-client (>=2.58.0,<3.0)
```

