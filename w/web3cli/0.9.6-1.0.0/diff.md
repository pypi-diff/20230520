# Comparing `tmp/web3cli-0.9.6.tar.gz` & `tmp/web3cli-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web3cli-0.9.6.tar", last modified: Sun Dec 11 20:04:43 2022, max compression
+gzip compressed data, was "web3cli-1.0.0.tar", last modified: Sat May 20 18:31:37 2023, max compression
```

## Comparing `web3cli-0.9.6.tar` & `web3cli-1.0.0.tar`

### file list

```diff
@@ -1,80 +1,165 @@
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1069 2022-10-24 15:49:55.999119 web3cli-0.9.6/LICENSE
--rw-r--r--   0 coccoinomane   (502) staff       (20)     8703 2022-12-11 19:42:34.523799 web3cli-0.9.6/README.md
--rw-r--r--   0 coccoinomane   (502) staff       (20)     2376 2022-12-11 20:04:17.698155 web3cli-0.9.6/pyproject.toml
--rw-r--r--   0 coccoinomane   (502) staff       (20)     6148 2022-11-13 07:56:22.807127 web3cli-0.9.6/src/web3cli/.DS_Store
--rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-11-18 22:32:14.016225 web3cli-0.9.6/src/web3cli/__init__.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-10-24 15:34:40.198985 web3cli-0.9.6/src/web3cli/controllers/__init__.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     2052 2022-12-03 21:33:10.100716 web3cli-0.9.6/src/web3cli/controllers/base_controller.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     2359 2022-12-03 21:55:45.786745 web3cli-0.9.6/src/web3cli/controllers/config_controller.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1108 2022-12-03 10:52:07.292763 web3cli-0.9.6/src/web3cli/controllers/controller.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     2538 2022-12-03 11:08:30.876281 web3cli-0.9.6/src/web3cli/controllers/db/address_controller.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     4018 2022-12-03 11:08:39.937873 web3cli-0.9.6/src/web3cli/controllers/db/chain_controller.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1232 2022-12-11 20:02:34.012601 web3cli-0.9.6/src/web3cli/controllers/db/db_base_controller.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     3548 2022-12-03 11:09:01.224477 web3cli-0.9.6/src/web3cli/controllers/db/rpc_controller.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     4205 2022-12-03 11:09:14.366589 web3cli-0.9.6/src/web3cli/controllers/db/signer_controller.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     3084 2022-12-03 21:56:25.229723 web3cli-0.9.6/src/web3cli/controllers/db/tx_controller.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     2126 2022-12-03 10:51:06.945706 web3cli-0.9.6/src/web3cli/controllers/key_controller.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1299 2022-12-03 12:55:44.118274 web3cli-0.9.6/src/web3cli/controllers/misc_controller.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     2279 2022-12-03 12:47:55.890188 web3cli-0.9.6/src/web3cli/controllers/send_controller.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      120 2022-11-03 17:39:28.958124 web3cli-0.9.6/src/web3cli/core/__init__.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1194 2022-12-01 17:32:47.153512 web3cli-0.9.6/src/web3cli/core/exceptions.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-11-03 17:39:28.958845 web3cli-0.9.6/src/web3cli/core/helpers/__init__.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1715 2022-12-01 17:32:41.983115 web3cli-0.9.6/src/web3cli/core/helpers/client_factory.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1059 2022-11-13 21:16:43.600419 web3cli-0.9.6/src/web3cli/core/helpers/crypto.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      879 2022-12-01 15:14:54.384063 web3cli-0.9.6/src/web3cli/core/helpers/database.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      434 2022-11-28 18:04:28.138080 web3cli-0.9.6/src/web3cli/core/helpers/format.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      562 2022-12-11 19:57:58.584818 web3cli-0.9.6/src/web3cli/core/helpers/input.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      327 2022-11-05 10:06:17.379240 web3cli-0.9.6/src/web3cli/core/helpers/os.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      516 2022-11-21 18:11:44.306582 web3cli-0.9.6/src/web3cli/core/helpers/rpc.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1209 2022-12-01 15:48:21.715482 web3cli-0.9.6/src/web3cli/core/helpers/yaml.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-11-05 09:21:32.723633 web3cli-0.9.6/src/web3cli/core/models/__init__.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     3449 2022-12-03 21:05:04.266707 web3cli-0.9.6/src/web3cli/core/models/address.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      771 2022-12-01 16:54:00.585577 web3cli-0.9.6/src/web3cli/core/models/base_model.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     5219 2022-12-03 21:02:52.946105 web3cli-0.9.6/src/web3cli/core/models/chain.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1556 2022-12-01 17:28:54.846253 web3cli-0.9.6/src/web3cli/core/models/signer.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1056 2022-12-02 22:09:26.397612 web3cli-0.9.6/src/web3cli/core/models/timestamps_model.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     2966 2022-12-03 21:05:11.976714 web3cli-0.9.6/src/web3cli/core/models/tx.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1036 2022-12-02 20:11:58.691980 web3cli-0.9.6/src/web3cli/core/models/types.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)       48 2022-11-18 22:43:37.360850 web3cli-0.9.6/src/web3cli/core/seeds/__init__.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1299 2022-12-03 17:12:38.552472 web3cli-0.9.6/src/web3cli/core/seeds/chain_seeds.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)       60 2022-11-20 21:14:50.670605 web3cli-0.9.6/src/web3cli/core/types.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-10-24 15:34:40.191413 web3cli-0.9.6/src/web3cli/helpers/__init__.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     3007 2022-12-03 11:09:23.233451 web3cli-0.9.6/src/web3cli/helpers/args.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      929 2022-12-03 11:09:26.353421 web3cli-0.9.6/src/web3cli/helpers/client_factory.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1258 2022-12-01 15:48:40.508984 web3cli-0.9.6/src/web3cli/helpers/config.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      936 2022-11-24 17:21:33.254156 web3cli-0.9.6/src/web3cli/helpers/crypto.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1124 2022-12-11 20:00:04.245201 web3cli-0.9.6/src/web3cli/helpers/database.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      347 2022-11-21 18:39:07.034800 web3cli-0.9.6/src/web3cli/helpers/misc.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      808 2022-12-03 18:29:40.979538 web3cli-0.9.6/src/web3cli/helpers/render.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     2113 2022-11-21 18:06:06.928432 web3cli-0.9.6/src/web3cli/helpers/send.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      434 2022-12-11 20:04:05.874534 web3cli-0.9.6/src/web3cli/helpers/version.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     2094 2022-11-28 18:19:24.889986 web3cli-0.9.6/src/web3cli/hooks.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     3897 2022-12-11 19:56:44.416663 web3cli-0.9.6/src/web3cli/main.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-10-24 15:34:40.196707 web3cli-0.9.6/src/web3cli/templates/__init__.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)       82 2022-12-03 16:44:27.366677 web3cli-0.9.6/src/web3cli/templates/balance.jinja2
--rw-r--r--   0 coccoinomane   (502) staff       (20)     6148 2022-12-03 17:32:49.089202 web3cli-0.9.6/tests/.DS_Store
--rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-11-10 21:50:51.296564 web3cli-0.9.6/tests/__init__.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     2463 2022-12-03 21:58:57.495576 web3cli-0.9.6/tests/brownie/build/tests.json
--rw-r--r--   0 coccoinomane   (502) staff       (20)       50 2022-12-03 17:35:04.016328 web3cli-0.9.6/tests/brownie/contracts/.gitignore
--rw-r--r--   0 coccoinomane   (502) staff       (20)     5737 2022-12-02 22:06:52.240730 web3cli-0.9.6/tests/conftest.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-11-10 21:50:51.297637 web3cli-0.9.6/tests/controllers/__init__.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     3800 2022-12-03 11:08:00.178773 web3cli-0.9.6/tests/controllers/db/test_address.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     3205 2022-12-03 11:02:45.632355 web3cli-0.9.6/tests/controllers/db/test_chain.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     3778 2022-12-03 10:58:08.499190 web3cli-0.9.6/tests/controllers/db/test_rpc.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     5040 2022-12-03 11:08:03.254225 web3cli-0.9.6/tests/controllers/db/test_signer.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     2643 2022-12-03 10:58:53.760955 web3cli-0.9.6/tests/controllers/db/test_tx.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     3030 2022-12-03 10:56:33.399744 web3cli-0.9.6/tests/controllers/test_base.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1816 2022-11-24 17:21:33.295121 web3cli-0.9.6/tests/controllers/test_key.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-11-10 21:50:51.301380 web3cli-0.9.6/tests/core/__init__.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-11-10 21:50:51.301610 web3cli-0.9.6/tests/core/helpers/__init__.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      530 2022-11-10 21:50:51.303151 web3cli-0.9.6/tests/core/helpers/test_crypto.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1183 2022-11-13 21:19:59.445849 web3cli-0.9.6/tests/helper.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-11-10 21:50:51.303802 web3cli-0.9.6/tests/helpers/__init__.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1676 2022-12-03 10:54:01.164673 web3cli-0.9.6/tests/helpers/test_client_factory.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      675 2022-11-21 18:49:29.825823 web3cli-0.9.6/tests/helpers/test_crypto.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1395 2022-11-23 09:21:24.664025 web3cli-0.9.6/tests/main.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)        0 2022-11-10 21:50:51.305787 web3cli-0.9.6/tests/resolvers/__init__.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     1514 2022-12-01 18:58:26.365291 web3cli-0.9.6/tests/resolvers/test_resolve_address.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)     3219 2022-12-03 17:14:55.639133 web3cli-0.9.6/tests/seeder.py
--rw-r--r--   0 coccoinomane   (502) staff       (20)      385 2022-12-03 11:01:40.965568 web3cli-0.9.6/tests/test_main.py
--rw-------   0 coccoinomane   (502) staff       (20)     9162 2022-12-11 20:04:43.466283 web3cli-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-10-24 15:49:55.999119 web3cli-1.0.0/LICENSE
+-rw-r--r--   0        0        0    10684 2023-05-20 18:28:19.647207 web3cli-1.0.0/README.md
+-rw-r--r--   0        0        0     3765 2023-05-20 18:27:43.878456 web3cli-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6148 2022-11-13 07:56:22.807127 web3cli-1.0.0/src/web3cli/.DS_Store
+-rw-r--r--   0        0        0        0 2022-11-18 22:32:14.016225 web3cli-1.0.0/src/web3cli/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-24 15:34:40.198985 web3cli-1.0.0/src/web3cli/controllers/__init__.py
+-rw-r--r--   0        0        0     4699 2023-05-20 18:26:40.921508 web3cli-1.0.0/src/web3cli/controllers/abi_controller.py
+-rw-r--r--   0        0        0     2005 2023-05-17 11:19:52.195517 web3cli-1.0.0/src/web3cli/controllers/app_key_controller.py
+-rw-r--r--   0        0        0     1171 2023-05-20 18:17:47.037441 web3cli-1.0.0/src/web3cli/controllers/base_controller.py
+-rw-r--r--   0        0        0     3116 2023-05-20 18:17:47.038161 web3cli-1.0.0/src/web3cli/controllers/call_controller.py
+-rw-r--r--   0        0        0     2372 2023-05-20 18:17:47.039146 web3cli-1.0.0/src/web3cli/controllers/config_controller.py
+-rw-r--r--   0        0        0     1109 2022-12-17 18:21:46.704206 web3cli-1.0.0/src/web3cli/controllers/controller.py
+-rw-r--r--   0        0        0        0 2023-03-25 21:06:13.922427 web3cli-1.0.0/src/web3cli/controllers/crud/__init__.py
+-rw-r--r--   0        0        0     2540 2023-05-20 18:17:47.040161 web3cli-1.0.0/src/web3cli/controllers/crud/address_controller.py
+-rw-r--r--   0        0        0     4429 2023-05-20 18:17:47.040993 web3cli-1.0.0/src/web3cli/controllers/crud/chain_controller.py
+-rw-r--r--   0        0        0     4795 2023-05-20 18:17:47.041550 web3cli-1.0.0/src/web3cli/controllers/crud/contract_controller.py
+-rw-r--r--   0        0        0     3052 2023-05-20 18:17:47.042307 web3cli-1.0.0/src/web3cli/controllers/crud/history_controller.py
+-rw-r--r--   0        0        0     2958 2023-05-20 18:17:47.043048 web3cli-1.0.0/src/web3cli/controllers/crud/rpc_controller.py
+-rw-r--r--   0        0        0     5286 2023-05-20 18:17:47.043661 web3cli-1.0.0/src/web3cli/controllers/crud/signer_controller.py
+-rw-r--r--   0        0        0     1346 2023-04-30 17:34:17.185968 web3cli-1.0.0/src/web3cli/controllers/db_controller.py
+-rw-r--r--   0        0        0     1433 2023-05-18 10:41:28.547083 web3cli-1.0.0/src/web3cli/controllers/keyfile_controller.py
+-rw-r--r--   0        0        0     3834 2023-05-20 18:17:47.044611 web3cli-1.0.0/src/web3cli/controllers/misc_controller.py
+-rw-r--r--   0        0        0     2359 2023-05-20 18:17:47.045353 web3cli-1.0.0/src/web3cli/controllers/send_controller.py
+-rw-r--r--   0        0        0     6878 2023-05-20 18:17:47.046015 web3cli-1.0.0/src/web3cli/controllers/swap_controller.py
+-rw-r--r--   0        0        0     3346 2023-05-20 18:17:47.046702 web3cli-1.0.0/src/web3cli/controllers/token_controller.py
+-rw-r--r--   0        0        0     2862 2023-05-20 18:17:47.047364 web3cli-1.0.0/src/web3cli/controllers/transact_controller.py
+-rw-r--r--   0        0        0     1408 2023-05-20 18:17:47.048248 web3cli-1.0.0/src/web3cli/controllers/tx_controller.py
+-rw-r--r--   0        0        0      341 2023-05-20 18:17:47.049010 web3cli-1.0.0/src/web3cli/exceptions.py
+-rw-r--r--   0        0        0        0 2022-10-24 15:34:40.191413 web3cli-1.0.0/src/web3cli/helpers/__init__.py
+-rw-r--r--   0        0        0    15889 2023-05-20 18:17:47.050167 web3cli-1.0.0/src/web3cli/helpers/args.py
+-rw-r--r--   0        0        0     2198 2023-05-20 18:17:47.051274 web3cli-1.0.0/src/web3cli/helpers/client_factory.py
+-rw-r--r--   0        0        0     1252 2022-12-28 16:44:58.644508 web3cli-1.0.0/src/web3cli/helpers/config.py
+-rw-r--r--   0        0        0     2092 2023-05-18 11:14:15.678582 web3cli-1.0.0/src/web3cli/helpers/crypto.py
+-rw-r--r--   0        0        0     1228 2023-02-11 17:24:24.959766 web3cli-1.0.0/src/web3cli/helpers/database.py
+-rw-r--r--   0        0        0     1261 2023-05-18 16:19:29.530143 web3cli-1.0.0/src/web3cli/helpers/render.py
+-rw-r--r--   0        0        0     4548 2023-05-20 18:17:47.052264 web3cli-1.0.0/src/web3cli/helpers/send.py
+-rw-r--r--   0        0        0     2178 2023-05-20 18:17:47.053233 web3cli-1.0.0/src/web3cli/helpers/signer.py
+-rw-r--r--   0        0        0     2132 2023-04-07 18:14:01.616983 web3cli-1.0.0/src/web3cli/helpers/tx.py
+-rw-r--r--   0        0        0      435 2023-05-20 18:27:43.878628 web3cli-1.0.0/src/web3cli/helpers/version.py
+-rw-r--r--   0        0        0     2595 2023-02-12 21:33:06.910919 web3cli-1.0.0/src/web3cli/hooks.py
+-rw-r--r--   0        0        0     7036 2023-05-20 18:17:47.054261 web3cli-1.0.0/src/web3cli/main.py
+-rw-r--r--   0        0        0        0 2023-01-29 11:30:42.897043 web3cli-1.0.0/src/web3cli/templates/__init__.py
+-rw-r--r--   0        0        0      243 2023-01-29 11:41:03.173746 web3cli-1.0.0/src/web3cli/templates/balance.jinja2
+-rw-r--r--   0        0        0      120 2022-11-03 17:39:28.958124 web3cli-1.0.0/src/web3core/__init__.py
+-rw-r--r--   0        0        0       72 2023-02-19 11:02:13.393953 web3cli-1.0.0/src/web3core/constants.py
+-rw-r--r--   0        0        0       90 2023-01-18 19:29:57.558367 web3cli-1.0.0/src/web3core/db.py
+-rw-r--r--   0        0        0     1762 2023-01-18 20:41:45.295870 web3cli-1.0.0/src/web3core/exceptions.py
+-rw-r--r--   0        0        0        0 2022-11-03 17:39:28.958845 web3cli-1.0.0/src/web3core/helpers/__init__.py
+-rw-r--r--   0        0        0     9448 2023-04-07 18:14:01.618698 web3cli-1.0.0/src/web3core/helpers/abi.py
+-rw-r--r--   0        0        0     1148 2023-05-17 09:47:21.910041 web3cli-1.0.0/src/web3core/helpers/blocks.py
+-rw-r--r--   0        0        0     3405 2023-05-20 18:17:47.055119 web3cli-1.0.0/src/web3core/helpers/client_factory.py
+-rw-r--r--   0        0        0     1060 2022-12-17 18:21:46.707584 web3cli-1.0.0/src/web3core/helpers/crypto.py
+-rw-r--r--   0        0        0      714 2023-02-11 17:32:11.986925 web3cli-1.0.0/src/web3core/helpers/database.py
+-rw-r--r--   0        0        0     1582 2023-04-07 18:14:01.619156 web3cli-1.0.0/src/web3core/helpers/dex.py
+-rw-r--r--   0        0        0      434 2022-12-19 20:01:36.985004 web3cli-1.0.0/src/web3core/helpers/format.py
+-rw-r--r--   0        0        0     2413 2023-05-18 08:42:25.689036 web3cli-1.0.0/src/web3core/helpers/misc.py
+-rw-r--r--   0        0        0      532 2022-12-16 06:48:29.391730 web3cli-1.0.0/src/web3core/helpers/os.py
+-rw-r--r--   0        0        0     1790 2023-04-07 18:14:01.619658 web3cli-1.0.0/src/web3core/helpers/resolve.py
+-rw-r--r--   0        0        0      515 2022-12-17 18:21:46.708465 web3cli-1.0.0/src/web3core/helpers/rpc.py
+-rw-r--r--   0        0        0     2158 2023-01-14 21:27:16.459461 web3cli-1.0.0/src/web3core/helpers/seed.py
+-rw-r--r--   0        0        0     4697 2023-04-07 18:14:01.620145 web3cli-1.0.0/src/web3core/helpers/tx.py
+-rw-r--r--   0        0        0      345 2023-01-29 18:12:45.184768 web3cli-1.0.0/src/web3core/helpers/validation.py
+-rw-r--r--   0        0        0     1207 2022-12-28 16:44:58.644659 web3cli-1.0.0/src/web3core/helpers/yaml.py
+-rw-r--r--   0        0        0      424 2023-01-18 19:29:57.562778 web3cli-1.0.0/src/web3core/models/__init__.py
+-rw-r--r--   0        0        0     1790 2023-01-18 19:29:57.563744 web3cli-1.0.0/src/web3core/models/address.py
+-rw-r--r--   0        0        0     3433 2023-05-20 18:17:47.055757 web3cli-1.0.0/src/web3core/models/base_model.py
+-rw-r--r--   0        0        0     4923 2023-03-25 21:22:51.453293 web3cli-1.0.0/src/web3core/models/chain.py
+-rw-r--r--   0        0        0     4255 2023-02-19 09:09:21.024153 web3cli-1.0.0/src/web3core/models/contract.py
+-rw-r--r--   0        0        0     1405 2023-05-18 09:25:11.305140 web3cli-1.0.0/src/web3core/models/signer.py
+-rw-r--r--   0        0        0     1054 2022-12-28 16:44:59.161817 web3cli-1.0.0/src/web3core/models/timestamps_model.py
+-rw-r--r--   0        0        0     2550 2022-12-28 16:44:59.162568 web3cli-1.0.0/src/web3core/models/tx.py
+-rw-r--r--   0        0        0     1449 2023-01-18 19:29:57.566552 web3cli-1.0.0/src/web3core/models/types.py
+-rw-r--r--   0        0        0       48 2022-11-18 22:43:37.360850 web3cli-1.0.0/src/web3core/seeds/__init__.py
+-rw-r--r--   0        0        0     2663 2023-04-07 18:14:01.620586 web3cli-1.0.0/src/web3core/seeds/chain_seeds.py
+-rw-r--r--   0        0        0      360 2023-02-19 10:31:30.690836 web3cli-1.0.0/src/web3core/seeds/contract_seeds.py
+-rw-r--r--   0        0        0    49489 2023-02-19 09:09:21.024661 web3cli-1.0.0/src/web3core/seeds/contract_type_seeds.py
+-rw-r--r--   0        0        0     9720 2023-02-27 16:48:07.675984 web3cli-1.0.0/src/web3core/seeds/contracts/arb_contract_seeds.py
+-rw-r--r--   0        0        0     1881 2023-02-27 19:24:54.136969 web3cli-1.0.0/src/web3core/seeds/contracts/avax_contract_seeds.py
+-rw-r--r--   0        0        0      480 2023-02-27 16:48:16.132079 web3cli-1.0.0/src/web3core/seeds/contracts/bnb_contract_seeds.py
+-rw-r--r--   0        0        0     1579 2023-02-27 16:48:24.467166 web3cli-1.0.0/src/web3core/seeds/contracts/eth_contract_seeds.py
+-rw-r--r--   0        0        0     1448 2023-02-19 10:37:03.165028 web3cli-1.0.0/src/web3core/types.py
+-rw-r--r--   0        0        0     6148 2023-02-28 16:18:46.901853 web3cli-1.0.0/tests/.DS_Store
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.296564 web3cli-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0    10244 2023-02-28 16:18:44.627516 web3cli-1.0.0/tests/ape/.DS_Store
+-rw-r--r--   0        0        0     2609 2023-04-06 17:43:03.934034 web3cli-1.0.0/tests/ape/.build/Factory_IERC20.json
+-rw-r--r--   0        0        0      536 2023-04-06 17:43:03.934442 web3cli-1.0.0/tests/ape/.build/Factory_IUniswapV2Callee.json
+-rw-r--r--   0        0        0     3605 2023-04-06 17:43:03.935802 web3cli-1.0.0/tests/ape/.build/Factory_IUniswapV2ERC20.json
+-rw-r--r--   0        0        0     2026 2023-04-06 17:43:03.936651 web3cli-1.0.0/tests/ape/.build/Factory_IUniswapV2Factory.json
+-rw-r--r--   0        0        0     7527 2023-04-06 17:43:03.938968 web3cli-1.0.0/tests/ape/.build/Factory_IUniswapV2Pair.json
+-rw-r--r--   0        0        0      862 2023-04-06 17:43:03.939241 web3cli-1.0.0/tests/ape/.build/Factory_Math.json
+-rw-r--r--   0        0        0      866 2023-04-06 17:43:03.939527 web3cli-1.0.0/tests/ape/.build/Factory_SafeMath.json
+-rw-r--r--   0        0        0      867 2023-04-06 17:43:03.939780 web3cli-1.0.0/tests/ape/.build/Factory_UQ112x112.json
+-rw-r--r--   0        0        0     2609 2023-04-06 17:43:03.916870 web3cli-1.0.0/tests/ape/.build/Router_IERC20.json
+-rw-r--r--   0        0        0     2026 2023-04-06 17:43:03.917744 web3cli-1.0.0/tests/ape/.build/Router_IUniswapV2Factory.json
+-rw-r--r--   0        0        0     7527 2023-04-06 17:43:03.920204 web3cli-1.0.0/tests/ape/.build/Router_IUniswapV2Pair.json
+-rw-r--r--   0        0        0     9213 2023-04-06 17:43:03.922797 web3cli-1.0.0/tests/ape/.build/Router_IUniswapV2Router01.json
+-rw-r--r--   0        0        0    11845 2023-04-06 17:43:03.926066 web3cli-1.0.0/tests/ape/.build/Router_IUniswapV2Router02.json
+-rw-r--r--   0        0        0      683 2023-04-06 17:43:03.926558 web3cli-1.0.0/tests/ape/.build/Router_IWETH.json
+-rw-r--r--   0        0        0      872 2023-04-06 17:43:03.926867 web3cli-1.0.0/tests/ape/.build/Router_SafeMath.json
+-rw-r--r--   0        0        0      879 2023-04-06 17:43:03.927162 web3cli-1.0.0/tests/ape/.build/Router_TransferHelper.json
+-rw-r--r--   0        0        0      881 2023-04-06 17:43:03.927462 web3cli-1.0.0/tests/ape/.build/Router_UniswapV2Library.json
+-rw-r--r--   0        0        0    14895 2023-04-06 17:43:03.932635 web3cli-1.0.0/tests/ape/.build/Token.json
+-rw-r--r--   0        0        0      791 2023-04-06 17:43:03.932974 web3cli-1.0.0/tests/ape/.build/Token_SafeMath.json
+-rw-r--r--   0        0        0    14014 2023-04-06 17:43:03.941015 web3cli-1.0.0/tests/ape/.build/UniswapV2ERC20.json
+-rw-r--r--   0        0        0    46097 2023-04-06 17:43:03.942289 web3cli-1.0.0/tests/ape/.build/UniswapV2Factory.json
+-rw-r--r--   0        0        0    44784 2023-04-06 17:43:03.944616 web3cli-1.0.0/tests/ape/.build/UniswapV2Pair.json
+-rw-r--r--   0        0        0    85730 2023-04-06 17:43:03.931232 web3cli-1.0.0/tests/ape/.build/UniswapV2Router02.json
+-rw-r--r--   0        0        0   324962 2023-05-20 18:27:45.835411 web3cli-1.0.0/tests/ape/.build/__local__.json
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.620721 web3cli-1.0.0/tests/ape/__init__.py
+-rw-r--r--   0        0        0     6148 2023-02-28 16:18:44.554061 web3cli-1.0.0/tests/ape/contracts/.DS_Store
+-rw-r--r--   0        0        0     4101 2023-04-07 18:14:01.621230 web3cli-1.0.0/tests/ape/contracts/token/Token.sol
+-rw-r--r--   0        0        0      646 2023-04-07 18:14:01.621775 web3cli-1.0.0/tests/ape/contracts/token/Token_SafeMath.sol
+-rw-r--r--   0        0        0     6148 2023-02-28 15:31:57.501753 web3cli-1.0.0/tests/ape/contracts/uniswap/.DS_Store
+-rw-r--r--   0        0        0    21725 2023-04-07 18:14:01.622322 web3cli-1.0.0/tests/ape/contracts/uniswap/UniswapV2Factory.sol
+-rw-r--r--   0        0        0    34078 2023-04-07 18:14:01.622848 web3cli-1.0.0/tests/ape/contracts/uniswap/UniswapV2Router02.sol
+-rw-r--r--   0        0        0      236 2023-04-07 18:14:01.623357 web3cli-1.0.0/tests/ape/scripts/__init__.py
+-rw-r--r--   0        0        0      347 2023-04-07 18:14:01.623719 web3cli-1.0.0/tests/ape/scripts/db.py
+-rw-r--r--   0        0        0      200 2023-04-07 18:14:01.624050 web3cli-1.0.0/tests/ape/scripts/token.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.624201 web3cli-1.0.0/tests/ape/tests/__init__.py
+-rw-r--r--   0        0        0    13902 2023-04-07 18:14:01.624793 web3cli-1.0.0/tests/ape/tests/fixtures.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.624997 web3cli-1.0.0/tests/ape/tests/helpers/__init__.py
+-rw-r--r--   0        0        0      371 2023-04-07 18:14:01.625481 web3cli-1.0.0/tests/ape/tests/helpers/ape.py
+-rw-r--r--   0        0        0      881 2023-04-07 18:14:01.625860 web3cli-1.0.0/tests/ape/tests/helpers/token.py
+-rw-r--r--   0        0        0     3790 2023-04-07 18:14:01.626436 web3cli-1.0.0/tests/ape/tests/helpers/uniswap.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.626729 web3cli-1.0.0/tests/ape/tests/token/__init__.py
+-rw-r--r--   0        0        0     1983 2023-04-07 18:14:01.627373 web3cli-1.0.0/tests/ape/tests/token/test_token_approve.py
+-rw-r--r--   0        0        0     2876 2023-04-07 18:14:01.627765 web3cli-1.0.0/tests/ape/tests/token/test_token_transfer.py
+-rw-r--r--   0        0        0     6467 2023-04-07 18:14:01.628071 web3cli-1.0.0/tests/ape/tests/token/test_token_transferFrom.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.628193 web3cli-1.0.0/tests/ape/tests/uniswap/__init__.py
+-rw-r--r--   0        0        0     4193 2023-04-07 18:14:01.628531 web3cli-1.0.0/tests/ape/tests/uniswap/test_v2_add_liquidity.py
+-rw-r--r--   0        0        0      794 2023-04-07 18:14:01.628890 web3cli-1.0.0/tests/ape/tests/uniswap/test_v2_create_pair.py
+-rw-r--r--   0        0        0      487 2023-04-07 18:14:01.629400 web3cli-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     1130 2023-04-07 12:55:47.114434 web3cli-1.0.0/tests/helper.py
+-rw-r--r--   0        0        0     3240 2023-04-07 18:14:01.629815 web3cli-1.0.0/tests/seed.py
+-rw-r--r--   0        0        0        0 2022-12-28 17:01:25.438908 web3cli-1.0.0/tests/web3cli/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.297637 web3cli-1.0.0/tests/web3cli/controllers/__init__.py
+-rw-r--r--   0        0        0     3754 2023-05-20 18:17:47.056601 web3cli-1.0.0/tests/web3cli/controllers/crud/test_address_controller.py
+-rw-r--r--   0        0        0     3517 2023-05-20 18:17:47.057300 web3cli-1.0.0/tests/web3cli/controllers/crud/test_chain_controller.py
+-rw-r--r--   0        0        0     8222 2023-05-20 18:17:47.058165 web3cli-1.0.0/tests/web3cli/controllers/crud/test_contract_controller.py
+-rw-r--r--   0        0        0     2870 2023-05-20 18:17:47.058996 web3cli-1.0.0/tests/web3cli/controllers/crud/test_history_controller.py
+-rw-r--r--   0        0        0     3762 2023-05-20 18:17:47.059822 web3cli-1.0.0/tests/web3cli/controllers/crud/test_rpc_controller.py
+-rw-r--r--   0        0        0     4933 2023-05-20 18:17:47.060483 web3cli-1.0.0/tests/web3cli/controllers/crud/test_signer_controller.py
+-rw-r--r--   0        0        0     1848 2023-05-18 10:32:19.351291 web3cli-1.0.0/tests/web3cli/controllers/test_appkey_controller.py
+-rw-r--r--   0        0        0     6339 2023-05-20 18:17:47.061301 web3cli-1.0.0/tests/web3cli/controllers/test_call_controller.py
+-rw-r--r--   0        0        0     1041 2023-03-25 21:24:05.581746 web3cli-1.0.0/tests/web3cli/controllers/test_db_controller.py
+-rw-r--r--   0        0        0     1702 2023-05-18 11:14:40.025134 web3cli-1.0.0/tests/web3cli/controllers/test_keyfile_controller.py
+-rw-r--r--   0        0        0     5688 2023-05-20 18:17:47.062163 web3cli-1.0.0/tests/web3cli/controllers/test_misc_controller.py
+-rw-r--r--   0        0        0     3415 2023-05-20 18:17:47.063638 web3cli-1.0.0/tests/web3cli/controllers/test_send_controller.py
+-rw-r--r--   0        0        0     9593 2023-05-20 18:17:47.064509 web3cli-1.0.0/tests/web3cli/controllers/test_transact_controller.py
+-rw-r--r--   0        0        0     1265 2023-04-07 18:14:01.631776 web3cli-1.0.0/tests/web3cli/controllers/test_tx_controller.py
+-rw-r--r--   0        0        0     1293 2023-04-07 18:14:01.632176 web3cli-1.0.0/tests/web3cli/fixtures.py
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.303802 web3cli-1.0.0/tests/web3cli/helpers/__init__.py
+-rw-r--r--   0        0        0      684 2022-12-28 17:00:06.651527 web3cli-1.0.0/tests/web3cli/helpers/test_crypto_helper.py
+-rw-r--r--   0        0        0     1455 2023-02-12 12:11:39.416778 web3cli-1.0.0/tests/web3cli/main.py
+-rw-r--r--   0        0        0     1171 2023-02-11 18:15:39.713968 web3cli-1.0.0/tests/web3cli/test_db.py
+-rw-r--r--   0        0        0      393 2023-02-11 18:16:36.584225 web3cli-1.0.0/tests/web3cli/test_main.py
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.301380 web3cli-1.0.0/tests/web3core/__init__.py
+-rw-r--r--   0        0        0     5362 2023-05-18 11:01:18.894137 web3cli-1.0.0/tests/web3core/fixtures.py
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.301610 web3cli-1.0.0/tests/web3core/helpers/__init__.py
+-rw-r--r--   0        0        0     8923 2023-01-28 12:36:51.002666 web3cli-1.0.0/tests/web3core/helpers/test_abi_helper.py
+-rw-r--r--   0        0        0      528 2022-12-28 16:44:57.745951 web3cli-1.0.0/tests/web3core/helpers/test_crypto_helper.py
+-rw-r--r--   0        0        0     4807 2023-02-19 09:09:21.027684 web3cli-1.0.0/tests/web3core/helpers/test_resolve_address_helper.py
+-rw-r--r--   0        0        0     1022 2023-01-29 17:56:31.054122 web3cli-1.0.0/tests/web3core/helpers/test_validation_helper.py
+-rw-r--r--   0        0        0     1783 2023-01-14 21:27:16.475375 web3cli-1.0.0/tests/web3core/models/test_contract_model.py
+-rw-r--r--   0        0        0    11141 1970-01-01 00:00:00.000000 web3cli-1.0.0/PKG-INFO
```

### Comparing `web3cli-0.9.6/LICENSE` & `web3cli-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.6/src/web3cli/.DS_Store` & `web3cli-1.0.0/src/web3cli/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-0.9.6/src/web3cli/controllers/config_controller.py` & `web3cli-1.0.0/src/web3cli/controllers/config_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,38 @@
+import argparse
+
 from cement import ex
