# Comparing `tmp/pyalarmdotcomajax-0.5.0b3.tar.gz` & `tmp/pyalarmdotcomajax-0.5.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalarmdotcomajax-0.5.0b3.tar", last modified: Thu May 18 17:22:36 2023, max compression
+gzip compressed data, was "pyalarmdotcomajax-0.5.0b4.tar", last modified: Sat May 20 18:25:04 2023, max compression
```

## Comparing `pyalarmdotcomajax-0.5.0b3.tar` & `pyalarmdotcomajax-0.5.0b4.tar`

### file list

```diff
@@ -1,62 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:22:36.594361 pyalarmdotcomajax-0.5.0b3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17973 2023-05-18 17:22:36.594361 pyalarmdotcomajax-0.5.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15945 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:22:36.590360 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/
--rw-r--r--   0 runner    (1001) docker     (123)    40766 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20083 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:22:36.594361 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/garage_door.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/image_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)    14474 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/thermostat.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/water_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    23212 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:22:36.594361 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:22:36.594361 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/garage_door.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/thermostat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/water_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/ws.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:22:36.590360 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17973 2023-05-18 17:22:36.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-18 17:22:36.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 17:22:36.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-18 17:22:36.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-18 17:22:36.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-18 17:22:36.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 17:22:36.000000 pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-18 17:22:36.598361 pyalarmdotcomajax-0.5.0b3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:22:36.594361 pyalarmdotcomajax-0.5.0b3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:22:36.594361 pyalarmdotcomajax-0.5.0b3/tests/responses/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/tests/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/tests/test_device_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/tests/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/tests/test_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-18 17:22:23.000000 pyalarmdotcomajax-0.5.0b3/tests/test_thermostat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:25:04.517009 pyalarmdotcomajax-0.5.0b4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17973 2023-05-20 18:25:04.517009 pyalarmdotcomajax-0.5.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15945 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:25:04.501009 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/
+-rw-r--r--   0 runner    (1001) docker     (123)    41492 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20518 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:25:04.509009 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/garage_door.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/image_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14474 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/water_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23212 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:25:04.509009 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:25:04.513009 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/garage_door.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/water_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:25:04.505009 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17973 2023-05-20 18:25:04.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-20 18:25:04.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 18:25:04.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-20 18:25:04.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-20 18:25:04.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-20 18:25:04.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 18:25:04.000000 pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-20 18:25:04.517009 pyalarmdotcomajax-0.5.0b4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:25:04.513009 pyalarmdotcomajax-0.5.0b4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:25:04.517009 pyalarmdotcomajax-0.5.0b4/tests/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/tests/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/tests/test_device_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/tests/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/tests/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-20 18:24:53.000000 pyalarmdotcomajax-0.5.0b4/tests/test_thermostat.py
```

### Comparing `pyalarmdotcomajax-0.5.0b3/LICENSE` & `pyalarmdotcomajax-0.5.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/PKG-INFO` & `pyalarmdotcomajax-0.5.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalarmdotcomajax
-Version: 0.5.0b3
+Version: 0.5.0b4
 Summary: Python Interface for Alarm.com
 Home-page: https://github.com/pyalarmdotcom/pyalarmdotcomajax
 Author: Justin Wong
 Author-email: 46082645+uvjustin@users.noreply.github.com
 Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com, 466460+elahd@users.noreply.github.com
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.0b3 Summary: Python
+Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.0b4 Summary: Python
 Interface for Alarm.com Home-page: https://github.com/pyalarmdotcom/
 pyalarmdotcomajax Author: Justin Wong Author-email:
 46082645+uvjustin@users.noreply.github.com Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com,
 466460+elahd@users.noreply.github.com License: MIT Keywords: Alarm.com,Security
 System,Home Assistant Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English Classifier: Environment :: Web
