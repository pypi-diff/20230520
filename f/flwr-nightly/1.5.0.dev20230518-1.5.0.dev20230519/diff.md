# Comparing `tmp/flwr_nightly-1.5.0.dev20230518.tar.gz` & `tmp/flwr_nightly-1.5.0.dev20230519.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flwr_nightly-1.5.0.dev20230518.tar", max compression
+gzip compressed data, was "flwr_nightly-1.5.0.dev20230519.tar", max compression
```

## Comparing `flwr_nightly-1.5.0.dev20230518.tar` & `flwr_nightly-1.5.0.dev20230519.tar`

### file list

```diff
@@ -1,110 +1,111 @@
--rw-r--r--   0        0        0    11358 2023-05-18 23:02:39.501273 flwr_nightly-1.5.0.dev20230518/LICENSE
--rw-r--r--   0        0        0    10297 2023-05-18 23:02:39.501273 flwr_nightly-1.5.0.dev20230518/README.md
--rw-r--r--   0        0        0     4268 2023-05-18 23:03:06.029362 flwr_nightly-1.5.0.dev20230518/pyproject.toml
--rw-r--r--   0        0        0      952 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/__init__.py
--rw-r--r--   0        0        0     1164 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/client/__init__.py
--rw-r--r--   0        0        0    12441 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/client/app.py
--rw-r--r--   0        0        0     6503 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/client/client.py
--rw-r--r--   0        0        0     3351 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      728 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/client/grpc_client/__init__.py
--rw-r--r--   0        0        0     4288 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/client/grpc_client/connection.py
--rw-r--r--   0        0        0      712 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/client/message_handler/__init__.py
--rw-r--r--   0        0        0     5077 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/client/message_handler/message_handler.py
--rw-r--r--   0        0        0     1686 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/client/message_handler/task_handler.py
--rw-r--r--   0        0        0     5100 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/client/numpy_client.py
--rw-r--r--   0        0        0      728 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/client/rest_client/__init__.py
--rw-r--r--   0        0        0     8194 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/client/rest_client/connection.py
--rw-r--r--   0        0        0     2877 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/common/__init__.py
--rw-r--r--   0        0        0     1876 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/common/address.py
--rw-r--r--   0        0        0      898 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/common/constant.py
--rw-r--r--   0        0        0      884 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/common/date.py
--rw-r--r--   0        0        0     1828 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/common/dp.py
--rw-r--r--   0        0        0     1894 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/common/grpc.py
--rw-r--r--   0        0        0     3483 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/common/logger.py
--rw-r--r--   0        0        0     2120 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/common/parameter.py
--rw-r--r--   0        0        0    16316 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/common/serde.py
--rw-r--r--   0        0        0     7805 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/common/telemetry.py
--rw-r--r--   0        0        0     3714 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/common/typing.py
--rw-r--r--   0        0        0      848 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/common/version.py
--rw-r--r--   0        0        0      809 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/driver/__init__.py
--rw-r--r--   0        0        0     4762 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/driver/app.py
--rw-r--r--   0        0        0     3909 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/driver/driver.py
--rw-r--r--   0        0        0     4414 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/driver/driver_client_manager.py
--rw-r--r--   0        0        0     5654 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/driver/driver_client_proxy.py
--rw-r--r--   0        0        0      676 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/__init__.py
--rw-r--r--   0        0        0     4663 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/driver_pb2.py
--rw-r--r--   0        0        0     3815 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/driver_pb2.pyi
--rw-r--r--   0        0        0     5727 2023-05-18 23:02:39.781288 flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/driver_pb2_grpc.py
--rw-r--r--   0        0        0     1617 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/driver_pb2_grpc.pyi
--rw-r--r--   0        0        0     4982 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/fleet_pb2.py
--rw-r--r--   0        0        0     4554 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/fleet_pb2.pyi
--rw-r--r--   0        0        0     4275 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/fleet_pb2_grpc.py
--rw-r--r--   0        0        0     1495 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/fleet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1188 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/node_pb2.py
--rw-r--r--   0        0        0      751 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/node_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/node_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/node_pb2_grpc.pyi
--rw-r--r--   0        0        0     3217 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/task_pb2.py
--rw-r--r--   0        0        0     4286 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/task_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/task_pb2_grpc.pyi
--rw-r--r--   0        0        0    18721 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/transport_pb2.py
--rw-r--r--   0        0        0    21497 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2598 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      766 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/py.typed
--rw-r--r--   0        0        0     1370 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/__init__.py
--rw-r--r--   0        0        0    23657 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/app.py
--rw-r--r--   0        0        0     5941 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/client_manager.py
--rw-r--r--   0        0        0     2228 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/client_proxy.py
--rw-r--r--   0        0        0     1058 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/criterion.py
--rw-r--r--   0        0        0      705 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/driver/__init__.py
--rw-r--r--   0        0        0     3919 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/driver/driver_servicer.py
--rw-r--r--   0        0        0      704 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/fleet/__init__.py
--rw-r--r--   0        0        0      728 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/fleet/grpc_bidi/__init__.py
--rw-r--r--   0        0        0     4467 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py
--rw-r--r--   0        0        0     5602 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py
--rw-r--r--   0        0        0     6416 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py
--rw-r--r--   0        0        0     4627 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py
--rw-r--r--   0        0        0    11523 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py
--rw-r--r--   0        0        0     6314 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py
--rw-r--r--   0        0        0      751 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/fleet/grpc_rere/__init__.py
--rw-r--r--   0        0        0     1638 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py
--rw-r--r--   0        0        0      724 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/fleet/message_handler/__init__.py
--rw-r--r--   0        0        0     2026 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/fleet/message_handler/message_handler.py
--rw-r--r--   0        0        0      728 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/fleet/rest_rere/__init__.py
--rw-r--r--   0        0        0     3718 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/fleet/rest_rere/rest_api.py
--rw-r--r--   0        0        0     4457 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/history.py
--rw-r--r--   0        0        0    15891 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/server.py
--rw-r--r--   0        0        0      996 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/state/__init__.py
--rw-r--r--   0        0        0     6521 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/state/in_memory_state.py
--rw-r--r--   0        0        0    19296 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/state/sqlite_state.py
--rw-r--r--   0        0        0     4805 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/state/state.py
--rw-r--r--   0        0        0     1648 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/state/state_factory.py
--rw-r--r--   0        0        0     1588 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/__init__.py
--rw-r--r--   0        0        0     4994 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/aggregate.py
--rw-r--r--   0        0        0     4519 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     4875 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5830 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6730 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/fedadagrad.py
--rw-r--r--   0        0        0     7012 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/fedadam.py
--rw-r--r--   0        0        0    11495 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/fedavg.py
--rw-r--r--   0        0        0     9985 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8805 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/fedavgm.py
--rw-r--r--   0        0        0     6321 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/fedmedian.py
--rw-r--r--   0        0        0     5393 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/fedopt.py
--rw-r--r--   0        0        0     7708 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/fedprox.py
--rw-r--r--   0        0        0     7624 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/fedxgb_nn_avg.py
--rw-r--r--   0        0        0     7044 2023-05-18 23:02:39.785289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/fedyogi.py
--rw-r--r--   0        0        0     6863 2023-05-18 23:02:39.789289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/krum.py
--rw-r--r--   0        0        0    10147 2023-05-18 23:02:39.789289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/qfedavg.py
--rw-r--r--   0        0        0     7484 2023-05-18 23:02:39.789289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/strategy.py
--rw-r--r--   0        0        0      901 2023-05-18 23:02:39.789289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/utils/__init__.py
--rw-r--r--   0        0        0     5114 2023-05-18 23:02:39.789289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/utils/tensorboard.py
--rw-r--r--   0        0        0     4941 2023-05-18 23:02:39.789289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/utils/validator.py
--rw-r--r--   0        0        0     1271 2023-05-18 23:02:39.789289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/simulation/__init__.py
--rw-r--r--   0        0        0     7777 2023-05-18 23:02:39.789289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/simulation/app.py
--rw-r--r--   0        0        0      727 2023-05-18 23:02:39.789289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0     5472 2023-05-18 23:02:39.789289 flwr_nightly-1.5.0.dev20230518/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0    12394 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230518/setup.py
--rw-r--r--   0        0        0    12772 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230518/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-05-19 23:02:42.853466 flwr_nightly-1.5.0.dev20230519/LICENSE
+-rw-r--r--   0        0        0    10297 2023-05-19 23:02:42.853466 flwr_nightly-1.5.0.dev20230519/README.md
+-rw-r--r--   0        0        0     4268 2023-05-19 23:03:07.641859 flwr_nightly-1.5.0.dev20230519/pyproject.toml
+-rw-r--r--   0        0        0      952 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/__init__.py
+-rw-r--r--   0        0        0     1164 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/__init__.py
+-rw-r--r--   0        0        0    13514 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/app.py
+-rw-r--r--   0        0        0     6503 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/client.py
+-rw-r--r--   0        0        0     3351 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      728 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0     4288 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/grpc_client/connection.py
+-rw-r--r--   0        0        0      712 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/message_handler/__init__.py
+-rw-r--r--   0        0        0     5077 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/message_handler/message_handler.py
+-rw-r--r--   0        0        0     1686 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/message_handler/task_handler.py
+-rw-r--r--   0        0        0     5100 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/numpy_client.py
+-rw-r--r--   0        0        0      728 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/rest_client/__init__.py
+-rw-r--r--   0        0        0     8194 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/rest_client/connection.py
+-rw-r--r--   0        0        0     2877 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/__init__.py
+-rw-r--r--   0        0        0     1876 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/address.py
+-rw-r--r--   0        0        0     1044 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/constant.py
+-rw-r--r--   0        0        0      884 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/date.py
+-rw-r--r--   0        0        0     1828 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/dp.py
+-rw-r--r--   0        0        0     1894 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/grpc.py
+-rw-r--r--   0        0        0     3483 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/logger.py
+-rw-r--r--   0        0        0     2120 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/parameter.py
+-rw-r--r--   0        0        0    16316 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/serde.py
+-rw-r--r--   0        0        0     7805 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/telemetry.py
+-rw-r--r--   0        0        0     3714 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/typing.py
+-rw-r--r--   0        0        0      848 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/version.py
+-rw-r--r--   0        0        0      809 2023-05-19 23:02:43.105469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/driver/__init__.py
+-rw-r--r--   0        0        0     4826 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/driver/app.py
+-rw-r--r--   0        0        0     3909 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/driver/driver.py
+-rw-r--r--   0        0        0     4414 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/driver/driver_client_manager.py
+-rw-r--r--   0        0        0     5654 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/driver/driver_client_proxy.py
+-rw-r--r--   0        0        0      676 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/__init__.py
+-rw-r--r--   0        0        0     4663 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/driver_pb2.py
+-rw-r--r--   0        0        0     3815 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/driver_pb2.pyi
+-rw-r--r--   0        0        0     5727 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/driver_pb2_grpc.py
+-rw-r--r--   0        0        0     1617 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/driver_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4982 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/fleet_pb2.py
+-rw-r--r--   0        0        0     4554 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/fleet_pb2.pyi
+-rw-r--r--   0        0        0     4275 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/fleet_pb2_grpc.py
+-rw-r--r--   0        0        0     1495 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/fleet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1188 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/node_pb2.py
+-rw-r--r--   0        0        0      751 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/node_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/node_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/node_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3217 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/task_pb2.py
+-rw-r--r--   0        0        0     4286 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0    18721 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/transport_pb2.py
+-rw-r--r--   0        0        0    21497 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2598 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      766 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/py.typed
+-rw-r--r--   0        0        0     1370 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/__init__.py
+-rw-r--r--   0        0        0    23751 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/app.py
+-rw-r--r--   0        0        0     5941 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/client_manager.py
+-rw-r--r--   0        0        0     2228 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/client_proxy.py
+-rw-r--r--   0        0        0     1058 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/criterion.py
+-rw-r--r--   0        0        0      705 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/driver/__init__.py
+-rw-r--r--   0        0        0     3919 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/driver/driver_servicer.py
+-rw-r--r--   0        0        0      704 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/__init__.py
+-rw-r--r--   0        0        0      728 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_bidi/__init__.py
+-rw-r--r--   0        0        0     4467 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py
+-rw-r--r--   0        0        0     5602 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py
+-rw-r--r--   0        0        0     6416 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py
+-rw-r--r--   0        0        0     4627 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11523 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py
+-rw-r--r--   0        0        0     6314 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py
+-rw-r--r--   0        0        0      751 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_rere/__init__.py
+-rw-r--r--   0        0        0     1638 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py
+-rw-r--r--   0        0        0      724 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/message_handler/__init__.py
+-rw-r--r--   0        0        0     2026 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/message_handler/message_handler.py
+-rw-r--r--   0        0        0      728 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/rest_rere/__init__.py
+-rw-r--r--   0        0        0     3718 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/rest_rere/rest_api.py
+-rw-r--r--   0        0        0     4457 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/history.py
+-rw-r--r--   0        0        0    15891 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/server.py
+-rw-r--r--   0        0        0      996 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/state/__init__.py
+-rw-r--r--   0        0        0     6521 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/state/in_memory_state.py
+-rw-r--r--   0        0        0    19296 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/state/sqlite_state.py
+-rw-r--r--   0        0        0     4805 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/state/state.py
+-rw-r--r--   0        0        0     1648 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/state/state_factory.py
+-rw-r--r--   0        0        0     1667 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/__init__.py
+-rw-r--r--   0        0        0     6105 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/aggregate.py
+-rw-r--r--   0        0        0     4519 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     4875 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     5830 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6730 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     7012 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedadam.py
+-rw-r--r--   0        0        0    11495 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedavg.py
+-rw-r--r--   0        0        0     9985 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     8805 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedavgm.py
+-rw-r--r--   0        0        0     6321 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedmedian.py
+-rw-r--r--   0        0        0     5393 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedopt.py
+-rw-r--r--   0        0        0     7708 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedprox.py
+-rw-r--r--   0        0        0     5924 2023-05-19 23:02:43.109469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedtrimmedavg.py
+-rw-r--r--   0        0        0     7624 2023-05-19 23:02:43.113469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedxgb_nn_avg.py
+-rw-r--r--   0        0        0     7044 2023-05-19 23:02:43.113469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedyogi.py
+-rw-r--r--   0        0        0     6863 2023-05-19 23:02:43.113469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/krum.py
+-rw-r--r--   0        0        0    10147 2023-05-19 23:02:43.113469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7484 2023-05-19 23:02:43.113469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/strategy.py
+-rw-r--r--   0        0        0      901 2023-05-19 23:02:43.113469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/utils/__init__.py
+-rw-r--r--   0        0        0     5114 2023-05-19 23:02:43.113469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/utils/tensorboard.py
+-rw-r--r--   0        0        0     4941 2023-05-19 23:02:43.113469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/utils/validator.py
+-rw-r--r--   0        0        0     1271 2023-05-19 23:02:43.113469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/simulation/__init__.py
+-rw-r--r--   0        0        0     7777 2023-05-19 23:02:43.113469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/simulation/app.py
+-rw-r--r--   0        0        0      727 2023-05-19 23:02:43.113469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0     5472 2023-05-19 23:02:43.113469 flwr_nightly-1.5.0.dev20230519/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0    12394 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230519/setup.py
+-rw-r--r--   0        0        0    12772 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230519/PKG-INFO
```

### Comparing `flwr_nightly-1.5.0.dev20230518/LICENSE` & `flwr_nightly-1.5.0.dev20230519/LICENSE`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/README.md` & `flwr_nightly-1.5.0.dev20230519/README.md`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/pyproject.toml` & `flwr_nightly-1.5.0.dev20230519/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flwr-nightly"
-version = "1.5.0-dev20230518"
+version = "1.5.0-dev20230519"
 description = "Flower: A Friendly Federated Learning Framework"
 license = "Apache-2.0"
 authors = ["The Flower Authors <hello@flower.dev>"]
 readme = "README.md"
 homepage = "https://flower.dev"
 repository = "https://github.com/adap/flower"
 documentation = "https://flower.dev"
