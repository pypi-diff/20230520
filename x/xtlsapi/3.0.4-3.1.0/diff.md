# Comparing `tmp/xtlsapi-3.0.4.tar.gz` & `tmp/xtlsapi-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtlsapi-3.0.4.tar", last modified: Thu May 18 16:05:30 2023, max compression
+gzip compressed data, was "xtlsapi-3.1.0.tar", last modified: Sat May 20 07:10:33 2023, max compression
```

## Comparing `xtlsapi-3.0.4.tar` & `xtlsapi-3.1.0.tar`

### file list

```diff
@@ -1,350 +1,354 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.782398 xtlsapi-3.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-18 16:05:30.782398 xtlsapi-3.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 16:05:30.782398 xtlsapi-3.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.762398 xtlsapi-3.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/tests/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.762398 xtlsapi-3.0.4/xtlsapi/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.762398 xtlsapi-3.0.4/xtlsapi/api_services/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/api_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/api_services/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.762398 xtlsapi-3.0.4/xtlsapi/api_services/handler/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/api_services/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/api_services/handler/add_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/api_services/handler/remove_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.762398 xtlsapi-3.0.4/xtlsapi/api_services/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/api_services/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/api_services/logger/restart_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.766398 xtlsapi-3.0.4/xtlsapi/api_services/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/api_services/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/api_services/stats/get_client_download_traffic.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/api_services/stats/get_client_upload_traffic.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/api_services/stats/get_inbound_download_traffic.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/api_services/stats/get_inbound_upload_traffic.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/api_services/stats/get_statsquery.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/api_services/stats/get_total_download_traffic.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/api_services/stats/get_total_upload_traffic.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.766398 xtlsapi-3.0.4/xtlsapi/client/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/client/SingboxClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/client/XrayClient.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.766398 xtlsapi-3.0.4/xtlsapi/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/exceptions/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/exceptions/email_already_exists.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/exceptions/email_not_found.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/exceptions/inbound_not_found.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.766398 xtlsapi-3.0.4/xtlsapi/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/ext/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/generate_from_xray_proto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.766398 xtlsapi-3.0.4/xtlsapi/singbox_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/singbox_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/singbox_api/build.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/singbox_api/stats.proto
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/singbox_api/stats_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/singbox_api/stats_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.770398 xtlsapi-3.0.4/xtlsapi/singbox_api_services/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/singbox_api_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/singbox_api_services/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.770398 xtlsapi-3.0.4/xtlsapi/singbox_api_services/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/singbox_api_services/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/singbox_api_services/stats/get_client_download_traffic.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/singbox_api_services/stats/get_client_upload_traffic.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/singbox_api_services/stats/get_inbound_download_traffic.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/singbox_api_services/stats/get_inbound_upload_traffic.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/singbox_api_services/stats/get_statsquery.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/singbox_api_services/stats/get_total_download_traffic.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/singbox_api_services/stats/get_total_upload_traffic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.770398 xtlsapi-3.0.4/xtlsapi/xray_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/a.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.770398 xtlsapi-3.0.4/xtlsapi/xray_api/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.770398 xtlsapi-3.0.4/xtlsapi/xray_api/app/commander/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/commander/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/commander/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/commander/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.770398 xtlsapi-3.0.4/xtlsapi/xray_api/app/dispatcher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/dispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/dispatcher/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/dispatcher/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.770398 xtlsapi-3.0.4/xtlsapi/xray_api/app/dns/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/dns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/dns/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/dns/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.770398 xtlsapi-3.0.4/xtlsapi/xray_api/app/dns/fakedns/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/dns/fakedns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/dns/fakedns/fakedns_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/dns/fakedns/fakedns_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.770398 xtlsapi-3.0.4/xtlsapi/xray_api/app/log/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/log/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.770398 xtlsapi-3.0.4/xtlsapi/xray_api/app/log/command/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/log/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/log/command/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/log/command/config_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/log/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/log/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.770398 xtlsapi-3.0.4/xtlsapi/xray_api/app/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/metrics/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/metrics/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.770398 xtlsapi-3.0.4/xtlsapi/xray_api/app/observatory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/observatory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.770398 xtlsapi-3.0.4/xtlsapi/xray_api/app/observatory/command/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/observatory/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/observatory/command/command_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/observatory/command/command_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/observatory/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/observatory/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.770398 xtlsapi-3.0.4/xtlsapi/xray_api/app/policy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/policy/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/policy/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.770398 xtlsapi-3.0.4/xtlsapi/xray_api/app/proxyman/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/proxyman/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.770398 xtlsapi-3.0.4/xtlsapi/xray_api/app/proxyman/command/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/proxyman/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/proxyman/command/command_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/proxyman/command/command_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/proxyman/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/proxyman/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.770398 xtlsapi-3.0.4/xtlsapi/xray_api/app/reverse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/reverse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/reverse/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/reverse/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.770398 xtlsapi-3.0.4/xtlsapi/xray_api/app/router/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/router/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.774398 xtlsapi-3.0.4/xtlsapi/xray_api/app/router/command/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/router/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/router/command/command_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/router/command/command_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/router/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/router/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.774398 xtlsapi-3.0.4/xtlsapi/xray_api/app/stats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/stats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.774398 xtlsapi-3.0.4/xtlsapi/xray_api/app/stats/command/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/stats/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/stats/command/command_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/stats/command/command_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/stats/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/app/stats/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.774398 xtlsapi-3.0.4/xtlsapi/xray_api/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.774398 xtlsapi-3.0.4/xtlsapi/xray_api/common/log/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/common/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/common/log/log_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/common/log/log_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.774398 xtlsapi-3.0.4/xtlsapi/xray_api/common/net/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/common/net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/common/net/address_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/common/net/address_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/common/net/destination_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/common/net/destination_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/common/net/network_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/common/net/network_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/common/net/port_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/common/net/port_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.774398 xtlsapi-3.0.4/xtlsapi/xray_api/common/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/common/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/common/protocol/headers_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/common/protocol/headers_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/common/protocol/server_spec_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/common/protocol/server_spec_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/common/protocol/user_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/common/protocol/user_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.774398 xtlsapi-3.0.4/xtlsapi/xray_api/common/serial/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/common/serial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/common/serial/typed_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/common/serial/typed_message_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.774398 xtlsapi-3.0.4/xtlsapi/xray_api/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/core/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/core/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.774398 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.774398 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/blackhole/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/blackhole/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/blackhole/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/blackhole/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.774398 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/dns/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/dns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/dns/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/dns/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.774398 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/dokodemo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/dokodemo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/dokodemo/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/dokodemo/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.774398 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/freedom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/freedom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/freedom/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/freedom/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.774398 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/http/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/http/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.774398 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/loopback/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/loopback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/loopback/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/loopback/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.778398 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/mtproto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/mtproto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/mtproto/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/mtproto/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.778398 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/shadowsocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/shadowsocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/shadowsocks/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/shadowsocks/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.778398 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/shadowsocks_2022/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/shadowsocks_2022/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/shadowsocks_2022/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/shadowsocks_2022/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.778398 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/socks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/socks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/socks/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/socks/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.778398 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/trojan/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/trojan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/trojan/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/trojan/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.778398 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vless/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vless/account_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vless/account_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.778398 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vless/encoding/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vless/encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vless/encoding/addons_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vless/encoding/addons_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.778398 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vless/inbound/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vless/inbound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vless/inbound/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vless/inbound/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.778398 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vless/outbound/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vless/outbound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vless/outbound/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vless/outbound/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.778398 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vmess/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vmess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vmess/account_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vmess/account_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.778398 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vmess/inbound/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vmess/inbound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vmess/inbound/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vmess/inbound/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.778398 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vmess/outbound/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vmess/outbound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vmess/outbound/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vmess/outbound/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.778398 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/wireguard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/wireguard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/wireguard/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/proxy/wireguard/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.778398 xtlsapi-3.0.4/xtlsapi/xray_api/transport/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.778398 xtlsapi-3.0.4/xtlsapi/xray_api/transport/global/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/global/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/global/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/global/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.778398 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.778398 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/domainsocket/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/domainsocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/domainsocket/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/domainsocket/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.778398 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/grpc/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/grpc/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.778398 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/grpc/encoding/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/grpc/encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/grpc/encoding/stream_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/grpc/encoding/stream_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.778398 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.778398 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/dns/
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/dns/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/dns/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.782398 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/http/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/http/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.782398 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/noop/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/noop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/noop/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/noop/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.782398 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/srtp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/srtp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/srtp/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/srtp/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.782398 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/tls/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/tls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/tls/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/tls/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.782398 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/utp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/utp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/utp/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/utp/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.782398 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/wechat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/wechat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/wechat/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/wechat/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.782398 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/wireguard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/wireguard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/wireguard/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/wireguard/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.782398 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/http/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/http/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.782398 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/kcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/kcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/kcp/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/kcp/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.782398 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/quic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/quic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/quic/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/quic/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.782398 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/reality/
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/reality/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/reality/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.782398 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/tcp/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/tcp/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.782398 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/tls/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/tls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/tls/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/tls/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.782398 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/udp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/udp/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/udp/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.782398 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/websocket/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/websocket/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.782398 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/xtls/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/xtls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/xtls/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 16:05:20.000000 xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/xtls/config_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:05:30.762398 xtlsapi-3.0.4/xtlsapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-18 16:05:30.000000 xtlsapi-3.0.4/xtlsapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-05-18 16:05:30.000000 xtlsapi-3.0.4/xtlsapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 16:05:30.000000 xtlsapi-3.0.4/xtlsapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-18 16:05:30.000000 xtlsapi-3.0.4/xtlsapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-18 16:05:30.000000 xtlsapi-3.0.4/xtlsapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-18 16:05:30.000000 xtlsapi-3.0.4/xtlsapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.109360 xtlsapi-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-20 07:10:33.109360 xtlsapi-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 07:10:33.113360 xtlsapi-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.053359 xtlsapi-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.057360 xtlsapi-3.1.0/xtlsapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.057360 xtlsapi-3.1.0/xtlsapi/api_services/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/api_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/api_services/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.057360 xtlsapi-3.1.0/xtlsapi/api_services/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/api_services/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/api_services/handler/add_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/api_services/handler/remove_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.057360 xtlsapi-3.1.0/xtlsapi/api_services/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/api_services/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/api_services/logger/restart_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.061360 xtlsapi-3.1.0/xtlsapi/api_services/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/api_services/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/api_services/stats/get_client_download_traffic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/api_services/stats/get_client_upload_traffic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/api_services/stats/get_inbound_download_traffic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/api_services/stats/get_inbound_upload_traffic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/api_services/stats/get_statsquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/api_services/stats/get_total_download_traffic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/api_services/stats/get_total_upload_traffic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.061360 xtlsapi-3.1.0/xtlsapi/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/client/SingboxClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/client/XrayClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.061360 xtlsapi-3.1.0/xtlsapi/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/exceptions/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/exceptions/email_already_exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/exceptions/email_not_found.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/exceptions/inbound_not_found.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.061360 xtlsapi-3.1.0/xtlsapi/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/ext/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/generate_from_xray_proto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.065359 xtlsapi-3.1.0/xtlsapi/singbox_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/singbox_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/singbox_api/build.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/singbox_api/extensions.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/singbox_api/extensions_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/singbox_api/extensions_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/singbox_api/stats.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/singbox_api/stats_old.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/singbox_api/stats_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/singbox_api/stats_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.065359 xtlsapi-3.1.0/xtlsapi/singbox_api_services/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/singbox_api_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/singbox_api_services/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.065359 xtlsapi-3.1.0/xtlsapi/singbox_api_services/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/singbox_api_services/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/singbox_api_services/stats/get_client_download_traffic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/singbox_api_services/stats/get_client_upload_traffic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/singbox_api_services/stats/get_inbound_download_traffic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/singbox_api_services/stats/get_inbound_upload_traffic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/singbox_api_services/stats/get_statsquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/singbox_api_services/stats/get_total_download_traffic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/singbox_api_services/stats/get_total_upload_traffic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.065359 xtlsapi-3.1.0/xtlsapi/xray_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/a.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.065359 xtlsapi-3.1.0/xtlsapi/xray_api/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.069360 xtlsapi-3.1.0/xtlsapi/xray_api/app/commander/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/commander/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/commander/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/commander/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.069360 xtlsapi-3.1.0/xtlsapi/xray_api/app/dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/dispatcher/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/dispatcher/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.069360 xtlsapi-3.1.0/xtlsapi/xray_api/app/dns/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/dns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/dns/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/dns/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.069360 xtlsapi-3.1.0/xtlsapi/xray_api/app/dns/fakedns/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/dns/fakedns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/dns/fakedns/fakedns_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/dns/fakedns/fakedns_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.069360 xtlsapi-3.1.0/xtlsapi/xray_api/app/log/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/log/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.069360 xtlsapi-3.1.0/xtlsapi/xray_api/app/log/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/log/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/log/command/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/log/command/config_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/log/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/log/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.073360 xtlsapi-3.1.0/xtlsapi/xray_api/app/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/metrics/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/metrics/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.073360 xtlsapi-3.1.0/xtlsapi/xray_api/app/observatory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/observatory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.073360 xtlsapi-3.1.0/xtlsapi/xray_api/app/observatory/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/observatory/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/observatory/command/command_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/observatory/command/command_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/observatory/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/observatory/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.073360 xtlsapi-3.1.0/xtlsapi/xray_api/app/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/policy/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/policy/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.073360 xtlsapi-3.1.0/xtlsapi/xray_api/app/proxyman/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/proxyman/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.073360 xtlsapi-3.1.0/xtlsapi/xray_api/app/proxyman/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/proxyman/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/proxyman/command/command_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/proxyman/command/command_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/proxyman/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/proxyman/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.077360 xtlsapi-3.1.0/xtlsapi/xray_api/app/reverse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/reverse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/reverse/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/reverse/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.077360 xtlsapi-3.1.0/xtlsapi/xray_api/app/router/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/router/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.077360 xtlsapi-3.1.0/xtlsapi/xray_api/app/router/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/router/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/router/command/command_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/router/command/command_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/router/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/router/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.077360 xtlsapi-3.1.0/xtlsapi/xray_api/app/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/stats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.077360 xtlsapi-3.1.0/xtlsapi/xray_api/app/stats/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/stats/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/stats/command/command_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/stats/command/command_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/stats/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/app/stats/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.077360 xtlsapi-3.1.0/xtlsapi/xray_api/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.077360 xtlsapi-3.1.0/xtlsapi/xray_api/common/log/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/common/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/common/log/log_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/common/log/log_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.081360 xtlsapi-3.1.0/xtlsapi/xray_api/common/net/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/common/net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/common/net/address_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/common/net/address_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/common/net/destination_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/common/net/destination_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/common/net/network_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/common/net/network_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/common/net/port_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/common/net/port_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.081360 xtlsapi-3.1.0/xtlsapi/xray_api/common/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/common/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/common/protocol/headers_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/common/protocol/headers_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/common/protocol/server_spec_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/common/protocol/server_spec_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/common/protocol/user_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/common/protocol/user_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.081360 xtlsapi-3.1.0/xtlsapi/xray_api/common/serial/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/common/serial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/common/serial/typed_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/common/serial/typed_message_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.085360 xtlsapi-3.1.0/xtlsapi/xray_api/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/core/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/core/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.085360 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.085360 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/blackhole/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/blackhole/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/blackhole/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/blackhole/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.085360 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/dns/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/dns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/dns/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/dns/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.085360 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/dokodemo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/dokodemo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/dokodemo/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/dokodemo/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.085360 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/freedom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/freedom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/freedom/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/freedom/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.085360 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/http/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/http/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.089360 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/loopback/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/loopback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/loopback/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/loopback/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.089360 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/mtproto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/mtproto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/mtproto/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/mtproto/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.089360 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/shadowsocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/shadowsocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/shadowsocks/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/shadowsocks/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.089360 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/shadowsocks_2022/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/shadowsocks_2022/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/shadowsocks_2022/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/shadowsocks_2022/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.089360 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/socks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/socks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/socks/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/socks/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.089360 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/trojan/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/trojan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/trojan/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/trojan/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.093360 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vless/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vless/account_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vless/account_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.093360 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vless/encoding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vless/encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vless/encoding/addons_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vless/encoding/addons_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.093360 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vless/inbound/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vless/inbound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vless/inbound/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vless/inbound/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.093360 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vless/outbound/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vless/outbound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vless/outbound/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vless/outbound/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.093360 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vmess/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vmess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vmess/account_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vmess/account_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.093360 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vmess/inbound/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vmess/inbound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vmess/inbound/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vmess/inbound/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.093360 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vmess/outbound/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vmess/outbound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vmess/outbound/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vmess/outbound/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.097360 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/wireguard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/wireguard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/wireguard/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/proxy/wireguard/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.097360 xtlsapi-3.1.0/xtlsapi/xray_api/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.097360 xtlsapi-3.1.0/xtlsapi/xray_api/transport/global/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/global/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/global/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/global/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.097360 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.097360 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/domainsocket/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/domainsocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/domainsocket/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/domainsocket/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.097360 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/grpc/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/grpc/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.101360 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/grpc/encoding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/grpc/encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/grpc/encoding/stream_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/grpc/encoding/stream_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.101360 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.101360 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/dns/
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/dns/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/dns/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.101360 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/http/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/http/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.101360 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/noop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/noop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/noop/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/noop/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.101360 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/srtp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/srtp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/srtp/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/srtp/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.101360 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/tls/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/tls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/tls/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/tls/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.105360 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/utp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/utp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/utp/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/utp/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.105360 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/wechat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/wechat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/wechat/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/wechat/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.105360 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/wireguard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/wireguard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/wireguard/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/wireguard/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.105360 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/http/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/http/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.105360 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/kcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/kcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/kcp/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/kcp/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.105360 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/quic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/quic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/quic/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/quic/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.109360 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/reality/
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/reality/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/reality/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.109360 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/tcp/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/tcp/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.109360 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/tls/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/tls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/tls/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/tls/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.109360 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/udp/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/udp/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.109360 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/websocket/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/websocket/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.109360 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/xtls/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/xtls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/xtls/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 07:10:20.000000 xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/xtls/config_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:10:33.057360 xtlsapi-3.1.0/xtlsapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-20 07:10:32.000000 xtlsapi-3.1.0/xtlsapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-05-20 07:10:33.000000 xtlsapi-3.1.0/xtlsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 07:10:32.000000 xtlsapi-3.1.0/xtlsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-20 07:10:32.000000 xtlsapi-3.1.0/xtlsapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-20 07:10:32.000000 xtlsapi-3.1.0/xtlsapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-20 07:10:32.000000 xtlsapi-3.1.0/xtlsapi.egg-info/top_level.txt
```

### Comparing `xtlsapi-3.0.4/HISTORY.md` & `xtlsapi-3.1.0/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
 