```

### Comparing `pyalarmdotcomajax-0.5.0b3/README.md` & `pyalarmdotcomajax-0.5.0b4/README.md`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/__init__.py` & `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import annotations
 
 import asyncio
 import contextlib
 import json
 import logging
 import re
-from collections.abc import Awaitable
+from collections.abc import Callable
 from datetime import datetime
 from enum import Enum
 from typing import TypedDict
 
 import aiohttp
 from bs4 import BeautifulSoup
 
@@ -38,20 +38,20 @@
 )
 from pyalarmdotcomajax.extensions import (
     CameraSkybellControllerExtension,
     ConfigurationOption,
     ControllerExtensions_t,
     ExtendedProperties,
 )
-from pyalarmdotcomajax.websockets.client import WebSocketClient
+from pyalarmdotcomajax.websockets.client import WebSocketClient, WebSocketState
 
 # TODO: Use error handler and exception handlers in _async_get_system_devices on other request functions.
 # TODO: Fix get raw server response function.
 
-__version__ = "0.5.0-beta.3"
+__version__ = "0.5.0-beta.4"
 
 log = logging.getLogger(__name__)
 
 
 class ExtensionResults(TypedDict):
     """Results of multi-device extension calls."""
 
@@ -59,19 +59,20 @@
     controller: ControllerExtensions_t
 
 
 class OtpType(Enum):
     """Alarm.com two factor authentication type."""
 
     # https://www.alarm.com/web/system/assets/customer-ember/enums/TwoFactorAuthenticationType.js
+    # Keep these lowercase. Strings.json in Home Assistant requires lowercase values.
 
-    DISABLED = 0
-    APP = 1
-    SMS = 2
-    EMAIL = 4
+    disabled = 0
+    app = 1
+    sms = 2
+    email = 4
 
 
 class AlarmController:
     """Base class for communicating with Alarm.com via API."""
 
     AJAX_HEADERS_TEMPLATE = {
         "Accept": "application/vnd.api+json",
@@ -113,15 +114,14 @@
 
     def __init__(
         self,
         username: str,
         password: str,
         websession: aiohttp.ClientSession,
         twofactorcookie: str | None = None,
-        notify_on_update_callback: Awaitable | None = None,
     ):
         """Manage access to Alarm.com API and builds devices."""
 
         #
         # SET
         #
         self._username: str = username
@@ -134,15 +134,17 @@
         #
 
         self._provider_name: str | None = None
         self._user_id: str | None = None
         self._user_email: str | None = None
         self._active_system_id: str | None = None
         self._ajax_headers: dict = self.AJAX_HEADERS_TEMPLATE
-        self.notify_on_update_callback: Awaitable | None = notify_on_update_callback
+
+        self._ws_state_callback: Callable[[WebSocketState], None] | None = None
+        self._websocket: WebSocketClient | None = None
 
         self._partition_map: dict = (
             {}
         )  # Individual devices don't list their associated partitions. This map is used to retrieve partition id when each device is created.
 
         self._installed_device_types: set[DeviceType] = (
             set()
@@ -197,14 +199,206 @@
     #
     ####################
     # PUBLIC FUNCTIONS #
     ####################
     #
     #
 
+    async def async_update(self) -> None:  # noqa: C901
+        """Fetch latest device data."""
+
+        log.debug("Calling update on Alarm.com")
+
+        has_image_sensors: bool = False
+
+        if not self._active_system_id:
+            self._active_system_id = await self._async_get_active_system()
+            has_image_sensors = await self._async_has_image_sensors(self._active_system_id)
+
+        with contextlib.suppress(DataFetchFailed, UnexpectedDataStructure):
+            await self._async_get_trouble_conditions()
+
+        #
+        # GET CORE DEVICE ATTRIBUTES
+        #
+
+        device_instances: dict[str, AllDevices_t] = {}
+        raw_devices: list[dict] = await self._async_get_system(self._active_system_id)
+        raw_devices.extend(await self._async_get_system_devices(self._active_system_id))
+
+        #
+        # QUERY MULTI-DEVICE EXTENSIONS
+        #
+
+        extension_results = await self._async_update__query_multi_device_extensions(raw_devices)
+
+        #
+        # QUERY IMAGE SENSORS
+        #
+        # Detailed image sensors data is not included in the main device catalog. It must be queried separately.
+        #
+        # TODO: Convert image sensors images to device extension. Merge entity_specific_data and settings; eliminate "additional endpoints" concept. Maybe push processing/placement into specific device class.
+
+        device_type_specific_data = {}
+
+        if has_image_sensors:
+            # Get detailed image sensor data and add to raw device list.
+            image_sensors = await self._async_get_devices_by_device_type(DeviceType.IMAGE_SENSOR)
+            raw_devices.extend(image_sensors)
+
+            # Get recent images
+            device_type_specific_data = await self._async_get_recent_images()
+
+        #
+        # BUILD PARTITIONS
+        #
+
+        # Ensure that partition map is built before devices are built.
+
+        for device in [
+            device
+            for device in raw_devices
+            if device["type"] == AttributeRegistry.get_relationship_id_from_devicetype(DeviceType.PARTITION)
+        ]:
+            partition_instance: AllDevices_t = await self._async_update__build_device(
+                device, device_type_specific_data, extension_results
+            )
+
+            for child, _ in partition_instance.children:
+                self._partition_map[child] = partition_instance.id_
+
+            device_instances.update({partition_instance.id_: partition_instance})
+
+            raw_devices.remove(device)
+
+            #
+            # BUILD ALL DEVICES IN PARTITION
+            #
+            # This ensures that partition map is built before devices are built.
+
+            for device in raw_devices:
+                try:
+                    device_instance: AllDevices_t = await self._async_update__build_device(
+                        device, device_type_specific_data, extension_results
+                    )
+
+                    device_instances.update({device_instance.id_: device_instance})
+
+                except UnsupportedDevice:
+                    continue
+
+        self.devices.update(device_instances, purge=True)
+
+    async def async_send_command(
+        self,
+        device_type: DeviceType,
+        event: BaseDevice.Command,
+        device_id: str | None = None,  # ID corresponds to device_type
+        msg_body: dict = {},  # Body of request. No abstractions here.
+        retry_on_failure: bool = True,  # Set to prevent infinite loops when function calls itself
+    ) -> bool:
+        """Send commands to Alarm.com."""
+        log.info("Sending %s to Alarm.com.", event)
+
+        msg_body["statePollOnly"] = False
+
+        try:
+            url = (
+                f"{AttributeRegistry.get_endpoints(device_type)['primary'].format(c.URL_BASE, device_id)}/{event.value}"
+            )
+        except KeyError as err:
+            raise UnsupportedDevice from err
+
+        log.debug("Url %s", url)
+
+        async with self._websession.post(url=url, json=msg_body, headers=self._ajax_headers) as resp:
+            log.debug("Response from Alarm.com %s", resp.status)
+
+            match str(resp.status):
+                case "200":
+                    # Update entities after calling state change.
+                    # TODO: Confirm that we can remove this call because of webhook support.
+                    # await self.async_update()
+                    return True
+
+                case "423":
+                    # User has read-only permission to the entity.
+                    err_msg = (
+                        f"{__name__}: User {self.user_email} has read-only access to"
+                        f" {device_type.name.lower()} {device_id}."
+                    )
+                    raise PermissionError(err_msg)
+
+                case "422":
+                    if isinstance(event, Partition.Command) and (msg_body.get("forceBypass") is True):
+                        # 422 sometimes occurs when forceBypass is True but there's nothing to bypass.
+                        log.debug(
+                            "Error executing %s, trying again without force bypass...",
+                            event.value,
+                        )
+
+                        # Not changing retry_on_failure. Changing forcebypass means that we won't re-enter this block.
+
+                        msg_body["forceBypass"] = False
+
+                        return await self.async_send_command(
+                            device_type=device_type,
+                            event=event,
+                            device_id=device_id,
+                            msg_body=msg_body,
+                        )
+
+                case "403":
+                    # May have been logged out, try again
+                    log.warning(
+                        "Error executing %s, NOT logging in and trying again...",
+                        event.value,
+                    )
+
+                    return False
+                    # if retry_on_failure:
+                    #     await self.async_login()
+                    #     return await self.async_send_command(
+                    #         device_type,
+                    #         event,
+                    #         device_id,
+                    #         msg_body,
+                    #         False,
+                    #     )
+
+        log.error(
+            f"{event.value} failed with HTTP code {resp.status}. URL: {url}\nJSON: {msg_body}\nHeaders:"
+            f" {self._ajax_headers}"
+        )
+        raise ConnectionError
+
+    #
+    # WEBSOCKET FUNCTIONS
+    #
+
+    def start_websocket(self, ws_state_callback: Callable[[WebSocketState], None] | None = None) -> None:
+        """Construct and return a websocket client."""
+
+        self._ws_state_callback = ws_state_callback
+
+        self._websocket = WebSocketClient(
+            self._websession, self._ajax_headers, self.devices, self._ws_state_callback
+        )
+        self._websocket.start()
+
+    def stop_websocket(self) -> None:
+        """Close websession and websocket to UniFi."""
+        log.info("Closing WebSocket connection.")
+        if self._websocket:
+            self._websocket.stop()
+
+    #
+    # AUTHENTICATION FUNCTIONS
+    #
+
     async def async_login(
         self,
     ) -> None:
         """Login to Alarm.com."""
         log.debug("Attempting to log in to Alarm.com")
 
         # TODO: Prevent login from making a ton of saved devices in ADC.
@@ -217,14 +411,16 @@
             if not self._two_factor_cookie:
                 async with self._websession.get(
                     url=AttributeRegistry.get_endpoints(DeviceType.SYSTEM)["primary"].format(c.URL_BASE, ""),
                     headers=self._ajax_headers,
                 ) as resp:
                     json_rsp = await resp.json()
 
+                    log.debug(f"Response from Alarm.com login: {resp.status} {resp.json()}")
+
                 for error in (errors := json_rsp.get("errors", {})):
                     if error.get("status") == "409" and error.get("detail") == "TwoFactorAuthenticationRequired":
                         log.debug("Two factor authentication code or cookie required.")
                         raise TwoFactor_OtpRequired
 
         except (DataFetchFailed, UnexpectedDataStructure) as err:
             raise ConnectionError from err
@@ -250,23 +446,23 @@
             ]
             log.info(f"Requires two-factor authentication. Enabled methods are {enabled_2fa_methods}")
             return enabled_2fa_methods
 
     async def async_request_otp(self, method: OtpType | None) -> None:
         """Request SMS/email OTP code from Alarm.com."""
 
-        if method not in (OtpType.EMAIL, OtpType.SMS):
+        if method not in (OtpType.email, OtpType.sms):
             return None
 
         try:
             log.debug("Requesting OTP code...")
 
             request_url = (
                 self.LOGIN_2FA_REQUEST_OTP_EMAIL_URL_TEMPLATE
-                if method == OtpType.EMAIL
+                if method == OtpType.email
                 else self.LOGIN_2FA_REQUEST_OTP_SMS_URL_TEMPLATE
             )
 
             async with self._websession.post(
                 url=request_url.format(c.URL_BASE, self._user_id),
                 headers=self._ajax_headers,
             ) as resp:
@@ -342,98 +538,32 @@
                 log.debug("Found two-factor authentication cookie: %s", cookie.value)
                 self._two_factor_cookie = {"twoFactorAuthenticationId": cookie.value} if cookie.value else {}
                 return str(cookie.value)
 
         log.error("Failed to find two-factor authentication cookie.")
         return None
 
-    async def async_update(self) -> None:  # noqa: C901
-        """Fetch latest device data."""
-
-        log.debug("Calling update on Alarm.com")
-
-        has_image_sensors: bool = False
-
-        if not self._active_system_id:
-            self._active_system_id = await self._async_get_active_system()
-            has_image_sensors = await self._async_has_image_sensors(self._active_system_id)
-
-        with contextlib.suppress(DataFetchFailed, UnexpectedDataStructure):
-            await self._async_get_trouble_conditions()
-
-        #
-        # GET CORE DEVICE ATTRIBUTES
-        #
-
-        device_instances: dict[str, AllDevices_t] = {}
-        raw_devices: list[dict] = await self._async_get_system(self._active_system_id)
-        raw_devices.extend(await self._async_get_system_devices(self._active_system_id))
-
-        #
-        # QUERY MULTI-DEVICE EXTENSIONS
-        #
-
-        extension_results = await self._async_update__query_multi_device_extensions(raw_devices)
-
-        #
-        # QUERY IMAGE SENSORS
-        #
-        # Detailed image sensors data is not included in the main device catalog. It must be queried separately.
-        #
-        # TODO: Convert image sensors images to device extension. Merge entity_specific_data and settings; eliminate "additional endpoints" concept. Maybe push processing/placement into specific device class.
-
-        device_type_specific_data = {}
-
-        if has_image_sensors:
-            # Get detailed image sensor data and add to raw device list.
-            image_sensors = await self._async_get_devices_by_device_type(DeviceType.IMAGE_SENSOR)
-            raw_devices.extend(image_sensors)
-
-            # Get recent images
-            device_type_specific_data = await self._async_get_recent_images()
-
-        #
-        # BUILD PARTITIONS
-        #
-
-        # Ensure that partition map is built before devices are built.
-
-        for device in [
-            device
-            for device in raw_devices
-            if device["type"] == AttributeRegistry.get_relationship_id_from_devicetype(DeviceType.PARTITION)
-        ]:
-            partition_instance: AllDevices_t = await self._async_update__build_device(
-                device, device_type_specific_data, extension_results
-            )
-
-            for child, _ in partition_instance.children:
-                self._partition_map[child] = partition_instance.id_
-
-            device_instances.update({partition_instance.id_: partition_instance})
-
-            raw_devices.remove(device)
-
-            #
-            # BUILD ALL DEVICES IN PARTITION
-            #
-            # This ensures that partition map is built before devices are built.
-
-            for device in raw_devices:
-                try:
-                    device_instance: AllDevices_t = await self._async_update__build_device(
-                        device, device_type_specific_data, extension_results
-                    )
+    #
+    #
+    #####################
+    # PRIVATE FUNCTIONS #
+    #####################
+    #
+    # Communicate directly with the ADC API
 
-                    device_instances.update({device_instance.id_: device_instance})
+    async def _async_keep_alive_login_check(self) -> bool:
+        """Check if we are logged in."""
 
-                except UnsupportedDevice:
-                    continue
+        async with self._websession.get(
+            url=self.KEEP_ALIVE_CHECK_URL_TEMPLATE.format(c.URL_BASE, int(round(datetime.now().timestamp()))),
+            headers=self._ajax_headers,
+        ) as resp:
+            text_rsp = await resp.text()
 
-        self.devices.update(device_instances, purge=True)
+        return bool(text_rsp == self.KEEP_ALIVE_CHECK_RESPONSE)
 
     async def _async_update__build_device(
         self,
         raw_device: dict,
         device_type_specific_data: dict[str, DeviceTypeSpecificData],
         extension_results: dict[str, ExtensionResults],
     ) -> AllDevices_t:
@@ -561,119 +691,14 @@
                     results[device_id] = {
                         "settings": device_properties.settings,
                         "controller": extension_controller,
                     }
 
         return results
 
-    async def async_send_command(
-        self,
-        device_type: DeviceType,
-        event: BaseDevice.Command,
-        device_id: str | None = None,  # ID corresponds to device_type
-        msg_body: dict = {},  # Body of request. No abstractions here.
-        retry_on_failure: bool = True,  # Set to prevent infinite loops when function calls itself
-    ) -> bool:
-        """Send commands to Alarm.com."""
-        log.info("Sending %s to Alarm.com.", event)
-
-        msg_body["statePollOnly"] = False
-
-        try:
-            url = (
-                f"{AttributeRegistry.get_endpoints(device_type)['primary'].format(c.URL_BASE, device_id)}/{event.value}"
-            )
-        except KeyError as err:
-            raise UnsupportedDevice from err
-
-        log.debug("Url %s", url)
-
-        async with self._websession.post(url=url, json=msg_body, headers=self._ajax_headers) as resp:
-            log.debug("Response from Alarm.com %s", resp.status)
-
-            match str(resp.status):
-                case "200":
-                    # Update entities after calling state change.
-                    # TODO: Confirm that we can remove this call because of webhook support.
-                    # await self.async_update()
-                    return True
-
-                case "423":
-                    # User has read-only permission to the entity.
-                    err_msg = (
-                        f"{__name__}: User {self.user_email} has read-only access to"
-                        f" {device_type.name.lower()} {device_id}."
-                    )
-                    raise PermissionError(err_msg)
-
-                case "422":
-                    if isinstance(event, Partition.Command) and (msg_body.get("forceBypass") is True):
-                        # 422 sometimes occurs when forceBypass is True but there's nothing to bypass.
-                        log.debug(
-                            "Error executing %s, trying again without force bypass...",
-                            event.value,
-                        )
-
-                        # Not changing retry_on_failure. Changing forcebypass means that we won't re-enter this block.
-
-                        msg_body["forceBypass"] = False
-
-                        return await self.async_send_command(
-                            device_type=device_type,
-                            event=event,
-                            device_id=device_id,
-                            msg_body=msg_body,
-                        )
-
-                case "403":
-                    # May have been logged out, try again
-                    log.warning(
-                        "Error executing %s, logging in and trying again...",
-                        event.value,
-                    )
-                    if retry_on_failure:
-                        await self.async_login()
-                        return await self.async_send_command(
-                            device_type,
-                            event,
-                            device_id,
-                            msg_body,
-                            False,
-                        )
-
-        log.error(
-            f"{event.value} failed with HTTP code {resp.status}. URL: {url}\nJSON: {msg_body}\nHeaders:"
-            f" {self._ajax_headers}"
-        )
-        raise ConnectionError
-
-    def get_websocket_client(self) -> WebSocketClient:
-        """Construct and return a websocket client."""
-
-        return WebSocketClient(self._websession, self._ajax_headers, self.devices)
-
-    async def _async_keep_alive_login_check(self) -> bool:
-        """Check if we are logged in."""
-
-        async with self._websession.get(
-            url=self.KEEP_ALIVE_CHECK_URL_TEMPLATE.format(c.URL_BASE, int(round(datetime.now().timestamp()))),
-            headers=self._ajax_headers,
-        ) as resp:
-            text_rsp = await resp.text()
-
-        return bool(text_rsp == self.KEEP_ALIVE_CHECK_RESPONSE)
-
-    #
-    #
-    #####################
-    # PRIVATE FUNCTIONS #
-    #####################
-    #
-    # Communicate directly with the ADC API
-
     async def _async_get_active_system(self) -> str:
         """Get active system for user account."""
 
         try:
             log.info("Getting active system.")
 
             async with self._websession.get(
```