```

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/__init__.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/client/__init__.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/client/app.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,20 @@
     GRPC_MAX_MESSAGE_LENGTH,
     EventType,
     event,
     ndarrays_to_parameters,
     parameters_to_ndarrays,
 )
 from flwr.common.address import parse_address
-from flwr.common.constant import MISSING_EXTRA_REST
+from flwr.common.constant import (
+    MISSING_EXTRA_REST,
+    TRANSPORT_TYPE_GRPC_BIDI,
+    TRANSPORT_TYPE_REST,
+    TRANSPORT_TYPES,
+)
 from flwr.common.logger import log
 from flwr.common.typing import (
     Code,
     EvaluateIns,
     EvaluateRes,
     FitIns,
     FitRes,
@@ -75,26 +80,26 @@
 Example
 -------
 
     0.5, 10, {"accuracy": 0.95}
 
 """
 
-
 ClientLike = Union[Client, NumPyClient]
 
 
 # pylint: disable=import-outside-toplevel,too-many-locals
 def start_client(
     *,
     server_address: str,
     client: Client,
     grpc_max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,
     root_certificates: Optional[Union[bytes, str]] = None,
-    rest: bool = False,
+    rest: bool = False,  # Deprecated in favor of `transport`
+    transport: Optional[str] = None,
 ) -> None:
     """Start a Flower client node which connects to a Flower server.
 
     Parameters
     ----------
     server_address : str
         The IPv4 or IPv6 address of the server. If the Flower
@@ -111,17 +116,22 @@
         same value (see `flwr.server.start_server`), otherwise it will not
         know about the increased limit and block larger messages.
     root_certificates : Optional[Union[bytes, str]] (default: None)
         The PEM-encoded root certificates as a byte string or a path string.
         If provided, a secure connection using the certificates will be
         established to an SSL-enabled Flower server.
     rest : bool (default: False)
+        DEPRECATED - USE 'transport' INSTEAD.
         Defines whether or not the client is interacting with the server using the
         experimental REST API. This feature is experimental, it might change
         considerably in future versions of Flower.
+    transport : Optional[str] (default: None)
+        Configure the transport layer. Allowed values:
+        - 'grpc-bidi': gRPC, bidirectional streaming
+        - 'rest': HTTP (experimental)
 
     Examples
     --------
     Starting a gRPC client with an insecure server connection:
 
     >>> start_client(
     >>>     server_address=localhost:8080,
@@ -143,28 +153,37 @@
     # Parse IP address
     parsed_address = parse_address(server_address)
     if not parsed_address:
         sys.exit(f"Server address ({server_address}) cannot be parsed.")
     host, port, is_v6 = parsed_address
     address = f"[{host}]:{port}" if is_v6 else f"{host}:{port}"
 
+    # Set the default transport layer
+    if transport is None:
+        transport = TRANSPORT_TYPE_REST if rest else TRANSPORT_TYPE_GRPC_BIDI
+
     # Use either gRPC bidirectional streaming or REST request/response
-    if rest:
+    if transport == TRANSPORT_TYPE_REST:
         try:
             from .rest_client.connection import http_request_response
         except ModuleNotFoundError:
             sys.exit(MISSING_EXTRA_REST)
         if server_address[:4] != "http":
             sys.exit(
                 "When using the REST API, please provide `https://` or "
                 "`http://` before the server address (e.g. `http://127.0.0.1:8080`)"
             )
         connection = http_request_response
