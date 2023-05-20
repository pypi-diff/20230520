# Comparing `tmp/autumn8-1.0.5rc8.tar.gz` & `tmp/autumn8-1.0.5rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autumn8-1.0.5rc8.tar", last modified: Tue May 16 14:36:46 2023, max compression
+gzip compressed data, was "autumn8-1.0.5rc9.tar", last modified: Tue May 16 16:05:51 2023, max compression
```

## Comparing `autumn8-1.0.5rc8.tar` & `autumn8-1.0.5rc9.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 14:36:46.039531 autumn8-1.0.5rc8/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-05-16 14:36:46.039531 autumn8-1.0.5rc8/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4612 2023-05-16 11:19:52.000000 autumn8-1.0.5rc8/README.md
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 14:36:46.029531 autumn8-1.0.5rc8/autumn8/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.0.5rc8/autumn8/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 14:36:46.029531 autumn8-1.0.5rc8/autumn8/cli/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.5rc8/autumn8/cli/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.0.5rc8/autumn8/cli/__main__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7999 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/cli/analyze.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1202 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/cli/cli_environment.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 14:36:46.029531 autumn8-1.0.5rc8/autumn8/cli/commands/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    13527 2023-05-16 14:35:59.000000 autumn8-1.0.5rc8/autumn8/cli/commands/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    16114 2023-05-16 13:13:29.000000 autumn8-1.0.5rc8/autumn8/cli/commands/models.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.0.5rc8/autumn8/cli/examples.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5170 2023-05-16 14:28:29.000000 autumn8-1.0.5rc8/autumn8/cli/interactive.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2887 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/cli/main.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5315 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/cli/options.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3296 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/cli/pending_uploads.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2487 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/cli/validation.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 14:36:46.039531 autumn8-1.0.5rc8/autumn8/common/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      102 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/common/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-05-16 14:31:36.000000 autumn8-1.0.5rc8/autumn8/common/_version.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 14:36:46.039531 autumn8-1.0.5rc8/autumn8/common/config/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       50 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/common/config/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6861 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/common/config/cloud_info.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.0.5rc8/autumn8/common/config/settings.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    65887 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/common/config/supported_instances.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      565 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/common/types.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 14:36:46.039531 autumn8-1.0.5rc8/autumn8/env/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4876 2023-04-13 16:57:54.000000 autumn8-1.0.5rc8/autumn8/env/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      246 2023-04-13 17:40:25.000000 autumn8-1.0.5rc8/autumn8/env/app.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       65 2023-04-13 16:50:50.000000 autumn8-1.0.5rc8/autumn8/env/cli.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       10 2023-04-13 16:53:19.000000 autumn8-1.0.5rc8/autumn8/env/predictor.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       11 2023-04-13 16:54:28.000000 autumn8-1.0.5rc8/autumn8/env/worker.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 14:36:46.039531 autumn8-1.0.5rc8/autumn8/examples/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.0.5rc8/autumn8/examples/convblock.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.0.5rc8/autumn8/examples/loadMnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/examples/mnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/examples/model.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/examples/sbert-alpha.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/examples/tensorflow_custom_layers.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 14:36:46.039531 autumn8-1.0.5rc8/autumn8/lib/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/lib/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 14:36:46.039531 autumn8-1.0.5rc8/autumn8/lib/api/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       31 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/lib/api/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4067 2023-05-16 14:26:52.000000 autumn8-1.0.5rc8/autumn8/lib/api/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    11953 2023-05-16 13:55:08.000000 autumn8-1.0.5rc8/autumn8/lib/api/lab.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1348 2023-05-16 11:19:37.000000 autumn8-1.0.5rc8/autumn8/lib/api/user.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1517 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/lib/api_creds.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      614 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/lib/asyncio.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1020 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/lib/http.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1176 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/lib/logging.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/lib/logging.yaml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.0.5rc8/autumn8/lib/package_resolver.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3582 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/lib/service.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 14:36:46.039531 autumn8-1.0.5rc8/autumn8/types/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1112 2023-05-16 14:30:08.000000 autumn8-1.0.5rc8/autumn8/types/deployment.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 14:36:46.029531 autumn8-1.0.5rc8/autumn8.egg-info/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-05-16 14:36:46.000000 autumn8-1.0.5rc8/autumn8.egg-info/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1464 2023-05-16 14:36:46.000000 autumn8-1.0.5rc8/autumn8.egg-info/SOURCES.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-05-16 14:36:46.000000 autumn8-1.0.5rc8/autumn8.egg-info/dependency_links.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-05-16 14:36:46.000000 autumn8-1.0.5rc8/autumn8.egg-info/entry_points.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      136 2023-05-16 14:36:46.000000 autumn8-1.0.5rc8/autumn8.egg-info/requires.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-05-16 14:36:46.000000 autumn8-1.0.5rc8/autumn8.egg-info/top_level.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1985 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/pyproject.toml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-05-16 14:36:46.039531 autumn8-1.0.5rc8/setup.cfg
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/setup.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 14:36:46.039531 autumn8-1.0.5rc8/tests/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      969 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/tests/test_io_bottleneck_detection.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/tests/test_settings.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 16:05:51.120751 autumn8-1.0.5rc9/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-05-16 16:05:51.120751 autumn8-1.0.5rc9/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4612 2023-05-16 11:19:52.000000 autumn8-1.0.5rc9/README.md
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 16:05:51.100751 autumn8-1.0.5rc9/autumn8/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.0.5rc9/autumn8/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 16:05:51.110751 autumn8-1.0.5rc9/autumn8/cli/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.5rc9/autumn8/cli/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.0.5rc9/autumn8/cli/__main__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7999 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/cli/analyze.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1202 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/cli/cli_environment.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 16:05:51.110751 autumn8-1.0.5rc9/autumn8/cli/commands/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    13527 2023-05-16 14:35:59.000000 autumn8-1.0.5rc9/autumn8/cli/commands/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    16235 2023-05-16 16:03:09.000000 autumn8-1.0.5rc9/autumn8/cli/commands/models.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.0.5rc9/autumn8/cli/examples.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5170 2023-05-16 14:28:29.000000 autumn8-1.0.5rc9/autumn8/cli/interactive.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2887 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/cli/main.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5315 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/cli/options.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3296 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/cli/pending_uploads.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2487 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/cli/validation.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 16:05:51.110751 autumn8-1.0.5rc9/autumn8/common/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      102 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/common/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-05-16 16:04:29.000000 autumn8-1.0.5rc9/autumn8/common/_version.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 16:05:51.110751 autumn8-1.0.5rc9/autumn8/common/config/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       50 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/common/config/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6861 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/common/config/cloud_info.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.0.5rc9/autumn8/common/config/settings.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    65887 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/common/config/supported_instances.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      565 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/common/types.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 16:05:51.110751 autumn8-1.0.5rc9/autumn8/env/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4876 2023-04-13 16:57:54.000000 autumn8-1.0.5rc9/autumn8/env/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      246 2023-04-13 17:40:25.000000 autumn8-1.0.5rc9/autumn8/env/app.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       65 2023-04-13 16:50:50.000000 autumn8-1.0.5rc9/autumn8/env/cli.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       10 2023-04-13 16:53:19.000000 autumn8-1.0.5rc9/autumn8/env/predictor.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       11 2023-04-13 16:54:28.000000 autumn8-1.0.5rc9/autumn8/env/worker.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 16:05:51.120751 autumn8-1.0.5rc9/autumn8/examples/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.0.5rc9/autumn8/examples/convblock.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.0.5rc9/autumn8/examples/loadMnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/examples/mnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/examples/model.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/examples/sbert-alpha.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/examples/tensorflow_custom_layers.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      108 2023-05-16 16:01:30.000000 autumn8-1.0.5rc9/autumn8/exceptions.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 16:05:51.120751 autumn8-1.0.5rc9/autumn8/lib/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/lib/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 16:05:51.120751 autumn8-1.0.5rc9/autumn8/lib/api/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       31 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/lib/api/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4067 2023-05-16 14:26:52.000000 autumn8-1.0.5rc9/autumn8/lib/api/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    11953 2023-05-16 13:55:08.000000 autumn8-1.0.5rc9/autumn8/lib/api/lab.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1348 2023-05-16 11:19:37.000000 autumn8-1.0.5rc9/autumn8/lib/api/user.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1595 2023-05-16 16:01:57.000000 autumn8-1.0.5rc9/autumn8/lib/api_creds.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      614 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/lib/asyncio.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1020 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/lib/http.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1176 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/lib/logging.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/lib/logging.yaml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.0.5rc9/autumn8/lib/package_resolver.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3582 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/autumn8/lib/service.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 16:05:51.120751 autumn8-1.0.5rc9/autumn8/types/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1112 2023-05-16 14:30:08.000000 autumn8-1.0.5rc9/autumn8/types/deployment.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 16:05:51.100751 autumn8-1.0.5rc9/autumn8.egg-info/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-05-16 16:05:51.000000 autumn8-1.0.5rc9/autumn8.egg-info/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1486 2023-05-16 16:05:51.000000 autumn8-1.0.5rc9/autumn8.egg-info/SOURCES.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-05-16 16:05:51.000000 autumn8-1.0.5rc9/autumn8.egg-info/dependency_links.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-05-16 16:05:51.000000 autumn8-1.0.5rc9/autumn8.egg-info/entry_points.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      136 2023-05-16 16:05:51.000000 autumn8-1.0.5rc9/autumn8.egg-info/requires.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-05-16 16:05:51.000000 autumn8-1.0.5rc9/autumn8.egg-info/top_level.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1985 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/pyproject.toml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-05-16 16:05:51.120751 autumn8-1.0.5rc9/setup.cfg
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/setup.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 16:05:51.120751 autumn8-1.0.5rc9/tests/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      969 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/tests/test_io_bottleneck_detection.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-05-14 21:36:00.000000 autumn8-1.0.5rc9/tests/test_settings.py
```

### Comparing `autumn8-1.0.5rc8/PKG-INFO` & `autumn8-1.0.5rc9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.0.5rc8
+Version: 1.0.5rc9
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.0.5rc8/README.md` & `autumn8-1.0.5rc9/README.md`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/autumn8/cli/analyze.py` & `autumn8-1.0.5rc9/autumn8/cli/analyze.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/autumn8/cli/cli_environment.py` & `autumn8-1.0.5rc9/autumn8/cli/cli_environment.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/autumn8/cli/commands/cloud.py` & `autumn8-1.0.5rc9/autumn8/cli/commands/cloud.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/autumn8/cli/commands/models.py` & `autumn8-1.0.5rc9/autumn8/cli/commands/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,28 +17,30 @@
 from autumn8.cli.examples import example_model_names
 from autumn8.cli.interactive import (
     announce_model_upload_response,
     normalize_args,
 )
 from autumn8.cli.validation import validate_input_dims_json, validate_input_file
 from autumn8.common.config.settings import supported_quants
+from autumn8.exceptions import UserActionRequiredException
 from autumn8.lib import api, api_creds, logging
 from autumn8.lib import service as autodl
 
 USER_ID_LENGTH = len(str(uuid.uuid4()))
 API_KEY_LENGTH = 32
 
 logger = logging.getLogger(__name__)
 
 
 @click.group(context_settings={"token_normalize_func": normalize_args})
 def model_commands_group():
     pass
 
 
+# TODO: move to commands/user.py
 @model_commands_group.command()
 @options.use_environment
 @options.use_quiet_mode
 @click.option(
     "-u",
     "--user_id",
     help="The ID of the user that the CLI will authenticate as in AutoDL.",
@@ -56,15 +58,15 @@
     )
     try:
         old_user_id, _ = api_creds.retrieve_api_creds()
         if old_user_id not in ["", None]:
             logger.warning(
                 f"Replacing existing credentials for the user with id={old_user_id}"
             )
-    except (NoSectionError, NoOptionError):
+    except (NoSectionError, NoOptionError, UserActionRequiredException):
         pass
 
     # using unsafe_ask so that the script is properly aborted on ^C
     # (instead of questionary passing `None` as the user's prompt answer)
     if user_id is None or len(user_id) != USER_ID_LENGTH:
         user_id = questionary.text(
             "User ID",
```