### Comparing `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/cli.py` & `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     InvalidConfigurationOption,
     TwoFactor_ConfigurationRequired,
     TwoFactor_OtpRequired,
     UnexpectedDataStructure,
 )
 from .extensions import ConfigurationOption
 from .helpers import ExtendedEnumMixin, slug_to_title
+from .websockets.client import WebSocketState
 
 CLI_CARD_BREAK = ""  # "--------"
 
 
 async def cli() -> None:
     """Support CLI development and testing. Not used in normal library operation."""
 
@@ -408,16 +409,32 @@
 # FUNCTIONS #
 #############
 
 
 async def _async_stream_realtime(alarm: AlarmController) -> None:
     """Stream real-time updates via WebSockets."""
 
-    ws_client = alarm.get_websocket_client()
-    await ws_client.async_connect()
+    def ws_state_handler(state: WebSocketState) -> None:
+        """Handle websocket connection state changes."""
+
+        print(f"Websocket state changed to: {state.name}")
+
+    alarm.start_websocket(ws_state_handler)
+
+    try:
+        # Keep event loop alive until cancelled.
+        while True:
+            await asyncio.sleep(1)
+
+    except asyncio.CancelledError:
+        pass
+
+    finally:
+        # Close connection when cancelled.
+        alarm.stop_websocket()
 
 
 def _human_output(alarm: AlarmController) -> dict:
     """Output user-friendly list of devices and statuses."""
 
     output = {}
 