-    else:
+    elif transport == TRANSPORT_TYPE_GRPC_BIDI:
         connection = grpc_connection
+    else:
+        raise ValueError(
+            f"Unknown transport type: {transport} (possible: {TRANSPORT_TYPES})"
+        )
+
     while True:
         sleep_duration: int = 0
         with connection(
             address,
             max_message_length=grpc_max_message_length,
             root_certificates=root_certificates,
         ) as conn:
@@ -197,15 +216,16 @@
 
 def start_numpy_client(
     *,
     server_address: str,
     client: NumPyClient,
     grpc_max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,
     root_certificates: Optional[bytes] = None,
-    rest: bool = False,
+    rest: bool = False,  # Deprecated in favor of `transport`
+    transport: Optional[str] = None,
 ) -> None:
     """Start a Flower NumPyClient which connects to a gRPC server.
 
     Parameters
     ----------
     server_address : str
         The IPv4 or IPv6 address of the server. If the Flower server runs on
@@ -221,17 +241,22 @@
         same value (see `flwr.server.start_server`), otherwise it will not
         know about the increased limit and block larger messages.
     root_certificates : bytes (default: None)
         The PEM-encoded root certificates as a byte string or a path string.
         If provided, a secure connection using the certificates will be
         established to an SSL-enabled Flower server.
     rest : bool (default: False)
+        DEPRECATED - USE 'transport' INSTEAD.
         Defines whether or not the client is interacting with the server using the
-        experimental REST API. This feature is experimental, it might be change
+        experimental REST API. This feature is experimental, it might change
         considerably in future versions of Flower.
+    transport : Optional[str] (default: None)
+        Configure the transport layer. Allowed values:
+        - 'grpc-bidi': gRPC, bidirectional streaming
+        - 'rest': HTTP (experimental)
 
     Examples
     --------
     Starting a client with an insecure server connection:
 
     >>> start_client(
     >>>     server_address=localhost:8080,
@@ -251,14 +276,15 @@
     # Start
     start_client(
         server_address=server_address,
         client=_wrap_numpy_client(client=client),
         grpc_max_message_length=grpc_max_message_length,
         root_certificates=root_certificates,
         rest=rest,
+        transport=transport,
     )
 
 
 def to_client(client_like: ClientLike) -> Client:
     """Take any Client-like object and return it as a Client."""
     if isinstance(client_like, NumPyClient):
         return _wrap_numpy_client(client=client_like)
```

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/client/client.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/client/dpfedavg_numpy_client.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/client/grpc_client/__init__.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/client/grpc_client/connection.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/grpc_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/client/message_handler/__init__.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/client/message_handler/message_handler.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/client/message_handler/task_handler.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/message_handler/task_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/client/numpy_client.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/client/rest_client/__init__.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/client/rest_client/connection.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/client/rest_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/common/__init__.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/common/address.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/address.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/common/constant.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,15 @@
-# Copyright 2020 Adap GmbH. All Rights Reserved.
+# Copyright 2022 Adap GmbH. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Flower constants."""
-
-
-MISSING_EXTRA_REST = """
-Extra dependencies required for using the REST-based Fleet API are missing.
-
-To use the REST API, install `flwr` with the `rest` extra:
-
-    `pip install flwr[rest]`.
-"""
+"""Flower fleet service."""
```

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/common/date.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/date.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/common/dp.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/dp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/common/grpc.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/common/logger.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/logger.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/common/parameter.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/parameter.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/common/serde.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/serde.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/common/telemetry.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/telemetry.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/common/typing.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/common/version.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/common/version.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/driver/__init__.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/driver/app.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/driver/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,17 +65,17 @@
         `round_timeout` in seconds (float, default: None).
     strategy : Optional[flwr.server.Strategy] (default: None).
         An implementation of the abstract base class
         `flwr.server.strategy.Strategy`. If no strategy is provided, then
         `start_server` will use `flwr.server.strategy.FedAvg`.
     client_manager : Optional[flwr.driver.DriverClientManager] (default: None)
         An implementation of the class
-        `flwr.server.DriverClientManager`. If no implementation is provided, then
-        `start_driver` will use
-        `flwr.server.client_manager.DriverClientManager(anonymous=False)`.
+        `flwr.driver.driver_client_manager.DriverClientManager`. If no
+        implementation is provided, then `start_driver` will use
+        `flwr.driver.driver_client_manager.DriverClientManager`.
     certificates : bytes (default: None)
         Tuple containing root certificate, server certificate, and private key
         to start a secure SSL-enabled server. The tuple is expected to have
         three bytes elements in the following order:
 
             * CA certificate.
             * server certificate.
@@ -84,19 +84,19 @@
     Returns
     -------
     hist : flwr.server.history.History
         Object containing training and evaluation metrics.
 
     Examples
     --------
-    Starting an insecure server:
+    Starting a driver that connects to an insecure server:
 
     >>> start_driver()
 
-    Starting an SSL-enabled server:
+    Starting a driver that connects to an SSL-enabled server:
 
     >>> start_driver(
     >>>     certificates=Path("/crts/root.pem").read_bytes()
     >>> )
     """
     event(EventType.START_DRIVER_ENTER)
```

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/driver/driver.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/driver/driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/driver/driver_client_manager.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/driver/driver_client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/driver/driver_client_proxy.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/driver/driver_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/__init__.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/driver_pb2.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/driver_pb2.pyi` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/driver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/driver_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/driver_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/driver_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/driver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/fleet_pb2.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/fleet_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/fleet_pb2.pyi` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/fleet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/fleet_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/fleet_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/fleet_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/fleet_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/node_pb2.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/node_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/node_pb2.pyi` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/task_pb2.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/task_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/task_pb2.pyi` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/transport_pb2.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/transport_pb2.pyi` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/transport_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/proto/transport_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/__init__.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/app.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,19 @@
 from types import FrameType
 from typing import List, Optional, Tuple
 
 import grpc
 
 from flwr.common import GRPC_MAX_MESSAGE_LENGTH, EventType, event
 from flwr.common.address import parse_address
-from flwr.common.constant import MISSING_EXTRA_REST
+from flwr.common.constant import (
+    MISSING_EXTRA_REST,
+    TRANSPORT_TYPE_GRPC_BIDI,
+    TRANSPORT_TYPE_REST,
+)
 from flwr.common.logger import log
 from flwr.proto.driver_pb2_grpc import add_DriverServicer_to_server
 from flwr.proto.transport_pb2_grpc import add_FlowerServiceServicer_to_server
 from flwr.server.client_manager import ClientManager, SimpleClientManager
 from flwr.server.driver.driver_servicer import DriverServicer
 from flwr.server.fleet.grpc_bidi.driver_client_manager import DriverClientManager
 from flwr.server.fleet.grpc_bidi.flower_service_servicer import FlowerServiceServicer
@@ -271,15 +275,15 @@
     # Initialize StateFactory
     state_factory = StateFactory(args.database)
 
     grpc_servers = []
     bckg_threads = []
 
     # Start Fleet API
-    if args.fleet_api_type == "rest":
+    if args.fleet_api_type == TRANSPORT_TYPE_REST:
         if (
             importlib.util.find_spec("fastapi")
             and importlib.util.find_spec("requests")
             and importlib.util.find_spec("starlette")
             and importlib.util.find_spec("uvicorn")
         ) is None:
             sys.exit(MISSING_EXTRA_REST)
@@ -297,15 +301,15 @@
                 args.ssl_certfile,
                 state_factory,
                 args.rest_fleet_api_workers,
             ),
         )
         fleet_thread.start()
         bckg_threads.append(fleet_thread)
-    elif args.fleet_api_type == "grpc":
+    elif args.fleet_api_type == TRANSPORT_TYPE_GRPC_BIDI:
         address_arg = args.grpc_fleet_api_address
         parsed_address = parse_address(address_arg)
         if not parsed_address:
             sys.exit(f"Fleet IP address ({address_arg}) cannot be parsed.")
         host, port, is_v6 = parsed_address
         address = f"[{host}]:{port}" if is_v6 else f"{host}:{port}"
         fleet_server = _run_fleet_api_grpc_bidi(
@@ -353,15 +357,15 @@
         state_factory=state_factory,
     )
 
     grpc_servers = [driver_server]
     bckg_threads = []
 
     # Start Fleet API
-    if args.fleet_api_type == "rest":
+    if args.fleet_api_type == TRANSPORT_TYPE_REST:
         if (
             importlib.util.find_spec("fastapi")
             and importlib.util.find_spec("requests")
             and importlib.util.find_spec("starlette")
             and importlib.util.find_spec("uvicorn")
         ) is None:
             sys.exit(MISSING_EXTRA_REST)
@@ -379,15 +383,15 @@
                 args.ssl_certfile,
                 state_factory,
                 args.rest_fleet_api_workers,
             ),
         )
         fleet_thread.start()
         bckg_threads.append(fleet_thread)
-    elif args.fleet_api_type == "grpc":
+    elif args.fleet_api_type == TRANSPORT_TYPE_GRPC_BIDI:
         address_arg = args.grpc_fleet_api_address
         parsed_address = parse_address(address_arg)
         if not parsed_address:
             sys.exit(f"Fleet IP address ({address_arg}) cannot be parsed.")
         host, port, is_v6 = parsed_address
         address = f"[{host}]:{port}" if is_v6 else f"{host}:{port}"
         fleet_server = _run_fleet_api_grpc_bidi(
@@ -647,66 +651,64 @@
         default=DATABASE,
     )
 
 
 def _add_args_driver_api(parser: argparse.ArgumentParser) -> None:
     parser.add_argument(
         "--driver-api-address",
-        help="The Driver API gRPC server address, which can be an IPv4, "
-        "IPv6, or a domain name.",
+        help="Driver API (gRPC) server address (IPv4, IPv6, or a domain name)",
         default=ADDRESS_DRIVER_API,
     )
 
 
 def _add_args_fleet_api(parser: argparse.ArgumentParser) -> None:
     # Fleet API transport layer type
     ex_group = parser.add_mutually_exclusive_group()
     ex_group.add_argument(
-        "--grpc",
+        "--grpc-bidi",
         action="store_const",
         dest="fleet_api_type",
-        const="grpc",
-        default="grpc",
-        help="Start a gRPC-based Fleet API server "
-        "(which is the default if no argument is provided).",
+        const=TRANSPORT_TYPE_GRPC_BIDI,
+        default=TRANSPORT_TYPE_GRPC_BIDI,
+        help="Start a Fleet API server (gRPC-bidi)",
     )
     ex_group.add_argument(
         "--rest",
         action="store_const",
         dest="fleet_api_type",
-        const="rest",
-        help="Start a REST-based Fleet API server",
+        const=TRANSPORT_TYPE_REST,
+        help="Start a Fleet API server (REST, experimental)",
     )
 
-    # Fleet API gRPC options
-    grpc_group = parser.add_argument_group("Fleet API gRPC server options", "")
-    grpc_group.add_argument(
-        "--grpc-fleet-api-address",
-        help="The Fleet API gRPC server address, which can be an IPv4, "
-        "IPv6, or a domain name.",
+    # Fleet API gRPC-bidi options
+    grpc_bidi_group = parser.add_argument_group(
+        "Fleet API (gRPC-bidi) server options", ""
+    )
+    grpc_bidi_group.add_argument(
+        "--grpc-bidi-fleet-api-address",
+        help="Fleet API (gRPC-bidi) server address (IPv4, IPv6, or a domain name)",
         default=ADDRESS_FLEET_API_GRPC_RERE,
     )
 
     # Fleet API REST options
-    rest_group = parser.add_argument_group("Fleet API REST server options", "")
+    rest_group = parser.add_argument_group("Fleet API (REST) server options", "")
     rest_group.add_argument(
         "--rest-fleet-api-address",
-        help="The Fleet API REST server address, which can be an IPv4, "
-        "IPv6, or a domain name.",
+        help="Fleet API (REST) server address (IPv4, IPv6, or a domain name)",
         default=ADDRESS_FLEET_API_REST,
     )
     rest_group.add_argument(
         "--ssl-certfile",
-        help="Fleet API REST server SSL certificate file (as a path str), "
+        help="Fleet API (REST) server SSL certificate file (as a path str), "
         "needed for using 'https'.",
         default=None,
     )
     rest_group.add_argument(
         "--ssl-keyfile",
-        help="Fleet API REST server SSL private key file (as a path str), "
+        help="Fleet API (REST) server SSL private key file (as a path str), "
         "needed for using 'https'.",
         default=None,
     )
     rest_group.add_argument(
         "--rest-fleet-api-workers",
         help="Set the number of concurrent workers for the Fleet API REST server.",
         type=int,
```

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/client_manager.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/client_proxy.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/criterion.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/criterion.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/driver/__init__.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/driver/driver_servicer.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/driver/driver_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/fleet/__init__.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/simulation/ray_transport/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# Copyright 2022 Adap GmbH. All Rights Reserved.
+# Copyright 2020 Adap GmbH. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Flower fleet service."""
+"""Ray-based Flower ClientProxy implementation."""
```

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/fleet/grpc_bidi/__init__.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_bidi/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/fleet/grpc_rere/__init__.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/fleet/message_handler/__init__.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/fleet/message_handler/message_handler.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/fleet/rest_rere/__init__.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/rest_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/fleet/rest_rere/rest_api.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/fleet/rest_rere/rest_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/history.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/history.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/server.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/state/__init__.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/state/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/state/in_memory_state.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/state/in_memory_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/state/sqlite_state.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/state/sqlite_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/state/state.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/state/state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/state/state_factory.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/state/state_factory.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/__init__.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from .fedadam import FedAdam as FedAdam
 from .fedavg import FedAvg as FedAvg
 from .fedavg_android import FedAvgAndroid as FedAvgAndroid
 from .fedavgm import FedAvgM as FedAvgM
 from .fedmedian import FedMedian as FedMedian
 from .fedopt import FedOpt as FedOpt
 from .fedprox import FedProx as FedProx
+from .fedtrimmedavg import FedTrimmedAvg as FedTrimmedAvg
 from .fedxgb_nn_avg import FedXgbNnAvg as FedXgbNnAvg
 from .fedyogi import FedYogi as FedYogi
 from .qfedavg import QFedAvg as QFedAvg
 from .strategy import Strategy as Strategy
 
 __all__ = [
     "FaultTolerantFedAvg",
@@ -38,9 +39,10 @@
     "FedAvgAndroid",
     "FedAvgM",
     "FedOpt",
     "FedProx",
     "FedYogi",
     "QFedAvg",
     "FedMedian",
+    "FedTrimmedAvg",
     "Strategy",
 ]
```

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/aggregate.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/aggregate.py`

 * *Files 18% similar despite different names*

```diff
@@ -128,7 +128,45 @@
     distance_matrix = np.zeros((len(weights), len(weights)))
     for i, _ in enumerate(flat_w):
         for j, _ in enumerate(flat_w):
             delta = flat_w[i] - flat_w[j]
             norm = np.linalg.norm(delta)  # type: ignore
             distance_matrix[i, j] = norm**2
     return distance_matrix