+Fix
+~~~
+- Singbox. [hiddify]
+
+
+3.0.4 (2023-05-18)
+------------------
+
 New
 ~~~
 - Add reset to statsquery. [hiddify]
 
 Fix
 ~~~
 - Bug. [hiddify]
 
+Other
+~~~~~
+- Release: version 3.0.4 🚀 [hiddify]
+
 
 3.0.3 (2023-05-18)
 ------------------
 
 Fix
 ~~~
 - Typo. [hiddify]
```

### Comparing `xtlsapi-3.0.4/LICENSE` & `xtlsapi-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/PKG-INFO` & `xtlsapi-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtlsapi
-Version: 3.0.4
+Version: 3.1.0
 Summary: Awesome xtlsapi created by hiddify
 Home-page: https://github.com/hiddify/xtlsapi/
 Author: hiddify
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `xtlsapi-3.0.4/README.md` & `xtlsapi-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/setup.py` & `xtlsapi-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/api_services/_base.py` & `xtlsapi-3.1.0/xtlsapi/api_services/_base.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/api_services/handler/add_client.py` & `xtlsapi-3.1.0/xtlsapi/api_services/handler/add_client.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/api_services/handler/remove_client.py` & `xtlsapi-3.1.0/xtlsapi/api_services/handler/remove_client.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/api_services/stats/__init__.py` & `xtlsapi-3.1.0/xtlsapi/api_services/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/api_services/stats/get_total_download_traffic.py` & `xtlsapi-3.1.0/xtlsapi/api_services/stats/get_total_download_traffic.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/api_services/stats/get_total_upload_traffic.py` & `xtlsapi-3.1.0/xtlsapi/api_services/stats/get_total_upload_traffic.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/cli.py` & `xtlsapi-3.1.0/xtlsapi/cli.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/ext/utils.py` & `xtlsapi-3.1.0/xtlsapi/ext/utils.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/generate_from_xray_proto.py` & `xtlsapi-3.1.0/xtlsapi/generate_from_xray_proto.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/singbox_api/stats.proto` & `xtlsapi-3.1.0/xtlsapi/singbox_api/stats_old.proto`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/singbox_api/stats_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/reality/config_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,27 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: stats.proto
+# source: transport/internet/reality/config.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0bstats.proto\x12\x15\x65xperimental.v2rayapi\".\n\x0fGetStatsRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05reset\x18\x02 \x01(\x08\"#\n\x04Stat\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x03\"=\n\x10GetStatsResponse\x12)\n\x04stat\x18\x01 \x01(\x0b\x32\x1b.experimental.v2rayapi.Stat\"U\n\x11QueryStatsRequest\x12\x0f\n\x07pattern\x18\x01 \x01(\t\x12\r\n\x05reset\x18\x02 \x01(\x08\x12\x10\n\x08patterns\x18\x03 \x03(\t\x12\x0e\n\x06regexp\x18\x04 \x01(\x08\"?\n\x12QueryStatsResponse\x12)\n\x04stat\x18\x01 \x03(\x0b\x32\x1b.experimental.v2rayapi.Stat\"\x11\n\x0fSysStatsRequest\"\xc2\x01\n\x10SysStatsResponse\x12\x14\n\x0cNumGoroutine\x18\x01 \x01(\r\x12\r\n\x05NumGC\x18\x02 \x01(\r\x12\r\n\x05\x41lloc\x18\x03 \x01(\x04\x12\x12\n\nTotalAlloc\x18\x04 \x01(\x04\x12\x0b\n\x03Sys\x18\x05 \x01(\x04\x12\x0f\n\x07Mallocs\x18\x06 \x01(\x04\x12\r\n\x05\x46rees\x18\x07 \x01(\x04\x12\x13\n\x0bLiveObjects\x18\x08 \x01(\x04\x12\x14\n\x0cPauseTotalNs\x18\t \x01(\x04\x12\x0e\n\x06Uptime\x18\n \x01(\r2\xb4\x02\n\x0cStatsService\x12]\n\x08GetStats\x12&.experimental.v2rayapi.GetStatsRequest\x1a\'.experimental.v2rayapi.GetStatsResponse\"\x00\x12\x63\n\nQueryStats\x12(.experimental.v2rayapi.QueryStatsRequest\x1a).experimental.v2rayapi.QueryStatsResponse\"\x00\x12`\n\x0bGetSysStats\x12&.experimental.v2rayapi.SysStatsRequest\x1a\'.experimental.v2rayapi.SysStatsResponse\"\x00\x42\x34Z2github.com/sagernet/sing-box/experimental/v2rayapib\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'transport/internet/reality/config.proto\x12\x1fxray.transport.internet.reality\"\xb9\x02\n\x06\x43onfig\x12\x0c\n\x04show\x18\x01 \x01(\x08\x12\x0c\n\x04\x64\x65st\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x0c\n\x04xver\x18\x04 \x01(\x04\x12\x14\n\x0cserver_names\x18\x05 \x03(\t\x12\x13\n\x0bprivate_key\x18\x06 \x01(\x0c\x12\x16\n\x0emin_client_ver\x18\x07 \x01(\x0c\x12\x16\n\x0emax_client_ver\x18\x08 \x01(\x0c\x12\x15\n\rmax_time_diff\x18\t \x01(\x04\x12\x11\n\tshort_ids\x18\n \x03(\x0c\x12\x13\n\x0b\x46ingerprint\x18\x15 \x01(\t\x12\x13\n\x0bserver_name\x18\x16 \x01(\t\x12\x12\n\npublic_key\x18\x17 \x01(\x0c\x12\x10\n\x08short_id\x18\x18 \x01(\x0c\x12\x10\n\x08spider_x\x18\x19 \x01(\t\x12\x10\n\x08spider_y\x18\x1a \x03(\x03\x42\x7f\n#com.xray.transport.internet.realityP\x01Z4github.com/xtls/xray-core/transport/internet/reality\xaa\x02\x1fXray.Transport.Internet.Realityb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'stats_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'transport.internet.reality.config_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z2github.com/sagernet/sing-box/experimental/v2rayapi'
-  _GETSTATSREQUEST._serialized_start=38
-  _GETSTATSREQUEST._serialized_end=84
-  _STAT._serialized_start=86
-  _STAT._serialized_end=121
-  _GETSTATSRESPONSE._serialized_start=123
-  _GETSTATSRESPONSE._serialized_end=184
-  _QUERYSTATSREQUEST._serialized_start=186
-  _QUERYSTATSREQUEST._serialized_end=271
-  _QUERYSTATSRESPONSE._serialized_start=273
-  _QUERYSTATSRESPONSE._serialized_end=336
-  _SYSSTATSREQUEST._serialized_start=338
-  _SYSSTATSREQUEST._serialized_end=355
-  _SYSSTATSRESPONSE._serialized_start=358
-  _SYSSTATSRESPONSE._serialized_end=552
-  _STATSSERVICE._serialized_start=555
-  _STATSSERVICE._serialized_end=863
+  DESCRIPTOR._serialized_options = b'\n#com.xray.transport.internet.realityP\001Z4github.com/xtls/xray-core/transport/internet/reality\252\002\037Xray.Transport.Internet.Reality'
+  _globals['_CONFIG']._serialized_start=77
+  _globals['_CONFIG']._serialized_end=390
 # @@protoc_insertion_point(module_scope)