### Comparing `autumn8-1.0.5rc8/autumn8/cli/examples.py` & `autumn8-1.0.5rc9/autumn8/cli/examples.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/autumn8/cli/interactive.py` & `autumn8-1.0.5rc9/autumn8/cli/interactive.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/autumn8/cli/main.py` & `autumn8-1.0.5rc9/autumn8/cli/main.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/autumn8/cli/options.py` & `autumn8-1.0.5rc9/autumn8/cli/options.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/autumn8/cli/pending_uploads.py` & `autumn8-1.0.5rc9/autumn8/cli/pending_uploads.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/autumn8/cli/validation.py` & `autumn8-1.0.5rc9/autumn8/cli/validation.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/autumn8/common/config/cloud_info.py` & `autumn8-1.0.5rc9/autumn8/common/config/cloud_info.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/autumn8/common/config/settings.py` & `autumn8-1.0.5rc9/autumn8/common/config/settings.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/autumn8/common/config/supported_instances.py` & `autumn8-1.0.5rc9/autumn8/common/config/supported_instances.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/autumn8/common/types.py` & `autumn8-1.0.5rc9/autumn8/common/types.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/autumn8/env/__init__.py` & `autumn8-1.0.5rc9/autumn8/env/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/autumn8/examples/mnist.py` & `autumn8-1.0.5rc9/autumn8/examples/mnist.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/autumn8/examples/model.py` & `autumn8-1.0.5rc9/autumn8/examples/model.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/autumn8/examples/sbert-alpha.py` & `autumn8-1.0.5rc9/autumn8/examples/sbert-alpha.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/autumn8/examples/tensorflow_custom_layers.py` & `autumn8-1.0.5rc9/autumn8/examples/tensorflow_custom_layers.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/autumn8/lib/__init__.py` & `autumn8-1.0.5rc9/autumn8/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/autumn8/lib/api/cloud.py` & `autumn8-1.0.5rc9/autumn8/lib/api/cloud.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/autumn8/lib/api/lab.py` & `autumn8-1.0.5rc9/autumn8/lib/api/lab.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/autumn8/lib/api/user.py` & `autumn8-1.0.5rc9/autumn8/lib/api/user.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/autumn8/lib/api_creds.py` & `autumn8-1.0.5rc9/autumn8/lib/api_creds.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import configparser
 import os
 from pathlib import Path
 
 import appdirs
 