+
+
+def _trim_mean(array: NDArray, proportiontocut: float) -> NDArray:
+    """Compute trimmed mean along axis=0.
+
+     It is based on the scipy implementation.
+
+    https://docs.scipy.org/doc/scipy/reference/generated/
+    scipy.stats.trim_mean.html.
+    """
+    axis = 0
+    nobs = array.shape[axis]
+    lowercut = int(proportiontocut * nobs)
+    uppercut = nobs - lowercut
+    if lowercut > uppercut:
+        raise ValueError("Proportion too big.")
+
+    atmp = np.partition(array, (lowercut, uppercut - 1), axis)
+
+    slice_list = [slice(None)] * atmp.ndim
+    slice_list[axis] = slice(lowercut, uppercut)
+    result: NDArray = np.mean(atmp[tuple(slice_list)], axis=axis)
+    return result
+
+
+def aggregate_trimmed_avg(
+    results: List[Tuple[NDArrays, int]], proportiontocut: float
+) -> NDArrays:
+    """Compute trimmed average."""
+    # Create a list of weights and ignore the number of examples
+    weights = [weights for weights, _ in results]
+
+    trimmed_w: NDArrays = [
+        _trim_mean(np.asarray(layer), proportiontocut=proportiontocut)
+        for layer in zip(*weights)
+    ]
+
+    return trimmed_w
```

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/dpfedavg_adaptive.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/dpfedavg_adaptive.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/dpfedavg_fixed.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/dpfedavg_fixed.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/fault_tolerant_fedavg.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/fedadagrad.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/fedadam.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedadam.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/fedavg.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/fedavg_android.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedavg_android.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/fedavgm.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedavgm.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/fedmedian.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedmedian.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/fedopt.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedopt.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/fedprox.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedprox.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/fedxgb_nn_avg.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedxgb_nn_avg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/fedyogi.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/fedyogi.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/krum.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/krum.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/qfedavg.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/qfedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/strategy/strategy.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/utils/__init__.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/utils/tensorboard.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/server/utils/validator.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/server/utils/validator.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/simulation/__init__.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/simulation/app.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/simulation/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/src/py/flwr/simulation/ray_transport/ray_client_proxy.py` & `flwr_nightly-1.5.0.dev20230519/src/py/flwr/simulation/ray_transport/ray_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230518/setup.py` & `flwr_nightly-1.5.0.dev20230519/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 {'console_scripts': ['flower-client = flwr.client:run_client',
                      'flower-driver-api = flwr.server:run_driver_api',
                      'flower-fleet-api = flwr.server:run_fleet_api',
                      'flower-server = flwr.server:run_server']}
 
 setup_kwargs = {
     'name': 'flwr-nightly',
-    'version': '1.5.0.dev20230518',
+    'version': '1.5.0.dev20230519',
     'description': 'Flower: A Friendly Federated Learning Framework',
     'long_description': '# Flower: A Friendly Federated Learning Framework\n\n<p align="center">\n  <a href="https://flower.dev/">\n    <img src="https://flower.dev/_next/image/?url=%2F_next%2Fstatic%2Fmedia%2Fflower_white_border.c2012e70.png&w=640&q=75" width="140px" alt="Flower Website" />\n  </a>\n</p>\n<p align="center">\n    <a href="https://flower.dev/">Website</a> |\n    <a href="https://flower.dev/blog">Blog</a> |\n    <a href="https://flower.dev/docs/">Docs</a> |\n    <a href="https://flower.dev/conf/flower-summit-2022">Conference</a> |\n    <a href="https://flower.dev/join-slack">Slack</a>\n    <br /><br />\n</p>\n\n[![GitHub license](https://img.shields.io/github/license/adap/flower)](https://github.com/adap/flower/blob/main/LICENSE)\n[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/adap/flower/blob/main/CONTRIBUTING.md)\n![Build](https://github.com/adap/flower/actions/workflows/flower.yml/badge.svg)\n![Downloads](https://pepy.tech/badge/flwr)\n[![Slack](https://img.shields.io/badge/Chat-Slack-red)](https://flower.dev/join-slack)\n\nFlower (`flwr`) is a framework for building federated learning systems. The\ndesign of Flower is based on a few guiding principles:\n\n* **Customizable**: Federated learning systems vary wildly from one use case to\n  another. Flower allows for a wide range of different configurations depending\n  on the needs of each individual use case.\n\n* **Extendable**: Flower originated from a research project at the University of\n  Oxford, so it was built with AI research in mind. Many components can be\n  extended and overridden to build new state-of-the-art systems.\n\n* **Framework-agnostic**: Different machine learning frameworks have different\n  strengths. Flower can be used with any machine learning framework, for\n  example, [PyTorch](https://pytorch.org),\n  [TensorFlow](https://tensorflow.org), [Hugging Face Transformers](https://huggingface.co/), [PyTorch Lightning](https://pytorchlightning.ai/), [MXNet](https://mxnet.apache.org/), [scikit-learn](https://scikit-learn.org/), [JAX](https://jax.readthedocs.io/), [TFLite](https://tensorflow.org/lite/), [fastai](https://www.fast.ai/), [Pandas](https://pandas.pydata.org/\n) for federated analytics, or even raw [NumPy](https://numpy.org/)\n  for users who enjoy computing gradients by hand.\n\n* **Understandable**: Flower is written with maintainability in mind. The\n  community is encouraged to both read and contribute to the codebase.\n\nMeet the Flower community on [flower.dev](https://flower.dev)!\n\n## Federated Learning Tutorial\n\nFlower\'s goal is to make federated learning accessible to everyone. This series of tutorials introduces the fundamentals of federated learning and how to implement them in Flower.\n\n0. **What is Federated Learning?**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-0-What-is-FL.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-0-What-is-FL.ipynb))\n\n1. **An Introduction to Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb))\n\n2. **Using Strategies in Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb))\n   \n3. **Building Strategies for Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-3-Building-a-Strategy-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-3-Building-a-Strategy-PyTorch.ipynb))\n   \n4. **Custom Clients for Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb))\n\nStay tuned, more tutorials are coming soon. Topics include **Privacy and Security in Federated Learning**, and **Scaling Federated Learning**.\n\n## Documentation\n\n[Flower Docs](https://flower.dev/docs):\n* [Installation](https://flower.dev/docs/installation.html)\n* [Quickstart (TensorFlow)](https://flower.dev/docs/quickstart-tensorflow.html)\n* [Quickstart (PyTorch)](https://flower.dev/docs/quickstart-pytorch.html)\n* [Quickstart (Hugging Face [code example])](https://flower.dev/docs/quickstart-huggingface.html)\n* [Quickstart (PyTorch Lightning [code example])](https://flower.dev/docs/quickstart-pytorch-lightning.html)\n* [Quickstart (MXNet)](https://flower.dev/docs/example-mxnet-walk-through.html)\n* [Quickstart (Pandas)](https://flower.dev/docs/quickstart-pandas.html)\n* [Quickstart (fastai)](https://flower.dev/docs/quickstart-fastai.html)\n* [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/quickstart_jax)\n* [Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist)\n* [Quickstart (TFLite on Android [code example])](https://github.com/adap/flower/tree/main/examples/android)\n\n## Flower Baselines\n\nFlower Baselines is a collection of community-contributed experiments that reproduce the experiments performed in popular federated learning publications. Researchers can build on Flower Baselines to quickly evaluate new ideas:\n\n* [FedAvg](https://arxiv.org/abs/1602.05629):\n  * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedavg_mnist)\n* [FedProx](https://arxiv.org/abs/1812.06127):\n  * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedprox_mnist)\n* [FedBN: Federated Learning on non-IID Features via Local Batch Normalization](https://arxiv.org/abs/2102.07623):\n  * [Convergence Rate](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedbn/convergence_rate)\n* [Adaptive Federated Optimization](https://arxiv.org/abs/2003.00295):\n  * [CIFAR-10/100](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/adaptive_federated_optimization)\n\nCheck the Flower documentation to learn more: [Using Baselines](https://flower.dev/docs/using-baselines.html)\n\nThe Flower community loves contributions! Make your work more visible and enable others to build on it by contributing it as a baseline: [Contributing Baselines](https://flower.dev/docs/contributing-baselines.html)\n\n## Flower Usage Examples\n\nSeveral code examples show different usage scenarios of Flower (in combination with popular machine learning frameworks such as PyTorch or TensorFlow).\n\nQuickstart examples:\n\n* [Quickstart (TensorFlow)](https://github.com/adap/flower/tree/main/examples/quickstart_tensorflow)\n* [Quickstart (PyTorch)](https://github.com/adap/flower/tree/main/examples/quickstart_pytorch)\n* [Quickstart (Hugging Face)](https://github.com/adap/flower/tree/main/examples/quickstart_huggingface)\n* [Quickstart (PyTorch Lightning)](https://github.com/adap/flower/tree/main/examples/quickstart_pytorch_lightning)\n* [Quickstart (fastai)](https://github.com/adap/flower/tree/main/examples/quickstart_fastai)\n* [Quickstart (Pandas)](https://github.com/adap/flower/tree/main/examples/quickstart_pandas)\n* [Quickstart (MXNet)](https://github.com/adap/flower/tree/main/examples/quickstart_mxnet)\n* [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/quickstart_jax)\n* [Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist)\n* [Quickstart (TFLite on Android)](https://github.com/adap/flower/tree/main/examples/android)\n\nOther [examples](https://github.com/adap/flower/tree/main/examples):\n\n* [Raspberry Pi & Nvidia Jetson Tutorial](https://github.com/adap/flower/tree/main/examples/embedded_devices)\n* [Android & TFLite](https://github.com/adap/flower/tree/main/examples/android)\n* [PyTorch: From Centralized to Federated](https://github.com/adap/flower/tree/main/examples/pytorch_from_centralized_to_federated)\n* [MXNet: From Centralized to Federated](https://github.com/adap/flower/tree/main/examples/mxnet_from_centralized_to_federated)\n* [Advanced Flower with TensorFlow/Keras](https://github.com/adap/flower/tree/main/examples/advanced_tensorflow)\n* [Advanced Flower with PyTorch](https://github.com/adap/flower/tree/main/examples/advanced_pytorch)\n* Single-Machine Simulation of Federated Learning Systems ([PyTorch](https://github.com/adap/flower/tree/main/examples/simulation_pytorch)) ([Tensorflow](https://github.com/adap/flower/tree/main/examples/simulation_tensorflow))\n\n## Community\n\nFlower is built by a wonderful community of researchers and engineers. [Join Slack](https://flower.dev/join-slack) to meet them, [contributions](#contributing-to-flower) are welcome.\n\n<a href="https://github.com/adap/flower/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=adap/flower" />\n</a>\n\n## Citation\n\nIf you publish work that uses Flower, please cite Flower as follows: \n\n```bibtex\n@article{beutel2020flower,\n  title={Flower: A Friendly Federated Learning Research Framework},\n  author={Beutel, Daniel J and Topal, Taner and Mathur, Akhil and Qiu, Xinchi and Fernandez-Marques, Javier and Gao, Yan and Sani, Lorenzo and Kwing, Hei Li and Parcollet, Titouan and Gusmão, Pedro PB de and Lane, Nicholas D}, \n  journal={arXiv preprint arXiv:2007.14390},\n  year={2020}\n}\n```\n\nPlease also consider adding your publication to the list of Flower-based publications in the docs, just open a Pull Request.\n\n## Contributing to Flower\n\nWe welcome contributions. Please see [CONTRIBUTING.md](CONTRIBUTING.md) to get started!\n',
     'author': 'The Flower Authors',
     'author_email': 'hello@flower.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://flower.dev',
```