@@ -527,15 +544,15 @@
     # Determine which OTP method to use
     #
 
     code: str | None
     selected_otp_method: OtpType
     if code := args.get("one_time_password"):
         # If an OTP is provided directly in the CLI, it's from an OTP app.
-        selected_otp_method = OtpType.APP
+        selected_otp_method = OtpType.app
     else:
         cprint(
             "Two factor authentication is enabled for this user.",
             attrs=["bold"],
         )
 
         # Get list of enabled OTP methods.
@@ -560,15 +577,15 @@
                 cprint("Valid OTP method was not entered.", "red")
                 sys.exit()
 
         #
         # Request OTP
         #
 
-        if selected_otp_method in (OtpType.EMAIL, OtpType.SMS):
+        if selected_otp_method in (OtpType.email, OtpType.sms):
             # Ask Alarm.com to send OTP if selected method is EMAIL or SMS.
             cprint(f"Requesting One-Time Password via {selected_otp_method.name}...")
             await alarm.async_request_otp(selected_otp_method)
 
     #
     # Prompt user for OTP
     #
@@ -595,15 +612,15 @@
         # Ensure an Enum subclass is provided
         if enum_type is None:
             raise ValueError("type must be assigned an Enum when using EnumAction")
         if not issubclass(enum_type, Enum):
             raise TypeError("type must be an Enum when using EnumAction")
 
         # Generate choices from the Enum