```

### Comparing `xtlsapi-3.0.4/xtlsapi/singbox_api/stats_pb2_grpc.py` & `xtlsapi-3.1.0/xtlsapi/singbox_api/stats_pb2_grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from . import stats_pb2 as stats__pb2
+import stats_pb2 as stats__pb2
 
 
 class StatsServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.GetStats = channel.unary_unary(
-                '/experimental.v2rayapi.StatsService/GetStats',
+                '/v2ray.core.app.stats.command.StatsService/GetStats',
                 request_serializer=stats__pb2.GetStatsRequest.SerializeToString,
                 response_deserializer=stats__pb2.GetStatsResponse.FromString,
                 )
         self.QueryStats = channel.unary_unary(
-                '/experimental.v2rayapi.StatsService/QueryStats',
+                '/v2ray.core.app.stats.command.StatsService/QueryStats',
                 request_serializer=stats__pb2.QueryStatsRequest.SerializeToString,
                 response_deserializer=stats__pb2.QueryStatsResponse.FromString,
                 )
         self.GetSysStats = channel.unary_unary(
-                '/experimental.v2rayapi.StatsService/GetSysStats',
+                '/v2ray.core.app.stats.command.StatsService/GetSysStats',
                 request_serializer=stats__pb2.SysStatsRequest.SerializeToString,
                 response_deserializer=stats__pb2.SysStatsResponse.FromString,
                 )
 
 
 class StatsServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