#### html2text {}

```diff
@@ -12,15 +12,15 @@
 python_version < "3.8"': ['importlib-metadata>=4.0.0,<5.0.0'], 'rest':
 ['requests>=2.28.2,<3.0.0', 'fastapi>=0.95.0,<0.96.0',
 'starlette>=0.26.1,<0.27.0', 'uvicorn[standard]>=0.21.1,<0.22.0'],
 'simulation': ['ray[default]>=2.4.0,<3.0.0']} entry_points = \
 {'console_scripts': ['flower-client = flwr.client:run_client', 'flower-driver-
 api = flwr.server:run_driver_api', 'flower-fleet-api = flwr.server:
 run_fleet_api', 'flower-server = flwr.server:run_server']} setup_kwargs =
-{ 'name': 'flwr-nightly', 'version': '1.5.0.dev20230518', 'description':
+{ 'name': 'flwr-nightly', 'version': '1.5.0.dev20230519', 'description':
 'Flower: A Friendly Federated Learning Framework', 'long_description': '#
 Flower: A Friendly Federated Learning Framework\n\n
                           \n \n_[Flower_Website]\n\n
 \n
            \n Website |\n Blog |\n Docs |\n Conference |\n Slack\n
 
                                       \n
```

### Comparing `flwr_nightly-1.5.0.dev20230518/PKG-INFO` & `flwr_nightly-1.5.0.dev20230519/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flwr-nightly
-Version: 1.5.0.dev20230518
+Version: 1.5.0.dev20230519
 Summary: Flower: A Friendly Federated Learning Framework
 Home-page: https://flower.dev
 License: Apache-2.0
 Author: The Flower Authors
 Author-email: hello@flower.dev
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flwr-nightly Version: 1.5.0.dev20230518 Summary:
+Metadata-Version: 2.1 Name: flwr-nightly Version: 1.5.0.dev20230519 Summary:
 Flower: A Friendly Federated Learning Framework Home-page: https://flower.dev
 License: Apache-2.0 Author: The Flower Authors Author-email: hello@flower.dev
 Requires-Python: >=3.7,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Operating System :: MacOS :: MacOS X Classifier:
 Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
```