-        kwargs.setdefault("choices", tuple(e.name for e in enum_type if e != OtpType.DISABLED))
+        kwargs.setdefault("choices", tuple(e.name for e in enum_type if e != OtpType.disabled))
 
         super().__init__(**kwargs)
 
         self._enum = enum_type
 
     def __call__(
         self,
```

### Comparing `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/__init__.py` & `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,15 +86,14 @@
         config_change_callback: Callable | None,
         children: list[tuple[str, DeviceType]],
         raw_device_data: dict,
         device_type_specific_data: DeviceTypeSpecificData | None = None,
         trouble_conditions: list | None = None,
         partition_id: str | None = None,
         settings: dict | None = None,  # slug: ConfigurationOption
-        external_update_callback: Callable | None = None,  # Called when device is updated via WebSockets.
     ) -> None:
         """Initialize base element class."""
 
         self._id_: str = id_
         self._family_raw: str | None = raw_device_data.get("type")
         self._attribs_raw: dict = raw_device_data.get("attributes", {})
         self._device_type_specific_data: DeviceTypeSpecificData = (
@@ -107,15 +106,16 @@
         self.children = children
         self.trouble_conditions: list[TroubleCondition] = trouble_conditions if trouble_conditions else []
 
         self._system_id: str | None = (
             raw_device_data.get("relationships", {}).get("system", {}).get("data", {}).get("id")
         )
         self._partition_id: str | None = partition_id
-        self.external_update_callback: Callable | None = external_update_callback
+
+        self.external_update_callback: list[Callable] = []
 
         self.process_device_type_specific_data()
 
         log.debug("Initialized %s %s", self._family_raw, self.name)
 
     #
     # Properties
@@ -141,14 +141,20 @@
     @property
     def name(self) -> None | str:
         """Return user-assigned device name."""
 
         return self._attribs_raw.get("description", None)
 
     @property
+    def attribs_raw(self) -> None | dict:
+        """Return raw attributes."""
+
+        return self._attribs_raw
+
+    @property
     def has_state(self) -> bool:
         """Return whether entity reports state."""
         return self._attribs_raw.get("hasState", False)
 
     @property
     def state(self) -> Enum | None:
         """Return state."""
@@ -239,42 +245,42 @@
     async def async_handle_external_state_change(self, raw_state: int) -> None:
         """Update device state when notified of externally-triggered change."""
 
         self._attribs_raw[self._ATTRIB_STATE] = raw_state
 
         log.info(f"{__name__} Got async update for {self.name} ({self.id_}) with new state: {self.state}.")
 
-        if self.external_update_callback:
-            self.external_update_callback
+        for external_callback in self.external_update_callback:
+            external_callback()
 
     async def async_handle_external_attribute_change(self, new_attribute: dict) -> None:
         """Update device attribute when notified of externally-triggered change."""
 
         self._attribs_raw.update(new_attribute)
 
-        if self.external_update_callback:
-            self.external_update_callback
+        for external_callback in self.external_update_callback:
+            external_callback()
 
     async def async_log_new_attribute(self, attribute_name: str, attribute_value: Any) -> None:
         """Log externally-triggered attribute change."""
 
         log.info(
             f"{__name__} Got async update for {self.name} ({self.id_}) with new {attribute_name}:"
             f" {attribute_value}."
         )
 
     def register_external_update_callback(self, callback: Callable) -> None:
         """Register callback to be called when device state changes."""
 
-        self.external_update_callback = callback
+        self.external_update_callback.append(callback)
 
-    def unregister_external_update_callback(self) -> None:
+    def unregister_external_update_callback(self, callback: Callable) -> None:
         """Unregister callback to be called when device state changes."""
 
-        self.external_update_callback = None
+        self.external_update_callback.remove(callback)
 
     # #
     # PLACEHOLDERS
     # #
 
     # All subclasses will have above functions. Only some will have the below and must be implemented as overloads.
     # Methods below are included here to silence mypy errors.
```

### Comparing `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/garage_door.py` & `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/garage_door.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/gate.py` & `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/gate.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/image_sensor.py` & `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/image_sensor.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/light.py` & `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/light.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/lock.py` & `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/lock.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/partition.py` & `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/partition.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/registry.py` & `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/registry.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/sensor.py` & `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/sensor.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/system.py` & `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/system.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/devices/thermostat.py` & `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/devices/thermostat.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         self,
         state: DeviceState | None = None,
         fan: tuple[FanMode, int] | None = None,  # int = duration
         cool_setpoint: float | None = None,
         heat_setpoint: float | None = None,
         schedule_mode: ScheduleMode | None = None,
     ) -> None:
-        """Send turn on command with optional brightness."""
+        """Send command to HVAC unit."""
 
         msg_body: dict[str, float | int] = {}
 
         # Make sure we're only being asked to set one attribute at a time.
         if (attrib_list := [state, fan, cool_setpoint, heat_setpoint, schedule_mode]).count(None) < len(
             attrib_list
         ) - 1:
```

### Comparing `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/errors.py` & `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/errors.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/extensions.py` & `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/extensions.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/helpers.py` & `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/helpers.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/client.py` & `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Functions for communicating with Alarm.com over WebSockets."""
 
 # noqa: T201
 
 from __future__ import annotations
 
+import asyncio
 import json
 import logging
+from collections.abc import Callable
 from enum import Enum
 
 import aiohttp
 from aiohttp import ClientSession
 
 from pyalarmdotcomajax import const as c
 from pyalarmdotcomajax.devices.garage_door import GarageDoor
@@ -34,14 +36,23 @@
     MonitoringEventMessage,
     process_raw_message,
 )
 
 log = logging.getLogger(__name__)
 
 
+class WebSocketState(Enum):
+    """Websocket state."""
+
+    DISCONNECTED = "disconnected"
+    RUNNING = "running"
+    STARTING = "starting"
+    STOPPED = "stopped"
+
+
 class WebSocketCloseCodes(Enum):
     """Enum for codes given by server on disconnect or reject."""
 
     Normal = 1000
     ServiceUnavailable = 1001
     TokenExpired = 1008
 
@@ -53,46 +64,105 @@
     WEBSOCKET_TOKEN_REQUEST_TEMPLATE = "{}web/api/websockets/token"  # noqa: S105
 
     def __init__(
         self,
         websession: ClientSession,
         ajax_headers: dict,
         device_registry: DeviceRegistry,
+        ws_state_callback: Callable[[WebSocketState], None] | None = None,
     ) -> None:
         """Initialize."""
         self._websession: ClientSession = websession
         self._ajax_headers: dict = ajax_headers
         self._device_registry: DeviceRegistry = device_registry
         self._ws_auth_token: str | None = None
+        self._ws_connection: aiohttp.ClientWebSocketResponse | None = None
+        self._state = WebSocketState.STOPPED
+        self._ws_state_callback = ws_state_callback
+        self._loop = asyncio.get_running_loop()
+
+    @property
+    def state(self) -> WebSocketState:
+        """State of websocket."""
+        return self._state
+
+    @state.setter
+    def state(self, value: WebSocketState) -> None:
+        """Set state of websocket."""
+        self._state = value
+        log.debug("Websocket %s", value)
 
-    async def async_connect(self) -> None:
+        if self._ws_state_callback:
+            self._ws_state_callback(value)
+
+    async def _connect(self) -> None:
         """Connect to Alarm.com WebSocket."""
 
         # Get authentication token for websocket communication
         try:
             self._ws_auth_token = await self._async_get_websocket_token()
             if not self._ws_auth_token:
                 raise AuthenticationFailed("async_connect(): Failed to get WebSocket authentication token.")
         except (DataFetchFailed, AuthenticationFailed) as err:
             raise AuthenticationFailed from err
 
-        # Connect to websocket endpoint
-        async with self._websession.ws_connect(
-            self.WEBSOCKET_ENDPOINT_TEMPLATE.format(self._ws_auth_token), headers=self._ajax_headers, timeout=30
-        ) as websocket:
-            async for msg in websocket:
-                # Message is JSON but encoded as text.
-                if msg.type != aiohttp.WSMsgType.TEXT:
-                    pass
-
-                try:
-                    await self._async_handle_message(json.loads(msg.data))
-                except (TypeError, ValueError):
-                    log.warning("Unable to parse message from Alarm.com: %s", msg.data)
-                    # TODO: On failure, refresh everything synchronous HTTP endpoints.
+        try:
+            # Connect to websocket endpoint
+            async with self._websession.ws_connect(
+                self.WEBSOCKET_ENDPOINT_TEMPLATE.format(self._ws_auth_token),
+                headers=self._ajax_headers,
+                timeout=30,
+            ) as websocket:
+                self.state = WebSocketState.RUNNING
+
+                async for msg in websocket:
+                    if self.state == WebSocketState.STOPPED:
+                        break
+
+                    # Message is JSON but encoded as text.
+                    if msg.type != aiohttp.WSMsgType.TEXT:
+                        pass
+                    elif msg.type == aiohttp.WSMsgType.CLOSED:
+                        log.warning("AIOHTTP websocket connection closed")
+                        break
+
+                    elif msg.type == aiohttp.WSMsgType.ERROR:
+                        log.error("AIOHTTP websocket error: '%s'", msg.data)
+                        break
+
+                    try:
+                        await self._async_handle_message(json.loads(msg.data))
+                    except (TypeError, ValueError):
+                        log.warning("Unable to parse message from Alarm.com: %s", msg.data)
+                        # TODO: On failure, refresh everything synchronous HTTP endpoints.
+                        pass
+
+        except aiohttp.ClientConnectorError:
+            if self.state != WebSocketState.STOPPED:
+                log.error("WebSocket client connection error")
+                self.state = WebSocketState.DISCONNECTED
+
+        except Exception as err:
+            if self.state != WebSocketState.STOPPED:
+                log.error("Unexpected WebSocket error %s", err)
+                self.state = WebSocketState.DISCONNECTED
+
+        else:
+            if self.state != WebSocketState.STOPPED:
+                self.state = WebSocketState.DISCONNECTED
+
+    def start(self) -> None:
+        """Start websocket and update its state."""
+        if self.state != WebSocketState.RUNNING:
+            self.state = WebSocketState.STARTING
+            self._loop.create_task(self._connect())
+
+    def stop(self) -> None:
+        """Close websocket connection."""
+        self.state = WebSocketState.STOPPED
 
     async def _async_handle_message(self, raw_message: dict) -> None:
         """Handle incoming message from Alarm.com."""
 
         log.debug(
             "\n====================[ WEBSOCKET MESSAGE: BEGIN ]====================\n"
             f"{json.dumps(raw_message, indent=4)}"
```

### Comparing `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/const.py` & `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/const.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,17 @@
     PropertyChangeType.LightColor,
 ]
 
 
 class EventType(Enum):
     """Enum for monitoring event types."""
 
+    #
     # Supported
+    #
     ArmedAway = 10
     ArmedNight = 113
     ArmedStay = 9
     Closed = 0
     Disarmed = 8
     DoorLocked = 91
     DoorUnlocked = 90
@@ -44,15 +46,17 @@
     SupervisionFaultDisarming = 47
     SwitchLevelChanged = 317
     ThermostatFanModeChanged = 120
     ThermostatModeChanged = 95
     ThermostatOffset = 105
     ThermostatSetPointChanged = 94
 
+    #
     # Not Supported
+    #
     Alarm = 1
     BypassStart = 13
     BypassEnd = 35
     SumpPumpAlertCriticalIssueMalfunction = 118
     SumpPumpAlertCriticalIssueOff = 117
     SumpPumpAlertIdle = 114
     SumpPumpAlertNormalOperation = 115
@@ -86,14 +90,17 @@
     PendingAlarm = 62
     PolicePanic = 22
     PolicePanicSuspectedAlarm = 64
     SilentPolicePanic = 73
     SilentPolicePanicSuspectedAlarm = 172
     ViewedByCentralStation = 158
 
+    # Undocumented
+    UserLoggedIn = 55
+
 
 SUPPORTED_MONITORING_EVENT_TYPES = [
     EventType.ArmedAway,
     EventType.ArmedNight,
     EventType.ArmedStay,
     EventType.Closed,
     EventType.Disarmed,
```

### Comparing `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/__init__.py` & `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/garage_door.py` & `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/garage_door.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/gate.py` & `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/gate.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/light.py` & `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/light.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/lock.py` & `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/lock.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/partition.py` & `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/partition.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/sensor.py` & `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/sensor.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/thermostat.py` & `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/thermostat.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/handler/water_sensor.py` & `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/handler/water_sensor.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax/websockets/messages.py` & `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax/websockets/messages.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax.egg-info/PKG-INFO` & `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalarmdotcomajax
-Version: 0.5.0b3
+Version: 0.5.0b4
 Summary: Python Interface for Alarm.com
 Home-page: https://github.com/pyalarmdotcom/pyalarmdotcomajax
 Author: Justin Wong
 Author-email: 46082645+uvjustin@users.noreply.github.com
 Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com, 466460+elahd@users.noreply.github.com
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.0b3 Summary: Python
+Metadata-Version: 2.1 Name: pyalarmdotcomajax Version: 0.5.0b4 Summary: Python
 Interface for Alarm.com Home-page: https://github.com/pyalarmdotcom/
 pyalarmdotcomajax Author: Justin Wong Author-email:
 46082645+uvjustin@users.noreply.github.com Maintainer: Elahd Bar-Shai
 Maintainer-email: 46082645+uvjustin@users.noreply.github.com,
 466460+elahd@users.noreply.github.com License: MIT Keywords: Alarm.com,Security
 System,Home Assistant Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English Classifier: Environment :: Web
```

### Comparing `pyalarmdotcomajax-0.5.0b3/pyalarmdotcomajax.egg-info/SOURCES.txt` & `pyalarmdotcomajax-0.5.0b4/pyalarmdotcomajax.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 pyalarmdotcomajax/__init__.py
 pyalarmdotcomajax/__main__.py
 pyalarmdotcomajax/cli.py
 pyalarmdotcomajax/const.py
 pyalarmdotcomajax/errors.py
 pyalarmdotcomajax/extensions.py
 pyalarmdotcomajax/helpers.py
-pyalarmdotcomajax/ws.py
 pyalarmdotcomajax.egg-info/PKG-INFO
 pyalarmdotcomajax.egg-info/SOURCES.txt
 pyalarmdotcomajax.egg-info/dependency_links.txt
 pyalarmdotcomajax.egg-info/entry_points.txt
 pyalarmdotcomajax.egg-info/requires.txt
 pyalarmdotcomajax.egg-info/top_level.txt
 pyalarmdotcomajax.egg-info/zip-safe
```

### Comparing `pyalarmdotcomajax-0.5.0b3/pyproject.toml` & `pyalarmdotcomajax-0.5.0b4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/setup.cfg` & `pyalarmdotcomajax-0.5.0b4/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/tests/__init__.py` & `pyalarmdotcomajax-0.5.0b4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/tests/conftest.py` & `pyalarmdotcomajax-0.5.0b4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/tests/test_controller.py` & `pyalarmdotcomajax-0.5.0b4/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/tests/test_device_extensions.py` & `pyalarmdotcomajax-0.5.0b4/tests/test_device_extensions.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/tests/test_partition.py` & `pyalarmdotcomajax-0.5.0b4/tests/test_partition.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/tests/test_sensors.py` & `pyalarmdotcomajax-0.5.0b4/tests/test_sensors.py`

 * *Files identical despite different names*

### Comparing `pyalarmdotcomajax-0.5.0b3/tests/test_thermostat.py` & `pyalarmdotcomajax-0.5.0b4/tests/test_thermostat.py`

 * *Files identical despite different names*