@@ -68,15 +68,15 @@
             'GetSysStats': grpc.unary_unary_rpc_method_handler(
                     servicer.GetSysStats,
                     request_deserializer=stats__pb2.SysStatsRequest.FromString,
                     response_serializer=stats__pb2.SysStatsResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'experimental.v2rayapi.StatsService', rpc_method_handlers)
+            'v2ray.core.app.stats.command.StatsService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class StatsService(object):
     """Missing associated documentation comment in .proto file."""
 
@@ -87,15 +87,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/experimental.v2rayapi.StatsService/GetStats',
+        return grpc.experimental.unary_unary(request, target, '/v2ray.core.app.stats.command.StatsService/GetStats',
             stats__pb2.GetStatsRequest.SerializeToString,
             stats__pb2.GetStatsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def QueryStats(request,
@@ -104,15 +104,15 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/experimental.v2rayapi.StatsService/QueryStats',
+        return grpc.experimental.unary_unary(request, target, '/v2ray.core.app.stats.command.StatsService/QueryStats',
             stats__pb2.QueryStatsRequest.SerializeToString,
             stats__pb2.QueryStatsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def GetSysStats(request,
@@ -121,12 +121,12 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/experimental.v2rayapi.StatsService/GetSysStats',
+        return grpc.experimental.unary_unary(request, target, '/v2ray.core.app.stats.command.StatsService/GetSysStats',
             stats__pb2.SysStatsRequest.SerializeToString,
             stats__pb2.SysStatsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `xtlsapi-3.0.4/xtlsapi/singbox_api_services/stats/__init__.py` & `xtlsapi-3.1.0/xtlsapi/singbox_api_services/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/singbox_api_services/stats/get_total_download_traffic.py` & `xtlsapi-3.1.0/xtlsapi/singbox_api_services/stats/get_total_download_traffic.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/app/commander/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/app/commander/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/app/dispatcher/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/app/dispatcher/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/app/dns/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/app/dns/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/app/dns/fakedns/fakedns_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/app/dns/fakedns/fakedns_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/app/log/command/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/app/log/command/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/app/log/command/config_pb2_grpc.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/app/log/command/config_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/app/log/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/app/log/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/app/metrics/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/app/metrics/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/app/observatory/command/command_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/app/observatory/command/command_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/app/observatory/command/command_pb2_grpc.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/app/observatory/command/command_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/app/observatory/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/app/observatory/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/app/policy/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/app/policy/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/app/proxyman/command/command_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/app/proxyman/command/command_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/app/proxyman/command/command_pb2_grpc.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/app/proxyman/command/command_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/app/proxyman/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/app/proxyman/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/app/reverse/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/app/reverse/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/app/router/command/command_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/app/router/command/command_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/app/router/command/command_pb2_grpc.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/app/router/command/command_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/app/router/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/app/router/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/app/stats/command/command_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/app/stats/command/command_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/app/stats/command/command_pb2_grpc.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/app/stats/command/command_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/app/stats/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/app/stats/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/common/log/log_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/common/log/log_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/common/net/address_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/common/net/address_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/common/net/destination_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/common/net/destination_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/common/net/network_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/common/net/network_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/common/net/port_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/common/net/port_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/common/protocol/headers_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/common/protocol/headers_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/common/protocol/server_spec_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/common/protocol/server_spec_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/common/protocol/user_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/common/protocol/user_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/common/serial/typed_message_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/common/serial/typed_message_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/core/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/core/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/proxy/blackhole/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/proxy/blackhole/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/proxy/dns/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/proxy/dns/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/proxy/dokodemo/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/proxy/dokodemo/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/proxy/freedom/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/proxy/freedom/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/proxy/http/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/proxy/http/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/proxy/loopback/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/proxy/loopback/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/proxy/mtproto/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/proxy/mtproto/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/proxy/shadowsocks/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/proxy/shadowsocks/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/proxy/shadowsocks_2022/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/proxy/shadowsocks_2022/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/proxy/socks/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/proxy/socks/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/proxy/trojan/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/proxy/trojan/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vless/account_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vless/account_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vless/encoding/addons_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vless/encoding/addons_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vless/inbound/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vless/inbound/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vless/outbound/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vless/outbound/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vmess/account_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vmess/account_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vmess/inbound/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vmess/inbound/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/proxy/vmess/outbound/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/proxy/vmess/outbound/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/proxy/wireguard/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/proxy/wireguard/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/transport/global/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/transport/global/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/domainsocket/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/domainsocket/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/grpc/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/grpc/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/grpc/encoding/stream_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/grpc/encoding/stream_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/grpc/encoding/stream_pb2_grpc.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/grpc/encoding/stream_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/dns/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/dns/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/http/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/http/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/noop/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/noop/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/srtp/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/srtp/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/tls/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/tls/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/utp/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/utp/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/wechat/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/wechat/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/headers/wireguard/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/headers/wireguard/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/http/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/http/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/kcp/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/kcp/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/quic/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/quic/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/reality/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/websocket/config_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: transport/internet/reality/config.proto
+# source: transport/internet/websocket/config.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'transport/internet/reality/config.proto\x12\x1fxray.transport.internet.reality\"\xb9\x02\n\x06\x43onfig\x12\x0c\n\x04show\x18\x01 \x01(\x08\x12\x0c\n\x04\x64\x65st\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x0c\n\x04xver\x18\x04 \x01(\x04\x12\x14\n\x0cserver_names\x18\x05 \x03(\t\x12\x13\n\x0bprivate_key\x18\x06 \x01(\x0c\x12\x16\n\x0emin_client_ver\x18\x07 \x01(\x0c\x12\x16\n\x0emax_client_ver\x18\x08 \x01(\x0c\x12\x15\n\rmax_time_diff\x18\t \x01(\x04\x12\x11\n\tshort_ids\x18\n \x03(\x0c\x12\x13\n\x0b\x46ingerprint\x18\x15 \x01(\t\x12\x13\n\x0bserver_name\x18\x16 \x01(\t\x12\x12\n\npublic_key\x18\x17 \x01(\x0c\x12\x10\n\x08short_id\x18\x18 \x01(\x0c\x12\x10\n\x08spider_x\x18\x19 \x01(\t\x12\x10\n\x08spider_y\x18\x1a \x03(\x03\x42\x7f\n#com.xray.transport.internet.realityP\x01Z4github.com/xtls/xray-core/transport/internet/reality\xaa\x02\x1fXray.Transport.Internet.Realityb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)transport/internet/websocket/config.proto\x12!xray.transport.internet.websocket\"$\n\x06Header\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\x82\x01\n\x06\x43onfig\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x39\n\x06header\x18\x03 \x03(\x0b\x32).xray.transport.internet.websocket.Header\x12\x1d\n\x15\x61\x63\x63\x65pt_proxy_protocol\x18\x04 \x01(\x08\x12\n\n\x02\x65\x64\x18\x05 \x01(\rJ\x04\x08\x01\x10\x02\x42\x85\x01\n%com.xray.transport.internet.websocketP\x01Z6github.com/xtls/xray-core/transport/internet/websocket\xaa\x02!Xray.Transport.Internet.Websocketb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'transport.internet.reality.config_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'transport.internet.websocket.config_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n#com.xray.transport.internet.realityP\001Z4github.com/xtls/xray-core/transport/internet/reality\252\002\037Xray.Transport.Internet.Reality'
-  _globals['_CONFIG']._serialized_start=77
-  _globals['_CONFIG']._serialized_end=390
+  DESCRIPTOR._serialized_options = b'\n%com.xray.transport.internet.websocketP\001Z6github.com/xtls/xray-core/transport/internet/websocket\252\002!Xray.Transport.Internet.Websocket'
+  _globals['_HEADER']._serialized_start=80
+  _globals['_HEADER']._serialized_end=116
+  _globals['_CONFIG']._serialized_start=119
+  _globals['_CONFIG']._serialized_end=249
 # @@protoc_insertion_point(module_scope)
```

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/tcp/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/tcp/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/tls/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/tls/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/udp/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/udp/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/websocket/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/singbox_api/extensions_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: transport/internet/websocket/config.proto
+# source: extensions.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)transport/internet/websocket/config.proto\x12!xray.transport.internet.websocket\"$\n\x06Header\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\x82\x01\n\x06\x43onfig\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x39\n\x06header\x18\x03 \x03(\x0b\x32).xray.transport.internet.websocket.Header\x12\x1d\n\x15\x61\x63\x63\x65pt_proxy_protocol\x18\x04 \x01(\x08\x12\n\n\x02\x65\x64\x18\x05 \x01(\rJ\x04\x08\x01\x10\x02\x42\x85\x01\n%com.xray.transport.internet.websocketP\x01Z6github.com/xtls/xray-core/transport/internet/websocket\xaa\x02!Xray.Transport.Internet.Websocketb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x65xtensions.proto\x12\x1av2ray.core.common.protoext\x1a google/protobuf/descriptor.proto\"Q\n\nMessageOpt\x12\x0c\n\x04type\x18\x01 \x03(\t\x12\x12\n\nshort_name\x18\x02 \x03(\t\x12!\n\x17transport_original_name\x18\xf1\x9f\x05 \x01(\t\"\xd0\x01\n\x08\x46ieldOpt\x12\x11\n\tany_wants\x18\x01 \x03(\t\x12\x16\n\x0e\x61llowed_values\x18\x02 \x03(\t\x12\x1b\n\x13\x61llowed_value_types\x18\x03 \x03(\t\x12#\n\x1b\x63onvert_time_read_file_into\x18\x04 \x01(\t\x12\x11\n\tforbidden\x18\x05 \x01(\x08\x12%\n\x1d\x63onvert_time_resource_loading\x18\x06 \x01(\t\x12\x1d\n\x15\x63onvert_time_parse_ip\x18\x07 \x01(\t:^\n\x0bmessage_opt\x12\x1f.google.protobuf.MessageOptions\x18\xd0\x86\x03 \x01(\x0b\x32&.v2ray.core.common.protoext.MessageOpt:X\n\tfield_opt\x12\x1d.google.protobuf.FieldOptions\x18\xd0\x86\x03 \x01(\x0b\x32$.v2ray.core.common.protoext.FieldOptBo\n\x1e\x63om.v2ray.core.common.protoextP\x01Z.github.com/v2fly/v2ray-core/v5/common/protoext\xaa\x02\x1aV2Ray.Core.Common.ProtoExtb\x06proto3')
 
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'transport.internet.websocket.config_pb2', _globals)
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'extensions_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
+  google_dot_protobuf_dot_descriptor__pb2.MessageOptions.RegisterExtension(message_opt)
+  google_dot_protobuf_dot_descriptor__pb2.FieldOptions.RegisterExtension(field_opt)
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n%com.xray.transport.internet.websocketP\001Z6github.com/xtls/xray-core/transport/internet/websocket\252\002!Xray.Transport.Internet.Websocket'
-  _globals['_HEADER']._serialized_start=80
-  _globals['_HEADER']._serialized_end=116
-  _globals['_CONFIG']._serialized_start=119
-  _globals['_CONFIG']._serialized_end=249
+  DESCRIPTOR._serialized_options = b'\n\036com.v2ray.core.common.protoextP\001Z.github.com/v2fly/v2ray-core/v5/common/protoext\252\002\032V2Ray.Core.Common.ProtoExt'
+  _MESSAGEOPT._serialized_start=82
+  _MESSAGEOPT._serialized_end=163
+  _FIELDOPT._serialized_start=166
+  _FIELDOPT._serialized_end=374
 # @@protoc_insertion_point(module_scope)
```

### Comparing `xtlsapi-3.0.4/xtlsapi/xray_api/transport/internet/xtls/config_pb2.py` & `xtlsapi-3.1.0/xtlsapi/xray_api/transport/internet/xtls/config_pb2.py`

 * *Files identical despite different names*

### Comparing `xtlsapi-3.0.4/xtlsapi.egg-info/PKG-INFO` & `xtlsapi-3.1.0/xtlsapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtlsapi
-Version: 3.0.4
+Version: 3.1.0
 Summary: Awesome xtlsapi created by hiddify
 Home-page: https://github.com/hiddify/xtlsapi/
 Author: hiddify
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `xtlsapi-3.0.4/xtlsapi.egg-info/SOURCES.txt` & `xtlsapi-3.1.0/xtlsapi.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,19 @@
 xtlsapi/exceptions/email_already_exists.py
 xtlsapi/exceptions/email_not_found.py
 xtlsapi/exceptions/inbound_not_found.py
 xtlsapi/ext/__init__.py
 xtlsapi/ext/utils.py
 xtlsapi/singbox_api/__init__.py
 xtlsapi/singbox_api/build.sh
+xtlsapi/singbox_api/extensions.proto
+xtlsapi/singbox_api/extensions_pb2.py
+xtlsapi/singbox_api/extensions_pb2_grpc.py
 xtlsapi/singbox_api/stats.proto
+xtlsapi/singbox_api/stats_old.proto
 xtlsapi/singbox_api/stats_pb2.py
 xtlsapi/singbox_api/stats_pb2_grpc.py
 xtlsapi/singbox_api_services/__init__.py
 xtlsapi/singbox_api_services/_base.py
 xtlsapi/singbox_api_services/stats/__init__.py
 xtlsapi/singbox_api_services/stats/get_client_download_traffic.py
 xtlsapi/singbox_api_services/stats/get_client_upload_traffic.py
```