+
 from web3cli.controllers.controller import Controller
 from web3cli.helpers.config import update_setting_in_config_file
-import argparse
 
 
 class ConfigController(Controller):
     """Handler of the `w3 config` commands"""
 
     class Meta:
         label = "config"
         help = "show, add or edit web3cli's setting values"
         stacked_type = "nested"
         stacked_on = "base"
+        aliases = ["option"]
 
     @ex(
         help="show the value of the given setting. If no setting is given, show all settings",
         arguments=[
             (
                 ["setting"],
                 {
                     "help": "setting to inspect, for example 'default_chain'",
                     "nargs": "?",
                 },
             ),
         ],
     )
     def get(self) -> None:
-        pass
         if self.app.pargs.setting:
             self.app.print(self.app.config.get("web3cli", self.app.pargs.setting))
         else:
             output = {}
             all_config = self.app.config.get_dict()
             for section in ["web3cli"]:
                 output[section] = all_config[section]
@@ -44,15 +46,15 @@
                 {
                     "help": "setting to set, for example 'default_chain'",
                 },
             ),
             (
                 ["value"],
                 {
-                    "help": "value for the setting, for example 'ethereum'",
+                    "help": "value for the setting, for example 'eth'",
                 },
             ),
             (
                 ["-g", "--global"],
                 {
                     "help": "whether to save the setting globally (default) or locally",
                     "dest": "is_global",
```

### Comparing `web3cli-0.9.6/src/web3cli/controllers/controller.py` & `web3cli-1.0.0/src/web3cli/controllers/controller.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any
+
+from cement import App
 from cement import Controller as CementController
 from cement.core.config import ConfigInterface
-from cement import App
 
 
 class Controller(CementController):
     """Extend this class to define new commands"""
 
     def _default(self) -> None:
         """Default action if no sub-command is passed."""
```

### Comparing `web3cli-0.9.6/src/web3cli/controllers/db/address_controller.py` & `web3cli-1.0.0/src/web3cli/controllers/crud/address_controller.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 from cement import ex
+
 from web3cli.controllers.controller import Controller
-from web3cli.core.models.address import Address
-from web3cli.core.exceptions import Web3CliError
-from web3cli.helpers.render import render_table
+from web3cli.exceptions import Web3CliError
+from web3cli.helpers.render import render_json, render_table
+from web3core.models.address import Address
 
 
 class AddressController(Controller):
-    """Handler of the `w3 db address` commands"""
+    """Handler of the `w3 address` CRUD commands"""
 
     class Meta:
         label = "address"
-        help = "add, list or delete addresses"
+        help = "add, edit, list or delete addresses"
         stacked_type = "nested"
-        stacked_on = "db"
+        stacked_on = "base"
 
     @ex(help="list address")
     def list(self) -> None:
         render_table(
             self.app,
             data=[
                 [a["name"], a["address"]]
                 for a in Address.get_all_as_dicts(Address.name)
             ],
             headers=["NAME", "ADDRESS"],
             wrap=42,
         )
 
     @ex(
-        help="show an address by its name",
+        help="show the details of the given address by name",
         arguments=[
             (["name"], {"help": "name of the address to show"}),
         ],
     )
     def get(self) -> None:
-        self.app.print(Address.get_address(self.app.pargs.name))
+        render_json(self.app, Address.get_as_dict(Address.name == self.app.pargs.name))
 
     @ex(
         help="add a new address",
-        aliases=["pippo pippa"],
         arguments=[
             (["name"], {"help": "name of the address"}),
             (["address"], {"help": "blockchain address (0x...)"}),
-            (["-d", "--description"], {"action": "store"}),
+            (["-d", "--desc"], {"action": "store"}),
             (
                 ["-u", "--update"],
                 {
                     "help": "if an address with the same name is present, overwrite it",
                     "action": "store_true",
                 },
             ),
@@ -54,15 +54,15 @@
     def add(self) -> None:
         address = Address.get_by_name(self.app.pargs.name)
         if not address or self.app.pargs.update:
             Address.upsert(
                 {
                     "name": self.app.pargs.name,
                     "address": self.app.pargs.address,
-                    "description": self.app.pargs.description,
+                    "desc": self.app.pargs.desc,
                 },
                 logger=self.app.log.info,
             )
         else:
             raise Web3CliError(
                 f"Address '{self.app.pargs.name}' already exists with value {address.address}. Use `--update` or `-u` to update the address."
             )
```

### Comparing `web3cli-0.9.6/src/web3cli/controllers/db/chain_controller.py` & `web3cli-1.0.0/src/web3cli/controllers/crud/chain_controller.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from cement import ex
+
 from web3cli.controllers.controller import Controller
-from web3cli.core.exceptions import ChainNotFound, Web3CliError
-from web3cli.core.models.chain import Chain
-from web3cli.core.models.types import ChainFields
-from web3cli.core.seeds.chain_seeds import chain_seeds
-from web3cli.helpers.render import render_table
+from web3cli.exceptions import Web3CliError
+from web3cli.helpers import args
+from web3cli.helpers.render import render_json, render_table
+from web3core.exceptions import ChainNotFound
+from web3core.models.chain import Chain
+from web3core.seeds import chain_seeds
 
 
 class ChainController(Controller):
-    """Handler of the `w3 db chain` commands"""
+    """Handler of the `w3 chain` CRUD commands"""
 
     class Meta:
         label = "chain"
         help = "add, list or delete chains"
         stacked_type = "nested"
-        stacked_on = "db"
+        stacked_on = "base"
 
     @ex(
         help="add a new chain",
         arguments=[
             (["name"], {"help": "unique name for the chain"}),
             (
                 ["chain_id"],
@@ -51,22 +53,24 @@
             (
                 ["-u", "--update"],
                 {
                     "help": "if a chain with the same name is present, overwrite it",
                     "action": "store_true",
                 },
             ),
+            (["-d", "--desc"], {"action": "store"}),
         ],
     )
     def add(self) -> None:
         chain = Chain.get_by_name(self.app.pargs.name)
         if not chain or self.app.pargs.update:
             chain = Chain.upsert(
                 {
                     "name": self.app.pargs.name,
+                    "desc": self.app.pargs.desc,
                     "chain_id": self.app.pargs.chain_id,
                     "coin": self.app.pargs.coin.upper(),
                     "tx_type": self.app.pargs.tx_type,
                     "middlewares": None
                     if self.app.pargs.poa
                     else "geth_poa_middleware",
                 },
@@ -88,17 +92,24 @@
             headers=["NAME", "CHAIN ID", "COIN", "TX TYPE", "RPCS"],
             data=[
                 [c.name, c.chain_id, c.coin, c.tx_type, len(c.get_rpcs())]
                 for c in Chain.get_all(Chain.name)
             ],
         )
 
-    @ex(help="get current chain")
+    @ex(
+        help="show the details of the given chain",
+        arguments=[(["name"], {"help": "the name of the chain to look up"})],
+    )
     def get(self) -> None:
-        self.app.print(self.app.chain)
+        render_json(self.app, Chain.get_as_dict(Chain.name == self.app.pargs.name))
+
+    @ex(help="get the active chain's name", arguments=[args.chain()])
+    def active(self) -> None:
+        self.app.print(self.app.chain.name)
 
     @ex(
         help="delete a chain",
         arguments=[
             (["name"], {"help": "name of the chain to delete"}),
         ],
     )
@@ -109,11 +120,11 @@
                 f"Chain '{self.app.pargs.name}' does not exist, can't delete it"
             )
         chain.delete_instance()
         self.app.log.info(f"Chain '{self.app.pargs.name}' deleted correctly")
 
     @ex(help="preload a few chains")
     def seed(self) -> None:
-        chains = Chain.seed(chain_seeds, self.app.log.info)
+        chains = Chain.seed(chain_seeds.all, self.app.log.info)
         self.app.log.info(
-            f"Imported {len(chains)} chains, run `w3 db chain list` to show them"
+            f"Imported {len(chains)} chains, run `w3 chain list` to show them"
         )
```

### Comparing `web3cli-0.9.6/src/web3cli/controllers/db/db_base_controller.py` & `web3cli-1.0.0/src/web3cli/controllers/db_controller.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 from cement import ex
+
 from web3cli.controllers.controller import Controller
-from web3cli.core.helpers.input import yes_or_exit
-from web3cli.helpers.database import delete_db_file, get_db_file
+from web3cli.helpers import args
+from web3cli.helpers.database import delete_db_file, get_db_filepath
+from web3core.helpers.misc import yes_or_exit
 
 
-class DbBaseController(Controller):
+class DbController(Controller):
     """Base controller for the `w3 db` command"""
 
     class Meta:
         label = "db"
         help = "Interact with the local database of web3cli"
         stacked_type = "nested"
         stacked_on = "base"
 
     @ex(
         help="delete the entire db: signers, addresses, chains, etc",
-        arguments=[
-            (
-                ["--force"],
-                {
-                    "help": "Delete without asking",
-                    "action": "store_true",
-                },
-            ),
-        ],
+        arguments=[args.force()],
     )
     def delete(self) -> None:
         if not self.app.pargs.force:
             yes_or_exit(
                 intro="WARNING: This will delete all stored info, such as signers, addresses, transactions and chains.\n",
                 logger=self.app.log.info,
             )
+        db_path = get_db_filepath(self.app)
+        if db_path == ":memory:":
+            self.app.log.info("Database is in-memory, nothing to delete")
+            return
         if delete_db_file(self.app):
-            self.app.log.info(f"Database file deleted ({get_db_file(self.app)})")
+            self.app.log.info(f"Database file deleted ({db_path})")
         else:
-            self.app.log.info(f"Database not found at {get_db_file(self.app)}")
+            self.app.log.info(f"Database not found at {db_path}")
+
+    @ex(help="show the path of the database file")
+    def where(self) -> None:
+        self.app.print(get_db_filepath(self.app))
```

### Comparing `web3cli-0.9.6/src/web3cli/controllers/db/signer_controller.py` & `web3cli-1.0.0/src/web3cli/controllers/crud/signer_controller.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,97 +1,128 @@
+import getpass
+
 from cement import ex
-from web3cli.controllers.controller import Controller
-from web3cli.core.models.signer import Signer
-from web3cli.core.exceptions import KeyIsInvalid, SignerNotFound, Web3CliError
-from web3cli.helpers.crypto import encrypt_string_with_app_key
 from eth_account import Account
-import getpass
 
-from web3cli.helpers.render import render_table
+from web3cli.controllers.controller import Controller
+from web3cli.exceptions import Web3CliError
+from web3cli.helpers import args
+from web3cli.helpers.crypto import decrypt_keyfile, encrypt_string_with_app_key
+from web3cli.helpers.render import render_json, render_table
+from web3cli.helpers.signer import get_signer
+from web3core.exceptions import KeyIsInvalid, SignerNotFound
+from web3core.helpers.misc import are_mutually_exclusive
+from web3core.models.signer import Signer
 
 
 class SignerController(Controller):
-    """Handler of the `w3 db signer` commands"""
+    """Handler of the `w3 signer` CRUD commands"""
 
     class Meta:
         label = "signer"
         help = "add, list or delete signers"
         stacked_type = "nested"
-        stacked_on = "db"
+        stacked_on = "base"
 
     @ex(help="list signers")
     def list(self) -> None:
         render_table(
             self.app,
             data=[
                 [s["name"], s["address"]] for s in Signer.get_all_as_dicts(Signer.name)
             ],
             headers=["NAME", "ADDRESS"],
             wrap=42,
         )
 
     @ex(
-        help="show the address of a signer by its name; without arguments, show the name of the active signer",
+        help="show the details of the given signer",
         arguments=[
             (
                 ["name"],
                 {
-                    "help": "name of the signer to show",
-                    "nargs": "?",
+                    "help": "the signer to show; can be either a name, address, private key or keyfile"
                 },
-            ),
+            )
         ],
     )
     def get(self) -> None:
-        if self.app.pargs.name:
-            self.app.print(Signer.get_address(self.app.pargs.name))
-        elif self.app.signer:
-            self.app.print(self.app.signer)
+        signer = get_signer(self.app, self.app.pargs.name).as_dict()
+        signer["key"] = "********"
+        render_json(self.app, signer)
+
+    @ex(
+        help="show the active signer's address",
+        arguments=[
+            (
+                ["--show-name"],
+                {
+                    "help": "show the name of the active signer, instead",
+                    "action": "store_true",
+                },
+            ),
+            args.signer(),
+        ],
+    )
+    def active(self) -> None:
+        if self.app.pargs.show_name:
+            self.app.print(self.app.signer.name)
         else:
-            raise SignerNotFound(
-                "Signer not set. Add one with `w3 db signer add <name>`"
-            )
+            self.app.print(self.app.signer.address)
 
     @ex(
         help="add a new signer; you will be asked for the private key",
         arguments=[
             (["name"], {"help": "name identifying the signer"}),
             (
                 ["--create"],
                 {
-                    "help": "generate a new private key instead, and use it to create the signer",
+                    "help": "generate a new private key instead, and use it to create the signer; then print the private key",
                     "action": "store_true",
                 },
             ),
             (
                 ["-p", "--private-key"],
                 {
                     "help": "optionally, provide the private key directly; if you do so, make sure you clean your command history afterwards",
                 },
             ),
+            (
+                ["--keyfile"],
+                {
+                    "help": "optionally, provide the path to a keyfile to import the private key from"
+                },
+            ),
         ],
     )
     def add(self) -> None:
         # Validate name
         if Signer.get_by_name(self.app.pargs.name):
             raise Web3CliError(
-                f"Signer with name '{self.app.pargs.name}' already exists; to delete it, use `w3 db signer delete {self.app.pargs.name}`"
+                f"Signer with name '{self.app.pargs.name}' already exists; to delete it, use `w3 signer delete {self.app.pargs.name}`"
             )
         # Validate optional args
-        if self.app.pargs.create and self.app.pargs.private_key:
+        if not are_mutually_exclusive(
+            self.app.pargs.create,
+            bool(self.app.pargs.keyfile),
+            bool(self.app.pargs.private_key),
+        ):
             raise Web3CliError(
-                "Arguments --create and --private-key are mutually exclusive"
+                "Arguments --create, --private-key and --keyfile cannot coexist"
             )
         # Case 1: private key passed via argument
         if self.app.pargs.private_key:
             key = self.app.pargs.private_key
         # Case 2: generate private key from scratch
         elif self.app.pargs.create:
             key = Account.create(self.app.app_key).key.hex()
-        # Case 3: let the user input the key (default)
+        # Case 3: json keyfile passed via argument
+        elif self.app.pargs.keyfile:
+            key = decrypt_keyfile(self.app.pargs.keyfile)
+        # Case 4: let the user input the key (default)
         else:
             key = getpass.getpass("Private key: ")
         # Verify key
         try:
             address = Account.from_key(key).address
         except:
             raise KeyIsInvalid(
@@ -102,14 +133,17 @@
             name=self.app.pargs.name,
             key=encrypt_string_with_app_key(self.app, key),
             address=address,
         )
         self.app.log.info(
             f"Signer '{self.app.pargs.name}' added correctly (address={address})"
         )
+        if self.app.pargs.create:
+            # Print private key
+            self.app.print(key)
 
     @ex(
         help="delete a signer",
         arguments=[
             (["name"], {"help": "name of the signer to delete"}),
         ],
     )
```

### Comparing `web3cli-0.9.6/src/web3cli/controllers/db/tx_controller.py` & `web3cli-1.0.0/src/web3cli/controllers/crud/history_controller.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,90 +1,91 @@
 from cement import ex
+from playhouse.shortcuts import model_to_dict
+
 from web3cli.controllers.controller import Controller
-from web3cli.core.models.tx import Tx
-from web3cli.core.exceptions import TxIsInvalid, Web3CliError
+from web3cli.exceptions import Web3CliError
+from web3cli.helpers import args
 from web3cli.helpers.render import render_table
-from web3cli.core.helpers.format import cut
-from playhouse.shortcuts import model_to_dict
+from web3core.helpers.format import cut
+from web3core.models.tx import Tx
 
 
-class TxController(Controller):
-    """Handler of the `w3 db tx` commands"""
+class HistoryController(Controller):
+    """Handler of the `w3 history` CRUD commands"""
 
     class Meta:
-        label = "tx"
-        help = "add, list or delete transactions"
+        label = "history"
+        help = "add, list or delete transactions to the transaction history"
         stacked_type = "nested"
-        stacked_on = "db"
+        stacked_on = "base"
 
-    @ex(help="list transactions")
+    @ex(help="list transactions in the history")
     def list(self) -> None:
         render_table(
             self.app,
             data=[
                 [tx.hash, tx.chain, tx.created_at_short(), cut(tx.from_, 10)]
                 for tx in Tx.get_all(Tx.created_at.desc())
             ],
             headers=["HASH", "CHAIN", "CREATED AT", "FROM"],
             wrap=66,
         )
 
     @ex(
-        help="show details of the given transaction",
+        help="show details of the given transaction in the history",
         arguments=[
             (["hash"], {"help": "hash of the transaction"}),
         ],
     )
     def get(self) -> None:
         tx = Tx.get_by_hash_or_raise(self.app.pargs.hash)
         self.app.render(model_to_dict(tx), indent=4, handler="json")
 
     @ex(
-        help="add a new transaction to the database",
+        help="add a new transaction to the history",
         arguments=[
             (["hash"], {"help": "hash of the transaction"}),
             (
                 ["from"],
                 {
                     "help": "address from which the tx was sent (0x...)",
                 },
             ),
             (["to"], {"help": "address to which the tx was sent (0x...)"}),
-            (["-d", "--description"], {"action": "store"}),
+            (["-d", "--desc"], {"action": "store"}),
             (
                 ["-u", "--update"],
                 {
                     "help": "if a transaction with the same hash is present, overwrite it",
                     "action": "store_true",
                 },
             ),
+            args.chain(),
         ],
     )
     def add(self) -> None:
-        if not Tx.is_valid_hash(self.app.pargs.hash):
-            raise TxIsInvalid(f"Invalid transaction hash given: {self.app.pargs.hash}")
         tx = Tx.get_by_hash(self.app.pargs.hash)
         if not tx or self.app.pargs.update:
             Tx.upsert(
                 {
                     "hash": self.app.pargs.hash,
-                    "chain": self.app.chain,
+                    "chain": self.app.chain.name,
                     "from_": getattr(self.app.pargs, "from"),
                     "to": self.app.pargs.to,
-                    "description": self.app.pargs.description,
+                    "desc": self.app.pargs.desc,
                 },
                 logger=self.app.log.info,
             )
         else:
             raise Web3CliError(
                 f"Transaction '{self.app.pargs.hash}' already exists. Use `--update` or `-u` to update it."
             )
 
     @ex(
-        help="delete a transaction",
+        help="delete a transaction from the history",
         arguments=[
             (["hash"], {"help": "hash of the tx to delete"}),
         ],
     )
     def delete(self) -> None:
         tx = Tx.get_by_hash_or_raise(self.app.pargs.hash)
         tx.delete_instance()
```

### Comparing `web3cli-0.9.6/src/web3cli/controllers/key_controller.py` & `web3cli-1.0.0/src/web3cli/controllers/app_key_controller.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,40 @@
+import secrets
+import sys
+
 from cement import ex
+
 from web3cli.controllers.controller import Controller
+from web3cli.helpers import args
 from web3cli.helpers.config import update_setting_in_config_file
-import secrets
-import sys
 
 
-class KeyController(Controller):
-    """Handler of the `w3 key` commands"""
+class AppKeyController(Controller):
+    """Handler of the `w3 app-key` commands"""
 
     class Meta:
-        label = "key"
-        help = "handle passwords and application keys"
+        label = "app-key"
+        help = "create the application key"
         stacked_type = "nested"
         stacked_on = "base"
 
     @ex(
         help="generate a new random password and set it as the app key",
         arguments=[
-            (
-                ["-f", "--force"],
-                {
-                    "help": "if an app key already exists, replace it without asking (all signers added with the old app key will need to be recreated)",
-                    "action": "store_true",
-                },
-            )
+            args.force(
+                help="replace the key if it already exists; all signers will need to be recreated"
+            ),
         ],
     )
     def create(self) -> None:
         # If the app key already exists, warn the user before replacing it
         key_exists = True if self.get_option("web3cli.app_key") else False
         if key_exists and not self.app.pargs.force:
             self.app.log.error(
-                "App key already exists, run `w3 key create --force` to replace it.\nIf you do so, signers added with the old key will need to be recreated."
+                "App key already exists, run `w3 app-key create --force` to replace it.\nIf you do so, signers added with the old key will need to be recreated."
             )
             self.app.exit_code = 0
             sys.exit()
 
         # Generate new app key and store it
         key = secrets.token_bytes(32)
         update_setting_in_config_file(
```

### Comparing `web3cli-0.9.6/src/web3cli/controllers/send_controller.py` & `web3cli-1.0.0/src/web3cli/controllers/send_controller.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,68 @@
 from cement import ex
+
 from web3cli.controllers.controller import Controller
-from web3cli.core.helpers.input import yes_or_exit
-from web3cli.core.models.address import Address
+from web3cli.helpers import args
 from web3cli.helpers.send import send_coin_or_token
+from web3core.helpers.misc import to_number, yes_or_exit
+from web3core.helpers.resolve import resolve_address
+from web3core.models.address import Address
+from web3core.models.signer import Signer
 
 
 class SendController(Controller):
     """Handler of the `w3 send` command"""
 
     class Meta:
         label = "send"
         help = "send native coins, tokens and NFTs"
         stacked_type = "embedded"
         stacked_on = "base"
 
     @ex(
-        help="Send a coin or token to the given address and show the transaction hash",
+        help="Send a coin or token to the given address, and show the transaction hash",
         arguments=[
             (
                 ["to"],
                 {
                     "help": "receiver of the funds; can be an actual address or an address tag",
                 },
             ),
-            (["amount"], {"help": "how much to send", "type": float}),
+            (["amount"], {"help": "how much to send"}),
             (
                 ["ticker"],
                 {"help": "ticker of the coin or token to send"},
             ),
             (
                 ["unit"],
                 {
-                    "help": "optionally specify the unit to use (wei, gwei, etc)",
+                    "help": "optionally specify the unit to use. For native-coins: wei, gwei, etc. For tokens: specify 'smallest' to send using the smallest unit of the token.",
                     "nargs": "?",
-                    "default": "ether",
-                },
-            ),
-            (
-                ["-f", "--force"],
-                {
-                    "help": "do not ask for confirmation",
-                    "action": "store_true",
                 },
             ),
+            *args.chain_and_rpc(),
+            *args.signer_and_gas(),
+            args.force(),
         ],
     )
     def send(self) -> None:
         # Parse arguments
-        to_address = Address.resolve_address(self.app.pargs.to)
+        to_address = resolve_address(self.app.pargs.to, [Address, Signer])
+        amount = to_number(self.app.pargs.amount)
+        ticker = self.app.pargs.ticker.lower()
         if not self.app.pargs.force:
-            what = f"{self.app.pargs.amount} {self.app.pargs.ticker}"
-            if self.app.pargs.unit != "ether":
-                what = f"{self.app.pargs.amount} {self.app.pargs.unit} units of {self.app.pargs.ticker}"
+            what = f"{amount} {ticker}"
+            if self.app.pargs.unit:
+                what = f"{amount} {self.app.pargs.unit} unit(s) of {ticker}"
             print(
-                f"You are about to send {what} on the {self.app.chain} chain from signer {self.app.signer} to {to_address}."
+                f"You are about to send {what} on the {self.app.chain.name} chain from {self.app.signer.address} to {to_address}."
             )
             yes_or_exit(logger=self.app.log.info)
         # Send
         tx_hash = send_coin_or_token(
             self.app,
-            ticker=self.app.pargs.ticker,
+            ticker=ticker,
             to=to_address,
-            amount=self.app.pargs.amount,
+            amount=amount,
             unit=self.app.pargs.unit,
         )
         self.app.print(tx_hash)
```

### Comparing `web3cli-0.9.6/src/web3cli/core/exceptions.py` & `web3cli-1.0.0/src/web3core/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,70 +1,101 @@
-class Web3CliError(Exception):
+class Web3CoreError(Exception):
     """Generic errors"""
 
     pass
 
 
-class ChainNotFound(Web3CliError):
+class NotSupportedYet(Web3CoreError):
+    """When a feature is not supported yet"""
+
+    pass
+
+
+class RecordNotFound(Web3CoreError):
+    """When a record from the database is not found"""
+
+    pass
+
+
+class ChainNotFound(RecordNotFound):
     """When a chain name is not found in the database"""
 
     pass
 
 
-class AddressNotFound(Web3CliError):
-    """When an address name is not found in the database"""
+class ChainNotResolved(Web3CoreError):
+    """When a string cannot be resolved to a chain"""
 
     pass
 
 
-class AddressIsInvalid(Web3CliError):
+class AddressIsInvalid(Web3CoreError):
     """When an address 0x... is not in a valid EVM format"""
 
     pass
 
 
-class AddressNotResolved(Web3CliError):
+class AddressNotResolved(Web3CoreError):
     """When a string cannot be resolved to a valid address"""
 
     pass
 
 
-class KeyIsInvalid(Web3CliError):
+class KeyIsInvalid(Web3CoreError):
     """When a non-valid private key is provided"""
 
     pass
 
 
-class RpcIsInvalid(Web3CliError):
+class RpcIsInvalid(Web3CoreError):
     """When a non-valid RPC is used"""
 
     pass
 
 
-class RpcNotFound(Web3CliError):
+class RpcNotFound(RecordNotFound):
     """When an RPC cannot be found in the DB"""
 
     pass
 
 
-class SignerNotFound(Web3CliError):
+class SignerNotFound(RecordNotFound):
     """When a signer does not exist in the DB"""
 
     pass
 
 
-class InvalidConfig(Web3CliError):
-    """When any configuration value cannot be found"""
+class TxNotFound(Web3CoreError):
+    """When a transaction hash is not found in the database"""
 
     pass
 
 
-class TxNotFound(Web3CliError):
-    """When a transaction hash is not found in the database"""
+class TxIsInvalid(Web3CoreError):
+    """When a transatction hash is not in a valid EVM format"""
 
     pass
 
 
-class TxIsInvalid(Web3CliError):
-    """When a transatction hash is not in a valid EVM format"""
+class ContractNotFound(RecordNotFound):
+    """When a contract name is not found in the database"""
+
+    pass
+
+
+class ContractIsInvalid(Web3CoreError):
+    """When a contract address or other field is not valid
+    EVM format"""
+
+    pass
+
+
+class ContractAbiNotResolved(Web3CoreError):
+    """When the ABI of a contract cannot be found"""
+
+    pass
+
+
+class AbiOverflow(Web3CoreError):
+    """When you pass an int or unit too big for the ABI type"""
 
     pass
```

### Comparing `web3cli-0.9.6/src/web3cli/core/helpers/client_factory.py` & `web3cli-1.0.0/src/web3cli/helpers/client_factory.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,78 @@
-from typing import Any, Type
-from web3cli.core.models.signer import Signer
-from web3cli.core.types import Logger
+from typing import Any, cast
+
+from cement import App
 from web3client.base_client import BaseClient
-from web3cli.core.models.chain import Chain
-from web3cli.core.helpers.crypto import decrypt_string
+
+from web3core.helpers.client_factory import make_base_client, make_base_wallet
+from web3core.helpers.client_factory import (
+    make_contract_client as make_contract_client_,
+)
+from web3core.helpers.client_factory import (
+    make_contract_wallet as make_contract_wallet_,
+)
+
+
+def make_client(app: App, log: bool = False, **client_args: Any) -> BaseClient:
+    """Client suitable to read from the blockchain"""
+    return cast(
+        BaseClient,
+        make_base_client(
+            chain=app.chain,
+            node_uri=app.rpc.url,
+            logger=app.log.info if log else None,
+            **client_args,
+        ),
+    )
+
+
+def make_wallet(app: App, log: bool = False, **client_args: Any) -> BaseClient:
+    """Client suitable to read from and write to the blockchain"""
+    return make_base_wallet(
+        chain=app.chain,
+        signer=app.signer,
+        password=app.app_key,
+        node_uri=app.rpc.url,
+        logger=app.log.info if log else None,
+        **client_args,
+    )
 
 
-def make_base_client(
-    chain_name: str,
-    node_uri: str = None,
-    base: Type[BaseClient] = BaseClient,
-    logger: Logger = lambda msg: None,
-    **clientArgs: Any,
+def make_contract_client(
+    app: App,
+    contract_name: str,
+    log: bool = False,
+    **client_args: Any,
 ) -> BaseClient:
-    """Return a brand new client configured for the given blockchain"""
-    chain: Chain = Chain.get_by_name_or_raise(chain_name)
-    if node_uri is None:
-        node_uri = chain.pick_rpc().url
-    if logger:
-        logger(f"Using chain {chain_name} with RPC {node_uri}")
-    client = base(nodeUri=node_uri, **clientArgs)
-    client.chainId = chain.chain_id
-    client.txType = chain.tx_type
-    middlewares = chain.middlewares.split(",") if chain.middlewares else []
-    client.setMiddlewares([Chain.parse_middleware(m) for m in middlewares])
-    return client
-
-
-def make_base_wallet(
-    chain_name: str,
-    signer_name: str,
-    password: bytes,
-    node_uri: str = None,
-    base: Type[BaseClient] = BaseClient,
-    logger: Logger = lambda msg: None,
-    **clientArgs: Any,
+    """Client suitable to interact with the given smart contract"""
+    return make_contract_client_(
+        contract_name=contract_name,
+        chain=app.chain,
+        node_uri=app.rpc.url,
+        logger=app.log.info if log else None,
+        **client_args,
+    )
+
+
+def make_contract_wallet(
+    app: App,
+    contract_name: str,
+    log: bool = False,
+    **client_args: Any,
+) -> BaseClient:
+    """Client suitable to interact with the given smart contract"""
+    return make_contract_wallet_(
+        contract_name=contract_name,
+        chain=app.chain,
+        signer=app.signer,
+        password=app.app_key,
+        node_uri=app.rpc.url,
+        logger=app.log.info if log else None,
+        **client_args,
+    )
+
+
+def make_erc20_wallet(
+    app: App, token_name: str, log: bool = False, **client_args: Any
 ) -> BaseClient:
-    """Return a brand new client configured for the given blockchain,
-    with signing support. You need to provide the name of the signer
-    from the DB, and a password to decrypt the signer's key."""
-    client = make_base_client(chain_name, node_uri, base, **clientArgs)
-    if logger:
-        logger(f"Using signer {signer_name}")
-    signer = Signer.get_by_name_or_raise(signer_name)
-    client.setAccount(decrypt_string(signer.key, password))
-    return client
+    """Client suitable to interact with the given ERC20 token"""
+    return make_contract_wallet(app, token_name, log, **client_args)
```

### Comparing `web3cli-0.9.6/src/web3cli/core/helpers/crypto.py` & `web3cli-1.0.0/src/web3core/helpers/crypto.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import secrets
+
 from cryptography.hazmat.primitives.ciphers.aead import AESGCM
 
 
 def encrypt(message: bytes, key: bytes) -> bytes:
     """Encrypt a message using AES256-GCM. Requires a 32 bytes key, e.g.
     secrets.token_bytes(32)
     Source: https://stackoverflow.com/a/59835994/2972183"""
```

### Comparing `web3cli-0.9.6/src/web3cli/core/helpers/rpc.py` & `web3cli-1.0.0/src/web3core/helpers/rpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from urllib.parse import urlparse
 
-
 HTTP_SCHEMES = {"http", "https"}
 WS_SCHEMES = {"ws", "wss"}
 
 
 def is_rpc_uri_valid(uri_string: str) -> bool:
     """Return True if the given string is a valid URI
     that can be used to access an RPC. Based on
```

### Comparing `web3cli-0.9.6/src/web3cli/core/helpers/yaml.py` & `web3cli-1.0.0/src/web3core/helpers/yaml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import os
 from typing import Any
+
 import ruamel.yaml
-import os
-from web3cli.core.types import Logger
+
+from web3core.types import Logger
 
 
 def set(
     filepath: str,
     setting: str,
     value: Any,
     logger: Logger = None,
```

### Comparing `web3cli-0.9.6/src/web3cli/core/models/address.py` & `web3cli-1.0.0/src/web3core/models/tx.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,95 +1,72 @@
 from __future__ import annotations
+
+import re
 from typing import Type
-from peewee import TextField
-from web3cli.core.models.base_model import BaseModel
-from web3cli.core.exceptions import (
-    AddressIsInvalid,
-    AddressNotFound,
-    AddressNotResolved,
-)
-import web3
-from web3cli.core.models.types import AddressFields
-from playhouse.shortcuts import update_model_from_dict
+
+from peewee import BigIntegerField, DateTimeField, TextField
 from playhouse.signals import pre_save
-from web3cli.core.types import Logger
+
+from web3core.exceptions import AddressIsInvalid, TxIsInvalid, TxNotFound
+from web3core.models.address import Address
+from web3core.models.timestamps_model import TimestampsModel
+from web3core.models.types import TxFields
+from web3core.types import Logger
 
 
-class Address(BaseModel):
+class Tx(TimestampsModel):
     class Meta:
-        table_name = "addresses"
+        table_name = "txs"
 
-    address = TextField()
-    name = TextField(unique=True)
-    description = TextField(null=True)
+    hash = TextField(unique=True)
+    chain = TextField()
+    to = TextField()
+    from_ = TextField(column_name="from")
+    value = TextField(null=True)
+    gas = BigIntegerField(null=True)
+    gas_price = TextField(null=True)
+    # timestamp = BigIntegerField(null=True)
+    # block = BigIntegerField(null=True)
+    desc = TextField(null=True)
+    data = TextField(null=True)
+    receipt = TextField(null=True)
+    created_at = DateTimeField(null=True)
+    updated_at = DateTimeField(null=True)
 
     @classmethod
-    def get_by_name(cls, name: str) -> Address:
-        """Return the address object with the given name, or None if
+    def get_by_hash(cls, hash: str) -> Tx:
+        """Return the tx object with the given hash, or None if
         it does not exist"""
-        return cls.get_or_none(cls.name == name)
+        return cls.get_or_none(cls.hash == hash)
 
     @classmethod
-    def get_by_name_or_raise(cls, name: str) -> Address:
-        """Return the address object with the given name; raise
+    def get_by_hash_or_raise(cls, hash: str) -> Tx:
+        """Return the tx object with the given hash; raise
         error if it does not exist"""
         try:
-            return cls.get(cls.name == name)
+            return cls.get(cls.hash == hash)
         except:
-            raise AddressNotFound(f"Address '{name}' does not exist")
-
-    @classmethod
-    def upsert(cls, fields: AddressFields, logger: Logger = None) -> Address:
-        """Create an address, or replace it if an address with the same
-        name already exists, maintaining its ID and relations."""
-        address: Address = Address.get_or_none(name=fields["name"])
-        if address:
-            address = update_model_from_dict(address, fields, ignore_unknown=True)
-            if logger:
-                logger(f"Address {address.name} updated")
-        else:
-            address = Address(**fields)
-            if logger:
-                logger(f"Address {address.name} created")
-        address.save()
-        return address
-
-    @classmethod
-    def is_valid_address(cls, address: str) -> bool:
-        """Is the address a valid EVM address?"""
-        return web3.main.is_address(address)
-
-    @classmethod
-    def is_valid_name(cls, name: str) -> bool:
-        """Return True if the given name is ok to be saved in the DB.
-        The only constraint is that the name is not a valid address,
-        because in that case it would mess up the address resolver"""
-        return not cls.is_valid_address(name)
+            raise TxNotFound(f"Transaction '{hash}' does not exist")
 
     @classmethod
-    def get_address(cls, name: str) -> str:
-        """Return the address with the given name; raise error
-        if no such address is found"""
-        address = Address.get_by_name_or_raise(name)
-        return address.address
-
-    @classmethod
-    def resolve_address(cls, address_or_name: str) -> str:
-        """Return the address with the given name, but if an actual valid
-        address is passed (0x...) then return it"""
-        try:
-            return (
-                address_or_name
-                if cls.is_valid_address(address_or_name)
-                else cls.get_address(address_or_name)
-            )
-        except AddressNotFound:
-            raise AddressNotResolved(
-                f"Could not resolve '{address_or_name}': neither a valid address nor a name of a stored address"
-            )
-
-
-@pre_save(sender=Address)
-def validate(model_class: Address, instance: Type[Address], created: bool) -> None:
-    """Validate the address which is about to be saved"""
-    if not Address.is_valid_address(instance.address):
-        raise AddressIsInvalid(f"Invalid address given: {instance.address}")
+    def is_valid_hash(cls, hash: str) -> bool:
+        """Is the hash a valid EVM tx hash?"""
+        pattern = re.compile(r"^0x[a-fA-F0-9]{64}")
+        return bool(re.fullmatch(pattern, hash))
+
+    @classmethod
+    def upsert(cls, fields: TxFields, logger: Logger = None) -> Tx:
+        """Create tx or update it if one with the same hash already exists"""
+        return cls.upsert_by_field(cls.hash, fields["hash"], fields, logger, True)
+
+
+@pre_save(sender=Tx)
+def validate(model_class: Tx, instance: Type[Tx], created: bool) -> None:
+    """Validate the transaction which is about to be saved"""
+    if not Tx.is_valid_hash(instance.hash):
+        raise TxIsInvalid(f"Invalid transaction hash: {instance.hash}")
+    if not Address.is_valid_address(instance.from_):
+        raise AddressIsInvalid(
+            f"Invalid 'from' address for transaction: {instance.from_}"
+        )
+    if not Address.is_valid_address(instance.to):
+        raise AddressIsInvalid(f"Invalid 'to' address for transaction: {instance.to}")
```

### Comparing `web3cli-0.9.6/src/web3cli/core/models/chain.py` & `web3cli-1.0.0/src/web3core/models/chain.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,95 +1,91 @@
 from __future__ import annotations
+
 from typing import List
-from peewee import TextField, IntegerField, ForeignKeyField
-from web3cli.core.exceptions import (
-    ChainNotFound,
+
+from peewee import ForeignKeyField, IntegerField, TextField
+from playhouse.shortcuts import dict_to_model
+from web3.middleware import geth_poa_middleware
+from web3.types import Middleware
+
+from web3core.exceptions import (
+    ChainNotResolved,
     RpcIsInvalid,
     RpcNotFound,
-    Web3CliError,
+    Web3CoreError,
 )
-from web3cli.core.helpers.rpc import is_rpc_uri_valid
-from web3cli.core.models.base_model import BaseModel
-from web3.types import Middleware
-from web3.middleware import geth_poa_middleware
-from web3cli.core.models.types import ChainFields
-from web3cli.core.types import Logger
-from playhouse.shortcuts import update_model_from_dict
+from web3core.helpers.rpc import is_rpc_uri_valid
+from web3core.models.base_model import BaseModel
+from web3core.models.types import ChainFields
+from web3core.seeds import chain_seeds
+from web3core.types import Logger
 
 
 class Chain(BaseModel):
     class Meta:
         table_name = "chains"
 
     name = TextField(unique=True)
+    desc = TextField(null=True)
     chain_id = IntegerField()
     coin = TextField()
     tx_type = IntegerField(default=2)
     middlewares = TextField(null=True)
 
     @classmethod
-    def get_by_name(cls, name: str) -> Chain:
-        """Return the chain object with the given name, or None if
-        it does not exist"""
-        return cls.get_or_none(cls.name == name)
-
-    @classmethod
-    def get_by_name_or_raise(cls, name: str) -> Chain:
-        """Return the chain object with the given name; raise
-        error if it does not exist"""
-        try:
-            return cls.get(cls.name == name)
-        except:
-            raise ChainNotFound(f"Chain '{name}' does not exist")
-
-    @classmethod
     def upsert(cls, fields: ChainFields, logger: Logger = None) -> Chain:
-        """Create a chain, or replace it if a chain with the same
-        name already exists, maintaining its ID and relations."""
-        chain: Chain = Chain.get_or_none(name=fields["name"])
-        if chain:
-            chain = update_model_from_dict(chain, fields, ignore_unknown=True)
-            if logger:
-                logger(f"Chain {chain.name} updated")
-        else:
-            chain = Chain(**fields)
-            if logger:
-                logger(f"Chain {chain.name} created")
-        chain.save()
-        return chain
+        """Create chain or update it if one with the same name already exists"""
+        return cls.upsert_by_field(cls.name, fields["name"], fields, logger, True)
 
     @classmethod
-    def seed_one(
-        cls, seed_chain: ChainFields, logger: Logger = lambda msg: None
-    ) -> Chain:
+    def seed_one(cls, seed: ChainFields, logger: Logger = lambda msg: None) -> Chain:
         """Create a chain and its RPCs in the db; if a chain with the
         same already exists, it will be replaced and new RPCs added."""
-        chain = Chain.upsert(seed_chain, logger)
-        for seed_rpc in seed_chain["rpcs"]:
+        chain = Chain.upsert(seed, logger)
+        for seed_rpc in seed["rpcs"]:
             chain.add_rpc(seed_rpc["url"], logger)
         return chain
 
     @classmethod
     def seed(
-        cls, chain_seeds: List[ChainFields], logger: Logger = lambda msg: None
+        cls, seeds: List[ChainFields], logger: Logger = lambda msg: None
     ) -> List[Chain]:
         """Populate the table with the given list of chains
         and RPCs, and return the list of created instances."""
-        return [Chain.seed_one(chain_seed, logger) for chain_seed in chain_seeds]
+        return [Chain.seed_one(seed, logger) for seed in seeds]
 
     @classmethod
     def parse_middleware(cls, middleware: str) -> Middleware:
         """Given the name of a Web3 middleware (e.g. geth_poa_middleware)
         return the corresponding Middleware function"""
         try:
             return {
                 "geth_poa_middleware": geth_poa_middleware,
             }[middleware]
         except:
-            raise Web3CliError(f"Middleware {middleware} not supported")
+            raise Web3CoreError(f"Middleware {middleware} not supported")
+
+    @classmethod
+    def resolve_chain(cls, name: str) -> Chain:
+        """Return the chain with the given name, looking first in
+        the database and then in the seed chains. If not found, raise
+        ChainNotResolved."""
+        # Look in the DB
+        chain = Chain.get_by_name(name)
+        if chain:
+            return chain
+
+        # Look in the seeds
+        for c in chain_seeds.all:
+            if c["name"] == name:
+                return dict_to_model(Chain, c, True)
+
+        raise ChainNotResolved(
+            f"Could not find chain '{name}', add it with `w3 chain add`"
+        )
 
     def add_rpc(self, rpc_url: str, logger: Logger = lambda msg: None) -> Rpc:
         """Add an RPC to the chain instance.
 
         The RPC will be created in its own table, if it does not exist
         yet, and linked to the chain via the pivot table chain_rpc"""
         # Validate RPC
```

### Comparing `web3cli-0.9.6/src/web3cli/core/models/timestamps_model.py` & `web3cli-1.0.0/src/web3core/models/timestamps_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import datetime as dt
 from typing import Type
+
 from playhouse.signals import pre_save
-from web3cli.core.models.base_model import BaseModel
+
+from web3core.models.base_model import BaseModel
 
 
 class TimestampsModel(BaseModel):
     """Extend this class to automatically populate the 'created_at'
     and 'updated_at' timestamps each time a record is created
     or updated."""
```

### Comparing `web3cli-0.9.6/src/web3cli/helpers/config.py` & `web3cli-1.0.0/src/web3cli/helpers/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from cement import App
-from typing import Any
-from web3cli.core.helpers import yaml
-from web3cli.core.helpers.os import create_folder
 import os
+from typing import Any
+
+from cement import App
+
+from web3core.helpers import yaml
+from web3core.helpers.os import create_folder
 
 
 def update_setting_in_config_file(
     app: App, setting: str, value: Any, do_log: bool = False, is_global: bool = True
 ) -> None:
     """Update the value of a setting in the configuration file.
     If is_global is True, update the global configuration file,
```

### Comparing `web3cli-0.9.6/src/web3cli/helpers/database.py` & `web3cli-1.0.0/src/web3cli/helpers/database.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,46 @@
-from cement import App
-from web3cli.core.exceptions import Web3CliError
-from web3cli.core.helpers.database import tables
 import os
 
+from cement import App
+
+from web3cli.exceptions import Web3CliError
+from web3core.db import DB
+from web3core.models import MODELS
+
 
 def db_ready_or_raise(app: App) -> None:
     """Check whether the DB is attached to the app and connected"""
     if not app.db.is_connection_usable():
         raise Web3CliError("Could not establish database connection")
 
 
-def get_db_file(app: App) -> str:
+def get_db_filepath(app: App) -> str:
     """Return the full path of the database file, from
     the configuration"""
-    return os.path.expanduser(app.config.get("web3cli", "db_file"))
+    return os.path.abspath(os.path.expanduser(app.config.get("web3cli", "db_file")))
 
 
 def maybe_delete_db_file(app: App) -> None:
     """Delete the database file if app.delete_db is True"""
     if app.delete_db:
         delete_db_file(app)
 
 
 def delete_db_file(app: App) -> bool:
     """Delete the database file; return True if the file was
     deleted, false if it was not found"""
-    file = get_db_file(app)
+    file = get_db_filepath(app)
     if os.path.isfile(file):
+        try:
+            DB.close()
+        except:
+            pass
         os.remove(file)
         return True
     return False
 
 
 def truncate_tables(app: App) -> None:
     """Empty all tables in the database"""
     db_ready_or_raise(app)
-    for table in tables:
-        table.delete().execute()
+    for model in MODELS:
+        model.delete().execute()
```

### Comparing `web3cli-0.9.6/src/web3cli/helpers/render.py` & `web3cli-1.0.0/src/web3cli/helpers/render.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-from math import inf
+import json
 from typing import Any, List
-from web3cli.core.helpers.format import wrap as wrap_
+
 from cement import App
+from web3 import Web3
+
+from web3core.helpers.format import wrap as wrap_
 
 
 def render_table(
     app: App, headers: List[str], data: List[List[Any]], wrap: int = None
 ) -> None:
     """Print data as a table"""
     app.render(
@@ -17,13 +20,28 @@
 
 def prepare_for_table(app: App, value: Any, wrap: int = None) -> str:
     """Prepare a value before it is printed in a table"""
     # Parse wrap parameter
     if wrap == None:
         wrap = app.config.get("web3cli", "output_table_wrap")
     elif wrap == 0:
-        wrap = inf
+        wrap = 100000
     # Wrap value
     try:
         return "\n".join(wrap_(s=value, n=wrap))
     except:
         return value
+
+
+def render_json(app: App, data: Any, indent: int = 4) -> None:
+    """Print data as a JSON"""
+    app.render(data, handler="json", indent=indent)
+
+
+def render_yaml(app: App, data: Any) -> None:
+    """Print data as a YAML"""
+    app.render(data, handler="yaml")
+
+
+def render_web3py(app: App, data: Any, indent: int = 4) -> None:
+    """Print data as a Python object"""
+    render_json(app, json.loads(Web3.to_json(data)), indent=indent)
```

### Comparing `web3cli-0.9.6/src/web3cli/hooks.py` & `web3cli-1.0.0/src/web3cli/hooks.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,64 +1,79 @@
 """Functions called at specific points of the app lifecylce"""
 
+import ast
 import secrets
+from os.path import isfile
+
 import cement
-from web3cli.core.helpers.database import init_db
-from web3cli.helpers.config import update_setting_in_config_file
-from web3cli.helpers.database import get_db_file
 from cement import App
-import ast
+from genericpath import isfile
+
+from web3cli.helpers.config import update_setting_in_config_file
+from web3cli.helpers.database import get_db_filepath
+from web3core.db import DB
+from web3core.helpers.database import init_db
+from web3core.helpers.seed import populate_db
+from web3core.models import MODELS
 
 ####################
 # Register hooks
 ####################
 
 
 def post_setup(app: App) -> None:
     """Callback to the post_setup hook, which is fired at the end
     of app.setup(), as soon as the app has finished parsing the
     configuration files, and before app.run(), where the CLI command
     will be run"""
     customize_extensions(app)
     maybe_create_app_key(app)
-    attach_db(app)
+    init_and_attach_db(app)
 
 
 def post_argument_parsing(app: App) -> None:
     """Callback to the post_argument_parsing hook, which is fired
     as one of the first steps of app.run(), after app.setup() has
     completed."""
     pass
 
 
 ####################
 # Implementation
 ####################
 
 
-def attach_db(app: App) -> None:
+def init_and_attach_db(app: App) -> None:
     """Attach the production database to the app object, so that the
-    controllers can access it"""
-    db_path = get_db_file(app)
-    app.extend("db", init_db(db_path))
+    controllers can access it. If the database file does not exist,
+    create it and seed it"""
+    db_path = get_db_filepath(app)
+    do_populate = (
+        not isfile(db_path) and app.config.get("web3cli", "populate_db") == True
+    )
+    if not isfile(db_path):
+        app.log.debug("Creating database...")
+    app.extend("db", init_db(DB, MODELS, db_path))
+    if do_populate:
+        populate_db()
 
 
 def maybe_create_app_key(app: App) -> None:
     """Create an app key if it does not exist already;
     extend the app object with the app key"""
     if not app.config.get("web3cli", "app_key"):
-        key = secrets.token_bytes(32)
+        new_key = secrets.token_bytes(32)
         update_setting_in_config_file(
             app,
             setting="app_key",
-            value=str(key),
+            value=str(new_key),
             do_log=False,
             is_global=True,
         )
-        app.config.set("web3cli", "app_key", str(key))
+        app.config.set("web3cli", "app_key", str(new_key))
 
     # Create the shortcut app.app_key
     key = app.config.get("web3cli", "app_key")
     app.extend("app_key", ast.literal_eval(key))
 
 
 def customize_extensions(app: App) -> None:
```

### Comparing `web3cli-0.9.6/tests/conftest.py` & `web3cli-1.0.0/tests/web3core/fixtures.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,165 +1,120 @@
 """
 PyTest Fixtures.
 """
 
-from typing import Any, Iterator, List, Dict
-from pytest import FixtureRequest
+from typing import Any, Dict, Iterator, List
+
 import pytest
-from cement import fs
-import secrets
-from tests.main import Web3CliTest
-from tests.seeder import seed_local_accounts, seed_local_chain
-from web3cli.core.models.types import AddressFields, ChainFields, TxFields
-from web3cli.core.seeds.chain_seeds import chain_seeds
-import brownie
-from brownie.network.account import Account
+from playhouse.sqlite_ext import SqliteExtDatabase
+
+from web3core.db import DB
+from web3core.helpers.database import init_db
+from web3core.models import MODELS
+from web3core.models.types import AddressFields, ChainFields, ContractFields, TxFields
+from web3core.seeds import chain_seeds, contract_seeds
+
+
+@pytest.fixture(scope="function")
+def db() -> Iterator[SqliteExtDatabase]:
+    init_db(DB, MODELS, ":memory:")
+    yield DB
+    DB.drop_tables(MODELS)
+    DB.close()
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def addresses() -> List[AddressFields]:
     return [
         {
             "name": "Ethereum foundation",
             "address": "0xde0b295669a9fd93d5f28d9ec85e40f4cb697bae",
-            "description": "Test wallet EF",
+            "desc": "Test wallet EF",
         },
         {
             "name": "Binance hot wallet",
             "address": "0x8894e0a0c962cb723c1976a4421c95949be2d4e3",
-            "description": "Test wallet BHW",
+            "desc": "Test wallet BHW",
         },
         {
             "name": "Alameda research",
             "address": "0xbefe4f86f189c1c817446b71eb6ac90e3cb68e60",
-            "description": "Test wallet AR",
+            "desc": "Test wallet AR",
         },
     ]
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def signers() -> List[Dict[str, Any]]:
     return [
         {
             "name": "vanity_1",
             "address": "0x0c2010dc4736bab060740D3968cf1dDF86196D81",
             "private_key": "d94e4166f0b3c85ffebed3e0eaa7f7680ae296cf8a7229d637472b7452c8602c",
+            "keyfile": '{"address": "0c2010dc4736bab060740d3968cf1ddf86196d81", "crypto": {"cipher": "aes-128-ctr", "cipherparams": {"iv": "44bb6afb52fa1eb4e273f2dc972aa9c9"}, "ciphertext": "ca4bd4f91bfc51a34e5fd72340cfe058ae77108c51fdad8413c1a7c1eb54ea5c", "kdf": "scrypt", "kdfparams": {"dklen": 32, "n": 262144, "r": 1, "p": 8, "salt": "34eb69126e4c28c3b96ff2bbafc30fd6"}, "mac": "e30f84c256b85ad757527a9963da856a3dc0c8ff7691eaa30dce8a6025db0044"}, "id": "5dcac562-ed62-42be-85af-458082ae5621", "version": 3}',
+            "keyfile_password": "secret_1",
         },
         {
             "name": "vanity_2",
             "address": "0x206D4d644c22dDFc343b3AD23bBc7A42c8B201fc",
             "private_key": "3bc2f9b05ac28389fd65fd40068a10f730ec66b6293f9cfd8fe804d212ce06bb",
+            "keyfile": '{"address": "206d4d644c22ddfc343b3ad23bbc7a42c8b201fc", "crypto": {"cipher": "aes-128-ctr", "cipherparams": {"iv": "8eb93057b97baef092028a49d729fadb"}, "ciphertext": "5bcb8cc45abc29098e6157953218f90ce992c410fefa5cd6ccba5f90301abbfc", "kdf": "scrypt", "kdfparams": {"dklen": 32, "n": 262144, "r": 1, "p": 8, "salt": "9a9bae4fbef319b359dbc1a19757898c"}, "mac": "a890fbe5e0472cecff264b50ed7be3d56c22082a45e836712604a117ccc2ea24"}, "id": "c77dd2d2-d657-4d4a-ab7c-b491c4be0eb9", "version": 3}',
+            "keyfile_password": "secret_2",
         },
         {
             "name": "vanity_3",
             "address": "0x9fF0c40eDe4585a5E9f0F00009ce79b6344cB663",
             "private_key": "f76c67c2dd62222a5ec747116a66c573f3795c53276c0cdeafbcb5f597e2f8d4",
+            "keyfile": '{"address": "9ff0c40ede4585a5e9f0f00009ce79b6344cb663", "crypto": {"cipher": "aes-128-ctr", "cipherparams": {"iv": "efddd96d2ce2f840af8b58d681d1330c"}, "ciphertext": "95d4fc9dde914a8cdb679fda7b0ead7312fcc3053bfeb82bd5f6ffa5db22da4b", "kdf": "scrypt", "kdfparams": {"dklen": 32, "n": 262144, "r": 1, "p": 8, "salt": "1dc311b9bd5c76ed686ef39003716294"}, "mac": "63cdddd9e8f3987dff63a88ef838cc24ecfeb7b568916f581deb061844850f5e"}, "id": "c78bb6ff-fb12-474a-bf84-5a6d6e8e8bcc", "version": 3}',
+            "keyfile_password": "secret_3",
         },
     ]
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def txs() -> List[TxFields]:
     return [
         {
             "hash": "0xbe62871b8c0545dd9034bcb8e802b0c024d2983ba1de663c5cbb1b02c9173609",
-            "chain": "ethereum",
+            "chain": "eth",
             "to": "0xd2b06119B51626F175375C8Fb5Baa0c0e54819f2",
             "from_": "0xFdEE07396b59aEE88555bfb6C683Ca8FF3Ffd35c",
             "value": "9461431800000000000",
             "gas": 21000,
             "gas_price": "19000000000",
-            "description": "A regular value transaction",
+            "desc": "A regular value transaction",
             "data": "",
             "receipt": "",
             "created_at": "2022-12-02 19:45:57.100147+01:00",
             "updated_at": "2022-12-02 19:45:57.100172+01:00",
         },
         {
             "hash": "0xdf92dbca5a2788c4c57ee76408d1ea35c3753b6ababb468a1d949af56e786338",
-            "chain": "ethereum",
+            "chain": "eth",
             "to": "0xdAC17F958D2ee523a2206206994597C13D831ec7",
             "from_": "0x13E464A06df694893f6B07E49b6d84D4bece04c9",
             "value": None,
             "gas": 63209,
             "gas_price": "12250771391",
-            "description": "An ERC-20 transfer (USDT)",
+            "desc": "An ERC-20 transfer (USDT)",
             "data": "0xa9059cbb0000000000000000000000002fe5dbe5b4cdf1a032ab230f258d129b38faf79f00000000000000000000000000000000000000000000000000000009f7142c00",
             "receipt": "",
             "created_at": "2021-12-01 19:45:57.100147+01:00",
             "updated_at": "2021-12-01 19:45:57.100172+01:00",
         },
     ]
 
 
-@pytest.fixture()
+@pytest.fixture(scope="session")
 def chains() -> List[ChainFields]:
-    return chain_seeds
-
-
-@pytest.fixture()
-def app_key() -> bytes:
-    """A randomly-generated key suitable to be used as application key"""
-    return secrets.token_bytes(32)
-
-
-@pytest.fixture(scope="function")
-def tmp(request: FixtureRequest) -> Any:
-    """Create a `tmp` object that geneates a unique temporary directory, and
-    file for each test function that requires it."""
-    t = fs.Tmp()
-    yield t
-    t.remove()
-
-
-@pytest.fixture()
-def base_app(app_key: bytes) -> Iterator[Web3CliTest]:
-    """An app instance that can be used for basic tests. Add
-    arguments with app.set_argv() and run the CLI with app.run()"""
-    app = Web3CliTest()
-    app.setup()
-    app.config.set("web3cli", "app_key", app_key)
-    yield app
-    app.close()
-
-
-@pytest.fixture()
-def app(
-    base_app: Web3CliTest, accounts: List[Account], accounts_keys: List[str]
-) -> str:
-    """An app instance that can be used for tests on the local ganache
-    network. It depends on the accounts fixture of brownie, which in
-    turn depends on devnetwork fixture, which activates ganache"""
-    seed_local_chain(base_app)
-    seed_local_accounts(base_app, accounts, accounts_keys)
-    return base_app
-
-
-@pytest.fixture()
-def accounts_keys() -> Iterator[List[str]]:
-    """Private keys of the local accounts created by brownie.
-    There are just the keys from the mnemonic phrase 'brownie'
-    following the standard path m/44'/60'/0'/0/{account_index}"""
-    yield [
-        "bbfbee4961061d506ffbb11dfea64eba16355cbf1d9c29613126ba7fec0aed5d",
-        "804365e293b9fab9bd11bddd39082396d56d30779efbb3ffb0a6089027902c4a",
-        "1f52464c2fb44e9b7e0808f2c5fe56d87b73eb3bca0e72c66f9f74d7c6c9a81f",
-        "905e216d8acdabbd095f11162327c5e6e80cc59a51283732cd4fe1299b33b7a6",
-        "e21bbdc4c57125bec3e05467423dfc3da8754d862140550fc7b3d2833ad1bdeb",
-        "b591fb79dd7065964210e7e527c87f97523da07ef8d16794f09750d5eef959b5",
-        "fe613f76efbfd03a16624ed8d96777966770f353e83d6f7611c11fdfcdfa48d1",
-        "52f94fdeaaf7c8551bda5924f2b52ff438125b9b5170c04ea2e268bd945ff155",
-        "a26ebb1df46424945009db72c7a7ba034027450784b93f34000169b35fd3adaa",
-        "3ff6c8dfd3ab60a14f2a2d4650387f71fe736b519d990073e650092faaa621fa",
-    ]
+    return chain_seeds.all
 
 
-@pytest.fixture()
-def alice() -> Account:
-    """A Brownie account preloaded in the local chain"""
-    yield brownie.accounts[0]
+@pytest.fixture(scope="session")
+def contracts() -> List[ContractFields]:
+    return contract_seeds.all
 
 
-@pytest.fixture()
-def bob() -> Account:
-    """A Brownie account preloaded in the local chain"""
-    yield brownie.accounts[1]
+@pytest.fixture(scope="session")
+def contract_without_abi(contracts: List[ContractFields]) -> ContractFields:
+    contracts[0]["abi"] = None
+    return contracts[0]
```

### Comparing `web3cli-0.9.6/tests/controllers/db/test_chain.py` & `web3cli-1.0.0/tests/web3cli/controllers/crud/test_chain_controller.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,90 +1,99 @@
-from tests.main import Web3CliTest
 from typing import List
-from tests.seeder import seed_chains
-from web3cli.core.exceptions import Web3CliError
-from web3cli.core.models.chain import Chain
+
 import pytest
-from web3cli.core.models.types import ChainFields
+
+from tests.web3cli.main import Web3CliTest
+from web3cli.exceptions import Web3CliError
+from web3core.exceptions import RecordNotFound
+from web3core.helpers.seed import seed_chains
+from web3core.models.chain import Chain
+from web3core.models.types import ChainFields
 
 
 def test_chain_list(chains: List[ChainFields]) -> None:
     with Web3CliTest() as app:
-        seed_chains(app, chains)
-        app.set_args(["db", "chain", "list"]).run()
+        seed_chains(chains)
+        app.set_args(["chain", "list"]).run()
         data, output = app.last_rendered
         for c in chains:
             assert c["name"] in output
             assert c["coin"] in output
 
 
 def test_chain_add(chains: List[ChainFields]) -> None:
     for c in chains:
         # Add the chain > ok!
         argv = [
-            "db",
             "chain",
             "add",
             c["name"],
             str(c["chain_id"]),
             c["coin"],
             "--tx-type",
             str(c["tx_type"]),
+            "--desc",
+            str(c["desc"]),
         ]
         if "geth_poa_middleware" in c["middlewares"]:
             argv.append("--poa")
         with Web3CliTest() as app:
             app.set_args(argv).run()
             assert Chain.select().count() == 1
             chain: Chain = Chain.get_by_name(c["name"])
             assert chain.chain_id == c["chain_id"]
             assert chain.coin == c["coin"]
+            assert chain.desc == c["desc"]
         # Add the chain again > exception!
         with Web3CliTest(delete_db=False) as app:
             with pytest.raises(Web3CliError, match=r"already exists"):
                 app.set_args(argv).run()
         # Add the chain again with --update option > ok!
         with Web3CliTest(delete_db=False) as app:
             updated_argv = argv + ["--update"]
-            updated_argv[5] = f"{c['coin']}_UPDATED"
+            updated_argv[4] = f"{c['coin']}_UPDATED"
             print(updated_argv)
             app.set_args(updated_argv).run()
             assert Chain.select().count() == 1
             updated_chain: Chain = Chain.get_by_name(c["name"])
             assert updated_chain.chain_id == c["chain_id"]
-            assert updated_chain.coin == updated_argv[5]
+            assert updated_chain.coin == updated_argv[4]
 
 
 def test_chain_get(chains: List[ChainFields]) -> None:
-    """With explicit argument > return argument value"""
     for chain in chains:
         with Web3CliTest() as app:
-            seed_chains(app, chains)
-            app.set_args(["--chain", chain["name"], "db", "chain", "get"]).run()
+            seed_chains(chains)
+            app.set_args(["chain", "get", chain["name"]]).run()
             data, output = app.last_rendered
-            assert data["out"] == chain["name"]
+            assert data["name"] == chain["name"]
+            assert data["chain_id"] == chain["chain_id"]
+            assert data["coin"] == chain["coin"]
+            assert data["tx_type"] == chain["tx_type"]
+            assert data["desc"] == chain["desc"]
+            assert data["middlewares"] == chain["middlewares"]
 
 
-def test_chain_get_no_args(chains: List[ChainFields]) -> None:
-    """Without any argument > return the default chain"""
+def test_chain_active(chains: List[ChainFields]) -> None:
     for chain in chains:
         with Web3CliTest() as app:
-            seed_chains(app, chains)
+            seed_chains(chains)
             app.config.set("web3cli", "default_chain", chain["name"])
-            app.set_args(["db", "chain", "get"]).run()
+            app.set_args(["chain", "active"]).run()
             data, output = app.last_rendered
             assert data["out"] == chain["name"]
 
 
 def test_chain_delete(chains: List[ChainFields]) -> None:
     for c in chains:
         with Web3CliTest() as app:
-            seed_chains(app, chains)
+            seed_chains(chains)
             app.set_args(
                 [
-                    "db",
                     "chain",
                     "delete",
                     c["name"],
                 ]
             ).run()
             assert Chain.select().count() == len(chains) - 1
+            with pytest.raises(RecordNotFound):
+                Chain.get_by_name_or_raise(c["name"])
```

### Comparing `web3cli-0.9.6/tests/controllers/db/test_rpc.py` & `web3cli-1.0.0/tests/web3cli/controllers/crud/test_rpc_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-from tests.main import Web3CliTest
 from typing import List
-from tests.seeder import seed_chains
-from web3cli.core.exceptions import RpcIsInvalid
-from web3cli.core.models.chain import Chain, Rpc
+
 import pytest
-from web3cli.core.models.types import ChainFields
+
+from tests.web3cli.main import Web3CliTest
+from web3core.exceptions import RpcIsInvalid
+from web3core.helpers.seed import seed_chains
+from web3core.models.chain import Chain, Rpc
+from web3core.models.types import ChainFields
 
 
 def test_rpc_list(chains: List[ChainFields]) -> None:
     with Web3CliTest() as app:
-        seed_chains(app, chains)
-        app.set_args(["db", "rpc", "list"]).run()
+        seed_chains(chains)
+        app.set_args(["rpc", "list"]).run()
         data, output = app.last_rendered
         for c in chains:
             for r in c["rpcs"]:
                 assert (
                     r["url"][0 : app.config.get("web3cli", "output_table_wrap")]
                     in output
                 )
@@ -22,73 +24,73 @@
 
 def test_rpc_add(chains: List[ChainFields]) -> None:
     c = chains[0]
     # Add two different RPCs > they should be in the DB
     test_rpcs = ["https://www.example-1.com", "https://www.example-2.com"]
     with Web3CliTest() as app:
         chain = Chain.create(name=c["name"], chain_id=c["chain_id"], coin=c["coin"])
-        app.set_args(["db", "rpc", "add", chain.name] + test_rpcs).run()
+        app.set_args(["rpc", "add", "--chain", chain.name] + test_rpcs).run()
         created_rpcs = chain.get_rpcs()
         assert len(created_rpcs) == len(test_rpcs)
         for i, rpc in enumerate(created_rpcs):
             assert rpc.url == test_rpcs[i]
     # Add the same RPCs again > they should not be added to the db
     with Web3CliTest(delete_db=False) as app:
-        app.set_args(["db", "rpc", "add", chain.name] + test_rpcs).run()
+        app.set_args(["rpc", "add", "--chain", chain.name] + test_rpcs).run()
         assert len(chain.get_rpcs()) == len(test_rpcs)
     # Add an RPC with a wrong URL > it should raise
     with Web3CliTest() as app:
         chain = Chain.create(name=c["name"], chain_id=c["chain_id"], coin=c["coin"])
         with pytest.raises(RpcIsInvalid):
-            app.set_args(["db", "rpc", "add", chain.name, "not a URI"]).run()
+            app.set_args(["rpc", "add", "not a URI", "--chain", chain.name]).run()
 
 
 def test_rpc_get_with_id_argument(chains: List[ChainFields]) -> None:
     """With ID argument > it should return the url of the RPC with given ID"""
     with Web3CliTest() as app:
-        seed_chains(app, chains)
+        seed_chains(chains)
         rpcs = Rpc.get_all()
     for rpc in rpcs:
         with Web3CliTest(delete_db=False) as app:
-            app.set_args(["db", "rpc", "get", str(rpc.id)]).run()
+            app.set_args(["rpc", "get", str(rpc.id)]).run()
             data, output = app.last_rendered
             assert data["out"] == rpc.url
 
 
 def test_rpc_get_with_rpc_argument(chains: List[ChainFields]) -> None:
     """With RPC argument > it should return the argument"""
     test_rpcs = ["https://www.example-1.com", "https://www.example-2.com"]
     for rpc_url in test_rpcs:
         with Web3CliTest() as app:
-            app.set_args(["--rpc", rpc_url, "db", "rpc", "get"]).run()
+            seed_chains(chains)
+            app.set_args(["rpc", "get", "--rpc", rpc_url]).run()
             data, output = app.last_rendered
             assert data["out"] == rpc_url
 
 
 def test_rpc_get_with_no_args(chains: List[ChainFields]) -> None:
     """Without arguments > should return an RPC of the user-provided chain"""
     for c in chains:
         with Web3CliTest() as app:
-            seed_chains(app, chains)
-            app.set_args(["--chain", c["name"], "db", "rpc", "get"]).run()
+            seed_chains(chains)
+            app.set_args(["rpc", "get", "--chain", c["name"]]).run()
             data, output = app.last_rendered
             chain: Chain = Chain.select().where(Chain.name == c["name"]).get()
             assert data["out"] in [r.url for r in chain.get_rpcs()]
 
 
 def test_rpc_delete(chains: List[ChainFields]) -> None:
     with Web3CliTest() as app:
-        seed_chains(app, chains)
+        seed_chains(chains)
         rpcs = Rpc.get_all()
     n_rpcs = len(rpcs)
     for i, rpc in enumerate(rpcs):
         with Web3CliTest(delete_db=False) as app:
             app.set_args(
                 [
-                    "db",
                     "rpc",
                     "delete",
                     str(rpc.id),
                 ]
             ).run()
             with pytest.raises(Exception):
                 Rpc.get(rpc.id)
```

### Comparing `web3cli-0.9.6/tests/controllers/db/test_tx.py` & `web3cli-1.0.0/tests/web3cli/controllers/crud/test_history_controller.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,90 +1,94 @@
 from typing import List
-from tests.main import Web3CliTest
-from web3cli.core.models.tx import Tx
-from tests.seeder import seed_txs
-from web3cli.core.models.types import TxFields
 
+import pytest
 
-def test_tx_list(txs: List[TxFields]) -> None:
+from tests.web3cli.main import Web3CliTest
+from web3core.exceptions import TxNotFound
+from web3core.helpers.seed import seed_chains, seed_txs
+from web3core.models.tx import Tx
+from web3core.models.types import ChainFields, TxFields
+
+
+def test_history_list(txs: List[TxFields]) -> None:
     """Add txs and check that they are listed from oldest to newest"""
     txs = sorted(txs, key=lambda t: t["created_at"], reverse=True)
     with Web3CliTest() as app:
-        seed_txs(app, txs)
-        app.set_args(["db", "tx", "list"]).run()
+        seed_txs(txs)
+        app.set_args(["history", "list"]).run()
         data, output = app.last_rendered
         for i in range(0, len(txs)):
             assert data[i][0] == txs[i]["hash"]
             assert data[i][1] == str(txs[i]["chain"])
 
 
-def test_tx_get(txs: List[TxFields]) -> None:
+def test_history_get(txs: List[TxFields]) -> None:
     for t in txs:
         with Web3CliTest() as app:
-            seed_txs(app, txs)
+            seed_txs(txs)
             app.set_args(
                 [
-                    "db",
-                    "tx",
+                    "history",
                     "get",
                     t["hash"],
                 ]
             ).run()
             data, output = app.last_rendered
             assert t["hash"] in output
             assert str(t["gas"]) in output
             assert t["gas_price"] in output
 
 
-def test_tx_add(txs: List[TxFields]) -> None:
+def test_history_add(txs: List[TxFields], chains: List[ChainFields]) -> None:
     for t in txs:
         with Web3CliTest() as app:
+            seed_chains(chains)
             app.set_args(
                 [
-                    "db",
-                    "tx",
+                    "history",
                     "add",
                     t["hash"],
                     t["from_"],
                     t["to"],
                 ]
             ).run()
             tx = Tx.get_by_hash(t["hash"])
             assert tx.select().count() == 1
-            assert Tx.from_ == t["from_"]
-            assert Tx.to == t["to"]
+            assert tx.from_ == t["from_"]
+            assert tx.to == t["to"]
 
 
-def test_tx_update(txs: List[TxFields]) -> None:
+def test_history_update(txs: List[TxFields], chains: List[ChainFields]) -> None:
     """Create tx 0, then update it with the data of tx 1,
     while keeping the same hash"""
     with Web3CliTest() as app:
-        seed_txs(app, [txs[0]])
+        seed_chains(chains)
+        seed_txs([txs[0]])
         app.set_args(
             argv=[
-                "db",
-                "tx",
+                "history",
                 "add",
                 txs[0]["hash"],
                 txs[1]["from_"],
                 txs[1]["to"],
                 "--update",
             ]
         ).run()
         tx = Tx.get_by_hash(txs[0]["hash"])
-        assert Tx.from_ == txs[1]["from_"]
-        assert Tx.to == txs[1]["to"]
+        assert tx.from_ == txs[1]["from_"]
+        assert tx.to == txs[1]["to"]
 
 
-def test_tx_delete(txs: List[TxFields]) -> None:
+def test_history_delete(txs: List[TxFields]) -> None:
     for t in txs:
         with Web3CliTest() as app:
-            seed_txs(app, txs)
+            seed_txs(txs)
             app.set_args(
                 [
-                    "db",
-                    "tx",
+                    "history",
                     "delete",
                     t["hash"],
                 ]
             ).run()
             assert Tx.select().count() == len(txs) - 1
+            with pytest.raises(TxNotFound):
+                Tx.get_by_hash_or_raise(t["hash"])
```

### Comparing `web3cli-0.9.6/tests/controllers/test_key.py` & `web3cli-1.0.0/tests/web3cli/controllers/test_appkey_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-from tests.main import Web3CliTest
 import ast
-from tests import helper
-import ruamel.yaml
 import os
 
+import ruamel.yaml
+
+from tests import helper
+from tests.web3cli.main import Web3CliTest
+
 
-def test_key_create() -> None:
+def test_appkey_create() -> None:
     with Web3CliTest() as app:
         # Delete config file and unset app_key
         helper.delete_test_config_file(app)
         app.config.set("web3cli", "app_key", None)
-        # Run the command `w3 key create`
+        # Run the command `w3 app-key create`
         app.set_args(
             [
-                "key",
+                "app-key",
                 "create",
             ]
         ).run()
         # Now the config file should exist...
         config_file = helper.get_test_config_file()
         assert os.path.isfile(config_file)
         # ... and it should contain the app key
@@ -25,22 +27,22 @@
         with open(config_file, "r") as file:
             config = yaml.load(file)
         app_key = config["web3cli"]["app_key"]
         assert type(app_key) is str
         assert type(ast.literal_eval(app_key)) is bytes
 
 
-def test_key_update() -> None:
+def test_appkey_update() -> None:
     with Web3CliTest() as app:
         # Take note of the app_key before it is updated
         old_key = app.config.get("web3cli", "app_key")
-        # Run the command `w3 key create --force`
+        # Run the command `w3 app-key create --force`
         app.set_args(
             [
-                "key",
+                "app-key",
                 "create",
                 "--force",
             ]
         ).run()
         # The config file should exist...
         config_file = helper.get_test_config_file()
         assert os.path.isfile(config_file)
```

### Comparing `web3cli-0.9.6/tests/core/helpers/test_crypto.py` & `web3cli-1.0.0/tests/web3core/helpers/test_crypto_helper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-from web3cli.core.helpers import crypto
 import secrets
+
 import pytest
 
+from web3core.helpers import crypto
+
 
 @pytest.mark.parametrize(
     "msg",
     [
         b"d94e4166f0b3c85ffebed3e0eaa7f7680ae296cf8a7229d637472b7452c8602c",
         b"3bc2f9b05ac28389fd65fd40068a10f730ec66b6293f9cfd8fe804d212ce06bb",
         b"f76c67c2dd62222a5ec747116a66c573f3795c53276c0cdeafbcb5f597e2f8d4",
```

### Comparing `web3cli-0.9.6/tests/helper.py` & `web3cli-1.0.0/tests/helper.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-"""Please note this file DOES NOT contain tests, but
-helper functions to better run tests"""
+"""Helper functions to better run tests"""
 
+import os
 import secrets
 import string
-from web3cli.core.helpers import yaml
 from typing import Any
+
 from web3cli.main import Web3Cli
-import os
+from web3core.helpers import yaml
 
 
 def get_test_config_file() -> str:
     """Path to the config file that the app will use while running tests"""
     return os.path.join(
         os.path.expanduser("~"), ".web3cli", "config", "web3cli_test.yml"
     )
```

### Comparing `web3cli-0.9.6/tests/helpers/test_crypto.py` & `web3cli-1.0.0/tests/web3cli/helpers/test_crypto_helper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from tests.main import Web3CliTest
-from web3cli.helpers import crypto
 import pytest
 
+from tests.web3cli.main import Web3CliTest
+from web3cli.helpers import crypto
+
 
 @pytest.mark.parametrize(
     "msg",
     [
         "d94e4166f0b3c85ffebed3e0eaa7f7680ae296cf8a7229d637472b7452c8602c",
         "3bc2f9b05ac28389fd65fd40068a10f730ec66b6293f9cfd8fe804d212ce06bb",
         "f76c67c2dd62222a5ec747116a66c573f3795c53276c0cdeafbcb5f597e2f8d4",
```

### Comparing `web3cli-0.9.6/tests/main.py` & `web3cli-1.0.0/tests/web3cli/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import os
 from typing import Any, List
+
 from cement import TestApp
+
+from tests import helper
 from web3cli import hooks
-from web3cli.main import Web3Cli, CONFIG
 from web3cli.helpers import database
-from tests import helper
+from web3cli.main import CONFIG, Web3Cli
 
 # Each time you run the test app, a brand new database
-# will be created
+# will be created, with no seeding
 CONFIG["web3cli"]["db_file"] = os.path.join(
     os.path.expanduser("~"), ".web3cli", "database", "web3cli_test.sqlite"
 )
+CONFIG["web3cli"]["populate_db"] = False
 
 
 class Web3CliTest(TestApp, Web3Cli):
     """A sub-class of Web3Cli that is better suited for testing."""
 
     def __init__(self, label: str = None, delete_db: bool = True, **kw: Any) -> None:
         super().__init__(label, **kw)
```

### Comparing `web3cli-0.9.6/tests/seeder.py` & `web3cli-1.0.0/tests/seed.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,89 +1,92 @@
-"""Please note this file DOES NOT contain tests, but
-helper functions to better run tests"""
+"""Helper functions to populate the DB for the tests"""
 
-from typing import Any, Dict, List
+from typing import List
 
-from web3cli.core.exceptions import Web3CliError
-from web3cli.core.models.chain import Chain
-from web3cli.core.models.tx import Tx
-from web3cli.core.models.types import AddressFields, ChainFields, TxFields
-from web3cli.core.seeds.chain_seeds import local_chain
+import ape
+from web3cli.exceptions import Web3CliError
 from web3cli.helpers.database import db_ready_or_raise
 from web3cli.main import Web3Cli
-from web3cli.core.models.address import Address
-from web3cli.core.models.signer import Signer
-from brownie.network.account import Account
-import brownie
+from web3core.helpers.seed import seed_chain
+from web3core.models.chain import Chain
+from web3core.models.contract import Contract
+from web3core.models.signer import Signer
+from web3core.seeds import chain_seeds
 
 
-def seed_chain(app: Web3Cli, chain: ChainFields, make_default: bool = True) -> Chain:
-    """Add the given chain to the database, and optionally
-    make it the default network"""
-    db_ready_or_raise(app)
+def seed_local_chain(app: Web3Cli, chain_name: str, make_default: bool = True) -> Chain:
+    """Add the given local chain to the DB and make it the default network"""
+    chain = seed_chain(getattr(chain_seeds, f"{chain_name}"))
     if make_default:
-        app.config.set("web3cli", "default_chain", local_chain["name"])
-    return Chain.seed_one(local_chain)
-
-
-def seed_chains(app: Web3Cli, chains: List[ChainFields]) -> List[Chain]:
-    """Add the given chains to the database"""
-    db_ready_or_raise(app)
-    return Chain.seed(chains)
-
-
-def seed_addresses(app: Web3Cli, addresses: List[AddressFields]) -> List[Address]:
-    """Add the given addresses to the database"""
-    db_ready_or_raise(app)
-    return [Address.create(**a) for a in addresses]
-
-
-def seed_signers(app: Web3Cli, signers: List[Dict[str, Any]]) -> List[Signer]:
-    """Add the given signers to the database"""
-    db_ready_or_raise(app)
-    return [
-        Signer.create_encrypt(name=s["name"], key=s["private_key"], pwd=app.app_key)
-        for s in signers
-    ]
-
-
-def seed_txs(app: Web3Cli, txs: List[TxFields]) -> List[Tx]:
-    """Add the given transactions to the database"""
-    db_ready_or_raise(app)
-    return [Tx.create(**t) for t in txs]
-
-
-def seed_local_chain(app: Web3Cli, make_default: bool = True) -> Chain:
-    """Add the local network as a chain, with name 'local' and
-    make it the default network"""
-    return seed_chain(app, local_chain, make_default)
+        app.config.set("web3cli", "default_chain", chain.name)
+    return chain
 
 
 def seed_local_accounts(
     app: Web3Cli,
-    accounts: List[Account],
+    accounts: ape.managers.accounts.AccountManager,
     accounts_keys: List[str],
     default_signer: str = None,
-) -> List[Account]:
-    """Create a signer for each of the given brownie accounts,
+) -> ape.managers.accounts.AccountManager:
+    """Create a signer for each of the given ape accounts,
     with numeric names: s0, s1, s2, etc.
 
     Accounts 0 and 1 will be added a second time with names 'alice'
     and 'bob', respectively.
 
     Optionally, set one of the accounts to be the default signer."""
     db_ready_or_raise(app)
     # Create alice and bob signers
     Signer.create_encrypt(name="alice", key=accounts_keys[0], pwd=app.app_key)
     Signer.create_encrypt(name="bob", key=accounts_keys[1], pwd=app.app_key)
-    # Create signers with names s0, s1, s2, ...
     for i, account in enumerate(accounts):
+        # Make sure keys are not exhausted
+        if i >= len(accounts_keys):
+            break
+        # Create signers with names s0, s1, s2, ...
         signer = Signer.create_encrypt(
             name=f"s{i}", key=accounts_keys[i], pwd=app.app_key
         )
         # Verify signer addresses
         if signer.address != account.address:
-            raise Web3CliError("Mismatch between brownie accounts and signers")
+            raise Web3CliError("Mismatch between ape accounts and signers")
     # Optionally set default signer
     if default_signer:
         app.config.set("web3cli", "default_signer", default_signer)
     return accounts
+
+
+def seed_local_contract(
+    app: Web3Cli,
+    name: str,
+    ape_contract: ape.contracts.ContractInstance,
+    type: str = None,
+    chain_name: str = None,
+) -> Contract:
+    """Create a contract in the DB for the given Brownie contract.
+
+    If you specify the contract type, that type's ABI will override
+    the ABI stored in the Brownie contract."""
+    db_ready_or_raise(app)
+    return Contract.create(
+        name=name,
+        desc=f"'{name}' contract imported from ape",
+        chain=chain_name or app.config.get("web3cli", "default_chain"),
+        address=ape_contract.address,
+        type=type,
+        abi=None if type else ape_contract.contract_type.dict()["abi"],
+    )
+
+
+def seed_local_token(
+    app: Web3Cli, token: ape.contracts.ContractInstance, chain_name: str = None
+) -> Contract:
+    """Create a contract in the DB for the given Brownie token"""
+    db_ready_or_raise(app)
+    return Contract.create(
+        name=token.symbol().lower(),
+        desc=token.name(),
+        chain=chain_name or app.config.get("web3cli", "default_chain"),
+        address=token.address,
+        type="erc20",
+        abi=token.contract_type.dict()["abi"],
+    )
```

### Comparing `web3cli-0.9.6/PKG-INFO` & `web3cli-1.0.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,573 +1,668 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 7765 6233  : 2.1.Name: web3
-00000020: 636c 690a 5665 7273 696f 6e3a 2030 2e39  cli.Version: 0.9
-00000030: 2e36 0a53 756d 6d61 7279 3a20 496e 7465  .6.Summary: Inte
-00000040: 7261 6374 2077 6974 6820 626c 6f63 6b63  ract with blockc
-00000050: 6861 696e 7320 616e 6420 736d 6172 7420  hains and smart 
-00000060: 636f 6e74 7261 6374 7320 7573 696e 6720  contracts using 
-00000070: 7468 6520 636f 6d6d 616e 6420 6c69 6e65  the command line
-00000080: 0a4c 6963 656e 7365 3a20 4d49 540a 4b65  .License: MIT.Ke
-00000090: 7977 6f72 6473 3a20 7765 6233 2c77 332c  ywords: web3,w3,
-000000a0: 636c 692c 6576 6d2c 626c 6f63 6b63 6861  cli,evm,blockcha
-000000b0: 696e 2c65 7468 6572 6575 6d2c 6269 6e61  in,ethereum,bina
-000000c0: 6e63 652c 6176 616c 616e 6368 650a 4175  nce,avalanche.Au
-000000d0: 7468 6f72 2d65 6d61 696c 3a20 636f 6363  thor-email: cocc
-000000e0: 6f69 6e6f 6d61 6e65 203c 636f 6363 6f69  oinomane <coccoi
-000000f0: 6e6f 6d61 6e65 4067 6d61 696c 2e63 6f6d  nomane@gmail.com
-00000100: 3e0a 5265 7175 6972 6573 2d50 7974 686f  >.Requires-Pytho
-00000110: 6e3a 203e 3d33 2e37 2e32 2c3c 332e 3131  n: >=3.7.2,<3.11
-00000120: 0a50 726f 6a65 6374 2d55 524c 3a20 686f  .Project-URL: ho
-00000130: 6d65 7061 6765 2c20 6874 7470 733a 2f2f  mepage, https://
-00000140: 6769 7468 7562 2e63 6f6d 2f63 6f63 636f  github.com/cocco
-00000150: 696e 6f6d 616e 652f 7765 6233 636c 690a  inomane/web3cli.
-00000160: 5072 6f6a 6563 742d 5552 4c3a 2072 6570  Project-URL: rep
-00000170: 6f73 6974 6f72 792c 2068 7474 7073 3a2f  ository, https:/
-00000180: 2f67 6974 6875 622e 636f 6d2f 636f 6363  /github.com/cocc
-00000190: 6f69 6e6f 6d61 6e65 2f77 6562 3363 6c69  oinomane/web3cli
-000001a0: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
-000001b0: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
-000001c0: 6d61 726b 646f 776e 0a0a 496e 7465 7261  markdown..Intera
-000001d0: 6374 2077 6974 6820 626c 6f63 6b63 6861  ct with blockcha
-000001e0: 696e 7320 616e 6420 736d 6172 7420 636f  ins and smart co
-000001f0: 6e74 7261 6374 7320 7573 696e 6720 7468  ntracts using th
-00000200: 6520 636f 6d6d 616e 6420 6c69 6e65 2e0a  e command line..
-00000210: 0a23 2046 6561 7475 7265 730a 0a2d 2045  .# Features..- E
-00000220: 6173 696c 7920 696e 7465 7261 6374 2077  asily interact w
-00000230: 6974 6820 4556 4d2d 636f 6d70 6174 6962  ith EVM-compatib
-00000240: 6c65 2063 6861 696e 7320 7573 696e 6720  le chains using 
-00000250: 796f 7572 2074 6572 6d69 6e61 6c0a 2d20  your terminal.- 
-00000260: 576f 726b 7320 7769 7468 2074 6865 206d  Works with the m
-00000270: 6f73 7420 706f 7075 6c61 7220 6368 6169  ost popular chai
-00000280: 6e73 3a20 4574 6865 7265 756d 2c20 4269  ns: Ethereum, Bi
-00000290: 6e61 6e63 652c 2041 7661 6c61 6e63 6865  nance, Avalanche
-000002a0: 2061 6e64 206d 6f72 6520 746f 2063 6f6d   and more to com
-000002b0: 650a 2d20 5361 7665 2061 6464 7265 7373  e.- Save address
-000002c0: 6573 2079 6f75 2075 7365 206f 6674 656e  es you use often
-000002d0: 2061 6e64 2061 6363 6573 7320 7468 656d   and access them
-000002e0: 2077 6974 6820 7468 6569 7220 7461 670a   with their tag.
-000002f0: 2d20 5365 6e64 2074 7261 6e73 6163 7469  - Send transacti
-00000300: 6f6e 7320 6672 6f6d 206d 756c 7469 706c  ons from multipl
-00000310: 6520 7369 676e 6572 730a 2d20 436f 6e63  e signers.- Conc
-00000320: 6174 656e 6174 6520 636f 6d6d 616e 6473  atenate commands
-00000330: 2074 6f20 6275 696c 6420 706f 7765 7266   to build powerf
-00000340: 756c 2073 6372 6970 7473 0a2d 205b 546f  ul scripts.- [To
-00000350: 2062 6520 696d 706c 656d 656e 7465 645d   be implemented]
-00000360: 3a20 5472 616e 7366 6572 2074 6f6b 656e  : Transfer token
-00000370: 732c 2075 7369 6e67 2074 6865 2074 6f6b  s, using the tok
-00000380: 656e 206e 616d 6520 2855 5344 432c 2055  en name (USDC, U
-00000390: 4e49 2c20 5745 5448 2c20 6574 6329 2069  NI, WETH, etc) i
-000003a0: 6e73 7465 6164 206f 6620 6974 7320 6164  nstead of its ad
-000003b0: 6472 6573 732e 0a2d 205b 546f 2062 6520  dress..- [To be 
-000003c0: 696d 706c 656d 656e 7465 645d 3a20 4465  implemented]: De
-000003d0: 4669 2073 7570 706f 7274 3a20 7365 6c6c  Fi support: sell
-000003e0: 2043 7572 7665 2773 2072 6577 6172 6473   Curve's rewards
-000003f0: 206f 6e20 556e 6973 7761 702c 2073 6574   on Uniswap, set
-00000400: 7570 2061 2044 4341 2070 6c61 6e20 6f6e  up a DCA plan on
-00000410: 2054 7261 6465 724a 6f65 2c20 6574 632e   TraderJoe, etc.
-00000420: 0a0a 0a23 2049 6e73 7461 6c6c 0a0a 6060  ...# Install..``
-00000430: 6062 6173 680a 7069 7033 2069 6e73 7461  `bash.pip3 insta
-00000440: 6c6c 202d 5520 7765 6233 636c 690a 6060  ll -U web3cli.``
-00000450: 600a 0a23 2053 696d 706c 6520 6578 616d  `..# Simple exam
-00000460: 706c 6573 0a0a 2d20 4164 6420 6368 6169  ples..- Add chai
-00000470: 6e73 2062 6566 6f72 6520 7573 696e 6720  ns before using 
-00000480: 7468 656d 3a0a 2020 2060 6060 0a20 2020  them:.   ```.   
-00000490: 7733 2064 6220 6368 6169 6e20 6164 6420  w3 db chain add 
-000004a0: 6574 6865 7265 756d 2031 2045 5448 202d  ethereum 1 ETH -
-000004b0: 2d74 782d 7479 7065 2032 202d 2d72 7063  -tx-type 2 --rpc
-000004c0: 2068 7474 7073 3a2f 2f63 6c6f 7564 666c   https://cloudfl
-000004d0: 6172 652d 6574 682e 636f 6d20 0a20 2020  are-eth.com .   
-000004e0: 7733 2064 6220 6368 6169 6e20 6164 6420  w3 db chain add 
-000004f0: 6269 6e61 6e63 6520 3536 2042 4e42 202d  binance 56 BNB -
-00000500: 2d72 7063 2068 7474 7073 3a2f 2f62 7363  -rpc https://bsc
-00000510: 2d64 6174 6173 6565 642e 6269 6e61 6e63  -dataseed.binanc
-00000520: 652e 6f72 672f 0a20 2020 7733 2064 6220  e.org/.   w3 db 
-00000530: 6368 6169 6e20 6164 6420 6176 616c 616e  chain add avalan
-00000540: 6368 6520 3433 3131 3420 2d2d 7270 6320  che 43114 --rpc 
-00000550: 6874 7470 733a 2f2f 6170 692e 6176 6178  https://api.avax
-00000560: 2e6e 6574 776f 726b 2f65 7874 2f62 632f  .network/ext/bc/
-00000570: 432f 7270 630a 2020 2060 6060 0a20 2020  C/rpc.   ```.   
-00000580: 2e2e 2e20 6f72 2069 6d70 6f72 7420 7468  ... or import th
-00000590: 656d 2069 6e20 6f6e 6520 676f 3a0a 2020  em in one go:.  
-000005a0: 2060 6060 0a20 2020 7733 2064 6220 6368   ```.   w3 db ch
-000005b0: 6169 6e20 7365 6564 0a20 2020 6060 600a  ain seed.   ```.
-000005c0: 0a2d 2047 6574 2074 6865 2045 5448 2062  .- Get the ETH b
-000005d0: 616c 616e 6365 206f 6620 7468 6520 4574  alance of the Et
-000005e0: 6865 7265 756d 2066 6f75 6e64 6174 696f  hereum foundatio
-000005f0: 6e3a 0a20 2020 6060 600a 2020 2077 3320  n:.   ```.   w3 
-00000600: 2d2d 6368 6169 6e20 6574 6865 7265 756d  --chain ethereum
-00000610: 2062 616c 616e 6365 2030 7864 6530 6232   balance 0xde0b2
-00000620: 3935 3636 3961 3966 6439 3364 3566 3238  95669a9fd93d5f28
-00000630: 6439 6563 3835 6534 3066 3463 6236 3937  d9ec85e40f4cb697
-00000640: 6261 650a 2020 2060 6060 0a20 2020 2e2e  bae.   ```.   ..
-00000650: 2e20 6f72 2074 6865 2042 4e42 2062 616c  . or the BNB bal
-00000660: 616e 6365 206f 6620 6120 4269 6e61 6e63  ance of a Binanc
-00000670: 6520 686f 7420 7761 6c6c 6574 206f 6e20  e hot wallet on 
-00000680: 424e 4220 6368 6169 6e3a 0a20 2020 6060  BNB chain:.   ``
-00000690: 600a 2020 2077 3320 2d2d 6368 6169 6e20  `.   w3 --chain 
-000006a0: 6269 6e61 6e63 6520 6261 6c61 6e63 6520  binance balance 
-000006b0: 3078 3838 3934 6530 6130 6339 3632 6362  0x8894e0a0c962cb
-000006c0: 3732 3363 3139 3736 6134 3432 3163 3935  723c1976a4421c95
-000006d0: 3934 3962 6532 6434 6533 0a20 2020 6060  949be2d4e3.   ``
-000006e0: 600a 0a2d 2054 6972 6564 206f 6620 7573  `..- Tired of us
-000006f0: 696e 6720 7468 6520 602d 2d63 6861 696e  ing the `--chain
-00000700: 6020 6172 6775 6d65 6e74 3f20 5365 7420  ` argument? Set 
-00000710: 6120 6465 6661 756c 7420 6368 6169 6e3a  a default chain:
-00000720: 0a20 2020 6060 600a 2020 2077 3320 636f  .   ```.   w3 co
-00000730: 6e66 6967 2073 6574 2064 6566 6175 6c74  nfig set default
-00000740: 5f63 6861 696e 2065 7468 6572 6575 6d0a  _chain ethereum.
-00000750: 2020 2077 3320 6261 6c61 6e63 6520 3078     w3 balance 0x
-00000760: 6465 3062 3239 3536 3639 6139 6664 3933  de0b295669a9fd93
-00000770: 6435 6632 3864 3965 6338 3565 3430 6634  d5f28d9ec85e40f4
-00000780: 6362 3639 3762 6165 0a20 2020 6060 600a  cb697bae.   ```.
-00000790: 0a2d 2054 6972 6564 206f 6620 7061 7374  .- Tired of past
-000007a0: 696e 6720 6164 6472 6573 7365 7320 6172  ing addresses ar
-000007b0: 6f75 6e64 3f20 5361 7665 2074 6865 6d20  ound? Save them 
-000007c0: 7769 7468 2061 6e20 6561 7379 2074 6f20  with an easy to 
-000007d0: 7265 6d65 6d62 6572 206e 616d 653a 0a20  remember name:. 
-000007e0: 2020 6060 600a 2020 2077 3320 6462 2061    ```.   w3 db a
-000007f0: 6464 7265 7373 2061 6464 2065 7468 6572  ddress add ether
-00000800: 6575 6d2d 666f 756e 6461 7469 6f6e 2030  eum-foundation 0
-00000810: 7864 6530 6232 3935 3636 3961 3966 6439  xde0b295669a9fd9
-00000820: 3364 3566 3238 6439 6563 3835 6534 3066  3d5f28d9ec85e40f
-00000830: 3463 6236 3937 6261 650a 2020 2077 3320  4cb697bae.   w3 
-00000840: 6261 6c61 6e63 6520 6574 6865 7265 756d  balance ethereum
-00000850: 2d66 6f75 6e64 6174 696f 6e0a 2020 2060  -foundation.   `
-00000860: 6060 0a0a 2d20 5761 6e74 2074 6f20 7365  ``..- Want to se
-00000870: 6e64 2074 7261 6e73 6163 7469 6f6e 733f  nd transactions?
-00000880: 2041 6464 2061 2073 6967 6e65 723a 0a20   Add a signer:. 
-00000890: 2020 6060 600a 2020 2077 3320 6462 2073    ```.   w3 db s
-000008a0: 6967 6e65 7220 6164 6420 6d79 2d77 616c  igner add my-wal
-000008b0: 6c65 740a 2020 2060 6060 0a20 2020 596f  let.   ```.   Yo
-000008c0: 7520 7769 6c6c 2062 6520 6173 6b65 6420  u will be asked 
-000008d0: 666f 7220 6120 7072 6976 6174 6520 6b65  for a private ke
-000008e0: 792c 2077 6869 6368 2077 696c 6c20 6265  y, which will be
-000008f0: 2073 6176 6564 206f 6e20 6469 736b 2069   saved on disk i
-00000900: 6e20 656e 6372 7970 7465 6420 666f 726d  n encrypted form
-00000910: 2e0a 0a0a 2d20 4f6e 6365 2079 6f75 2068  ....- Once you h
-00000920: 6176 6520 6120 7369 676e 6572 2c20 796f  ave a signer, yo
-00000930: 7520 6361 6e20 7365 6e64 2031 2045 5448  u can send 1 ETH
-00000940: 2074 6f20 7468 6520 4574 6865 7265 756d   to the Ethereum
-00000950: 2066 6f75 6e64 6174 696f 6e3a 0a20 2020   foundation:.   
-00000960: 6060 6062 6173 680a 2020 2077 3320 7365  ```bash.   w3 se
-00000970: 6e64 2065 7468 6572 6575 6d2d 666f 756e  nd ethereum-foun
-00000980: 6461 7469 6f6e 2031 2045 5448 0a20 2020  dation 1 ETH.   
-00000990: 6060 600a 2020 206f 7220 6d61 7962 6520  ```.   or maybe 
-000009a0: 6974 2773 2062 6574 7465 7220 746f 2073  it's better to s
-000009b0: 656e 6420 6a75 7374 2031 2067 7765 693a  end just 1 gwei:
-000009c0: 0a20 2020 6060 600a 2020 2077 3320 7365  .   ```.   w3 se
-000009d0: 6e64 2065 7468 6572 6575 6d2d 666f 756e  nd ethereum-foun
-000009e0: 6461 7469 6f6e 2031 2045 5448 2067 7765  dation 1 ETH gwe
-000009f0: 690a 2020 2060 6060 0a0a 2d20 4e65 6564  i.   ```..- Need
-00000a00: 2074 6f20 7369 676e 2061 206d 6573 7361   to sign a messa
-00000a10: 6765 3f20 5468 6973 2077 696c 6c20 7072  ge? This will pr
-00000a20: 696e 7420 7468 6520 7768 6f6c 6520 7369  int the whole si
-00000a30: 676e 6564 206d 6573 7361 6765 3a0a 2020  gned message:.  
-00000a40: 2060 6060 6261 7368 0a20 2020 7733 2073   ```bash.   w3 s
-00000a50: 6967 6e20 2248 656c 6c6f 2077 6f72 6c64  ign "Hello world
-00000a60: 2122 0a20 2020 6060 600a 0a23 2041 6464  !".   ```..# Add
-00000a70: 7265 7373 2062 6f6f 6b0a 0a60 7733 6020  ress book..`w3` 
-00000a80: 6361 6e20 7374 6f72 6520 7461 6773 206a  can store tags j
-00000a90: 7573 7420 6c69 6b65 2079 6f75 2077 6f75  ust like you wou
-00000aa0: 6c64 2064 6f20 6f6e 2065 7468 6572 7363  ld do on ethersc
-00000ab0: 616e 2e69 6f20 6f72 2062 7363 7363 616e  an.io or bscscan
-00000ac0: 2e63 6f6d 3a0a 0a60 6060 6261 7368 0a77  .com:..```bash.w
-00000ad0: 3320 6462 2061 6464 7265 7373 2061 6464  3 db address add
-00000ae0: 2022 4574 6865 7265 756d 2066 6f75 6e64   "Ethereum found
-00000af0: 6174 696f 6e22 2030 7864 6530 6232 3935  ation" 0xde0b295
-00000b00: 3636 3961 3966 6439 3364 3566 3238 6439  669a9fd93d5f28d9
-00000b10: 6563 3835 6534 3066 3463 6236 3937 6261  ec85e40f4cb697ba
-00000b20: 650a 7733 2064 6220 6164 6472 6573 7320  e.w3 db address 
-00000b30: 6164 6420 2242 696e 616e 6365 2068 6f74  add "Binance hot
-00000b40: 2077 616c 6c65 7422 2030 7838 3839 3465   wallet" 0x8894e
-00000b50: 3061 3063 3936 3263 6237 3233 6331 3937  0a0c962cb723c197
-00000b60: 3661 3434 3231 6339 3539 3439 6265 3264  6a4421c95949be2d
-00000b70: 3465 330a 6060 600a 0a59 6f75 2063 616e  4e3.```..You can
-00000b80: 2075 7365 2074 6865 7365 2074 6167 7320   use these tags 
-00000b90: 696e 7374 6561 6420 6f66 2074 6865 2061  instead of the a
-00000ba0: 6374 7561 6c20 6164 6472 6573 7365 733a  ctual addresses:
-00000bb0: 0a0a 6060 6062 6173 680a 7733 2062 616c  ..```bash.w3 bal
-00000bc0: 616e 6365 2022 4574 6865 7265 756d 2066  ance "Ethereum f
-00000bd0: 6f75 6e64 6174 696f 6e22 0a77 3320 2d2d  oundation".w3 --
-00000be0: 6368 6169 6e20 6269 6e61 6e63 6520 6261  chain binance ba
-00000bf0: 6c61 6e63 6520 2242 696e 616e 6365 2068  lance "Binance h
-00000c00: 6f74 2077 616c 6c65 7422 0a60 6060 0a0a  ot wallet".```..
-00000c10: 546f 2073 6565 2074 6865 206c 6973 7420  To see the list 
-00000c20: 6f66 2073 6176 6564 2061 6464 7265 7373  of saved address
-00000c30: 6573 2c20 7275 6e3a 0a0a 6060 6062 6173  es, run:..```bas
-00000c40: 680a 7733 2064 6220 6164 6472 6573 7320  h.w3 db address 
-00000c50: 6c69 7374 0a60 6060 0a0a 7768 6963 6820  list.```..which 
-00000c60: 7769 6c6c 2070 726f 6475 6365 2074 6865  will produce the
-00000c70: 2066 6f6c 6c6f 7769 6e67 206f 7574 7075   following outpu
-00000c80: 743a 0a0a 6060 600a 7c20 4c41 4245 4c20  t:..```.| LABEL 
-00000c90: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00000ca0: 4144 4452 4553 5320 2020 2020 2020 2020  ADDRESS         
-00000cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000cc0: 2020 2020 2020 2020 2020 207c 0a7c 2d2d             |.|--
-00000cd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000ce0: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
-00000cf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000d00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000d10: 7c0a 7c20 4269 6e61 6e63 6520 686f 7420  |.| Binance hot 
-00000d20: 7761 6c6c 6574 2020 7c20 3078 3838 3934  wallet  | 0x8894
-00000d30: 6530 6130 6339 3632 6362 3732 3363 3139  e0a0c962cb723c19
-00000d40: 3736 6134 3432 3163 3935 3934 3962 6532  76a4421c95949be2
-00000d50: 6434 6533 207c 0a7c 2045 7468 6572 6575  d4e3 |.| Ethereu
-00000d60: 6d20 666f 756e 6461 7469 6f6e 207c 2030  m foundation | 0
-00000d70: 7864 6530 6232 3935 3636 3961 3966 6439  xde0b295669a9fd9
-00000d80: 3364 3566 3238 6439 6563 3835 6534 3066  3d5f28d9ec85e40f
-00000d90: 3463 6236 3937 6261 6520 7c0a 6060 600a  4cb697bae |.```.
-00000da0: 0a54 6f20 7365 6520 616c 6c20 7468 6520  .To see all the 
-00000db0: 6163 7469 6f6e 7320 7468 6174 2063 616e  actions that can
-00000dc0: 2062 6520 646f 6e65 2077 6974 6820 6164   be done with ad
-00000dd0: 6472 6573 7365 732c 2072 756e 2060 7733  dresses, run `w3
-00000de0: 2064 6220 6164 6472 6573 7360 2e0a 0a23   db address`...#
-00000df0: 2053 6967 6e20 2620 7365 6e64 0a0a 596f   Sign & send..Yo
-00000e00: 7520 6361 6e20 7573 6520 6077 6562 3363  u can use `web3c
-00000e10: 6c69 6020 746f 2073 656e 6420 7472 616e  li` to send tran
-00000e20: 7361 6374 696f 6e73 2074 6f20 7468 6520  sactions to the 
-00000e30: 626c 6f63 6b63 6861 696e 206f 7220 746f  blockchain or to
-00000e40: 2073 6967 6e20 6d65 7373 6167 6573 2e20   sign messages. 
-00000e50: 546f 2064 6f20 736f 2c20 796f 7520 6669  To do so, you fi
-00000e60: 7273 7420 6e65 6564 2074 6f20 6465 6669  rst need to defi
-00000e70: 6e65 2061 2073 6967 6e65 723a 0a0a 6060  ne a signer:..``
-00000e80: 6062 6173 680a 7733 2064 6220 7369 676e  `bash.w3 db sign
-00000e90: 6572 2061 6464 206d 795f 7369 676e 6572  er add my_signer
-00000ea0: 0a60 6060 0a0a 596f 7520 7769 6c6c 2062  .```..You will b
-00000eb0: 6520 7072 6f6d 7074 6564 2074 6f20 696e  e prompted to in
-00000ec0: 7365 7274 2061 2070 7269 7661 7465 206b  sert a private k
-00000ed0: 6579 2c20 7768 6963 6820 7769 6c6c 2062  ey, which will b
-00000ee0: 6520 656e 6372 7970 7465 6420 616e 6420  e encrypted and 
-00000ef0: 7374 6f72 6564 2069 6e20 7468 6520 6461  stored in the da
-00000f00: 7461 6261 7365 2e20 4665 656c 2066 7265  tabase. Feel fre
-00000f10: 6520 746f 2064 6f20 736f 2077 6974 6820  e to do so with 
-00000f20: 7468 6973 2074 6573 7420 7072 6976 6174  this test privat
-00000f30: 6520 6b65 793a 2060 6439 3465 3431 3636  e key: `d94e4166
-00000f40: 6630 6233 6338 3566 6665 6265 6433 6530  f0b3c85ffebed3e0
-00000f50: 6561 6137 6637 3638 3061 6532 3936 6366  eaa7f7680ae296cf
-00000f60: 3861 3732 3239 6436 3337 3437 3262 3734  8a7229d637472b74
-00000f70: 3532 6338 3630 3263 602e 0a0a 596f 7520  52c8602c`...You 
-00000f80: 6361 6e20 616c 736f 2063 7265 6174 6520  can also create 
-00000f90: 6120 6272 616e 6420 6e65 7720 7761 6c6c  a brand new wall
-00000fa0: 6574 206f 6e20 7468 6520 676f 2c20 7769  et on the go, wi
-00000fb0: 7468 6f75 7420 7468 6520 6e65 6564 2074  thout the need t
-00000fc0: 6f20 7072 6f76 6964 6520 6120 6b65 793a  o provide a key:
-00000fd0: 0a0a 6060 600a 7733 2064 6220 7369 676e  ..```.w3 db sign
-00000fe0: 6572 2061 6464 206d 792d 7761 6c6c 6574  er add my-wallet
-00000ff0: 202d 2d63 7265 6174 650a 6060 600a 0a23   --create.```..#
-00001000: 2323 2045 7861 6d70 6c65 730a 0a4f 6e63  ## Examples..Onc
-00001010: 6520 796f 7520 6861 7665 2061 6464 6564  e you have added
-00001020: 2061 2073 6967 6e65 722c 2079 6f75 2063   a signer, you c
-00001030: 616e 2075 7365 2061 6e79 206f 6620 7468  an use any of th
-00001040: 6520 636f 6d6d 616e 6473 2074 6861 7420  e commands that 
-00001050: 6e65 6564 2061 2070 7269 7661 7465 206b  need a private k
-00001060: 6579 2c20 6173 2073 686f 776e 2069 6e20  ey, as shown in 
-00001070: 7468 6520 666f 6c6c 6f77 696e 6720 6578  the following ex
-00001080: 616d 706c 6573 2e0a 0a2a 2a53 6967 6e20  amples...**Sign 
-00001090: 6120 6d65 7373 6167 652a 2a3a 0a0a 6060  a message**:..``
-000010a0: 6062 6173 680a 7733 2073 6967 6e20 2248  `bash.w3 sign "H
-000010b0: 656c 6c6f 2077 6f72 6c64 2122 0a60 6060  ello world!".```
-000010c0: 0a0a 4f75 7470 7574 3a0a 0a60 6060 7079  ..Output:..```py
-000010d0: 7468 6f6e 0a7b 276d 6573 7361 6765 4861  thon.{'messageHa
-000010e0: 7368 273a 2048 6578 4279 7465 7328 2730  sh': HexBytes('0
-000010f0: 7838 3134 3461 3666 6132 3662 6532 3532  x8144a6fa26be252
-00001100: 6238 3634 3536 3439 3166 6263 6434 3363  b86456491fbcd43c
-00001110: 3164 6537 6530 3232 3234 3138 3435 6666  1de7e022241845ff
-00001120: 6561 3163 3364 6630 3636 6637 6366 6564  ea1c3df066f7cfed
-00001130: 6527 292c 0a20 2772 273a 2032 3930 3634  e'),. 'r': 29064
-00001140: 3739 3233 3636 3335 3533 3233 3734 3039  7923663553237409
-00001150: 3530 3938 3533 3731 3130 3538 3935 3936  5098537110589596
-00001160: 3138 3538 3339 3832 3338 3938 3038 3833  1858398238980883
-00001170: 3737 3331 3933 3530 3138 3831 3237 3637  7731935018812767
-00001180: 3035 3232 3834 3831 2c0a 2027 7327 3a20  05228481,. 's': 
-00001190: 3335 3031 3738 3237 3039 3135 3430 3935  3501782709154095
-000011a0: 3238 3538 3433 3132 3233 3834 3930 3230  2858431223849020
-000011b0: 3130 3433 3031 3434 3839 3134 3738 3339  1043014489147839
-000011c0: 3939 3237 3731 3131 3039 3038 3038 3735  9927711109080875
-000011d0: 3430 3432 3231 3234 3339 3433 312c 0a20  4042212439431,. 
-000011e0: 2773 6967 6e61 7475 7265 273a 2048 6578  'signature': Hex
-000011f0: 4279 7465 7328 2730 7834 3034 3231 3665  Bytes('0x404216e
-00001200: 6132 3332 6235 3238 3936 3130 6137 3438  a232b5289610a748
-00001210: 3364 6537 3436 6665 6433 6339 3462 3665  3de746fed3c94b6e
-00001220: 3663 3262 3862 6636 3263 6535 3238 3638  6c2b8bf62ce52868
-00001230: 3530 6666 3334 3663 3134 6436 6236 3334  50ff346c14d6b634
-00001240: 3435 3130 3761 3964 3965 3334 3237 3230  45107a9d9e342720
-00001250: 6538 3865 3832 6133 6666 3739 3464 6436  e88e82a3ff794dd6
-00001260: 6264 3235 3539 3331 6235 3532 6465 6466  bd255931b552dedf
-00001270: 3265 3234 3364 3538 3731 6327 292c 0a20  2e243d5871c'),. 
-00001280: 2776 273a 2032 387d 0a60 6060 0a0a 2a2a  'v': 28}.```..**
-00001290: 5365 6e64 2045 5448 2c20 424e 422c 2041  Send ETH, BNB, A
-000012a0: 5641 582c 2065 7463 2a2a 3a0a 0a54 6869  VAX, etc**:..Thi
-000012b0: 7320 6973 2074 6f20 6265 2069 6d70 6c65  s is to be imple
-000012c0: 6d65 6e74 6564 2079 6574 2c20 6275 7420  mented yet, but 
-000012d0: 7468 6520 6964 6561 2069 7320 746f 2073  the idea is to s
-000012e0: 656e 6420 6675 6e64 7320 7769 7468 2074  end funds with t
-000012f0: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
-00001300: 6d61 6e64 3a0a 0a60 6060 6261 7368 0a77  mand:..```bash.w
-00001310: 3320 7365 6e64 203c 6164 6472 6573 733e  3 send <address>
-00001320: 2030 2e30 3031 2045 5448 0a60 6060 0a0a   0.001 ETH.```..
-00001330: 7768 6572 6520 6061 6464 7265 7373 6020  where `address` 
-00001340: 6973 2065 6974 6865 7220 616e 2061 6464  is either an add
-00001350: 7265 7373 2066 726f 6d20 7468 6520 6164  ress from the ad
-00001360: 6472 6573 7320 626f 6f6b 2c20 6f72 2061  dress book, or a
-00001370: 2060 3078 2e2e 6020 6865 7820 7374 7269   `0x..` hex stri
-00001380: 6e67 2e0a 0a23 2323 204d 756c 7469 706c  ng...### Multipl
-00001390: 6520 7369 676e 6572 730a 0a41 6464 206d  e signers..Add m
-000013a0: 6f72 6520 7369 676e 6572 7320 7769 7468  ore signers with
-000013b0: 2060 7733 2064 6220 7369 676e 6572 2061   `w3 db signer a
-000013c0: 6464 6020 616e 6420 7365 6c65 6374 2077  dd` and select w
-000013d0: 6869 6368 206f 6e65 2074 6f20 7573 6520  hich one to use 
-000013e0: 7769 7468 2074 6865 2060 2d2d 7369 676e  with the `--sign
-000013f0: 6572 6020 666c 6167 3a0a 0a60 6060 6261  er` flag:..```ba
-00001400: 7368 0a77 3320 2d2d 7369 676e 6572 206d  sh.w3 --signer m
-00001410: 795f 7369 676e 6572 203c 636f 6d6d 616e  y_signer <comman
-00001420: 643e 0a77 3320 2d73 206d 795f 7369 676e  d>.w3 -s my_sign
-00001430: 6572 203c 636f 6d6d 616e 643e 2023 2073  er <command> # s
-00001440: 686f 7274 2076 6572 7369 6f6e 0a60 6060  hort version.```
-00001450: 0a0a 4966 2079 6f75 2070 6c61 6e20 746f  ..If you plan to
-00001460: 2075 7365 2074 6865 2073 616d 6520 7369   use the same si
-00001470: 676e 6572 2066 6f72 2061 2077 6869 6c65  gner for a while
-00001480: 2c20 6d61 6b65 2069 7420 7468 6520 2a2a  , make it the **
-00001490: 6465 6661 756c 7420 7369 676e 6572 2a2a  default signer**
-000014a0: 2077 6974 6820 7468 6520 636f 6d6d 616e   with the comman
-000014b0: 643a 0a0a 6060 600a 7733 2063 6f6e 6669  d:..```.w3 confi
-000014c0: 6720 7365 7420 6465 6661 756c 745f 7369  g set default_si
-000014d0: 676e 6572 206d 795f 7369 676e 6572 0a60  gner my_signer.`
-000014e0: 6060 0a0a 0a23 2053 6574 7469 6e67 730a  ``...# Settings.
-000014f0: 0a53 6574 7469 6e67 7320 6172 6520 7265  .Settings are re
-00001500: 6164 2066 726f 6d20 7468 6520 636f 6e66  ad from the conf
-00001510: 6967 7572 6174 696f 6e20 6669 6c65 2060  iguration file `
-00001520: 7e2f 2e77 6562 3363 6c69 2f63 6f6e 6669  ~/.web3cli/confi
-00001530: 672f 7765 6233 636c 692e 7961 6d6c 602c  g/web3cli.yaml`,
-00001540: 206f 7220 6672 6f6d 2065 6e76 6972 6f6e   or from environ
-00001550: 6d65 6e74 2076 6172 6961 626c 6573 2e20  ment variables. 
-00001560: 2854 6865 2073 796d 626f 6c20 607e 6020  (The symbol `~` 
-00001570: 7265 6665 7273 2074 6f20 7468 6520 686f  refers to the ho
-00001580: 6d65 2066 6f6c 6465 7220 6f66 2079 6f75  me folder of you
-00001590: 7220 7573 6572 2e29 0a53 6565 2074 6865  r user.).See the
-000015a0: 205b 6578 616d 706c 6520 636f 6e66 6967   [example config
-000015b0: 7572 6174 696f 6e20 6669 6c65 5d28 2e2f  uration file](./
-000015c0: 7765 6233 636c 692e 6578 616d 706c 652e  web3cli.example.
-000015d0: 796d 6c29 2066 6f72 2061 206c 6973 7420  yml) for a list 
-000015e0: 6f66 2061 7661 696c 6162 6c65 2073 6574  of available set
-000015f0: 7469 6e67 732e 0a0a 2323 2320 456e 7669  tings...### Envi
-00001600: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
-00001610: 730a 0a41 6c6c 2073 6574 7469 6e67 7320  s..All settings 
-00001620: 6361 6e20 6265 206f 7665 7272 6964 6465  can be overridde
-00001630: 6e20 7669 6120 656e 7669 726f 6e6d 656e  n via environmen
-00001640: 7420 7661 7269 6162 6c65 732e 0a46 6f72  t variables..For
-00001650: 2065 7861 6d70 6c65 2c20 7468 6520 7365   example, the se
-00001660: 7474 696e 6773 2060 7765 6233 636c 692e  ttings `web3cli.
-00001670: 6465 6661 756c 745f 6368 6169 6e60 2063  default_chain` c
-00001680: 616e 2062 6520 6f76 6572 7269 6464 656e  an be overridden
-00001690: 2062 7920 7365 7474 696e 6720 7468 6520   by setting the 
-000016a0: 656e 7620 7661 7269 6162 6c65 2060 5745  env variable `WE
-000016b0: 4233 434c 495f 4445 4641 554c 545f 4348  B3CLI_DEFAULT_CH
-000016c0: 4149 4e60 3a0a 0a60 6060 6261 7368 0a57  AIN`:..```bash.W
-000016d0: 4542 3343 4c49 5f44 4546 4155 4c54 5f43  EB3CLI_DEFAULT_C
-000016e0: 4841 494e 3d61 7661 6c61 6e63 6865 2077  HAIN=avalanche w
-000016f0: 3320 6462 2063 6861 696e 2067 6574 0a0a  3 db chain get..
-00001700: 6f75 7470 7574 3e20 6176 616c 616e 6368  output> avalanch
-00001710: 650a 6060 600a 0a23 2323 2046 6f6c 6465  e.```..### Folde
-00001720: 722d 7370 6563 6966 6963 2073 6574 7469  r-specific setti
-00001730: 6e67 730a 0a54 6f20 6861 7665 2073 6574  ngs..To have set
-00001740: 7469 6e67 7320 7468 6174 2061 7070 6c79  tings that apply
-00001750: 206f 6e6c 7920 746f 2074 6865 2063 7572   only to the cur
-00001760: 7265 6e74 2066 6f6c 6465 722c 2063 7265  rent folder, cre
-00001770: 6174 6520 6120 6077 6562 3363 6c69 2e79  ate a `web3cli.y
-00001780: 616d 6c60 2066 696c 6520 696e 2074 6861  aml` file in tha
-00001790: 7420 666f 6c64 6572 2061 6e64 2065 7865  t folder and exe
-000017a0: 6375 7465 2060 7733 6020 6672 6f6d 2074  cute `w3` from t
-000017b0: 6861 7420 666f 6c64 6572 2e0a 0a53 6574  hat folder...Set
-000017c0: 7469 6e67 7320 7370 6563 6966 6965 6420  tings specified 
-000017d0: 696e 2060 7765 6233 636c 692e 7961 6d6c  in `web3cli.yaml
-000017e0: 6020 7769 6c6c 206f 7665 7272 6964 6520  ` will override 
-000017f0: 7468 6f73 6520 696e 2079 6f75 7220 686f  those in your ho
-00001800: 6d65 2066 6f6c 6465 722e 2045 6e76 6972  me folder. Envir
-00001810: 6f6e 6d65 6e74 2076 6172 6961 626c 6573  onment variables
-00001820: 2077 696c 6c20 7374 696c 6c20 6765 7420   will still get 
-00001830: 7468 6520 7072 6563 6564 656e 6365 2e0a  the precedence..
-00001840: 0a23 2323 2045 6469 7420 636f 6e66 6967  .### Edit config
-00001850: 7572 6174 696f 6e20 7669 6120 7468 6520  uration via the 
-00001860: 434c 490a 0a59 6f75 2063 616e 2065 6469  CLI..You can edi
-00001870: 7420 7468 6520 636f 6e66 6967 7572 6174  t the configurat
-00001880: 696f 6e20 6669 6c65 7320 7573 696e 6720  ion files using 
-00001890: 6077 3320 636f 6e66 6967 602e 2046 6f72  `w3 config`. For
-000018a0: 2065 7861 6d70 6c65 3a0a 0a2d 2053 686f   example:..- Sho
-000018b0: 7720 7468 6520 7661 6c75 6520 6f66 2061  w the value of a
-000018c0: 2073 696e 676c 6520 7365 7474 696e 673a   single setting:
-000018d0: 0a20 2020 6060 6062 6173 680a 2020 2070  .   ```bash.   p
-000018e0: 646d 2077 3320 636f 6e66 6967 2067 6574  dm w3 config get
-000018f0: 2064 6566 6175 6c74 5f63 6861 696e 0a20   default_chain. 
-00001900: 2020 6060 600a 2d20 5368 6f77 2061 6c6c    ```.- Show all
-00001910: 2073 6574 7469 6e67 733a 0a20 2020 6060   settings:.   ``
-00001920: 6062 6173 680a 2020 2070 646d 2077 3320  `bash.   pdm w3 
-00001930: 636f 6e66 6967 2067 6574 0a20 2020 6060  config get.   ``
-00001940: 600a 2d20 4564 6974 2061 2073 6574 7469  `.- Edit a setti
-00001950: 6e67 2076 616c 7565 2061 7420 7468 6520  ng value at the 
-00001960: 676c 6f62 616c 206c 6576 656c 2028 607e  global level (`~
-00001970: 2f2e 7765 6233 636c 692f 6461 7461 6261  /.web3cli/databa
-00001980: 7365 2f77 6562 3363 6c69 2e73 716c 6974  se/web3cli.sqlit
-00001990: 6560 293a 0a20 2020 6060 6062 6173 680a  e`):.   ```bash.
-000019a0: 2020 2070 646d 2077 3320 636f 6e66 6967     pdm w3 config
-000019b0: 2073 6574 2064 6566 6175 6c74 5f63 6861   set default_cha
-000019c0: 696e 2061 7661 6c61 6e63 6865 0a20 2020  in avalanche.   
-000019d0: 6060 600a 2d20 4564 6974 2061 2073 6574  ```.- Edit a set
-000019e0: 7469 6e67 2076 616c 7565 2061 7420 7468  ting value at th
-000019f0: 6520 6c6f 6361 6c20 6c65 7665 6c20 2860  e local level (`
-00001a00: 7765 6233 636c 692e 796d 6c60 293a 0a20  web3cli.yml`):. 
-00001a10: 2020 6060 6062 6173 680a 2020 2070 646d    ```bash.   pdm
-00001a20: 2077 3320 636f 6e66 6967 2073 6574 2064   w3 config set d
-00001a30: 6566 6175 6c74 5f63 6861 696e 2061 7661  efault_chain ava
-00001a40: 6c61 6e63 6865 202d 2d6e 6f2d 676c 6f62  lanche --no-glob
-00001a50: 616c 0a20 2020 6060 600a 0a23 2043 6f6e  al.   ```..# Con
-00001a60: 7472 6962 7574 6520 e29d a4ef b88f 0a0a  tribute ........
-00001a70: 5075 6c6c 2072 6571 7565 7374 7320 6172  Pull requests ar
-00001a80: 6520 7765 6c63 6f6d 6521 0a0a 312e 2049  e welcome!..1. I
-00001a90: 6e73 7461 6c6c 2061 6e64 2063 6f6e 6669  nstall and confi
-00001aa0: 6775 7265 205b 5044 4d5d 2868 7474 7073  gure [PDM](https
-00001ab0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7064  ://github.com/pd
-00001ac0: 6d2d 7072 6f6a 6563 742f 7064 6d2f 293a  m-project/pdm/):
-00001ad0: 0a20 2020 6060 6062 6173 680a 2020 2063  .   ```bash.   c
-00001ae0: 7572 6c20 2d73 534c 2068 7474 7073 3a2f  url -sSL https:/
-00001af0: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
-00001b00: 6f6e 7465 6e74 2e63 6f6d 2f70 646d 2d70  ontent.com/pdm-p
-00001b10: 726f 6a65 6374 2f70 646d 2f6d 6169 6e2f  roject/pdm/main/
-00001b20: 696e 7374 616c 6c2d 7064 6d2e 7079 207c  install-pdm.py |
-00001b30: 2070 7974 686f 6e33 202d 0a20 2020 6060   python3 -.   ``
-00001b40: 600a 322e 2049 6e73 7461 6c6c 2064 6570  `.2. Install dep
-00001b50: 656e 6465 6e63 6965 733a 200a 2020 2060  endencies: .   `
-00001b60: 6060 6261 7368 0a20 2020 7064 6d20 696e  ``bash.   pdm in
-00001b70: 7374 616c 6c0a 2020 2060 6060 0a33 2e20  stall.   ```.3. 
-00001b80: 546f 2072 756e 2074 6865 2043 4c49 2061  To run the CLI a
-00001b90: 6761 696e 7374 2079 6f75 7220 6368 616e  gainst your chan
-00001ba0: 6765 733a 200a 2020 2060 6060 6261 7368  ges: .   ```bash
-00001bb0: 0a20 2020 7064 6d20 7733 203c 636f 6d6d  .   pdm w3 <comm
-00001bc0: 616e 643e 0a20 2020 6060 600a 0a0a 2323  and>.   ```...##
-00001bd0: 2320 5465 7374 730a 0a54 6f20 7275 6e20  # Tests..To run 
-00001be0: 7465 7374 732c 2066 6972 7374 2069 6e73  tests, first ins
-00001bf0: 7461 6c6c 205b 6067 616e 6163 6865 605d  tall [`ganache`]
-00001c00: 2868 7474 7073 3a2f 2f77 7777 2e6e 706d  (https://www.npm
-00001c10: 6a73 2e63 6f6d 2f70 6163 6b61 6765 2f67  js.com/package/g
-00001c20: 616e 6163 6865 2920 6f6e 2061 7420 6c65  anache) on at le
-00001c30: 6173 7420 6e6f 6465 2031 382c 2074 6865  ast node 18, the
-00001c40: 6e20 7275 6e3a 0a0a 6060 6062 6173 680a  n run:..```bash.
-00001c50: 7064 6d20 7465 7374 0a60 6060 0a0a 2320  pdm test.```..# 
-00001c60: 4163 6b6e 6f77 6c65 6467 656d 656e 7473  Acknowledgements
-00001c70: 0a0a 5468 616e 6b20 796f 7520 7665 7279  ..Thank you very
-00001c80: 206d 7563 6820 746f 2074 6865 205b 7765   much to the [we
-00001c90: 6233 2e70 795d 2868 7474 7073 3a2f 2f67  b3.py](https://g
-00001ca0: 6974 6875 622e 636f 6d2f 6574 6865 7265  ithub.com/ethere
-00001cb0: 756d 2f77 6562 332e 7079 2920 616e 6420  um/web3.py) and 
-00001cc0: 5b60 6272 6f77 6e69 6560 5d28 6874 7470  [`brownie`](http
-00001cd0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f65  s://github.com/e
-00001ce0: 7468 2d62 726f 776e 6965 2f62 726f 776e  th-brownie/brown
-00001cf0: 6965 2920 7465 616d 733a 2060 7765 6233  ie) teams: `web3
-00001d00: 6020 776f 756c 6420 6e6f 7420 6578 6973  ` would not exis
-00001d10: 7420 7769 7468 6f75 7420 796f 7572 2065  t without your e
-00001d20: 6666 6f72 7473 210a 0a0a 2320 544f 444f  fforts!...# TODO
-00001d30: 0a2d 2044 6566 696e 6520 636f 6d6d 616e  .- Define comman
-00001d40: 6420 7368 6f72 7463 7574 7320 7573 696e  d shortcuts usin
-00001d50: 6720 6172 6770 6172 7365 2061 6c69 6173  g argparse alias
-00001d60: 6573 2c20 652e 672e 2060 7733 2061 6464  es, e.g. `w3 add
-00001d70: 2d63 6861 696e 6020 696e 7374 6561 6420  -chain` instead 
-00001d80: 6f66 2060 7733 2064 6220 6368 6169 6e20  of `w3 db chain 
-00001d90: 6164 6460 0a2d 2055 7365 2064 6966 6665  add`.- Use diffe
-00001da0: 7265 6e74 2064 6220 6669 6c65 2066 6f72  rent db file for
-00001db0: 2064 6576 2065 6e76 6972 6f6e 6d65 6e74   dev environment
-00001dc0: 0a2d 2052 4541 444d 453a 2045 7870 6c61  .- README: Expla
-00001dd0: 696e 206a 736f 6e20 6f75 7470 7574 202b  in json output +
-00001de0: 2074 7269 636b 2060 7c20 7079 7468 6f6e   trick `| python
-00001df0: 3320 2d6d 6a73 6f6e 2e74 6f6f 6c60 0a2d  3 -mjson.tool`.-
-00001e00: 2049 6d70 6c65 6d65 6e74 2060 7733 2062   Implement `w3 b
-00001e10: 6c6f 636b 600a 2d20 496d 706c 656d 656e  lock`.- Implemen
-00001e20: 7420 6077 3320 7478 2066 6574 6368 600a  t `w3 tx fetch`.
-00001e30: 2d20 4d6f 7665 2074 6573 7473 2f73 6565  - Move tests/see
-00001e40: 6465 7220 746f 2063 6f72 6520 2869 6e20  der to core (in 
-00001e50: 6d6f 6465 6c73 3f29 0a2d 2054 6573 7473  models?).- Tests
-00001e60: 3a20 7573 6520 6c6f 6e64 6f6e 2068 6172  : use london har
-00001e70: 6466 6f72 6b20 696e 7374 6561 6420 6f66  dfork instead of
-00001e80: 2069 7374 616e 6275 6c3f 0a2d 2053 656e   istanbul?.- Sen
-00001e90: 6420 636f 6d6d 616e 643a 206f 7074 696f  d command: optio
-00001ea0: 6e20 746f 2077 6169 7420 666f 7220 7265  n to wait for re
-00001eb0: 6365 6970 740a 2d20 5265 7472 7920 7472  ceipt.- Retry tr
-00001ec0: 616e 7361 6374 696f 6e73 2075 6e74 696c  ansactions until
-00001ed0: 2067 6173 2066 6565 2067 6f65 7320 6265   gas fee goes be
-00001ee0: 6c6f 7720 7820 6777 6569 0a2d 2052 4541  low x gwei.- REA
-00001ef0: 444d 4520 6261 6467 6573 3a20 7765 6233  DME badges: web3
-00001f00: 2e70 792c 2062 726f 776e 6965 2c20 5044  .py, brownie, PD
-00001f10: 4d2c 2063 656d 656e 740a 2d20 5265 736f  M, cement.- Reso
-00001f20: 6c76 6520 6164 6472 6573 7320 7368 6f75  lve address shou
-00001f30: 6c64 206c 6f6f 6b20 616c 736f 2069 6e20  ld look also in 
-00001f40: 7369 676e 6174 7572 6520 6e61 6d65 7320  signature names 
-00001f50: 286d 616b 6520 7369 676e 6572 2026 2061  (make signer & a
-00001f60: 6464 7265 7373 206e 616d 6573 2075 6e69  ddress names uni
-00001f70: 7175 653f 290a 2d20 4164 6472 6573 7320  que?).- Address 
-00001f80: 626f 6f6b 3a20 6865 6c70 6572 206d 6574  book: helper met
-00001f90: 686f 6420 746f 2075 6e2d 7265 736f 6c76  hod to un-resolv
-00001fa0: 6520 6164 6472 6573 7320 2866 726f 6d20  e address (from 
-00001fb0: 3078 2074 6f20 6e61 6d65 2c20 6966 2069  0x to name, if i
-00001fc0: 7420 6578 6973 7473 292c 2075 7365 6675  t exists), usefu
-00001fd0: 6c20 666f 7220 6077 3320 7478 206c 6973  l for `w3 tx lis
-00001fe0: 7460 0a2d 2052 7063 3a20 6368 6563 6b20  t`.- Rpc: check 
-00001ff0: 7468 6174 2063 6861 696e 2773 2063 6861  that chain's cha
-00002000: 696e 5f69 6420 696e 2044 4220 636f 7272  in_id in DB corr
-00002010: 6573 706f 6e64 7320 746f 2063 6861 696e  esponds to chain
-00002020: 5f69 6420 6f66 2052 5043 0a2d 2043 6861  _id of RPC.- Cha
-00002030: 696e 3a20 5072 656c 6f61 6420 6368 6169  in: Preload chai
-00002040: 6e73 2066 726f 6d20 6874 7470 733a 2f2f  ns from https://
-00002050: 6368 6169 6e69 642e 6e65 7477 6f72 6b2f  chainid.network/
-00002060: 6368 6169 6e73 2e6a 736f 6e0a 2d20 436f  chains.json.- Co
-00002070: 6d6d 616e 643a 2060 7733 2069 6e69 7460  mmand: `w3 init`
-00002080: 2074 6f20 696d 706f 7274 2063 6861 696e   to import chain
-00002090: 202b 2061 6464 2073 6967 6e65 720a 2d20   + add signer.- 
-000020a0: 5769 6e64 6f77 733a 2074 6573 7420 6f6e  Windows: test on
-000020b0: 2061 2057 696e 646f 7773 206d 6163 6869   a Windows machi
-000020c0: 6e65 0a2d 2044 6f20 6e6f 7420 6d65 7373  ne.- Do not mess
-000020d0: 2077 6974 6820 4442 2075 6e6c 6573 7320   with DB unless 
-000020e0: 6e65 6564 6564 2062 7920 7468 6520 636f  needed by the co
-000020f0: 6d6d 616e 640a 2d20 446f 206e 6f74 206d  mmand.- Do not m
-00002100: 6573 7320 7769 7468 2073 6967 6e65 7273  ess with signers
-00002110: 2075 6e6c 6573 7320 6e65 6564 6564 2062   unless needed b
-00002120: 7920 7468 6520 636f 6d6d 616e 640a 2d20  y the command.- 
-00002130: 4175 746f 636f 6d70 6c65 7465 2063 6f6d  Autocomplete com
-00002140: 6d61 6e64 730a 2d20 5465 7374 733a 2073  mands.- Tests: s
-00002150: 686f 756c 6420 7765 2063 6861 6e67 6520  hould we change 
-00002160: 6576 6d5f 7665 7273 696f 6e20 696e 2067  evm_version in g
-00002170: 616e 6163 6865 2066 6f72 206e 6f6e 2d65  anache for non-e
-00002180: 7468 6572 6575 6d20 6368 6169 6e73 3f20  thereum chains? 
-00002190: 2873 6565 2043 4c49 5f46 4c41 4753 2062  (see CLI_FLAGS b
-000021a0: 726f 776e 6965 2f6e 6574 776f 726b 2f72  rownie/network/r
-000021b0: 7063 2f67 616e 6163 6865 2e70 7929 0a2d  pc/ganache.py).-
-000021c0: 2041 7574 6f63 6f6d 706c 6574 6520 6164   Autocomplete ad
-000021d0: 6472 6573 7365 7320 616e 6420 7369 676e  dresses and sign
-000021e0: 6572 730a 2d20 436f 6e66 6967 3a20 6e6f  ers.- Config: no
-000021f0: 6e2d 7374 7269 6e67 2073 7570 706f 7274  n-string support
-00002200: 2069 6e20 6063 6f6e 6669 6720 7365 7460   in `config set`
-00002210: 0a2d 2047 6173 3a20 5570 7065 7220 6c69  .- Gas: Upper li
-00002220: 6d69 7420 6f6e 2062 6173 6566 6565 2076  mit on basefee v
-00002230: 6961 2067 6c6f 6261 6c20 6172 6775 6d65  ia global argume
-00002240: 6e74 2f73 6574 7469 6e67 0a2d 2044 7279  nt/setting.- Dry
-00002250: 2d72 756e 3a20 5072 696e 7420 7478 2069  -run: Print tx i
-00002260: 6e73 7465 6164 206f 6620 7365 6e64 696e  nstead of sendin
-00002270: 6720 6974 2c20 7669 6120 676c 6f62 616c  g it, via global
-00002280: 2061 7267 756d 656e 742f 7365 7474 696e   argument/settin
-00002290: 670a 2d20 5573 6520 6368 6169 6e73 2061  g.- Use chains a
-000022a0: 6e64 2074 6f6b 656e 7320 6672 6f6d 206f  nd tokens from o
-000022b0: 7468 6572 2073 6f75 7263 6573 2028 652e  ther sources (e.
-000022c0: 672e 2065 7468 6572 6575 6d2d 6c69 7374  g. ethereum-list
-000022d0: 7329 0a2d 2065 7468 504d 2072 6567 6973  s).- ethPM regis
-000022e0: 7472 7920 2f20 6574 6865 7273 6361 6e20  try / etherscan 
-000022f0: 746f 2070 756c 6c20 736d 6172 7420 636f  to pull smart co
-00002300: 6e74 7261 6374 2069 6e74 6572 6661 6365  ntract interface
-00002310: 733f 2045 2e67 2e20 6874 7470 733a 2f2f  s? E.g. https://
-00002320: 6574 682d 6272 6f77 6e69 652e 7265 6164  eth-brownie.read
-00002330: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-00002340: 7465 7374 2f63 6f72 652d 636f 6e74 7261  test/core-contra
-00002350: 6374 732e 6874 6d6c 2366 6574 6368 696e  cts.html#fetchin
-00002360: 672d 6672 6f6d 2d61 2d72 656d 6f74 652d  g-from-a-remote-
-00002370: 736f 7572 6365 0a2d 2052 6563 6f72 6420  source.- Record 
-00002380: 7472 616e 7361 6374 696f 6e20 696e 2054  transaction in T
-00002390: 7873 2074 6162 6c65 0a2d 2046 6978 2075  xs table.- Fix u
-000023a0: 7361 6765 206d 6573 7361 6765 2028 7374  sage message (st
-000023b0: 696c 6c20 7265 6665 7273 2074 6f20 6077  ill refers to `w
-000023c0: 6562 3363 6c69 6029 0a0a                 eb3cli`)..
+00000000: 3c21 2d2d 2068 7474 7073 3a2f 2f73 6869  <!-- https://shi
+00000010: 656c 6473 2e69 6f2f 202d 2d3e 200a 3c70  elds.io/ --> .<p
+00000020: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+00000030: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
+00000040: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000050: 2f63 6f63 636f 696e 6f6d 616e 652f 7765  /coccoinomane/we
+00000060: 6233 636c 692f 7075 6c73 6522 2061 6c74  b3cli/pulse" alt
+00000070: 3d22 4163 7469 7669 7479 223e 3c69 6d67  ="Activity"><img
+00000080: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+00000090: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
+000000a0: 6875 622f 636f 6d6d 6974 2d61 6374 6976  hub/commit-activ
+000000b0: 6974 792f 6d2f 6261 6467 6573 2f73 6869  ity/m/badges/shi
+000000c0: 656c 6473 3f63 6f6c 6f72 3d30 3039 3035  elds?color=00905
+000000d0: 3122 2f3e 3c2f 613e 0a20 2020 203c 696d  1"/></a>.    <im
+000000e0: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
+000000f0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
+00000100: 7468 7562 2f6c 6173 742d 636f 6d6d 6974  thub/last-commit
+00000110: 2f63 6f63 636f 696e 6f6d 616e 652f 7765  /coccoinomane/we
+00000120: 6233 636c 693f 636f 6c6f 723d 3030 3930  b3cli?color=0090
+00000130: 3531 222f 3e0a 3c2f 703e 0a3c 7020 616c  51"/>.</p>.<p al
+00000140: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
+00000150: 2020 2020 2020 3c61 2068 7265 663d 2268        <a href="h
+00000160: 7474 7073 3a2f 2f77 7777 2e61 6c63 6865  ttps://www.alche
+00000170: 6d79 2e63 6f6d 2f64 6170 7073 2f77 6562  my.com/dapps/web
+00000180: 3363 6c69 223e 3c69 6d67 2073 7479 6c65  3cli"><img style
+00000190: 3d22 7769 6474 683a 3135 3070 783b 6865  ="width:150px;he
+000001a0: 6967 6874 3a33 3370 7822 2073 7263 3d22  ight:33px" src="
+000001b0: 6874 7470 733a 2f2f 7374 6174 6963 2e61  https://static.a
+000001c0: 6c63 6865 6d79 6170 692e 696f 2f69 6d61  lchemyapi.io/ima
+000001d0: 6765 732f 6d61 726b 6574 696e 672f 6261  ges/marketing/ba
+000001e0: 6467 652e 706e 6722 2f3e 3c2f 613e 0a3c  dge.png"/></a>.<
+000001f0: 2f70 3e0a 0a49 6e74 6572 6163 7420 7769  /p>..Interact wi
+00000200: 7468 2062 6c6f 636b 6368 6169 6e73 2061  th blockchains a
+00000210: 6e64 2073 6d61 7274 2063 6f6e 7472 6163  nd smart contrac
+00000220: 7473 2075 7369 6e67 2074 6865 2063 6f6d  ts using the com
+00000230: 6d61 6e64 206c 696e 653a 206e 6f20 636f  mand line: no co
+00000240: 6469 6e67 206e 6565 6465 6421 0a0a 2320  ding needed!..# 
+00000250: 5461 626c 6520 6f66 2063 6f6e 7465 6e74  Table of content
+00000260: 730a 0a2d 205b 4665 6174 7572 6573 5d28  s..- [Features](
+00000270: 2366 6561 7475 7265 7329 0a2d 205b 496e  #features).- [In
+00000280: 7374 616c 6c5d 2823 696e 7374 616c 6c29  stall](#install)
+00000290: 0a2d 205b 5369 6d70 6c65 2065 7861 6d70  .- [Simple examp
+000002a0: 6c65 735d 2823 7369 6d70 6c65 2d65 7861  les](#simple-exa
+000002b0: 6d70 6c65 7329 0a2d 205b 4164 7661 6e63  mples).- [Advanc
+000002c0: 6564 2065 7861 6d70 6c65 735d 2823 6164  ed examples](#ad
+000002d0: 7661 6e63 6564 2d65 7861 6d70 6c65 7329  vanced-examples)
+000002e0: 0a2d 205b 536d 6172 7420 436f 6e74 7261  .- [Smart Contra
+000002f0: 6374 2073 7570 706f 7274 5d28 2373 6d61  ct support](#sma
+00000300: 7274 2d63 6f6e 7472 6163 742d 7375 7070  rt-contract-supp
+00000310: 6f72 7429 0a20 2020 202b 205b 5265 6164  ort).    + [Read
+00000320: 2066 726f 6d20 6120 736d 6172 7420 636f   from a smart co
+00000330: 6e74 7261 6374 5d28 2372 6561 642d 6672  ntract](#read-fr
+00000340: 6f6d 2d61 2d73 6d61 7274 2d63 6f6e 7472  om-a-smart-contr
+00000350: 6163 7429 0a20 2020 202b 205b 5772 6974  act).    + [Writ
+00000360: 6520 746f 2061 2073 6d61 7274 2063 6f6e  e to a smart con
+00000370: 7472 6163 745d 2823 7772 6974 652d 746f  tract](#write-to
+00000380: 2d61 2d73 6d61 7274 2d63 6f6e 7472 6163  -a-smart-contrac
+00000390: 7429 0a2d 205b 4d75 6c74 6963 6861 696e  t).- [Multichain
+000003a0: 2073 7570 706f 7274 5d28 236d 756c 7469   support](#multi
+000003b0: 6368 6169 6e2d 7375 7070 6f72 7429 0a2d  chain-support).-
+000003c0: 205b 5573 6520 6375 7374 6f6d 2052 5043   [Use custom RPC
+000003d0: 5d28 2375 7365 2d63 7573 746f 6d2d 7270  ](#use-custom-rp
+000003e0: 6329 0a2d 205b 4164 6420 6375 7374 6f6d  c).- [Add custom
+000003f0: 2063 6861 696e 735d 2823 6164 642d 6375   chains](#add-cu
+00000400: 7374 6f6d 2d63 6861 696e 7329 0a2d 205b  stom-chains).- [
+00000410: 4164 6472 6573 7320 626f 6f6b 5d28 2361  Address book](#a
+00000420: 6464 7265 7373 2d62 6f6f 6b29 0a2d 205b  ddress-book).- [
+00000430: 5761 6c6c 6574 206d 616e 6167 656d 656e  Wallet managemen
+00000440: 745d 2823 7761 6c6c 6574 2d6d 616e 6167  t](#wallet-manag
+00000450: 656d 656e 7429 0a20 2020 202b 205b 4465  ement).    + [De
+00000460: 6661 756c 7420 7369 676e 6572 5d28 2364  fault signer](#d
+00000470: 6566 6175 6c74 2d73 6967 6e65 7229 0a20  efault-signer). 
+00000480: 2020 202b 205b 4372 6561 7465 206e 6577     + [Create new
+00000490: 2070 7269 7661 7465 206b 6579 735d 2823   private keys](#
+000004a0: 6372 6561 7465 2d6e 6577 2d70 7269 7661  create-new-priva
+000004b0: 7465 2d6b 6579 7329 0a2d 205b 446f 6375  te-keys).- [Docu
+000004c0: 6d65 6e74 6174 696f 6e5d 2823 646f 6375  mentation](#docu
+000004d0: 6d65 6e74 6174 696f 6e29 0a2d 205b 436f  mentation).- [Co
+000004e0: 6e74 7269 6275 7469 6e67 5d28 2363 6f6e  ntributing](#con
+000004f0: 7472 6962 7574 696e 6729 0a2d 205b 4163  tributing).- [Ac
+00000500: 6b6e 6f77 6c65 6467 656d 656e 7473 5d28  knowledgements](
+00000510: 2361 636b 6e6f 776c 6564 6765 6d65 6e74  #acknowledgement
+00000520: 7329 0a0a 2320 4665 6174 7572 6573 0a0a  s)..# Features..
+00000530: 2d20 496e 7465 7261 6374 2077 6974 6820  - Interact with 
+00000540: 4574 6865 7265 756d 2061 6e64 2045 564d  Ethereum and EVM
+00000550: 2d63 6f6d 7061 7469 626c 6520 6368 6169  -compatible chai
+00000560: 6e73 2076 6961 2079 6f75 7220 7465 726d  ns via your term
+00000570: 696e 616c 0a2d 2042 7970 6173 7320 736c  inal.- Bypass sl
+00000580: 7567 6769 7368 2061 6e64 2070 6f74 656e  uggish and poten
+00000590: 7469 616c 6c79 2063 6f6d 7072 6f6d 6973  tially compromis
+000005a0: 6564 2066 726f 6e74 656e 6473 0a2d 204e  ed frontends.- N
+000005b0: 6f20 636f 6e66 6967 7572 6174 696f 6e20  o configuration 
+000005c0: 6e65 6564 6564 0a2d 204c 6162 656c 2061  needed.- Label a
+000005d0: 6464 7265 7373 6573 2c20 746f 6b65 6e73  ddresses, tokens
+000005e0: 2061 6e64 2063 6f6e 7472 6163 7473 2066   and contracts f
+000005f0: 6f72 2065 6173 6520 6f66 2075 7365 0a2d  or ease of use.-
+00000600: 2053 7761 7020 7769 7468 2055 6e69 7377   Swap with Unisw
+00000610: 6170 2c20 5472 6164 6572 4a6f 652c 2050  ap, TraderJoe, P
+00000620: 616e 6361 6b65 5377 6170 2c20 6574 630a  ancakeSwap, etc.
+00000630: 2d20 5472 616e 7366 6572 2074 6f6b 656e  - Transfer token
+00000640: 7320 7669 6120 7468 6569 7220 7469 636b  s via their tick
+00000650: 6572 0a2d 2043 6f6e 6361 7465 6e61 7465  er.- Concatenate
+00000660: 2063 6f6d 6d61 6e64 7320 746f 2062 7569   commands to bui
+00000670: 6c64 2070 6f77 6572 6675 6c20 7363 7269  ld powerful scri
+00000680: 7074 730a 2d20 496d 706f 7274 2073 6967  pts.- Import sig
+00000690: 6e65 7273 2076 6961 2070 7269 7661 7465  ners via private
+000006a0: 206b 6579 206f 7220 6b65 7966 696c 650a   key or keyfile.
+000006b0: 2d20 5468 6f72 6f75 6768 6c79 2074 6573  - Thoroughly tes
+000006c0: 7465 6420 7573 696e 6720 7468 6520 5b41  ted using the [A
+000006d0: 7065 2046 7261 6d65 776f 726b 5d28 6874  pe Framework](ht
+000006e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000006f0: 2f41 7065 576f 7258 2f61 7065 2927 7320  /ApeWorX/ape)'s 
+00000700: 7465 7374 696e 6720 6672 616d 6577 6f72  testing framewor
+00000710: 6b0a 2d20 5b57 696e 646f 7773 2063 6f6d  k.- [Windows com
+00000720: 7061 7469 626c 655d 2868 7474 7073 3a2f  patible](https:/
+00000730: 2f67 6974 6875 622e 636f 6d2f 636f 6363  /github.com/cocc
+00000740: 6f69 6e6f 6d61 6e65 2f77 6562 3363 6c69  oinomane/web3cli
+00000750: 2f77 696b 692f 2546 3025 3946 2541 4125  /wiki/%F0%9F%AA%
+00000760: 3946 2d52 756e 2d77 6562 3363 6c69 2d6f  9F-Run-web3cli-o
+00000770: 6e2d 5769 6e64 6f77 7329 0a0a 536f 6f6e  n-Windows)..Soon
+00000780: 3a0a 0a2d 2053 6574 2075 7020 7363 6865  :..- Set up sche
+00000790: 6475 6c65 6420 6275 7973 2061 6e64 2073  duled buys and s
+000007a0: 656c 6c73 2028 4443 4129 0a2d 2041 7574  ells (DCA).- Aut
+000007b0: 6f6d 6174 6963 616c 6c79 2062 7579 2077  omatically buy w
+000007c0: 6865 6e20 736c 6970 7061 6765 2069 7320  hen slippage is 
+000007d0: 6c6f 7720 656e 6f75 6768 0a2d 2047 6574  low enough.- Get
+000007e0: 206e 6f74 6966 6965 6420 6f6e 2054 656c   notified on Tel
+000007f0: 6567 7261 6d20 7768 656e 2061 2070 6169  egram when a pai
+00000800: 7220 6973 206c 6971 7569 6420 656e 6f75  r is liquid enou
+00000810: 6768 2c20 6f72 2075 6e62 616c 616e 6365  gh, or unbalance
+00000820: 640a 2d20 416e 616c 797a 6520 6f6e 2d63  d.- Analyze on-c
+00000830: 6861 696e 2064 6174 6120 666f 7220 7461  hain data for ta
+00000840: 7820 6f72 2073 6c65 7574 6869 6e67 2070  x or sleuthing p
+00000850: 7572 706f 7365 730a 2d20 436c 6169 6d20  urposes.- Claim 
+00000860: 616e 6420 7265 696e 7665 7374 2079 6965  and reinvest yie
+00000870: 6c64 2066 726f 6d20 4465 4669 2070 726f  ld from DeFi pro
+00000880: 746f 636f 6c73 0a0a 0a23 2049 6e73 7461  tocols...# Insta
+00000890: 6c6c 0a0a 4d61 6b65 2073 7572 6520 796f  ll..Make sure yo
+000008a0: 7520 6861 7665 2061 7420 6c65 6173 7420  u have at least 
+000008b0: 5079 7468 6f6e 2033 2e37 2069 6e73 7461  Python 3.7 insta
+000008c0: 6c6c 6564 2c20 7468 656e 2072 756e 3a0a  lled, then run:.
+000008d0: 0a60 6060 6261 7368 0a70 6970 3320 696e  .```bash.pip3 in
+000008e0: 7374 616c 6c20 2d55 2077 6562 3363 6c69  stall -U web3cli
+000008f0: 0a60 6060 0a0a 5769 6e64 6f77 7320 7573  .```..Windows us
+00000900: 6572 3f20 5b48 6572 6527 7320 6120 7475  er? [Here's a tu
+00000910: 746f 7269 616c 2066 6f72 2079 6f75 5d28  torial for you](
+00000920: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000930: 6f6d 2f63 6f63 636f 696e 6f6d 616e 652f  om/coccoinomane/
+00000940: 7765 6233 636c 692f 7769 6b69 2f25 4630  web3cli/wiki/%F0
+00000950: 2539 4625 4141 2539 462d 5275 6e2d 7765  %9F%AA%9F-Run-we
+00000960: 6233 636c 692d 6f6e 2d57 696e 646f 7773  b3cli-on-Windows
+00000970: 2921 0a0a 2320 5369 6d70 6c65 2065 7861  )!..# Simple exa
+00000980: 6d70 6c65 730a 0a2d 2047 6574 2074 6865  mples..- Get the
+00000990: 2045 5448 2062 616c 616e 6365 206f 6620   ETH balance of 
+000009a0: 616e 7920 6164 6472 6573 733a 0a20 2020  any address:.   
+000009b0: 6060 600a 2020 2077 3320 6261 6c61 6e63  ```.   w3 balanc
+000009c0: 6520 3078 6465 3062 3239 3536 3639 6139  e 0xde0b295669a9
+000009d0: 6664 3933 6435 6632 3864 3965 6338 3565  fd93d5f28d9ec85e
+000009e0: 3430 6634 6362 3639 3762 6165 0a20 2020  40f4cb697bae.   
+000009f0: 6060 600a 0a2d 2053 6176 6520 6164 6472  ```..- Save addr
+00000a00: 6573 7365 7320 7769 7468 2065 6173 792d  esses with easy-
+00000a10: 746f 2d72 656d 6265 7220 7461 6773 3a0a  to-rember tags:.
+00000a20: 2020 2060 6060 0a20 2020 7733 2061 6464     ```.   w3 add
+00000a30: 7265 7373 2061 6464 2075 6e69 6365 6620  ress add unicef 
+00000a40: 3078 6135 3962 3239 6437 6462 6339 3739  0xa59b29d7dbc979
+00000a50: 3464 3165 3766 3435 3132 3363 3438 6232  4d1e7f45123c48b2
+00000a60: 6238 6430 6133 3436 3336 0a20 2020 6060  b8d0a34636.   ``
+00000a70: 600a 2020 2074 6865 6e20 7573 6520 7468  `.   then use th
+00000a80: 6520 7461 6720 696e 2061 6e79 2063 6f6d  e tag in any com
+00000a90: 6d61 6e64 3a0a 2020 2060 6060 0a20 2020  mand:.   ```.   
+00000aa0: 7733 2062 616c 616e 6365 2075 6e69 6365  w3 balance unice
+00000ab0: 660a 2020 2060 6060 0a0a 2d20 4665 7463  f.   ```..- Fetc
+00000ac0: 6820 626c 6f63 6b73 2066 726f 6d20 7468  h blocks from th
+00000ad0: 6520 626c 6f63 6b63 6861 696e 2c20 696e  e blockchain, in
+00000ae0: 2065 6173 792d 746f 2d72 6561 6420 4a53   easy-to-read JS
+00000af0: 4f4e 2066 6f72 6d61 743a 0a20 2020 6060  ON format:.   ``
+00000b00: 6062 6173 680a 2020 2077 3320 626c 6f63  `bash.   w3 bloc
+00000b10: 6b20 6c61 7465 7374 0a20 2020 7733 2062  k latest.   w3 b
+00000b20: 6c6f 636b 2066 696e 616c 697a 6564 0a20  lock finalized. 
+00000b30: 2020 7733 2062 6c6f 636b 2036 3039 3433    w3 block 60943
+00000b40: 3035 0a20 2020 6060 600a 0a2d 2046 6574  05.   ```..- Fet
+00000b50: 6368 2074 7261 6e73 6163 7469 6f6e 7320  ch transactions 
+00000b60: 2620 7265 6365 6970 7473 2066 726f 6d20  & receipts from 
+00000b70: 7468 6520 626c 6f63 6b63 6861 696e 3a0a  the blockchain:.
+00000b80: 2020 2060 6060 6261 7368 0a20 2020 7733     ```bash.   w3
+00000b90: 2074 7820 6765 7420 3078 3362 6264 6363   tx get 0x3bbdcc
+00000ba0: 3263 3737 3231 3532 3166 3763 3736 3762  2c7721521f7c767b
+00000bb0: 3738 3733 6363 6238 3537 6630 3831 3661  7873ccb857f0816a
+00000bc0: 6339 3465 3966 3332 6335 3630 3166 3462  c94e9f32c5601f4b
+00000bd0: 3135 6338 3764 3165 6631 0a20 2020 7733  15c87d1ef1.   w3
+00000be0: 2074 7820 7263 2030 7833 6262 6463 6332   tx rc 0x3bbdcc2
+00000bf0: 6337 3732 3135 3231 6637 6337 3637 6237  c7721521f7c767b7
+00000c00: 3837 3363 6362 3835 3766 3038 3136 6163  873ccb857f0816ac
+00000c10: 3934 6539 6633 3263 3536 3031 6634 6231  94e9f32c5601f4b1
+00000c20: 3563 3837 6431 6566 310a 2020 2060 6060  5c87d1ef1.   ```
+00000c30: 0a0a 2d20 4578 7472 6163 7420 7369 6e67  ..- Extract sing
+00000c40: 6c65 2066 6965 6c64 7320 6672 6f6d 2062  le fields from b
+00000c50: 6c6f 636b 7320 6f72 2074 7261 6e73 6163  locks or transac
+00000c60: 7469 6f6e 732c 2075 7369 6e67 2060 6a71  tions, using `jq
+00000c70: 6020 286d 6f72 6520 6465 7461 696c 7320  ` (more details 
+00000c80: 5b69 6e20 7468 6520 5769 6b69 5d28 6874  [in the Wiki](ht
+00000c90: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000ca0: 2f63 6f63 636f 696e 6f6d 616e 652f 7765  /coccoinomane/we
+00000cb0: 6233 636c 692f 7769 6b69 2f25 4532 2538  b3cli/wiki/%E2%8
+00000cc0: 3625 4141 2545 4625 4238 2538 462d 4f75  6%AA%EF%B8%8F-Ou
+00000cd0: 7470 7574 2d70 726f 6365 7373 696e 6729  tput-processing)
+00000ce0: 293a 0a20 2020 6060 6062 6173 680a 2020  ):.   ```bash.  
+00000cf0: 2077 3320 626c 6f63 6b20 6c61 7465 7374   w3 block latest
+00000d00: 207c 206a 7120 2d72 2027 2e62 6173 6546   | jq -r '.baseF
+00000d10: 6565 5065 7247 6173 270a 2020 2060 6060  eePerGas'.   ```
+00000d20: 0a0a 2d20 5369 676e 206d 6573 7361 6765  ..- Sign message
+00000d30: 733a 0a20 2020 6060 6062 6173 680a 2020  s:.   ```bash.  
+00000d40: 2077 3320 7369 676e 2027 4865 6c6c 6f20   w3 sign 'Hello 
+00000d50: 776f 726c 6421 270a 2020 2060 6060 0a0a  world!'.   ```..
+00000d60: 2320 4164 7661 6e63 6564 2065 7861 6d70  # Advanced examp
+00000d70: 6c65 730a 0a2d 2053 656e 6420 636f 696e  les..- Send coin
+00000d80: 7320 6f72 2074 6f6b 656e 7320 746f 2061  s or tokens to a
+00000d90: 6e79 2061 6464 7265 7373 3a0a 2020 2060  ny address:.   `
+00000da0: 6060 0a20 2020 7733 2073 656e 6420 756e  ``.   w3 send un
+00000db0: 6963 6566 2031 2045 5448 2020 2020 2020  icef 1 ETH      
+00000dc0: 2320 7365 6e64 2031 2045 5448 2c20 6173  # send 1 ETH, as
+00000dd0: 6b20 666f 7220 636f 6e66 6972 6d61 7469  k for confirmati
+00000de0: 6f6e 0a20 2020 7733 2073 656e 6420 756e  on.   w3 send un
+00000df0: 6963 6566 2031 2045 5448 2067 7765 6920  icef 1 ETH gwei 
+00000e00: 2320 7365 6e64 2031 2067 7765 692c 2061  # send 1 gwei, a
+00000e10: 736b 2066 6f72 2063 6f6e 6669 726d 6174  sk for confirmat
+00000e20: 696f 6e0a 2020 2077 3320 7365 6e64 2075  ion.   w3 send u
+00000e30: 6e69 6365 6620 3120 7573 6463 2020 2020  nicef 1 usdc    
+00000e40: 2023 2073 656e 6420 3120 5553 4443 0a20   # send 1 USDC. 
+00000e50: 2020 6060 600a 0a2d 2053 7761 7020 746f    ```..- Swap to
+00000e60: 6b65 6e73 206f 6e20 6120 4445 583a 0a20  kens on a DEX:. 
+00000e70: 2020 6060 600a 2020 2077 3320 7377 6170    ```.   w3 swap
+00000e80: 2075 6e69 7377 6170 5f76 3220 3120 7573   uniswap_v2 1 us
+00000e90: 6463 2075 7364 7420 2020 2020 2320 7377  dc usdt     # sw
+00000ea0: 6170 2031 2055 5344 4320 666f 7220 5553  ap 1 USDC for US
+00000eb0: 4454 206f 6e20 556e 6973 7761 700a 2020  DT on Uniswap.  
+00000ec0: 2077 3361 7661 7820 7377 6170 2074 7261   w3avax swap tra
+00000ed0: 6465 726a 6f65 2031 2075 7364 6320 7761  derjoe 1 usdc wa
+00000ee0: 7661 7820 2320 7377 6170 2031 2055 5344  vax # swap 1 USD
+00000ef0: 4320 666f 7220 5741 5641 5820 6f6e 2054  C for WAVAX on T
+00000f00: 7261 6465 724a 6f65 0a20 2020 6060 600a  raderJoe.   ```.
+00000f10: 0a23 2053 6d61 7274 2043 6f6e 7472 6163  .# Smart Contrac
+00000f20: 7420 7375 7070 6f72 740a 0a60 7765 6233  t support..`web3
+00000f30: 636c 6960 2063 6f6d 6573 2070 7265 6c6f  cli` comes prelo
+00000f40: 6164 6564 2077 6974 6820 736f 6d65 2070  aded with some p
+00000f50: 6f70 756c 6172 2073 6d61 7274 2063 6f6e  opular smart con
+00000f60: 7472 6163 7473 2c20 696e 636c 7564 696e  tracts, includin
+00000f70: 6720 4552 4332 3020 746f 6b65 6e73 2061  g ERC20 tokens a
+00000f80: 6e64 2055 6e69 7377 6170 2063 6c6f 6e65  nd Uniswap clone
+00000f90: 732e 0a0a 5365 6520 7468 6520 6176 6169  s...See the avai
+00000fa0: 6c61 626c 6520 636f 6e74 7261 6374 7320  lable contracts 
+00000fb0: 7769 7468 2060 7733 2063 6f6e 7472 6163  with `w3 contrac
+00000fc0: 7420 6c69 7374 603a 0a0a 6060 600a 7733  t list`:..```.w3
+00000fd0: 2063 6f6e 7472 6163 7420 6c69 7374 2020   contract list  
+00000fe0: 2020 2020 2020 2020 2020 2020 2320 636f              # co
+00000ff0: 6e74 7261 6374 7320 6f6e 2045 7468 6572  ntracts on Ether
+00001000: 6575 6d0a 7733 2063 6f6e 7472 6163 7420  eum.w3 contract 
+00001010: 6c69 7374 202d 2d63 6861 696e 2062 6e62  list --chain bnb
+00001020: 2020 2320 636f 6e74 7261 6374 7320 6f6e    # contracts on
+00001030: 2042 4e42 2063 6861 696e 0a60 6060 0a0a   BNB chain.```..
+00001040: 596f 7520 6361 6e20 616c 736f 2061 6464  You can also add
+00001050: 2063 7573 746f 6d20 636f 6e74 7261 6374   custom contract
+00001060: 7320 7769 7468 2060 7733 2063 6f6e 7472  s with `w3 contr
+00001070: 6163 7420 6164 6460 3a0a 0a60 6060 0a77  act add`:..```.w
+00001080: 3320 636f 6e74 7261 6374 2061 6464 2077  3 contract add w
+00001090: 6574 6820 3078 4330 3261 6141 3339 6232  eth 0xC02aaA39b2
+000010a0: 3233 4645 3844 3041 3065 3543 3446 3237  23FE8D0A0e5C4F27
+000010b0: 6541 4439 3038 3343 3735 3643 6332 202d  eAD9083C756Cc2 -
+000010c0: 2d74 7970 6520 6572 6332 300a 6060 600a  -type erc20.```.
+000010d0: 0a53 6565 2061 7661 696c 6162 6c65 2066  .See available f
+000010e0: 756e 6374 696f 6e73 2061 6e64 2065 7665  unctions and eve
+000010f0: 6e74 7320 6f6e 2061 2063 6f6e 7472 6163  nts on a contrac
+00001100: 7420 7769 7468 2060 7733 2061 6269 2066  t with `w3 abi f
+00001110: 756e 6374 696f 6e73 6020 616e 6420 6077  unctions` and `w
+00001120: 3320 6162 6920 6576 656e 7473 603a 0a0a  3 abi events`:..
+00001130: 6060 600a 7733 2061 6269 2066 6e73 2077  ```.w3 abi fns w
+00001140: 6574 6820 2020 2020 2020 2020 2020 2320  eth           # 
+00001150: 6675 6e63 7469 6f6e 7320 6f6e 2057 4554  functions on WET
+00001160: 4820 746f 6b65 6e0a 7733 2061 6269 2065  H token.w3 abi e
+00001170: 7673 2075 6e69 7377 6170 5f76 3220 2020  vs uniswap_v2   
+00001180: 2020 2320 6576 656e 7473 206f 6e20 556e    # events on Un
+00001190: 6973 7761 7020 5632 0a77 3320 6162 6920  iswap V2.w3 abi 
+000011a0: 666e 7320 2d2d 6162 6920 6162 692e 6a73  fns --abi abi.js
+000011b0: 6f6e 2023 2066 756e 6374 696f 6e73 206f  on # functions o
+000011c0: 6620 616e 2061 7262 6974 7261 7279 2041  f an arbitrary A
+000011d0: 4249 0a60 6060 0a0a 2323 2320 5265 6164  BI.```..### Read
+000011e0: 2066 726f 6d20 6120 736d 6172 7420 636f   from a smart co
+000011f0: 6e74 7261 6374 0a0a 546f 2072 6561 6420  ntract..To read 
+00001200: 6672 6f6d 2061 2073 6d61 7274 2063 6f6e  from a smart con
+00001210: 7472 6163 742c 2075 7365 2060 7733 2063  tract, use `w3 c
+00001220: 616c 6c60 2e20 466f 7220 6578 616d 706c  all`. For exampl
+00001230: 652c 2074 6f20 6765 7420 7468 6520 746f  e, to get the to
+00001240: 7461 6c0a 7375 7070 6c79 206f 6620 7468  tal.supply of th
+00001250: 6520 5745 5448 2074 6f6b 656e 2c20 7275  e WETH token, ru
+00001260: 6e3a 0a0a 6060 600a 7733 2063 616c 6c20  n:..```.w3 call 
+00001270: 7765 7468 2074 6f74 616c 5375 7070 6c79  weth totalSupply
+00001280: 0a60 6060 0a0a 4675 6e63 7469 6f6e 2061  .```..Function a
+00001290: 7267 756d 656e 7473 2061 7265 2070 6172  rguments are par
+000012a0: 7365 6420 6175 746f 6d61 7469 6361 6c6c  sed automaticall
+000012b0: 792c 2073 6f20 796f 7520 6361 6e20 6361  y, so you can ca
+000012c0: 6c6c 2060 6261 6c61 6e63 654f 6660 2077  ll `balanceOf` w
+000012d0: 6974 683a 0a0a 6060 600a 7733 2063 616c  ith:..```.w3 cal
+000012e0: 6c20 7765 7468 2062 616c 616e 6365 4f66  l weth balanceOf
+000012f0: 2030 7841 3539 4232 3964 3764 6243 3937   0xA59B29d7dbC97
+00001300: 3934 6431 6537 6634 3531 3233 4334 3862  94d1e7f45123C48b
+00001310: 3262 3864 3061 3334 3633 360a 6060 600a  2b8d0a34636.```.
+00001320: 0a59 6f75 2063 616e 2061 6c73 6f20 646f  .You can also do
+00001330: 206d 6f72 6520 636f 6d70 6c65 7820 7374   more complex st
+00001340: 7566 6620 6c69 6b65 3a0a 0a60 6060 6261  uff like:..```ba
+00001350: 7368 0a23 2067 6574 2074 6865 2061 6d6f  sh.# get the amo
+00001360: 756e 7420 6f66 2055 5344 5420 796f 7520  unt of USDT you 
+00001370: 6765 7420 666f 7220 3130 3020 5553 4443  get for 100 USDC
+00001380: 0a77 3320 6361 6c6c 2075 6e69 7377 6170  .w3 call uniswap
+00001390: 5f76 3220 6765 7441 6d6f 756e 7473 4f75  _v2 getAmountsOu
+000013a0: 7420 3130 3065 3620 7573 6463 2c75 7364  t 100e6 usdc,usd
+000013b0: 7420 7c20 6a71 202d 7220 272e 5b31 5d27  t | jq -r '.[1]'
+000013c0: 200a 6060 600a 0a23 2323 2057 7269 7465   .```..### Write
+000013d0: 2074 6f20 6120 736d 6172 7420 636f 6e74   to a smart cont
+000013e0: 7261 6374 0a0a 546f 2077 7269 7465 2074  ract..To write t
+000013f0: 6f20 7468 6520 626c 6f63 6b63 6861 696e  o the blockchain
+00001400: 2c20 7573 6520 6077 3320 7472 616e 7361  , use `w3 transa
+00001410: 6374 602e 2046 6f72 2065 7861 6d70 6c65  ct`. For example
+00001420: 2c20 746f 2074 7261 6e73 6665 7220 3120  , to transfer 1 
+00001430: 4554 4820 746f 200a 6164 6472 6573 732c  ETH to .address,
+00001440: 2072 756e 3a0a 0a60 6060 0a77 3320 7472   run:..```.w3 tr
+00001450: 616e 7361 6374 2077 6574 6820 7472 616e  ansact weth tran
+00001460: 7366 6572 203c 6164 6472 6573 733e 2031  sfer <address> 1
+00001470: 6531 380a 6060 600a 0a54 6f20 7377 6170  e18.```..To swap
+00001480: 2031 2055 5344 4320 666f 7220 5553 4454   1 USDC for USDT
+00001490: 206f 6e20 556e 6973 7761 702c 2061 6363   on Uniswap, acc
+000014a0: 6570 7469 6e67 206e 6f20 6c65 7373 2074  epting no less t
+000014b0: 6861 6e20 302e 3920 5553 4454 2069 6e20  han 0.9 USDT in 
+000014c0: 7265 7475 726e 2c20 7275 6e3a 0a0a 6060  return, run:..``
+000014d0: 600a 7733 2074 7261 6e73 6163 7420 7573  `.w3 transact us
+000014e0: 6463 2061 7070 726f 7665 2075 6e69 7377  dc approve unisw
+000014f0: 6170 5f76 3220 3165 360a 7733 2074 7261  ap_v2 1e6.w3 tra
+00001500: 6e73 6163 7420 756e 6973 7761 705f 7632  nsact uniswap_v2
+00001510: 2073 7761 7045 7861 6374 546f 6b65 6e73   swapExactTokens
+00001520: 466f 7254 6f6b 656e 7320 3165 3620 302e  ForTokens 1e6 0.
+00001530: 3965 3620 7573 6463 2c75 7364 7420 3c72  9e6 usdc,usdt <r
+00001540: 6563 6569 7665 7220 6164 6472 6573 733e  eceiver address>
+00001550: 2039 6539 0a60 6060 0a0a 2320 4d75 6c74   9e9.```..# Mult
+00001560: 6963 6861 696e 2073 7570 706f 7274 0a0a  ichain support..
+00001570: 6077 6562 3363 6c69 6020 636f 6d65 7320  `web3cli` comes 
+00001580: 7769 7468 206f 7574 2d6f 662d 7468 652d  with out-of-the-
+00001590: 626f 7820 7375 7070 6f72 7420 666f 7220  box support for 
+000015a0: 6d61 6e79 2063 6861 696e 732e 2020 546f  many chains.  To
+000015b0: 2073 6565 2074 6865 206c 6973 7420 6f66   see the list of
+000015c0: 2061 7661 696c 6162 6c65 2063 6861 696e   available chain
+000015d0: 732c 205b 7669 7369 7420 7468 6520 5769  s, [visit the Wi
+000015e0: 6b69 5d28 6874 7470 733a 2f2f 6769 7468  ki](https://gith
+000015f0: 7562 2e63 6f6d 2f63 6f63 636f 696e 6f6d  ub.com/coccoinom
+00001600: 616e 652f 7765 6233 636c 692f 7769 6b69  ane/web3cli/wiki
+00001610: 2f25 4532 2539 4225 3933 2d53 7570 706f  /%E2%9B%93-Suppo
+00001620: 7274 6564 2d63 6861 696e 7329 206f 7220  rted-chains) or 
+00001630: 7275 6e20 7468 6520 636f 6d6d 616e 6420  run the command 
+00001640: 6077 3320 6368 6169 6e20 6c69 7374 602e  `w3 chain list`.
+00001650: 0a0a 5061 7373 2074 6865 2063 6861 696e  ..Pass the chain
+00001660: 206e 616d 6520 7573 696e 6720 7468 6520   name using the 
+00001670: 666c 6167 2060 2d2d 6368 6169 6e60 206f  flag `--chain` o
+00001680: 7220 7468 6520 7368 6f72 7468 616e 6420  r the shorthand 
+00001690: 602d 6360 3a0a 0a60 6060 0a77 3320 6261  `-c`:..```.w3 ba
+000016a0: 6c61 6e63 6520 3078 3838 3934 6530 6130  lance 0x8894e0a0
+000016b0: 6339 3632 6362 3732 3363 3139 3736 6134  c962cb723c1976a4
+000016c0: 3432 3163 3935 3934 3962 6532 6434 6533  421c95949be2d4e3
+000016d0: 202d 2d63 6861 696e 2062 6e62 2020 2320   --chain bnb  # 
+000016e0: 626e 6220 6368 6169 6e0a 7733 2062 616c  bnb chain.w3 bal
+000016f0: 616e 6365 2030 7838 3839 3465 3061 3063  ance 0x8894e0a0c
+00001700: 3936 3263 6237 3233 6331 3937 3661 3434  962cb723c1976a44
+00001710: 3231 6339 3539 3439 6265 3264 3465 3320  21c95949be2d4e3 
+00001720: 2d2d 6368 6169 6e20 6176 6178 2023 2061  --chain avax # a
+00001730: 7661 7820 6368 6169 6e0a 6060 600a 0a59  vax chain.```..Y
+00001740: 6f75 2063 616e 2061 6c73 6f20 7573 6520  ou can also use 
+00001750: 6f6e 6520 6f66 2074 6865 2070 726f 7669  one of the provi
+00001760: 6465 6420 616c 6961 7365 732c 206c 696b  ded aliases, lik
+00001770: 6520 6077 3362 6e62 602c 2060 7733 6176  e `w3bnb`, `w3av
+00001780: 6178 602c 206f 7220 6077 3361 7262 603a  ax`, or `w3arb`:
+00001790: 0a0a 6060 600a 7733 626e 6220 6261 6c61  ..```.w3bnb bala
+000017a0: 6e63 6520 3078 3838 3934 6530 6130 6339  nce 0x8894e0a0c9
+000017b0: 3632 6362 3732 3363 3139 3736 6134 3432  62cb723c1976a442
+000017c0: 3163 3935 3934 3962 6532 6434 6533 2020  1c95949be2d4e3  
+000017d0: 2320 626e 6220 6368 6169 6e0a 7733 6176  # bnb chain.w3av
+000017e0: 6178 2062 616c 616e 6365 2030 7838 3839  ax balance 0x889
+000017f0: 3465 3061 3063 3936 3263 6237 3233 6331  4e0a0c962cb723c1
+00001800: 3937 3661 3434 3231 6339 3539 3439 6265  976a4421c95949be
+00001810: 3264 3465 3320 2320 6176 6178 2063 6861  2d4e3 # avax cha
+00001820: 696e 0a60 6060 0a0a 4966 2079 6f75 2061  in.```..If you a
+00001830: 7265 2066 6f63 7573 7369 6e67 206f 6e20  re focussing on 
+00001840: 6120 7370 6563 6966 6963 2063 6861 696e  a specific chain
+00001850: 2c20 7365 7420 6974 2061 7320 7468 6520  , set it as the 
+00001860: 6465 6661 756c 743a 0a0a 6060 600a 7733  default:..```.w3
+00001870: 2063 6f6e 6669 6720 7365 7420 6465 6661   config set defa
+00001880: 756c 745f 6368 6169 6e20 626e 620a 7733  ult_chain bnb.w3
+00001890: 2062 616c 616e 6365 2030 7838 3839 3465   balance 0x8894e
+000018a0: 3061 3063 3936 3263 6237 3233 6331 3937  0a0c962cb723c197
+000018b0: 3661 3434 3231 6339 3539 3439 6265 3264  6a4421c95949be2d
+000018c0: 3465 3320 2020 2020 2020 2020 2020 2020  4e3             
+000018d0: 2320 626e 6220 6368 6169 6e0a 7733 2062  # bnb chain.w3 b
+000018e0: 616c 616e 6365 2030 7838 3839 3465 3061  alance 0x8894e0a
+000018f0: 3063 3936 3263 6237 3233 6331 3937 3661  0c962cb723c1976a
+00001900: 3434 3231 6339 3539 3439 6265 3264 3465  4421c95949be2d4e
+00001910: 3320 2d2d 6368 6169 6e20 6574 6820 2320  3 --chain eth # 
+00001920: 6574 6820 6368 6169 6e0a 6060 600a 0a23  eth chain.```..#
+00001930: 2055 7365 2063 7573 746f 6d20 5250 430a   Use custom RPC.
+00001940: 0a42 7920 6465 6661 756c 742c 2060 7765  .By default, `we
+00001950: 6233 636c 6960 2077 696c 6c20 636f 6e6e  b3cli` will conn
+00001960: 6563 7420 746f 2074 6865 2062 6c6f 636b  ect to the block
+00001970: 6368 6169 6e20 7573 696e 6720 6120 7072  chain using a pr
+00001980: 652d 636f 6e66 6967 7572 6564 2070 7562  e-configured pub
+00001990: 6c69 6320 6e6f 6465 2e20 2059 6f75 2063  lic node.  You c
+000019a0: 616e 2073 6565 2074 6865 206c 6973 7420  an see the list 
+000019b0: 6f66 2073 7563 6820 6e6f 6465 7320 7769  of such nodes wi
+000019c0: 7468 2074 6865 2063 6f6d 6d61 6e64 2060  th the command `
+000019d0: 7733 2072 7063 206c 6973 7460 2e0a 0a54  w3 rpc list`...T
+000019e0: 6f20 7573 6520 6120 6375 7374 6f6d 206d  o use a custom m
+000019f0: 6f64 652c 2070 6c65 6173 6520 7370 6563  ode, please spec
+00001a00: 6966 7920 7468 6520 602d 2d72 7063 6020  ify the `--rpc` 
+00001a10: 666c 6167 2e20 2046 6f72 2065 7861 6d70  flag.  For examp
+00001a20: 6c65 2c20 746f 2075 7365 2041 6e6b 7227  le, to use Ankr'
+00001a30: 7320 6e6f 6465 2074 6f20 4574 6865 7265  s node to Ethere
+00001a40: 756d 3a0a 0a60 6060 6261 7368 0a77 3320  um:..```bash.w3 
+00001a50: 626c 6f63 6b20 6c61 7465 7374 202d 2d72  block latest --r
+00001a60: 7063 2068 7474 7073 3a2f 2f72 7063 2e61  pc https://rpc.a
+00001a70: 6e6b 722e 636f 6d2f 6574 680a 6060 600a  nkr.com/eth.```.
+00001a80: 0a55 7369 6e67 2061 2063 7573 746f 6d20  .Using a custom 
+00001a90: 6e6f 6465 2069 7320 6d6f 7374 2075 7365  node is most use
+00001aa0: 6675 6c20 696e 2074 6865 2066 6f6c 6c6f  ful in the follo
+00001ab0: 7769 6e67 2073 6974 7561 7469 6f6e 733a  wing situations:
+00001ac0: 0a0a 312e 2059 6f75 2077 616e 7420 746f  ..1. You want to
+00001ad0: 2075 7365 2061 206e 6f64 6520 6672 6f6d   use a node from
+00001ae0: 2061 206e 6f64 6520 7072 6f76 6964 6572   a node provider
+00001af0: 2c20 652e 672e 2049 6e66 7572 613a 0a20  , e.g. Infura:. 
+00001b00: 2020 6060 6062 6173 680a 2020 2077 3320    ```bash.   w3 
+00001b10: 626c 6f63 6b20 2d2d 7270 6320 6874 7470  block --rpc http
+00001b20: 733a 2f2f 6574 682d 6d61 696e 6e65 742e  s://eth-mainnet.
+00001b30: 672e 616c 6368 656d 792e 636f 6d2f 7632  g.alchemy.com/v2
+00001b40: 2f7b 594f 5552 2d41 5049 2d4b 4559 7d0a  /{YOUR-API-KEY}.
+00001b50: 2020 2060 6060 0a32 2e20 596f 7520 7761     ```.2. You wa
+00001b60: 6e74 2074 6f20 7573 6520 6120 7072 6976  nt to use a priv
+00001b70: 6174 6520 6e6f 6465 3a0a 2020 2060 6060  ate node:.   ```
+00001b80: 6261 7368 0a20 2020 7733 2062 6c6f 636b  bash.   w3 block
+00001b90: 202d 2d72 7063 2068 7474 703a 2f2f 3132   --rpc http://12
+00001ba0: 372e 302e 302e 313a 3835 3435 0a20 2020  7.0.0.1:8545.   
+00001bb0: 7733 2062 6c6f 636b 202d 2d72 7063 2077  w3 block --rpc w
+00001bc0: 733a 2f2f 3132 372e 302e 302e 313a 3835  s://127.0.0.1:85
+00001bd0: 3436 0a20 2020 6060 600a 332e 2059 6f75  46.   ```.3. You
+00001be0: 2077 616e 7420 746f 2075 7365 2061 2074   want to use a t
+00001bf0: 6573 746e 6574 2063 6861 696e 3a0a 2020  estnet chain:.  
+00001c00: 2060 6060 6261 7368 0a20 2020 7733 6574   ```bash.   w3et
+00001c10: 6820 626c 6f63 6b20 2d2d 7270 6320 6874  h block --rpc ht
+00001c20: 7470 733a 2f2f 7270 632e 616e 6b72 2e63  tps://rpc.ankr.c
+00001c30: 6f6d 2f65 7468 5f67 6f65 726c 690a 2020  om/eth_goerli.  
+00001c40: 2077 3362 6e62 2062 6c6f 636b 202d 2d72   w3bnb block --r
+00001c50: 7063 2068 7474 7073 3a2f 2f64 6174 612d  pc https://data-
+00001c60: 7365 6564 2d70 7265 6273 632d 312d 7331  seed-prebsc-1-s1
+00001c70: 2e62 696e 616e 6365 2e6f 7267 3a38 3534  .binance.org:854
+00001c80: 352f 0a20 2020 6060 600a 0a0a 2320 4164  5/.   ```...# Ad
+00001c90: 6420 6375 7374 6f6d 2063 6861 696e 730a  d custom chains.
+00001ca0: 0a41 6464 206e 6577 2063 6861 696e 7320  .Add new chains 
+00001cb0: 7769 7468 2060 7733 2063 6861 696e 2061  with `w3 chain a
+00001cc0: 6464 603a 0a0a 6060 600a 7733 2063 6861  dd`:..```.w3 cha
+00001cd0: 696e 2061 6464 2063 726f 6e6f 7320 3235  in add cronos 25
+00001ce0: 2043 524f 202d 2d74 782d 7479 7065 2032   CRO --tx-type 2
+00001cf0: 202d 2d72 7063 2068 7474 7073 3a2f 2f65   --rpc https://e
+00001d00: 766d 2e63 726f 6e6f 732e 6f72 670a 6060  vm.cronos.org.``
+00001d10: 600a 0a55 7365 2074 6865 2063 7573 746f  `..Use the custo
+00001d20: 6d20 6368 6169 6e20 7769 7468 2060 2d2d  m chain with `--
+00001d30: 6368 6169 6e60 3a0a 0a60 6060 0a77 3320  chain`:..```.w3 
+00001d40: 6261 6c61 6e63 6520 3078 3764 6539 6162  balance 0x7de9ab
+00001d50: 3165 3661 3630 6163 3761 3730 6365 3936  1e6a60ac7a70ce96
+00001d60: 6431 6439 3561 3064 6663 6563 6637 6266  d1d95a0dfcecf7bf
+00001d70: 6237 202d 2d63 6861 696e 2063 726f 6e6f  b7 --chain crono
+00001d80: 730a 6060 600a 0a4c 6973 7420 6578 6973  s.```..List exis
+00001d90: 7469 6e67 2063 6861 696e 7320 7769 7468  ting chains with
+00001da0: 2060 7733 2063 6861 696e 206c 6973 7460   `w3 chain list`
+00001db0: 2c20 616e 6420 6465 6c65 7465 2074 6865  , and delete the
+00001dc0: 6d20 7769 7468 2060 7733 2063 6861 696e  m with `w3 chain
+00001dd0: 2064 656c 6574 6560 2e0a 0a0a 2320 4164   delete`....# Ad
+00001de0: 6472 6573 7320 626f 6f6b 0a0a 6077 3360  dress book..`w3`
+00001df0: 2063 616e 2073 746f 7265 2074 6167 7320   can store tags 
+00001e00: 6a75 7374 206c 696b 6520 796f 7520 776f  just like you wo
+00001e10: 756c 6420 646f 206f 6e20 6574 6865 7273  uld do on ethers
+00001e20: 6361 6e2e 696f 206f 7220 6273 6373 6361  can.io or bscsca
+00001e30: 6e2e 636f 6d3a 0a0a 6060 6062 6173 680a  n.com:..```bash.
+00001e40: 7733 2061 6464 7265 7373 2061 6464 2065  w3 address add e
+00001e50: 7468 6572 6575 6d5f 666f 756e 6461 7469  thereum_foundati
+00001e60: 6f6e 2030 7864 6530 6232 3935 3636 3961  on 0xde0b295669a
+00001e70: 3966 6439 3364 3566 3238 6439 6563 3835  9fd93d5f28d9ec85
+00001e80: 6534 3066 3463 6236 3937 6261 650a 7733  e40f4cb697bae.w3
+00001e90: 2061 6464 7265 7373 2061 6464 2062 696e   address add bin
+00001ea0: 616e 6365 5f68 6f74 5f77 616c 6c65 7420  ance_hot_wallet 
+00001eb0: 3078 3838 3934 6530 6130 6339 3632 6362  0x8894e0a0c962cb
+00001ec0: 3732 3363 3139 3736 6134 3432 3163 3935  723c1976a4421c95
+00001ed0: 3934 3962 6532 6434 6533 0a60 6060 0a0a  949be2d4e3.```..
+00001ee0: 596f 7520 6361 6e20 7573 6520 7468 6573  You can use thes
+00001ef0: 6520 7461 6773 2069 6e73 7465 6164 206f  e tags instead o
+00001f00: 6620 7468 6520 6163 7475 616c 2061 6464  f the actual add
+00001f10: 7265 7373 6573 3a0a 0a60 6060 6261 7368  resses:..```bash
+00001f20: 0a77 3320 6261 6c61 6e63 6520 6574 6865  .w3 balance ethe
+00001f30: 7265 756d 5f66 6f75 6e64 6174 696f 6e0a  reum_foundation.
+00001f40: 7733 2062 616c 616e 6365 2062 696e 616e  w3 balance binan
+00001f50: 6365 5f68 6f74 5f77 616c 6c65 7420 2d2d  ce_hot_wallet --
+00001f60: 6368 6169 6e20 626e 620a 6060 600a 0a54  chain bnb.```..T
+00001f70: 6f20 7365 6520 7468 6520 6c69 7374 206f  o see the list o
+00001f80: 6620 7361 7665 6420 6164 6472 6573 7365  f saved addresse
+00001f90: 732c 2072 756e 2060 7733 2061 6464 7265  s, run `w3 addre
+00001fa0: 7373 206c 6973 7460 2c20 746f 2064 656c  ss list`, to del
+00001fb0: 6574 6520 616e 2061 6464 7265 7373 2075  ete an address u
+00001fc0: 7365 2060 7733 2061 6464 7265 7373 2064  se `w3 address d
+00001fd0: 656c 6574 6560 2e0a 0a23 2057 616c 6c65  elete`...# Walle
+00001fe0: 7420 6d61 6e61 6765 6d65 6e74 0a0a 436f  t management..Co
+00001ff0: 6d6d 616e 6473 2073 7563 6820 6173 2060  mmands such as `
+00002000: 7733 2073 656e 6460 2061 6e64 2060 7733  w3 send` and `w3
+00002010: 2073 7761 7060 2072 6571 7569 7265 2074   swap` require t
+00002020: 6861 7420 796f 7520 7370 6563 6966 7920  hat you specify 
+00002030: 7768 6f20 6973 2067 6f69 6e67 2074 6f20  who is going to 
+00002040: 7369 676e 2074 6865 2074 7261 6e73 6163  sign the transac
+00002050: 7469 6f6e 732e 2020 596f 7520 6361 6e20  tions.  You can 
+00002060: 7370 6563 6966 7920 7468 6520 7369 676e  specify the sign
+00002070: 6572 2077 6974 6820 7468 6520 602d 2d73  er with the `--s
+00002080: 6967 6e65 7260 206f 7220 602d 7360 2066  igner` or `-s` f
+00002090: 6c61 673a 0a0a 6060 6062 6173 680a 7733  lag:..```bash.w3
+000020a0: 203c 636f 6d6d 616e 643e 202d 2d73 6967   <command> --sig
+000020b0: 6e65 7220 6d79 2d73 6967 6e65 720a 6060  ner my-signer.``
+000020c0: 600a 0a48 6572 652c 2060 6d79 5f73 6967  `..Here, `my_sig
+000020d0: 6e65 7260 2063 616e 2062 6520 616e 7920  ner` can be any 
+000020e0: 6f66 2074 6865 7365 2074 6869 6e67 733a  of these things:
+000020f0: 0a0a 2d20 5468 6520 6e61 6d65 206f 7220  ..- The name or 
+00002100: 7468 6520 6164 6472 6573 7320 6f66 2061  the address of a
+00002110: 2073 6967 6e65 7220 7468 6174 2079 6f75   signer that you
+00002120: 2070 7265 7669 6f75 736c 7920 7265 6769   previously regi
+00002130: 7374 6572 6564 2077 6974 6820 6077 3320  stered with `w3 
+00002140: 7369 676e 6572 2061 6464 206d 795f 7369  signer add my_si
+00002150: 676e 6572 602e 2020 5369 676e 6572 7320  gner`.  Signers 
+00002160: 6372 6561 7465 6420 696e 2074 6869 7320  created in this 
+00002170: 7761 7920 6172 6520 656e 6372 7970 7465  way are encrypte
+00002180: 6420 7769 7468 2074 6865 2061 7070 206b  d with the app k
+00002190: 6579 2061 6e64 2073 746f 7265 6420 696e  ey and stored in
+000021a0: 2074 6865 2064 6174 6162 6173 652e 2020   the database.  
+000021b0: 4174 2061 6e79 2074 696d 652c 2079 6f75  At any time, you
+000021c0: 2063 616e 2073 6565 2074 6865 206c 6973   can see the lis
+000021d0: 7420 6f66 2072 6567 6973 7465 7265 6420  t of registered 
+000021e0: 7573 6572 7320 6279 2072 756e 6e69 6e67  users by running
+000021f0: 2060 7733 2073 6967 6e65 7220 6c69 7374   `w3 signer list
+00002200: 602e 0a2d 2054 6865 2070 6174 6820 746f  `..- The path to
+00002210: 2061 2066 696c 6520 7468 6174 2079 6f75   a file that you
+00002220: 2070 7265 7669 6f75 736c 7920 6372 6561   previously crea
+00002230: 7465 6420 7769 7468 2060 7733 206b 6579  ted with `w3 key
+00002240: 6669 6c65 2063 7265 6174 6560 2e20 2041  file create`.  A
+00002250: 206b 6579 6669 6c65 2069 7320 6120 7369   keyfile is a si
+00002260: 6d70 6c65 204a 534f 4e20 6669 6c65 2074  mple JSON file t
+00002270: 6861 7420 636f 6e74 6169 6e73 2079 6f75  hat contains you
+00002280: 7220 7072 6976 6174 6520 6b65 7920 696e  r private key in
+00002290: 2070 6173 7377 6f72 642d 656e 6372 7970   password-encryp
+000022a0: 7465 6420 666f 726d 2e20 2046 6565 6c20  ted form.  Feel 
+000022b0: 6672 6565 2074 6f20 7573 6520 6b65 7966  free to use keyf
+000022c0: 696c 6573 2067 656e 6572 6174 6564 2062  iles generated b
+000022d0: 7920 6f74 6865 7220 746f 6f6c 732c 206c  y other tools, l
+000022e0: 696b 6520 6765 7468 2c20 7061 7269 7479  ike geth, parity
+000022f0: 2c20 6272 6f77 6e69 652c 2065 7463 2e0a  , brownie, etc..
+00002300: 2d20 5468 6520 6163 7475 616c 2070 7269  - The actual pri
+00002310: 7661 7465 206b 6579 206f 6620 7468 6520  vate key of the 
+00002320: 7369 676e 6572 2074 6861 7420 796f 7520  signer that you 
+00002330: 7761 6e74 2074 6f20 7573 652e 2020 5468  want to use.  Th
+00002340: 6973 2069 7320 756e 7361 6665 2c20 7573  is is unsafe, us
+00002350: 6520 6974 2061 7420 796f 7572 206f 776e  e it at your own
+00002360: 2072 6973 6b21 0a0a 506c 6561 7365 206e   risk!..Please n
+00002370: 6f74 6520 7468 6174 2077 6865 6e20 7468  ote that when th
+00002380: 6520 602d 2d73 6967 6e65 7260 2066 6c61  e `--signer` fla
+00002390: 6720 6973 206e 6f74 2070 726f 7669 6465  g is not provide
+000023a0: 642c 2061 6e64 2074 6865 7265 2069 7320  d, and there is 
+000023b0: 6f6e 6c79 206f 6e65 2072 6567 6973 7465  only one registe
+000023c0: 7265 6420 7369 676e 6572 2c20 7468 656e  red signer, then
+000023d0: 2074 6869 7320 7769 6c6c 2062 6520 7573   this will be us
+000023e0: 6564 2e0a 0a0a 2323 2320 4465 6661 756c  ed....### Defaul
+000023f0: 7420 7369 676e 6572 0a0a 4966 2079 6f75  t signer..If you
+00002400: 2070 6c61 6e20 746f 2075 7365 2074 6865   plan to use the
+00002410: 2073 616d 6520 7369 676e 6572 2066 6f72   same signer for
+00002420: 2061 2077 6869 6c65 2c20 6d61 6b65 2069   a while, make i
+00002430: 7420 7468 6520 2a2a 6465 6661 756c 7420  t the **default 
+00002440: 7369 676e 6572 2a2a 2077 6974 6820 7468  signer** with th
+00002450: 6520 636f 6d6d 616e 643a 0a0a 6060 6062  e command:..```b
+00002460: 6173 680a 7733 2063 6f6e 6669 6720 7365  ash.w3 config se
+00002470: 7420 6465 6661 756c 745f 7369 676e 6572  t default_signer
+00002480: 206d 795f 7369 676e 6572 0a60 6060 0a0a   my_signer.```..
+00002490: 496e 2074 6869 7320 7761 792c 2079 6f75  In this way, you
+000024a0: 2077 696c 6c20 6e6f 7420 6861 7665 2074   will not have t
+000024b0: 6f20 7370 6563 6966 7920 7468 6520 602d  o specify the `-
+000024c0: 2d73 6967 6e65 7260 2066 6c61 6720 616e  -signer` flag an
+000024d0: 796d 6f72 652e 0a0a 0a23 2323 2043 7265  ymore....### Cre
+000024e0: 6174 6520 6e65 7720 7072 6976 6174 6520  ate new private 
+000024f0: 6b65 7973 0a0a 596f 7520 6361 6e20 616c  keys..You can al
+00002500: 736f 2063 7265 6174 6520 6120 6272 616e  so create a bran
+00002510: 6420 6e65 7720 7761 6c6c 6574 206f 6e20  d new wallet on 
+00002520: 7468 6520 676f 2c20 7769 7468 6f75 7420  the go, without 
+00002530: 7468 6520 6e65 6564 2074 6f20 7072 6f76  the need to prov
+00002540: 6964 6520 6120 6b65 792c 2062 7920 7573  ide a key, by us
+00002550: 696e 6720 7468 6520 602d 2d63 7265 6174  ing the `--creat
+00002560: 6560 2066 6c61 673a 0a0a 6060 6062 6173  e` flag:..```bas
+00002570: 680a 7733 2073 6967 6e65 7220 6164 6420  h.w3 signer add 
+00002580: 6d79 5f77 616c 6c65 7420 2d2d 6372 6561  my_wallet --crea
+00002590: 7465 0a60 6060 0a0a 5468 6520 7265 7375  te.```..The resu
+000025a0: 6c74 696e 6720 7072 6976 6174 6520 6b65  lting private ke
+000025b0: 7920 7769 6c6c 2062 6520 7072 696e 7465  y will be printe
+000025c0: 6420 746f 2073 6372 6565 6e2e 0a0a 2320  d to screen...# 
+000025d0: 446f 6375 6d65 6e74 6174 696f 6e0a 0a43  Documentation..C
+000025e0: 6865 636b 2074 6865 205b 7072 6f6a 6563  heck the [projec
+000025f0: 7427 7320 7769 6b69 206f 6e20 4769 7468  t's wiki on Gith
+00002600: 7562 5d28 6874 7470 733a 2f2f 6769 7468  ub](https://gith
+00002610: 7562 2e63 6f6d 2f63 6f63 636f 696e 6f6d  ub.com/coccoinom
+00002620: 616e 652f 7765 6233 636c 692f 7769 6b69  ane/web3cli/wiki
+00002630: 2f29 2e20 496e 2070 6172 7469 6375 6c61  /). In particula
+00002640: 723a 0a0a 2d20 5bf0 9fab a120 4c69 7374  r:..- [.... List
+00002650: 206f 6620 636f 6d6d 616e 6473 5d28 6874   of commands](ht
+00002660: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00002670: 2f63 6f63 636f 696e 6f6d 616e 652f 7765  /coccoinomane/we
+00002680: 6233 636c 692f 7769 6b69 2f25 4630 2539  b3cli/wiki/%F0%9
+00002690: 4625 4142 2541 312d 4c69 7374 2d6f 662d  F%AB%A1-List-of-
+000026a0: 636f 6d6d 616e 6473 290a 2d20 5be2 9b93  commands).- [...
+000026b0: 2041 6c6c 2073 7570 706f 7274 6564 2063   All supported c
+000026c0: 6861 696e 735d 2868 7474 7073 3a2f 2f67  hains](https://g
+000026d0: 6974 6875 622e 636f 6d2f 636f 6363 6f69  ithub.com/coccoi
+000026e0: 6e6f 6d61 6e65 2f77 6562 3363 6c69 2f77  nomane/web3cli/w
+000026f0: 696b 692f 2545 3225 3942 2539 332d 5375  iki/%E2%9B%93-Su
+00002700: 7070 6f72 7465 642d 6368 6169 6e73 290a  pported-chains).
+00002710: 2d20 5bf0 9f93 9d20 436f 6e66 6967 7572  - [.... Configur
+00002720: 6174 696f 6e5d 2868 7474 7073 3a2f 2f67  ation](https://g
+00002730: 6974 6875 622e 636f 6d2f 636f 6363 6f69  ithub.com/coccoi
+00002740: 6e6f 6d61 6e65 2f77 6562 3363 6c69 2f77  nomane/web3cli/w
+00002750: 696b 692f 2546 3025 3946 2539 3325 3944  iki/%F0%9F%93%9D
+00002760: 2d43 6f6e 6669 6775 7261 7469 6f6e 290a  -Configuration).
+00002770: 2d20 5bf0 9faa 9f20 5275 6e20 7765 6233  - [.... Run web3
+00002780: 636c 6920 6f6e 2057 696e 646f 7773 5d28  cli on Windows](
+00002790: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000027a0: 6f6d 2f63 6f63 636f 696e 6f6d 616e 652f  om/coccoinomane/
+000027b0: 7765 6233 636c 692f 7769 6b69 2f25 4630  web3cli/wiki/%F0
+000027c0: 2539 4625 4141 2539 462d 5275 6e2d 7765  %9F%AA%9F-Run-we
+000027d0: 6233 636c 692d 6f6e 2d57 696e 646f 7773  b3cli-on-Windows
+000027e0: 290a 2d20 5be2 86aa efb8 8f20 4f75 7470  ).- [...... Outp
+000027f0: 7574 2070 726f 6365 7373 696e 675d 2868  ut processing](h
+00002800: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00002810: 6d2f 636f 6363 6f69 6e6f 6d61 6e65 2f77  m/coccoinomane/w
+00002820: 6562 3363 6c69 2f77 696b 692f 2545 3225  eb3cli/wiki/%E2%
+00002830: 3836 2541 4125 4546 2542 3825 3846 2d4f  86%AA%EF%B8%8F-O
+00002840: 7574 7075 742d 7072 6f63 6573 7369 6e67  utput-processing
+00002850: 290a 0a23 2043 6f6e 7472 6962 7574 696e  )..# Contributin
+00002860: 670a 0a41 6c6c 2063 6f6e 7472 6962 7574  g..All contribut
+00002870: 696f 6e73 2061 7265 2077 656c 636f 6d65  ions are welcome
+00002880: 2120 546f 2073 7461 7274 2069 6d70 726f  ! To start impro
+00002890: 7669 6e67 2060 7765 6233 636c 6960 2c20  ving `web3cli`, 
+000028a0: 706c 6561 7365 2072 6566 6572 2074 6f20  please refer to 
+000028b0: 6f75 7220 5b5f 5f63 6f6e 7472 6962 7574  our [__contribut
+000028c0: 696f 6e20 6775 6964 655f 5f5d 282e 2f43  ion guide__](./C
+000028d0: 4f4e 5452 4942 5554 494e 472e 6d64 292e  ONTRIBUTING.md).
+000028e0: 0a0a 2320 4163 6b6e 6f77 6c65 6467 656d  ..# Acknowledgem
+000028f0: 656e 7473 0a0a 5468 616e 6b20 796f 7520  ents..Thank you 
+00002900: 7665 7279 206d 7563 6820 746f 2074 6865  very much to the
+00002910: 2063 6f6d 6d75 6e69 7469 6573 2062 6568   communities beh
+00002920: 696e 6420 5b77 6562 332e 7079 5d28 6874  ind [web3.py](ht
+00002930: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00002940: 2f65 7468 6572 6575 6d2f 7765 6233 2e70  /ethereum/web3.p
+00002950: 7929 2061 6e64 2074 6865 205b 4170 6520  y) and the [Ape 
+00002960: 4672 616d 6577 6f72 6b5d 2868 7474 7073  Framework](https
+00002970: 3a2f 2f67 6974 6875 622e 636f 6d2f 4170  ://github.com/Ap
+00002980: 6557 6f72 582f 6170 6529 3a20 6077 6562  eWorX/ape): `web
+00002990: 3363 6c69 6020 776f 756c 6420 6e6f 7420  3cli` would not 
+000029a0: 6578 6973 7420 7769 7468 6f75 7420 796f  exist without yo
+000029b0: 7572 2065 6666 6f72 7473 210a            ur efforts!.
```