+from autumn8.exceptions import UserActionRequiredException
+
 APP_NAME = "autumn8"
 APP_AUTHOR = "autumn8"
 
 
 def store_api_creds(user_id, api_key):
     app_config_dir = appdirs.user_config_dir(APP_NAME, APP_AUTHOR)
     app_config_path = os.path.join(app_config_dir, "autumn8.ini")
@@ -36,10 +38,10 @@
             config.add_section("api_access")
 
         user_id = config.get("api_access", "user_id")
         api_key = config.get("api_access", "api_key")
         return user_id, api_key
     # TODO: pick a more specific set of exceptions here
     except Exception as exc:
-        raise Exception(
+        raise UserActionRequiredException(
             f"API key is missing! To configure API access, please visit your profile page and generate an API key, then run `autumn8-cli login`"
         ) from exc
```

### Comparing `autumn8-1.0.5rc8/autumn8/lib/asyncio.py` & `autumn8-1.0.5rc9/autumn8/lib/asyncio.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/autumn8/lib/http.py` & `autumn8-1.0.5rc9/autumn8/lib/http.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/autumn8/lib/logging.py` & `autumn8-1.0.5rc9/autumn8/lib/logging.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/autumn8/lib/logging.yaml` & `autumn8-1.0.5rc9/autumn8/lib/logging.yaml`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/autumn8/lib/package_resolver.py` & `autumn8-1.0.5rc9/autumn8/lib/package_resolver.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/autumn8/lib/service.py` & `autumn8-1.0.5rc9/autumn8/lib/service.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/autumn8/types/deployment.py` & `autumn8-1.0.5rc9/autumn8/types/deployment.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/autumn8.egg-info/PKG-INFO` & `autumn8-1.0.5rc9/autumn8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.0.5rc8
+Version: 1.0.5rc9
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.0.5rc8/autumn8.egg-info/SOURCES.txt` & `autumn8-1.0.5rc9/autumn8.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 README.md
 pyproject.toml
 setup.py
 autumn8/__init__.py
+autumn8/exceptions.py
 autumn8.egg-info/PKG-INFO
 autumn8.egg-info/SOURCES.txt
 autumn8.egg-info/dependency_links.txt
 autumn8.egg-info/entry_points.txt
 autumn8.egg-info/requires.txt
 autumn8.egg-info/top_level.txt
 autumn8/cli/__init__.py
```

### Comparing `autumn8-1.0.5rc8/pyproject.toml` & `autumn8-1.0.5rc9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/tests/test_io_bottleneck_detection.py` & `autumn8-1.0.5rc9/tests/test_io_bottleneck_detection.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc8/tests/test_settings.py` & `autumn8-1.0.5rc9/tests/test_settings.py`

 * *Files identical despite different names*

