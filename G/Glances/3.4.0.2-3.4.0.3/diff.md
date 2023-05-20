# Comparing `tmp/Glances-3.4.0.2.tar.gz` & `tmp/Glances-3.4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Glances-3.4.0.2.tar", last modified: Thu May 18 15:46:21 2023, max compression
+gzip compressed data, was "Glances-3.4.0.3.tar", last modified: Sat May 20 14:49:57 2023, max compression
```

## Comparing `Glances-3.4.0.2.tar` & `Glances-3.4.0.3.tar`

### file list

```diff
@@ -1,335 +1,335 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.140455 Glances-3.4.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-18 15:46:13.000000 Glances-3.4.0.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-05-18 15:46:13.000000 Glances-3.4.0.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    42098 2023-05-18 15:46:13.000000 Glances-3.4.0.2/COPYING
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.096455 Glances-3.4.0.2/Glances.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-05-18 15:46:21.000000 Glances-3.4.0.2/Glances.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-05-18 15:46:21.000000 Glances-3.4.0.2/Glances.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:46:21.000000 Glances-3.4.0.2/Glances.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-18 15:46:21.000000 Glances-3.4.0.2/Glances.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-18 15:46:21.000000 Glances-3.4.0.2/Glances.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-18 15:46:21.000000 Glances-3.4.0.2/Glances.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-18 15:46:13.000000 Glances-3.4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    70747 2023-05-18 15:46:13.000000 Glances-3.4.0.2/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-05-18 15:46:21.140455 Glances-3.4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16100 2023-05-18 15:46:13.000000 Glances-3.4.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.096455 Glances-3.4.0.2/conf/
--rw-r--r--   0 runner    (1001) docker     (123)    20996 2023-05-18 15:46:13.000000 Glances-3.4.0.2/conf/glances.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.100455 Glances-3.4.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.112455 Glances-3.4.0.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    29273 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/amp-dropbox.png
--rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/amp-python-warning.png
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/amp-python.png
--rw-r--r--   0 runner    (1001) docker     (123)    80498 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/amps.png
--rw-r--r--   0 runner    (1001) docker     (123)    13916 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/aws.png
--rw-r--r--   0 runner    (1001) docker     (123)    44160 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/browser.png
--rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/cloud.png
--rw-r--r--   0 runner    (1001) docker     (123)     9442 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/connected.png
--rw-r--r--   0 runner    (1001) docker     (123)    29245 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/connections.png
--rw-r--r--   0 runner    (1001) docker     (123)    34093 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/containers.png
--rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/cpu-wide.png
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/cpu.png
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/disconnected.png
--rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/diskio.png
--rw-r--r--   0 runner    (1001) docker     (123)    24808 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/events.png
--rw-r--r--   0 runner    (1001) docker     (123)    13715 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/folders.png
--rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/fs.png
--rw-r--r--   0 runner    (1001) docker     (123)    56273 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/glances-architecture.excalidraw
--rw-r--r--   0 runner    (1001) docker     (123)   123499 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/glances-architecture.png
--rw-r--r--   0 runner    (1001) docker     (123)   215750 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/glances-flame.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/glances-influxdb.png
--rw-r--r--   0 runner    (1001) docker     (123)    33567 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/glances-memory-profiling-with-history.png
--rw-r--r--   0 runner    (1001) docker     (123)    31797 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/glances-memory-profiling-without-history.png
--rw-r--r--   0 runner    (1001) docker     (123)   293649 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/glances-responsive-webdesign.png
--rw-r--r--   0 runner    (1001) docker     (123)   357638 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/glances-summary.png
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/gpu.png
--rw-r--r--   0 runner    (1001) docker     (123)   141657 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/grafana.png
--rw-r--r--   0 runner    (1001) docker     (123)   187140 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/graph-load.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14415 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/hddtemp.png
--rw-r--r--   0 runner    (1001) docker     (123)    19879 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/header.png
--rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/ip.png
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/irq.png
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/load.png
--rw-r--r--   0 runner    (1001) docker     (123)    20009 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/loadpercent.png
--rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/mem-wide.png
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/mem.png
--rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/monitored.png
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/network.png
--rw-r--r--   0 runner    (1001) docker     (123)    21132 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/per-cpu.png
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/pergpu.png
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/ports.png
--rw-r--r--   0 runner    (1001) docker     (123)    63154 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/processlist-extended.png
--rw-r--r--   0 runner    (1001) docker     (123)   160408 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/processlist-filter.png
--rw-r--r--   0 runner    (1001) docker     (123)    53684 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/processlist-top.png
--rw-r--r--   0 runner    (1001) docker     (123)   227401 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/processlist-wide.png
--rw-r--r--   0 runner    (1001) docker     (123)   151590 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/processlist.png
--rw-r--r--   0 runner    (1001) docker     (123)    25081 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/prometheus_exporter.png
--rw-r--r--   0 runner    (1001) docker     (123)    91914 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/prometheus_server.png
--rw-r--r--   0 runner    (1001) docker     (123)    27582 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/quicklook-percpu.png
--rw-r--r--   0 runner    (1001) docker     (123)    17789 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/quicklook.png
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/raid.png
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/reddit.png
--rw-r--r--   0 runner    (1001) docker     (123)  1089975 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/screencast.gif
--rw-r--r--   0 runner    (1001) docker     (123)   265567 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/screenshot-web.png
--rw-r--r--   0 runner    (1001) docker     (123)    36097 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/screenshot-web2.png
--rw-r--r--   0 runner    (1001) docker     (123)  1098062 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/screenshot-wide.png
--rw-r--r--   0 runner    (1001) docker     (123)   508044 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/screenshot.png
--rw-r--r--   0 runner    (1001) docker     (123)    16125 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/sensors.png
--rw-r--r--   0 runner    (1001) docker     (123)    21500 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/smart.png
--rw-r--r--   0 runner    (1001) docker     (123)    41952 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/sparkline.png
--rw-r--r--   0 runner    (1001) docker     (123)    23021 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/trend.png
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/twitter-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_static/wifi.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.112455 Glances-3.4.0.2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/_templates/links.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.116455 Glances-3.4.0.2/docs/aoa/
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/actions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/amps.rst
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/cloud.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/connections.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/containers.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/cpu.rst
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/diskio.rst
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/events.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/folders.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/fs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/gpu.rst
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/hddtemp.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/header.rst
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/irq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/load.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/memory.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/network.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/ports.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/ps.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/quicklook.rst
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/raid.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/sensors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/smart.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/aoa/wifi.rst
--rw-r--r--   0 runner    (1001) docker     (123)    44330 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/api.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/build.sh
--rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/cmds.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/config.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.116455 Glances-3.4.0.2/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/dev/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)   328258 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/dev/glances-cprofile.png
--rw-r--r--   0 runner    (1001) docker     (123)     7159 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/docker.rst
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/glances.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.116455 Glances-3.4.0.2/docs/gw/
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/cassandra.rst
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/couchdb.rst
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/csv.rst
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/elastic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/graph.rst
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/graphite.rst
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/influxdb.rst
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/json.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/kafka.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/mongodb.rst
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/mqtt.rst
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/opentsdb.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/prometheus.rst
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/rabbitmq.rst
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/restful.rst
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/riemann.rst
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/statsd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/gw/zeromq.rst
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.120455 Glances-3.4.0.2/docs/man/
--rw-r--r--   0 runner    (1001) docker     (123)    17939 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/man/glances.1
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/objects.inv
--rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-18 15:46:13.000000 Glances-3.4.0.2/docs/support.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.124455 Glances-3.4.0.2/glances/
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.124455 Glances-3.4.0.2/glances/amps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/amps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/amps/glances_amp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/amps/glances_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/amps/glances_nginx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/amps/glances_systemd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/amps/glances_systemv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/amps_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/autodiscover.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/client_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/cpu_percent.py
--rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.128455 Glances-3.4.0.2/glances/exports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_cassandra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_couchdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_graphite.py
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_influxdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_influxdb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_opentsdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_prometheus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_restful.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_riemann.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_statsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/exports/glances_zeromq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/folder_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    29248 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outdated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.128455 Glances-3.4.0.2/glances/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/glances_bars.py
--rw-r--r--   0 runner    (1001) docker     (123)    21397 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/glances_bottle.py
--rw-r--r--   0 runner    (1001) docker     (123)    49367 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/glances_curses.py
--rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/glances_curses_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/glances_sparklines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/glances_stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/glances_stdout_apidoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/glances_stdout_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/glances_stdout_issue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/glances_stdout_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/glances_unicode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.128455 Glances-3.4.0.2/glances/outputs/static/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/.eslintrc.js
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/.prettierrc.js
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.128455 Glances-3.4.0.2/glances/outputs/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/css/bootstrap.less
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/css/style.scss
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/css/variables.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.128455 Glances-3.4.0.2/glances/outputs/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    43588 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/images/glances.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.132455 Glances-3.4.0.2/glances/outputs/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    17135 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/App.vue
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/app.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.132455 Glances-3.4.0.2/glances/outputs/static/js/components/
--rw-r--r--   0 runner    (1001) docker     (123)    11318 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/help.vue
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-alert.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-amps.vue
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-cloud.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-connections.vue
--rw-r--r--   0 runner    (1001) docker     (123)     7148 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-containers.vue
--rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-cpu.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-diskio.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-folders.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-fs.vue
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-gpu.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-ip.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-irq.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-load.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-mem-more.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-mem.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-memswap.vue
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-network.vue
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-now.vue
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-percpu.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-ports.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-process.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-processcount.vue
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-processlist.vue
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-quicklook.vue
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-raid.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-sensors.vue
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-system.vue
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-uptime.vue
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/components/plugin-wifi.vue
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/filters.js
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/services.js
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/js/store.js
--rw-r--r--   0 runner    (1001) docker     (123)   445972 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.132455 Glances-3.4.0.2/glances/outputs/static/public/
--rw-r--r--   0 runner    (1001) docker     (123)    43588 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/public/87708faeed9a66b0fcdb.png
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/public/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)   444157 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/public/glances.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.136455 Glances-3.4.0.2/glances/outputs/static/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/templates/index.html.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/outputs/static/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/password.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/password_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.140455 Glances-3.4.0.2/glances/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.140455 Glances-3.4.0.2/glances/plugins/containers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13743 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/containers/glances_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/containers/glances_podman.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/containers/stats_streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_amps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    16847 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    15759 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_diskio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_folders.py
--rw-r--r--   0 runner    (1001) docker     (123)    10639 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_fs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_help.py
--rw-r--r--   0 runner    (1001) docker     (123)    10957 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_irq.py
--rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_load.py
--rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_mem.py
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_memswap.py
--rw-r--r--   0 runner    (1001) docker     (123)    15881 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_now.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_percpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    42555 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_processcount.py
--rw-r--r--   0 runner    (1001) docker     (123)    34269 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_processlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_psutilversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_quicklook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_raid.py
--rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_smart.py
--rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_uptime.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/glances_wifi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:21.140455 Glances-3.4.0.2/glances/plugins/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/sensors/glances_batpercent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/plugins/sensors/glances_hddtemp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/ports_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    23868 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/programs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/secure.py
--rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/snmp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/standalone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/static_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/stats_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/stats_client_snmp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/stats_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/thresholds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/web_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-18 15:46:13.000000 Glances-3.4.0.2/glances/webserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-18 15:46:13.000000 Glances-3.4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:46:21.140455 Glances-3.4.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4992 2023-05-18 15:46:13.000000 Glances-3.4.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:49:57.574536 Glances-3.4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-20 14:49:46.000000 Glances-3.4.0.3/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-05-20 14:49:46.000000 Glances-3.4.0.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    42098 2023-05-20 14:49:46.000000 Glances-3.4.0.3/COPYING
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:49:57.526535 Glances-3.4.0.3/Glances.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-05-20 14:49:57.000000 Glances-3.4.0.3/Glances.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-05-20 14:49:57.000000 Glances-3.4.0.3/Glances.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 14:49:57.000000 Glances-3.4.0.3/Glances.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-20 14:49:57.000000 Glances-3.4.0.3/Glances.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-20 14:49:57.000000 Glances-3.4.0.3/Glances.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-20 14:49:57.000000 Glances-3.4.0.3/Glances.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-20 14:49:46.000000 Glances-3.4.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    71000 2023-05-20 14:49:46.000000 Glances-3.4.0.3/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-05-20 14:49:57.574536 Glances-3.4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16100 2023-05-20 14:49:46.000000 Glances-3.4.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:49:57.526535 Glances-3.4.0.3/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)    20996 2023-05-20 14:49:46.000000 Glances-3.4.0.3/conf/glances.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:49:57.530535 Glances-3.4.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:49:57.542536 Glances-3.4.0.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    29273 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/amp-dropbox.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/amp-python-warning.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/amp-python.png
+-rw-r--r--   0 runner    (1001) docker     (123)    80498 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/amps.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13916 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/aws.png
+-rw-r--r--   0 runner    (1001) docker     (123)    44160 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/browser.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/cloud.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9442 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/connected.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29245 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/connections.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34093 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/containers.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/cpu-wide.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/cpu.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/disconnected.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/diskio.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24808 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/events.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13715 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/folders.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/fs.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56273 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/glances-architecture.excalidraw
+-rw-r--r--   0 runner    (1001) docker     (123)   123499 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/glances-architecture.png
+-rw-r--r--   0 runner    (1001) docker     (123)   215750 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/glances-flame.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/glances-influxdb.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33567 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/glances-memory-profiling-with-history.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31797 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/glances-memory-profiling-without-history.png
+-rw-r--r--   0 runner    (1001) docker     (123)   293649 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/glances-responsive-webdesign.png
+-rw-r--r--   0 runner    (1001) docker     (123)   357638 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/glances-summary.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/gpu.png
+-rw-r--r--   0 runner    (1001) docker     (123)   141657 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/grafana.png
+-rw-r--r--   0 runner    (1001) docker     (123)   187140 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/graph-load.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14415 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/hddtemp.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19879 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/header.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/ip.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/irq.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/load.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20009 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/loadpercent.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/mem-wide.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/mem.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/monitored.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/network.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21132 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/per-cpu.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/pergpu.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/ports.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63154 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/processlist-extended.png
+-rw-r--r--   0 runner    (1001) docker     (123)   160408 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/processlist-filter.png
+-rw-r--r--   0 runner    (1001) docker     (123)    53684 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/processlist-top.png
+-rw-r--r--   0 runner    (1001) docker     (123)   227401 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/processlist-wide.png
+-rw-r--r--   0 runner    (1001) docker     (123)   151590 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/processlist.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25081 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/prometheus_exporter.png
+-rw-r--r--   0 runner    (1001) docker     (123)    91914 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/prometheus_server.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27582 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/quicklook-percpu.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17789 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/quicklook.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/raid.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/reddit.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1089975 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/screencast.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   265567 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/screenshot-web.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36097 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/screenshot-web2.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1098062 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/screenshot-wide.png
+-rw-r--r--   0 runner    (1001) docker     (123)   508044 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16125 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/sensors.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21500 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/smart.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41952 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/sparkline.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23021 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/trend.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/twitter-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_static/wifi.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:49:57.542536 Glances-3.4.0.3/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/_templates/links.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:49:57.546536 Glances-3.4.0.3/docs/aoa/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/aoa/actions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/aoa/amps.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/aoa/cloud.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/aoa/connections.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/aoa/containers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/aoa/cpu.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/aoa/diskio.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/aoa/events.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/aoa/folders.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/aoa/fs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/aoa/gpu.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/aoa/hddtemp.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/aoa/header.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/aoa/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/aoa/irq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/aoa/load.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/aoa/memory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/aoa/network.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/aoa/ports.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/aoa/ps.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/aoa/quicklook.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/aoa/raid.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/aoa/sensors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/aoa/smart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/aoa/wifi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    45693 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/api.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/build.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/cmds.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/config.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:49:57.546536 Glances-3.4.0.3/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/dev/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   328258 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/dev/glances-cprofile.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7159 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/docker.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/glances.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:49:57.550536 Glances-3.4.0.3/docs/gw/
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/gw/cassandra.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/gw/couchdb.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/gw/csv.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/gw/elastic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/gw/graph.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/gw/graphite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/gw/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/gw/influxdb.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/gw/json.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/gw/kafka.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/gw/mongodb.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/gw/mqtt.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/gw/opentsdb.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/gw/prometheus.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/gw/rabbitmq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/gw/restful.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/gw/riemann.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/gw/statsd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/gw/zeromq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:49:57.550536 Glances-3.4.0.3/docs/man/
+-rw-r--r--   0 runner    (1001) docker     (123)    17939 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/man/glances.1
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-20 14:49:46.000000 Glances-3.4.0.3/docs/support.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:49:57.554536 Glances-3.4.0.3/glances/
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:49:57.554536 Glances-3.4.0.3/glances/amps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/amps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/amps/glances_amp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/amps/glances_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/amps/glances_nginx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/amps/glances_systemd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/amps/glances_systemv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/amps_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/autodiscover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/client_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/cpu_percent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:49:57.558536 Glances-3.4.0.3/glances/exports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/exports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/exports/glances_cassandra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/exports/glances_couchdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/exports/glances_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/exports/glances_elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/exports/glances_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/exports/glances_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/exports/glances_graphite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/exports/glances_influxdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/exports/glances_influxdb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/exports/glances_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/exports/glances_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/exports/glances_mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/exports/glances_mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/exports/glances_opentsdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/exports/glances_prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/exports/glances_rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/exports/glances_restful.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/exports/glances_riemann.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/exports/glances_statsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/exports/glances_zeromq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/folder_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29248 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outdated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:49:57.558536 Glances-3.4.0.3/glances/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/glances_bars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21397 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/glances_bottle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49367 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/glances_curses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/glances_curses_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/glances_sparklines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/glances_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/glances_stdout_apidoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/glances_stdout_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/glances_stdout_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/glances_stdout_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/glances_unicode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:49:57.558536 Glances-3.4.0.3/glances/outputs/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/.eslintrc.js
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/.prettierrc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:49:57.562536 Glances-3.4.0.3/glances/outputs/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/css/bootstrap.less
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/css/style.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/css/variables.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:49:57.562536 Glances-3.4.0.3/glances/outputs/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    43588 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/images/glances.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:49:57.562536 Glances-3.4.0.3/glances/outputs/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    17135 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/App.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/app.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:49:57.566536 Glances-3.4.0.3/glances/outputs/static/js/components/
+-rw-r--r--   0 runner    (1001) docker     (123)    11318 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/components/help.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/components/plugin-alert.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/components/plugin-amps.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/components/plugin-cloud.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/components/plugin-connections.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     7148 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/components/plugin-containers.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/components/plugin-cpu.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/components/plugin-diskio.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/components/plugin-folders.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/components/plugin-fs.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/components/plugin-gpu.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/components/plugin-ip.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/components/plugin-irq.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/components/plugin-load.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/components/plugin-mem-more.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/components/plugin-mem.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/components/plugin-memswap.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/components/plugin-network.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/components/plugin-now.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/components/plugin-percpu.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/components/plugin-ports.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/components/plugin-process.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/components/plugin-processcount.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/components/plugin-processlist.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/components/plugin-quicklook.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/components/plugin-raid.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/components/plugin-sensors.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/components/plugin-system.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/components/plugin-uptime.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/components/plugin-wifi.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/filters.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/services.js
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/js/store.js
+-rw-r--r--   0 runner    (1001) docker     (123)   445972 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:49:57.566536 Glances-3.4.0.3/glances/outputs/static/public/
+-rw-r--r--   0 runner    (1001) docker     (123)    43588 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/public/87708faeed9a66b0fcdb.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/public/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   444236 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/public/glances.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:49:57.566536 Glances-3.4.0.3/glances/outputs/static/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/templates/index.html.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/outputs/static/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/password_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:49:57.570536 Glances-3.4.0.3/glances/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:49:57.574536 Glances-3.4.0.3/glances/plugins/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13743 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/containers/glances_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/containers/glances_podman.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/containers/stats_streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_amps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16847 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15759 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_diskio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10639 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10957 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_irq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_mem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_memswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15881 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_now.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_percpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42555 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_processcount.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34269 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_processlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_psutilversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_quicklook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_raid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_smart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_uptime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/glances_wifi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:49:57.574536 Glances-3.4.0.3/glances/plugins/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/sensors/glances_batpercent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/plugins/sensors/glances_hddtemp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/ports_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23868 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/programs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/secure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/snmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/standalone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/static_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/stats_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/stats_client_snmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/stats_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/thresholds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/web_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-20 14:49:46.000000 Glances-3.4.0.3/glances/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-20 14:49:46.000000 Glances-3.4.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 14:49:57.574536 Glances-3.4.0.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4992 2023-05-20 14:49:46.000000 Glances-3.4.0.3/setup.py
```

### Comparing `Glances-3.4.0.2/AUTHORS` & `Glances-3.4.0.3/AUTHORS`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/CONTRIBUTING.md` & `Glances-3.4.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/COPYING` & `Glances-3.4.0.3/COPYING`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/Glances.egg-info/PKG-INFO` & `Glances-3.4.0.3/Glances.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Glances
-Version: 3.4.0.2
+Version: 3.4.0.3
 Summary: A cross-platform curses-based monitoring tool
 Home-page: https://github.com/nicolargo/glances
 Author: Nicolas Hennion
 Author-email: nicolas@nicolargo.com
 License: LGPLv3
 Keywords: cli curses monitoring system
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Glances-3.4.0.2/Glances.egg-info/SOURCES.txt` & `Glances-3.4.0.3/Glances.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/Glances.egg-info/requires.txt` & `Glances-3.4.0.3/Glances.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/NEWS.rst` & `Glances-3.4.0.3/NEWS.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 ==============================================================================
                                 Glances changelog
 ==============================================================================
 
 ===============
+Version 3.4.0.3
+===============
+
+Bugs corrected:
+
+    * Add glances binary to '/usr/local/bin' + Update ENV PATH to include '/venv/bin' in Dockerfiles #2419
+    * No more threshold display in the WebUI cpu/mem and memswap plugins #2420
+
+===============
 Version 3.4.0.2
 ===============
 
 Bugs corrected:
 
     * Cannot start Glances 3.4.0.1 on Windows 10: SIGHUP not defined #2408
     * Influxdb2 export not working #2407
```

### Comparing `Glances-3.4.0.2/PKG-INFO` & `Glances-3.4.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Glances
-Version: 3.4.0.2
+Version: 3.4.0.3
 Summary: A cross-platform curses-based monitoring tool
 Home-page: https://github.com/nicolargo/glances
 Author: Nicolas Hennion
 Author-email: nicolas@nicolargo.com
 License: LGPLv3
 Keywords: cli curses monitoring system
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Glances-3.4.0.2/README.rst` & `Glances-3.4.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/conf/glances.conf` & `Glances-3.4.0.3/conf/glances.conf`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/Makefile` & `Glances-3.4.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/amp-dropbox.png` & `Glances-3.4.0.3/docs/_static/amp-dropbox.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/amp-python-warning.png` & `Glances-3.4.0.3/docs/_static/amp-python-warning.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/amp-python.png` & `Glances-3.4.0.3/docs/_static/amp-python.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/amps.png` & `Glances-3.4.0.3/docs/_static/amps.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/aws.png` & `Glances-3.4.0.3/docs/_static/aws.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/browser.png` & `Glances-3.4.0.3/docs/_static/browser.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/cloud.png` & `Glances-3.4.0.3/docs/_static/cloud.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/connected.png` & `Glances-3.4.0.3/docs/_static/connected.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/connections.png` & `Glances-3.4.0.3/docs/_static/connections.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/containers.png` & `Glances-3.4.0.3/docs/_static/containers.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/cpu-wide.png` & `Glances-3.4.0.3/docs/_static/cpu-wide.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/cpu.png` & `Glances-3.4.0.3/docs/_static/cpu.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/disconnected.png` & `Glances-3.4.0.3/docs/_static/disconnected.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/diskio.png` & `Glances-3.4.0.3/docs/_static/diskio.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/events.png` & `Glances-3.4.0.3/docs/_static/events.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/folders.png` & `Glances-3.4.0.3/docs/_static/folders.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/fs.png` & `Glances-3.4.0.3/docs/_static/fs.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/glances-architecture.excalidraw` & `Glances-3.4.0.3/docs/_static/glances-architecture.excalidraw`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/glances-architecture.png` & `Glances-3.4.0.3/docs/_static/glances-architecture.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/glances-flame.svg` & `Glances-3.4.0.3/docs/_static/glances-flame.svg`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/glances-influxdb.png` & `Glances-3.4.0.3/docs/_static/glances-influxdb.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/glances-memory-profiling-with-history.png` & `Glances-3.4.0.3/docs/_static/glances-memory-profiling-with-history.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/glances-memory-profiling-without-history.png` & `Glances-3.4.0.3/docs/_static/glances-memory-profiling-without-history.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/glances-responsive-webdesign.png` & `Glances-3.4.0.3/docs/_static/glances-responsive-webdesign.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/glances-summary.png` & `Glances-3.4.0.3/docs/_static/glances-summary.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/gpu.png` & `Glances-3.4.0.3/docs/_static/gpu.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/grafana.png` & `Glances-3.4.0.3/docs/_static/grafana.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/graph-load.svg` & `Glances-3.4.0.3/docs/_static/graph-load.svg`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/hddtemp.png` & `Glances-3.4.0.3/docs/_static/hddtemp.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/header.png` & `Glances-3.4.0.3/docs/_static/header.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/ip.png` & `Glances-3.4.0.3/docs/_static/ip.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/irq.png` & `Glances-3.4.0.3/docs/_static/irq.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/load.png` & `Glances-3.4.0.3/docs/_static/load.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/loadpercent.png` & `Glances-3.4.0.3/docs/_static/loadpercent.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/mem-wide.png` & `Glances-3.4.0.3/docs/_static/mem-wide.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/mem.png` & `Glances-3.4.0.3/docs/_static/mem.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/monitored.png` & `Glances-3.4.0.3/docs/_static/monitored.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/network.png` & `Glances-3.4.0.3/docs/_static/network.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/per-cpu.png` & `Glances-3.4.0.3/docs/_static/per-cpu.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/pergpu.png` & `Glances-3.4.0.3/docs/_static/pergpu.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/ports.png` & `Glances-3.4.0.3/docs/_static/ports.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/processlist-extended.png` & `Glances-3.4.0.3/docs/_static/processlist-extended.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/processlist-filter.png` & `Glances-3.4.0.3/docs/_static/processlist-filter.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/processlist-top.png` & `Glances-3.4.0.3/docs/_static/processlist-top.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/processlist-wide.png` & `Glances-3.4.0.3/docs/_static/processlist-wide.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/processlist.png` & `Glances-3.4.0.3/docs/_static/processlist.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/prometheus_exporter.png` & `Glances-3.4.0.3/docs/_static/prometheus_exporter.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/prometheus_server.png` & `Glances-3.4.0.3/docs/_static/prometheus_server.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/quicklook-percpu.png` & `Glances-3.4.0.3/docs/_static/quicklook-percpu.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/quicklook.png` & `Glances-3.4.0.3/docs/_static/quicklook.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/raid.png` & `Glances-3.4.0.3/docs/_static/raid.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/reddit.png` & `Glances-3.4.0.3/docs/_static/reddit.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/screencast.gif` & `Glances-3.4.0.3/docs/_static/screencast.gif`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/screenshot-web.png` & `Glances-3.4.0.3/docs/_static/screenshot-web.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/screenshot-web2.png` & `Glances-3.4.0.3/docs/_static/screenshot-web2.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/screenshot-wide.png` & `Glances-3.4.0.3/docs/_static/screenshot-wide.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/screenshot.png` & `Glances-3.4.0.3/docs/_static/screenshot.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/sensors.png` & `Glances-3.4.0.3/docs/_static/sensors.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/smart.png` & `Glances-3.4.0.3/docs/_static/smart.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/sparkline.png` & `Glances-3.4.0.3/docs/_static/sparkline.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/trend.png` & `Glances-3.4.0.3/docs/_static/trend.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/twitter-icon.png` & `Glances-3.4.0.3/docs/_static/twitter-icon.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/_static/wifi.png` & `Glances-3.4.0.3/docs/_static/wifi.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/aoa/actions.rst` & `Glances-3.4.0.3/docs/aoa/actions.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/aoa/amps.rst` & `Glances-3.4.0.3/docs/aoa/amps.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/aoa/connections.rst` & `Glances-3.4.0.3/docs/aoa/connections.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/aoa/containers.rst` & `Glances-3.4.0.3/docs/aoa/containers.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/aoa/cpu.rst` & `Glances-3.4.0.3/docs/aoa/cpu.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/aoa/diskio.rst` & `Glances-3.4.0.3/docs/aoa/diskio.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/aoa/events.rst` & `Glances-3.4.0.3/docs/aoa/events.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/aoa/folders.rst` & `Glances-3.4.0.3/docs/aoa/folders.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/aoa/fs.rst` & `Glances-3.4.0.3/docs/aoa/fs.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/aoa/gpu.rst` & `Glances-3.4.0.3/docs/aoa/gpu.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/aoa/hddtemp.rst` & `Glances-3.4.0.3/docs/aoa/hddtemp.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/aoa/header.rst` & `Glances-3.4.0.3/docs/aoa/header.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/aoa/index.rst` & `Glances-3.4.0.3/docs/aoa/index.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/aoa/irq.rst` & `Glances-3.4.0.3/docs/aoa/irq.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/aoa/load.rst` & `Glances-3.4.0.3/docs/aoa/load.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/aoa/memory.rst` & `Glances-3.4.0.3/docs/aoa/memory.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/aoa/network.rst` & `Glances-3.4.0.3/docs/aoa/network.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/aoa/ports.rst` & `Glances-3.4.0.3/docs/aoa/ports.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/aoa/ps.rst` & `Glances-3.4.0.3/docs/aoa/ps.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/aoa/quicklook.rst` & `Glances-3.4.0.3/docs/aoa/quicklook.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/aoa/sensors.rst` & `Glances-3.4.0.3/docs/aoa/sensors.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/aoa/smart.rst` & `Glances-3.4.0.3/docs/aoa/smart.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/aoa/wifi.rst` & `Glances-3.4.0.3/docs/aoa/wifi.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/api.rst` & `Glances-3.4.0.3/docs/api.rst`

 * *Files 8% similar despite different names*

```diff
@@ -56,38 +56,57 @@
      "raid",
      "sensors",
      "smart",
      "system",
      "uptime",
      "wifi"]
 
+GET alert
+---------
+
+Get plugin stats::
+
+    # curl http://localhost:61208/api/3/alert
+    [[1684593857.0,
+      -1,
+      "WARNING",
+      "MEM",
+      74.95383222581204,
+      74.95383222581204,
+      74.95383222581204,
+      74.95383222581204,
+      1,
+      [],
+      "",
+      "memory_percent"]]
+
 GET amps
 --------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/amps
     [{"count": 0,
       "countmax": None,
       "countmin": 1.0,
       "key": "name",
       "name": "Dropbox",
       "refresh": 3.0,
       "regex": True,
       "result": None,
-      "timer": 1.053581953048706},
+      "timer": 1.7997314929962158},
      {"count": 0,
       "countmax": 20.0,
       "countmin": None,
       "key": "name",
       "name": "Python",
       "refresh": 3.0,
       "regex": True,
       "result": None,
-      "timer": 1.0533969402313232}]
+      "timer": 1.7995269298553467}]
 
 Get a specific field::
 
     # curl http://localhost:61208/api/3/amps/name
     {"name": ["Dropbox", "Python", "Conntrack", "Nginx", "Systemd", "SystemV"]}
 
 Get a specific item when field matchs the given value::
@@ -97,15 +116,15 @@
                   "countmax": None,
                   "countmin": 1.0,
                   "key": "name",
                   "name": "Dropbox",
                   "refresh": 3.0,
                   "regex": True,
                   "result": None,
-                  "timer": 1.053581953048706}]}
+                  "timer": 1.7997314929962158}]}
 
 GET connections
 ---------------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/connections
@@ -124,37 +143,37 @@
     # curl http://localhost:61208/api/3/containers
     {"containers": [{"Command": ["top"],
                      "Created": "2023-05-08T15:29:34.918692365+02:00",
                      "Id": "4b7f732d43e4bc5d92fe5298cba025b550e6a608754c1c38f9a90aaecd46b8f9",
                      "Image": "["docker.io/library/ubuntu:latest"]",
                      "Status": "running",
                      "Uptime": "1 weeks",
-                     "cpu": {"total": 1.2768348293282041e-06},
-                     "cpu_percent": 1.2768348293282041e-06,
+                     "cpu": {"total": 2.2993346332214973e-06},
+                     "cpu_percent": 2.2993346332214973e-06,
                      "engine": "podman",
                      "io": {"ior": 0.0, "iow": 0.0, "time_since_update": 1},
                      "io_r": 0.0,
                      "io_w": 0.0,
                      "key": "name",
-                     "memory": {"limit": 7836184576.0, "usage": 1282048.0},
-                     "memory_usage": 1282048.0,
+                     "memory": {"limit": 7836184576.0, "usage": 1142784.0},
+                     "memory_usage": 1142784.0,
                      "name": "frosty_bouman",
                      "network": {"rx": 0.0, "time_since_update": 1, "tx": 0.0},
                      "network_rx": 0.0,
                      "network_tx": 0.0,
                      "pod_id": "8d0f1c783def",
                      "pod_name": "frosty_bouman"},
                     {"Command": [],
                      "Created": "2022-10-22T14:23:03.120912374+02:00",
                      "Id": "9491515251edcd5bb5dc17205d7ee573c0be96fe0b08b0a12a7e2cea874565ea",
                      "Image": "["k8s.gcr.io/pause:3.5"]",
                      "Status": "running",
                      "Uptime": "1 weeks",
-                     "cpu": {"total": 2.6911269370551856e-10},
-                     "cpu_percent": 2.6911269370551856e-10,
+                     "cpu": {"total": 2.754373096346692e-10},
+                     "cpu_percent": 2.754373096346692e-10,
                      "engine": "podman",
                      "io": {"ior": 0.0, "iow": 0.0, "time_since_update": 1},
                      "io_r": 0.0,
                      "io_w": 0.0,
                      "key": "name",
                      "memory": {"limit": 7836184576.0, "usage": 208896.0},
                      "memory_usage": 208896.0,
@@ -165,15 +184,15 @@
                      "pod_id": "8d0f1c783def",
                      "pod_name": "8d0f1c783def-infra"},
                     {"Command": ["/portainer"],
                      "Created": "2022-10-29T14:59:10.266701439Z",
                      "Id": "3abd51c615968482d9ccff5afc629f267f6dda113ed68b75b432615fae3b49fb",
                      "Image": ["portainer/portainer-ce:2.9.3"],
                      "Status": "running",
-                     "Uptime": "5 days",
+                     "Uptime": "7 hours",
                      "cpu": {"total": 0.0},
                      "cpu_percent": 0.0,
                      "engine": "docker",
                      "io": {},
                      "io_r": None,
                      "io_w": None,
                      "key": "name",
@@ -208,29 +227,29 @@
 -------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/cpu
     {"cpucore": 4,
      "ctx_switches": 0,
-     "guest": 0.0,
+     "guest": 1.1,
      "guest_nice": 0.0,
-     "idle": 55.9,
+     "idle": 38.7,
      "interrupts": 0,
-     "iowait": 0.0,
+     "iowait": 3.2,
      "irq": 0.0,
      "nice": 0.0,
      "soft_interrupts": 0,
-     "softirq": 0.0,
+     "softirq": 0.4,
      "steal": 0.0,
      "syscalls": 0,
-     "system": 6.6,
+     "system": 7.7,
      "time_since_update": 1,
-     "total": 42.1,
-     "user": 37.5}
+     "total": 62.2,
+     "user": 50.0}
 
 Fields descriptions:
 
 * **total**: Sum of all CPU percentages (except idle) (unit is *percent*)
 * **system**: percent time spent in kernel space. System CPU time is the time spent running code in the Operating System kernel (unit is *percent*)
 * **user**: CPU percent time spent in user space. User CPU time is the time spent on the processor running your program's code (or code in libraries) (unit is *percent*)
 * **iowait**: *(Linux)*: percent time spent by the CPU waiting for I/O operations to complete (unit is *percent*)
@@ -245,15 +264,15 @@
 * **syscalls**: number of system calls per second. Always 0 on Linux OS (unit is *number*)
 * **cpucore**: Total number of CPU core (unit is *number*)
 * **time_since_update**: Number of seconds since last update (unit is *seconds*)
 
 Get a specific field::
 
     # curl http://localhost:61208/api/3/cpu/total
-    {"total": 42.1}
+    {"total": 62.2}
 
 GET diskio
 ----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/diskio
@@ -291,21 +310,21 @@
 GET fs
 ------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/fs
     [{"device_name": "/dev/mapper/ubuntu--gnome--vg-root",
-      "free": 3450388480,
+      "free": 4763168768,
       "fs_type": "ext4",
       "key": "mnt_point",
       "mnt_point": "/",
-      "percent": 98.5,
+      "percent": 97.9,
       "size": 243334156288,
-      "used": 227496312832},
+      "used": 226183532544},
      {"device_name": "zsfpool",
       "free": 41811968,
       "fs_type": "zfs",
       "key": "mnt_point",
       "mnt_point": "/zsfpool",
       "percent": 0.3,
       "size": 41943040,
@@ -316,21 +335,21 @@
     # curl http://localhost:61208/api/3/fs/mnt_point
     {"mnt_point": ["/", "/zsfpool", "/var/snap/firefox/common/host-hunspell"]}
 
 Get a specific item when field matchs the given value::
 
     # curl http://localhost:61208/api/3/fs/mnt_point//
     {"/": [{"device_name": "/dev/mapper/ubuntu--gnome--vg-root",
-            "free": 3450388480,
+            "free": 4763168768,
             "fs_type": "ext4",
             "key": "mnt_point",
             "mnt_point": "/",
-            "percent": 98.5,
+            "percent": 97.9,
             "size": 243334156288,
-            "used": 227496312832}]}
+            "used": 226183532544}]}
 
 GET ip
 ------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/ip
@@ -348,44 +367,47 @@
 
 GET load
 --------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/load
-    {"cpucore": 4, "min1": 1.8046875, "min15": 1.51025390625, "min5": 1.6845703125}
+    {"cpucore": 4,
+     "min1": 3.00634765625,
+     "min15": 1.19775390625,
+     "min5": 1.4345703125}
 
 Fields descriptions:
 
 * **min1**: Average sum of the number of processes waiting in the run-queue plus the number currently executing over 1 minute (unit is *float*)
 * **min5**: Average sum of the number of processes waiting in the run-queue plus the number currently executing over 5 minutes (unit is *float*)
 * **min15**: Average sum of the number of processes waiting in the run-queue plus the number currently executing over 15 minutes (unit is *float*)
 * **cpucore**: Total number of CPU core (unit is *number*)
 
 Get a specific field::
 
     # curl http://localhost:61208/api/3/load/min1
-    {"min1": 1.8046875}
+    {"min1": 3.00634765625}
 
 GET mem
 -------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/mem
-    {"active": 2122240000,
-     "available": 2791682048,
-     "buffers": 85512192,
-     "cached": 2199904256,
-     "free": 2791682048,
-     "inactive": 3360813056,
-     "percent": 64.4,
-     "shared": 575238144,
+    {"active": 3130548224,
+     "available": 1962663936,
+     "buffers": 142680064,
+     "cached": 2079936512,
+     "free": 1962663936,
+     "inactive": 3094474752,
+     "percent": 75.0,
+     "shared": 498302976,
      "total": 7836184576,
-     "used": 5044502528}
+     "used": 5873520640}
 
 Fields descriptions:
 
 * **total**: Total physical memory available (unit is *bytes*)
 * **available**: The actual amount of available memory that can be given instantly to processes that request more memory in bytes; this is calculated by summing different memory values depending on the platform (e.g. free + buffers + cached on Linux) and it is supposed to be used to monitor actual memory usage in a cross platform fashion (unit is *bytes*)
 * **percent**: The percentage usage calculated as (total - available) / total * 100 (unit is *percent*)
 * **used**: Memory used, calculated differently depending on the platform and designed for informational purposes only (unit is *bytes*)
@@ -404,21 +426,21 @@
 
 GET memswap
 -----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/memswap
-    {"free": 4049227776,
-     "percent": 49.9,
-     "sin": 4989526016,
-     "sout": 8589299712,
+    {"free": 3018182656,
+     "percent": 62.7,
+     "sin": 10520571904,
+     "sout": 16592646144,
      "time_since_update": 1,
      "total": 8082419712,
-     "used": 4033191936}
+     "used": 5064237056}
 
 Fields descriptions:
 
 * **total**: Total swap memory (unit is *bytes*)
 * **used**: Used swap memory (unit is *bytes*)
 * **free**: Free swap memory (unit is *bytes*)
 * **percent**: Used swap memory in percentage (unit is *percent*)
@@ -434,37 +456,37 @@
 GET network
 -----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/network
     [{"alias": None,
-      "cumulative_cx": 194497112,
-      "cumulative_rx": 97248556,
-      "cumulative_tx": 97248556,
-      "cx": 3794,
+      "cumulative_cx": 344481682,
+      "cumulative_rx": 172240841,
+      "cumulative_tx": 172240841,
+      "cx": 7770,
       "interface_name": "lo",
       "is_up": True,
       "key": "interface_name",
-      "rx": 1897,
+      "rx": 3885,
       "speed": 0,
       "time_since_update": 1,
-      "tx": 1897},
+      "tx": 3885},
      {"alias": None,
-      "cumulative_cx": 13127976036,
-      "cumulative_rx": 12705380323,
-      "cumulative_tx": 422595713,
-      "cx": 39560,
+      "cumulative_cx": 22624441944,
+      "cumulative_rx": 21888194655,
+      "cumulative_tx": 736247289,
+      "cx": 146685,
       "interface_name": "wlp2s0",
       "is_up": True,
       "key": "interface_name",
-      "rx": 26691,
+      "rx": 135811,
       "speed": 0,
       "time_since_update": 1,
-      "tx": 12869}]
+      "tx": 10874}]
 
 Fields descriptions:
 
 * **interface_name**: Interface name (unit is *string*)
 * **alias**: Interface alias name (optional) (unit is *string*)
 * **rx**: The received/input rate (in bit per second) (unit is *bps*)
 * **tx**: The sent/output rate (in bit per second) (unit is *bps*)
@@ -480,73 +502,74 @@
 
     # curl http://localhost:61208/api/3/network/interface_name
     {"interface_name": ["lo",
                         "wlp2s0",
                         "docker0",
                         "br_grafana",
                         "mpqemubr0",
-                        "vethcddb0e6",
-                        "vboxnet0"]}
+                        "vboxnet0",
+                        "tap-1e376645a40",
+                        "veth54fd604"]}
 
 Get a specific item when field matchs the given value::
 
     # curl http://localhost:61208/api/3/network/interface_name/lo
     {"lo": [{"alias": None,
-             "cumulative_cx": 194497112,
-             "cumulative_rx": 97248556,
-             "cumulative_tx": 97248556,
-             "cx": 3794,
+             "cumulative_cx": 344481682,
+             "cumulative_rx": 172240841,
+             "cumulative_tx": 172240841,
+             "cx": 7770,
              "interface_name": "lo",
              "is_up": True,
              "key": "interface_name",
-             "rx": 1897,
+             "rx": 3885,
              "speed": 0,
              "time_since_update": 1,
-             "tx": 1897}]}
+             "tx": 3885}]}
 
 GET now
 -------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/now
-    "2023-05-18 17:40:44 CEST"
+    "2023-05-20 16:44:16 CEST"
 
 GET percpu
 ----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/percpu
     [{"cpu_number": 0,
-      "guest": 0.0,
+      "guest": 1.5,
       "guest_nice": 0.0,
-      "idle": 71.1,
-      "iowait": 0.0,
+      "idle": 26.2,
+      "iowait": 1.5,
       "irq": 0.0,
       "key": "cpu_number",
       "nice": 0.0,
       "softirq": 0.0,
       "steal": 0.0,
-      "system": 6.2,
-      "total": 28.9,
-      "user": 22.7},
+      "system": 4.4,
+      "total": 73.8,
+      "user": 68.0},
      {"cpu_number": 1,
       "guest": 0.0,
       "guest_nice": 0.0,
-      "idle": 72.1,
-      "iowait": 0.0,
+      "idle": 39.4,
+      "iowait": 1.0,
       "irq": 0.0,
       "key": "cpu_number",
       "nice": 0.0,
       "softirq": 0.0,
       "steal": 0.0,
-      "system": 8.5,
-      "total": 27.9,
-      "user": 19.4}]
+      "system": 4.8,
+      "total": 60.6,
+      "user": 54.8}]
 
 Get a specific field::
 
     # curl http://localhost:61208/api/3/percpu/cpu_number
     {"cpu_number": [0, 1, 2, 3]}
 
 GET ports
@@ -557,15 +580,15 @@
     # curl http://localhost:61208/api/3/ports
     [{"description": "DefaultGateway",
       "host": "192.168.0.254",
       "indice": "port_0",
       "port": 0,
       "refresh": 30,
       "rtt_warning": None,
-      "status": 0.004474,
+      "status": 0.00792,
       "timeout": 3}]
 
 Get a specific field::
 
     # curl http://localhost:61208/api/3/ports/host
     {"host": ["192.168.0.254"]}
 
@@ -574,307 +597,322 @@
     # curl http://localhost:61208/api/3/ports/host/192.168.0.254
     {"192.168.0.254": [{"description": "DefaultGateway",
                         "host": "192.168.0.254",
                         "indice": "port_0",
                         "port": 0,
                         "refresh": 30,
                         "rtt_warning": None,
-                        "status": 0.004474,
+                        "status": 0.00792,
                         "timeout": 3}]}
 
 GET processcount
 ----------------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/processcount
-    {"pid_max": 0, "running": 2, "sleeping": 326, "thread": 1750, "total": 392}
+    {"pid_max": 0, "running": 1, "sleeping": 347, "thread": 1761, "total": 415}
 
 Get a specific field::
 
     # curl http://localhost:61208/api/3/processcount/total
-    {"total": 392}
+    {"total": 415}
 
 GET processlist
 ---------------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/processlist
     [{"cmdline": ["/snap/firefox/2605/usr/lib/firefox/firefox"],
       "cpu_percent": 0.0,
-      "cpu_times": [9681.14, 2938.04, 7162.98, 1045.12, 0.0],
+      "cpu_times": [16463.82, 5059.85, 11961.09, 1725.84, 0.0],
       "gids": [1000, 1000, 1000],
-      "io_counters": [5914563584, 9486209024, 0, 0, 0],
+      "io_counters": [9699624960, 15455608832, 0, 0, 0],
       "key": "pid",
-      "memory_info": [409571328, 21839839232, 109895680, 618496, 0, 1071738880, 0],
-      "memory_percent": 5.226667698134628,
+      "memory_info": [524517376, 22345007104, 90595328, 618496, 0, 1481629696, 0],
+      "memory_percent": 6.693530134632704,
       "name": "firefox",
       "nice": 0,
-      "num_threads": 174,
+      "num_threads": 171,
       "pid": 10541,
       "status": "S",
       "time_since_update": 1,
       "username": "nicolargo"},
-     {"cmdline": ["/snap/firefox/2605/usr/lib/firefox/firefox",
-                  "-contentproc",
-                  "-childID",
-                  "2",
-                  "-isForBrowser",
-                  "-prefsLen",
-                  "27003",
-                  "-prefMapSize",
-                  "241898",
-                  "-jsInitLen",
-                  "240056",
-                  "-parentBuildID",
-                  "20230424185118",
-                  "-appDir",
-                  "/snap/firefox/2605/usr/lib/firefox/browser",
-                  "{dbcbe484-8536-44ea-aa85-ba683b538aa8}",
-                  "10541",
-                  "true",
-                  "tab"],
+     {"cmdline": ["/snap/multipass/8465/usr/bin/qemu-system-x86_64",
+                  "-bios",
+                  "OVMF.fd",
+                  "--enable-kvm",
+                  "-cpu",
+                  "host",
+                  "-nic",
+                  "tap,ifname=tap-1e376645a40,script=no,downscript=no,model=virtio-net-pci,mac=52:54:00:05:05:17",
+                  "-device",
+                  "virtio-scsi-pci,id=scsi0",
+                  "-drive",
+                  "file=/var/snap/multipass/common/data/multipassd/vault/instances/primary/ubuntu-22.04-server-cloudimg-amd64.img,if=none,format=qcow2,discard=unmap,id=hda",
+                  "-device",
+                  "scsi-hd,drive=hda,bus=scsi0.0",
+                  "-smp",
+                  "1",
+                  "-m",
+                  "1024M",
+                  "-qmp",
+                  "stdio",
+                  "-chardev",
+                  "null,id=char0",
+                  "-serial",
+                  "chardev:char0",
+                  "-nographic",
+                  "-cdrom",
+                  "/var/snap/multipass/common/data/multipassd/vault/instances/primary/cloud-init-config.iso"],
       "cpu_percent": 0.0,
-      "cpu_times": [1257.75, 117.29, 0.0, 0.0, 0.0],
-      "gids": [1000, 1000, 1000],
-      "io_counters": [301149184, 0, 0, 0, 0],
+      "cpu_times": [846.85, 90.96, 0.0, 0.0, 0.0],
+      "gids": [0, 0, 0],
+      "io_counters": [0, 0, 0, 0, 0],
       "key": "pid",
-      "memory_info": [371560448, 3219562496, 60375040, 618496, 0, 553922560, 0],
-      "memory_percent": 4.741598980937532,
-      "name": "Isolated Web Co",
+      "memory_info": [510238720, 3458437120, 2822144, 5304320, 0, 1366933504, 0],
+      "memory_percent": 6.511315743668364,
+      "name": "qemu-system-x86_64",
       "nice": 0,
-      "num_threads": 22,
-      "pid": 10770,
+      "num_threads": 4,
+      "pid": 354319,
       "status": "S",
       "time_since_update": 1,
-      "username": "nicolargo"}]
+      "username": "root"}]
 
 Get a specific field::
 
     # curl http://localhost:61208/api/3/processlist/pid
     {"pid": [10541,
+             354319,
              10770,
-             59195,
-             60503,
              11043,
-             59454,
+             374779,
+             374071,
              3927,
+             469948,
+             374587,
+             317865,
              10778,
              10774,
-             55857,
-             296364,
-             277461,
-             293836,
-             261989,
-             307573,
-             297410,
+             429788,
+             59195,
+             469241,
+             399766,
+             430971,
+             372037,
              11646,
-             4288,
              59069,
-             314895,
-             10790,
-             315078,
-             315445,
-             314927,
-             294622,
+             374904,
              10733,
-             306969,
-             59523,
-             313257,
-             421,
+             480322,
+             480143,
+             480228,
+             374842,
+             435889,
+             10790,
              59161,
-             315564,
-             315575,
-             60104,
-             60232,
-             4385,
-             195248,
+             480580,
+             59523,
              4243,
+             421,
+             480591,
+             466459,
+             374575,
+             374705,
              3810,
-             315023,
-             59182,
-             2398,
-             281405,
-             307822,
+             457618,
+             466460,
+             374905,
+             372303,
+             4385,
              165661,
-             59525,
-             56140,
-             1771,
-             4023,
-             60191,
-             313283,
+             417207,
+             463383,
              1618,
-             60192,
-             2636,
-             3730,
+             1771,
+             372048,
+             372151,
+             2398,
+             372186,
+             372172,
+             59182,
              4339,
-             11380,
+             374703,
+             313257,
+             2636,
+             431242,
+             374702,
+             4023,
+             4666,
              1,
-             60489,
+             3730,
+             4179,
+             59663,
              1584,
-             3115,
-             299963,
-             195141,
-             4090,
+             427863,
              4075,
-             4000,
-             313650,
-             4666,
-             59663,
-             3719,
-             4179,
+             10710,
              17997,
+             430855,
+             4308,
+             4091,
              1630,
              1605,
-             4086,
-             4091,
-             60106,
-             4169,
-             4046,
              4403,
-             3908,
-             143263,
-             4308,
-             60134,
-             143262,
-             74953,
-             4126,
-             1794,
+             4000,
              4009,
-             3901,
+             4090,
              3991,
-             36919,
-             3956,
-             4442,
+             3719,
              11381,
-             4080,
-             1583,
-             3743,
-             4302,
-             2116,
+             11380,
+             1794,
+             372168,
+             431219,
+             479905,
+             372170,
+             354726,
+             4169,
+             372169,
+             4086,
+             1727,
+             4033,
+             3745,
+             4105,
+             3901,
              3710,
+             4442,
+             3908,
+             4046,
              4127,
-             4105,
-             59126,
-             289122,
+             36919,
+             1631,
+             3743,
+             14243,
+             1583,
+             4302,
+             3956,
+             1379,
+             418247,
+             74953,
+             4126,
+             3748,
+             3115,
              20173,
-             2168,
-             2607,
-             3745,
-             10710,
-             56119,
+             14266,
+             1591,
              4196,
+             59126,
+             2116,
              4005,
-             1379,
-             4244,
-             289100,
+             1764,
+             4316,
+             4145,
+             4097,
+             4080,
+             1627,
+             2168,
+             2607,
+             1818,
+             3989,
+             1579,
+             1628,
+             3925,
              4079,
+             4244,
+             4157,
+             3970,
+             59127,
+             2554,
              4099,
-             227509,
-             1818,
+             1612,
+             3819,
+             1380,
              4078,
+             10848,
              2341,
-             14266,
-             59127,
              1566,
-             2554,
-             4145,
-             1591,
-             16182,
-             14243,
+             227509,
+             1598,
              1624,
-             1628,
-             3925,
-             1764,
-             3947,
-             1612,
-             3939,
              4119,
-             4316,
-             1598,
-             3819,
              4074,
-             3952,
+             3825,
+             3947,
              4098,
-             4107,
-             3748,
-             3970,
-             4033,
-             313277,
              4062,
-             3989,
-             4157,
-             3825,
-             10848,
+             3939,
+             4107,
              3975,
              3753,
+             3952,
+             1575,
              1606,
+             313277,
              461,
-             1631,
-             3934,
-             1579,
-             4097,
-             1825,
-             1627,
-             1575,
-             315523,
+             354741,
              1593,
-             1616,
+             480538,
+             3934,
+             3728,
              12480,
-             261973,
              3888,
+             1616,
              59145,
-             1377,
              12489,
-             3727,
-             1380,
+             1377,
              1582,
              18045,
-             1964,
              4332,
-             3728,
+             1964,
+             1825,
+             3727,
+             59130,
              1634,
-             3118,
-             2361,
+             16182,
              1391,
-             1727,
+             2361,
+             2605,
+             1577,
+             3118,
              2604,
              1390,
-             2605,
              12483,
              1567,
+             431184,
              20396,
+             354739,
+             431178,
+             431203,
              20180,
-             315563,
+             480579,
+             431197,
              4072,
              2358,
-             20400,
-             59130,
-             3498,
+             469137,
+             3503,
              12492,
-             314768,
-             56087,
-             56106,
-             1725,
              1726,
+             1725,
              3794,
+             3498,
              3499,
-             56100,
-             56081,
-             3503,
              3720,
+             20400,
+             313283,
              2345,
-             4593,
              2382,
+             4593,
              2360,
-             20185,
-             1637,
              1392,
-             1577,
+             1637,
+             3573,
+             20185,
              2,
              3,
              4,
              5,
              6,
              8,
              10,
@@ -994,81 +1032,97 @@
              1031,
              1032,
              1033,
              1034,
              1035,
              1036,
              1037,
-             2138,
-             2140,
-             2141,
-             2142,
-             2143,
              2394,
              2410,
              2422,
              2491,
              2492,
              2493,
              2506,
              2508,
              2510,
              2515,
              2525,
-             3573,
              3988,
              12486,
-             288792,
-             288793,
-             288795,
-             304692,
-             306042,
-             307710,
-             307711,
-             307713,
-             307714,
-             307715,
-             307764,
-             309333,
-             310964,
-             311618,
-             311630,
-             313395,
              313404,
-             313720,
-             313725,
-             313896,
-             314273,
-             314367,
-             314371,
-             314524,
-             315132,
-             315249,
-             315374]}
+             354325,
+             354329,
+             417249,
+             417250,
+             417251,
+             417252,
+             417254,
+             417255,
+             417257,
+             417258,
+             417259,
+             417260,
+             417261,
+             417262,
+             417263,
+             417264,
+             417265,
+             417266,
+             417267,
+             427608,
+             427609,
+             427611,
+             454059,
+             459092,
+             463267,
+             463268,
+             463271,
+             463272,
+             463274,
+             463320,
+             467345,
+             467496,
+             468536,
+             468902,
+             469637,
+             469929,
+             470092,
+             471704,
+             476042,
+             477638,
+             478302,
+             479060,
+             479698,
+             479767,
+             480036,
+             480278,
+             480424,
+             480454]}
 
 Get a specific item when field matchs the given value::
 
     # curl http://localhost:61208/api/3/processlist/pid/10541
     {"10541": [{"cmdline": ["/snap/firefox/2605/usr/lib/firefox/firefox"],
                 "cpu_percent": 0.0,
-                "cpu_times": [9681.14, 2938.04, 7162.98, 1045.12, 0.0],
+                "cpu_times": [16463.82, 5059.85, 11961.09, 1725.84, 0.0],
                 "gids": [1000, 1000, 1000],
-                "io_counters": [5914563584, 9486209024, 0, 0, 0],
+                "io_counters": [9699624960, 15455608832, 0, 0, 0],
                 "key": "pid",
-                "memory_info": [409571328,
-                                21839839232,
-                                109895680,
+                "memory_info": [524517376,
+                                22345007104,
+                                90595328,
                                 618496,
                                 0,
-                                1071738880,
+                                1481629696,
                                 0],
-                "memory_percent": 5.226667698134628,
+                "memory_percent": 6.693530134632704,
                 "name": "firefox",
                 "nice": 0,
-                "num_threads": 174,
+                "num_threads": 171,
                 "pid": 10541,
                 "status": "S",
                 "time_since_update": 1,
                 "username": "nicolargo"}]}
 
 GET psutilversion
 -----------------
@@ -1080,77 +1134,77 @@
 
 GET quicklook
 -------------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/quicklook
-    {"cpu": 42.1,
+    {"cpu": 62.2,
      "cpu_hz": 2025000000.0,
-     "cpu_hz_current": 1264730000.0,
+     "cpu_hz_current": 1273980750.0,
      "cpu_name": "Intel(R) Core(TM) i7-4500U CPU @ 1.80GHz",
-     "mem": 64.4,
+     "mem": 75.0,
      "percpu": [{"cpu_number": 0,
-                 "guest": 0.0,
+                 "guest": 1.5,
                  "guest_nice": 0.0,
-                 "idle": 71.1,
-                 "iowait": 0.0,
+                 "idle": 26.2,
+                 "iowait": 1.5,
                  "irq": 0.0,
                  "key": "cpu_number",
                  "nice": 0.0,
                  "softirq": 0.0,
                  "steal": 0.0,
-                 "system": 6.2,
-                 "total": 28.9,
-                 "user": 22.7},
+                 "system": 4.4,
+                 "total": 73.8,
+                 "user": 68.0},
                 {"cpu_number": 1,
                  "guest": 0.0,
                  "guest_nice": 0.0,
-                 "idle": 72.1,
-                 "iowait": 0.0,
+                 "idle": 39.4,
+                 "iowait": 1.0,
                  "irq": 0.0,
                  "key": "cpu_number",
                  "nice": 0.0,
                  "softirq": 0.0,
                  "steal": 0.0,
-                 "system": 8.5,
-                 "total": 27.9,
-                 "user": 19.4},
+                 "system": 4.8,
+                 "total": 60.6,
+                 "user": 54.8},
                 {"cpu_number": 2,
-                 "guest": 0.0,
+                 "guest": 0.5,
                  "guest_nice": 0.0,
-                 "idle": 27.9,
-                 "iowait": 0.0,
+                 "idle": 36.0,
+                 "iowait": 4.3,
                  "irq": 0.0,
                  "key": "cpu_number",
                  "nice": 0.0,
-                 "softirq": 0.0,
+                 "softirq": 0.9,
                  "steal": 0.0,
-                 "system": 3.3,
-                 "total": 72.1,
-                 "user": 68.9},
+                 "system": 9.5,
+                 "total": 64.0,
+                 "user": 49.3},
                 {"cpu_number": 3,
-                 "guest": 0.0,
+                 "guest": 2.8,
                  "guest_nice": 0.0,
-                 "idle": 58.9,
-                 "iowait": 0.0,
+                 "idle": 36.6,
+                 "iowait": 6.5,
                  "irq": 0.0,
                  "key": "cpu_number",
                  "nice": 0.0,
                  "softirq": 0.0,
                  "steal": 0.0,
-                 "system": 4.8,
-                 "total": 41.1,
-                 "user": 36.3}],
-     "swap": 49.9}
+                 "system": 12.5,
+                 "total": 63.4,
+                 "user": 44.4}],
+     "swap": 62.7}
 
 Get a specific field::
 
     # curl http://localhost:61208/api/3/quicklook/cpu
-    {"cpu": 42.1}
+    {"cpu": 62.2}
 
 GET sensors
 -----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/sensors
@@ -1213,15 +1267,15 @@
 
 GET uptime
 ----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/3/uptime
-    "10 days, 4:38:59"
+    "12 days, 3:42:29"
 
 GET all stats
 -------------
 
 Get all Glances stats::
 
     # curl http://localhost:61208/api/3/all
@@ -1229,41 +1283,41 @@
 
 GET stats history
 -----------------
 
 History of a plugin::
 
     # curl http://localhost:61208/api/3/cpu/history
-    {"system": [["2023-05-18T17:40:45.904909", 6.6],
-                ["2023-05-18T17:40:47.072443", 6.6],
-                ["2023-05-18T17:40:48.253286", 3.3]],
-     "user": [["2023-05-18T17:40:45.904887", 37.5],
-              ["2023-05-18T17:40:47.072437", 37.5],
-              ["2023-05-18T17:40:48.253279", 18.3]]}
+    {"system": [["2023-05-20T16:44:17.685943", 7.7],
+                ["2023-05-20T16:44:18.817737", 7.7],
+                ["2023-05-20T16:44:19.996995", 1.1]],
+     "user": [["2023-05-20T16:44:17.685935", 50.0],
+              ["2023-05-20T16:44:18.817731", 50.0],
+              ["2023-05-20T16:44:19.996988", 4.3]]}
 
 Limit history to last 2 values::
 
     # curl http://localhost:61208/api/3/cpu/history/2
-    {"system": [["2023-05-18T17:40:47.072443", 6.6],
-                ["2023-05-18T17:40:48.253286", 3.3]],
-     "user": [["2023-05-18T17:40:47.072437", 37.5],
-              ["2023-05-18T17:40:48.253279", 18.3]]}
+    {"system": [["2023-05-20T16:44:18.817737", 7.7],
+                ["2023-05-20T16:44:19.996995", 1.1]],
+     "user": [["2023-05-20T16:44:18.817731", 50.0],
+              ["2023-05-20T16:44:19.996988", 4.3]]}
 
 History for a specific field::
 
     # curl http://localhost:61208/api/3/cpu/system/history
-    {"system": [["2023-05-18T17:40:45.904909", 6.6],
-                ["2023-05-18T17:40:47.072443", 6.6],
-                ["2023-05-18T17:40:48.253286", 3.3]]}
+    {"system": [["2023-05-20T16:44:17.685943", 7.7],
+                ["2023-05-20T16:44:18.817737", 7.7],
+                ["2023-05-20T16:44:19.996995", 1.1]]}
 
 Limit history for a specific field to last 2 values::
 
     # curl http://localhost:61208/api/3/cpu/system/history
-    {"system": [["2023-05-18T17:40:47.072443", 6.6],
-                ["2023-05-18T17:40:48.253286", 3.3]]}
+    {"system": [["2023-05-20T16:44:18.817737", 7.7],
+                ["2023-05-20T16:44:19.996995", 1.1]]}
 
 GET limits (used for thresholds)
 --------------------------------
 
 All limits/thresholds::
 
     # curl http://localhost:61208/api/3/all/limits
```

### Comparing `Glances-3.4.0.2/docs/cmds.rst` & `Glances-3.4.0.3/docs/cmds.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/conf.py` & `Glances-3.4.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/config.rst` & `Glances-3.4.0.3/docs/config.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/dev/glances-cprofile.png` & `Glances-3.4.0.3/docs/dev/glances-cprofile.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/docker.rst` & `Glances-3.4.0.3/docs/docker.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/glances.rst` & `Glances-3.4.0.3/docs/glances.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/gw/cassandra.rst` & `Glances-3.4.0.3/docs/gw/cassandra.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/gw/couchdb.rst` & `Glances-3.4.0.3/docs/gw/couchdb.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/gw/csv.rst` & `Glances-3.4.0.3/docs/gw/csv.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/gw/graph.rst` & `Glances-3.4.0.3/docs/gw/graph.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/gw/graphite.rst` & `Glances-3.4.0.3/docs/gw/graphite.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/gw/influxdb.rst` & `Glances-3.4.0.3/docs/gw/influxdb.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/gw/kafka.rst` & `Glances-3.4.0.3/docs/gw/kafka.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/gw/mongodb.rst` & `Glances-3.4.0.3/docs/gw/mongodb.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/gw/mqtt.rst` & `Glances-3.4.0.3/docs/gw/mqtt.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/gw/prometheus.rst` & `Glances-3.4.0.3/docs/gw/prometheus.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/gw/restful.rst` & `Glances-3.4.0.3/docs/gw/restful.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/gw/statsd.rst` & `Glances-3.4.0.3/docs/gw/statsd.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/gw/zeromq.rst` & `Glances-3.4.0.3/docs/gw/zeromq.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/index.rst` & `Glances-3.4.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/install.rst` & `Glances-3.4.0.3/docs/install.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/make.bat` & `Glances-3.4.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/man/glances.1` & `Glances-3.4.0.3/docs/man/glances.1`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "GLANCES" "1" "May 18, 2023" "3.4.0.2" "Glances"
+.TH "GLANCES" "1" "May 20, 2023" "3.4.0.3" "Glances"
 .SH NAME
 glances \- An eye on your system
 .SH SYNOPSIS
 .sp
 \fBglances\fP [OPTIONS]
 .SH DESCRIPTION
 .sp
```

### Comparing `Glances-3.4.0.2/docs/objects.inv` & `Glances-3.4.0.3/docs/objects.inv`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/docs/quickstart.rst` & `Glances-3.4.0.3/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/__init__.py` & `Glances-3.4.0.3/glances/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import platform
 import signal
 import sys
 
 # Global name
 # Version should start and end with a numerical char
 # See https://packaging.python.org/specifications/core-metadata/#version
-__version__ = '3.4.0.2'
+__version__ = '3.4.0.3'
 __author__ = 'Nicolas Hennion <nicolas@nicolargo.com>'
 __license__ = 'LGPLv3'
 
 # Import psutil
 try:
     from psutil import __version__ as psutil_version
 except ImportError:
```

### Comparing `Glances-3.4.0.2/glances/actions.py` & `Glances-3.4.0.3/glances/actions.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/amps/glances_amp.py` & `Glances-3.4.0.3/glances/amps/glances_amp.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/amps/glances_default.py` & `Glances-3.4.0.3/glances/amps/glances_default.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/amps/glances_nginx.py` & `Glances-3.4.0.3/glances/amps/glances_nginx.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/amps/glances_systemd.py` & `Glances-3.4.0.3/glances/amps/glances_systemd.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/amps/glances_systemv.py` & `Glances-3.4.0.3/glances/amps/glances_systemv.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/amps_list.py` & `Glances-3.4.0.3/glances/amps_list.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/attribute.py` & `Glances-3.4.0.3/glances/attribute.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/autodiscover.py` & `Glances-3.4.0.3/glances/autodiscover.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/client.py` & `Glances-3.4.0.3/glances/client.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/client_browser.py` & `Glances-3.4.0.3/glances/client_browser.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/compat.py` & `Glances-3.4.0.3/glances/compat.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/config.py` & `Glances-3.4.0.3/glances/config.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/cpu_percent.py` & `Glances-3.4.0.3/glances/cpu_percent.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/events.py` & `Glances-3.4.0.3/glances/events.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/exports/glances_cassandra.py` & `Glances-3.4.0.3/glances/exports/glances_cassandra.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/exports/glances_couchdb.py` & `Glances-3.4.0.3/glances/exports/glances_couchdb.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/exports/glances_csv.py` & `Glances-3.4.0.3/glances/exports/glances_csv.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/exports/glances_elasticsearch.py` & `Glances-3.4.0.3/glances/exports/glances_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/exports/glances_export.py` & `Glances-3.4.0.3/glances/exports/glances_export.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/exports/glances_graph.py` & `Glances-3.4.0.3/glances/exports/glances_graph.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/exports/glances_graphite.py` & `Glances-3.4.0.3/glances/exports/glances_graphite.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/exports/glances_influxdb.py` & `Glances-3.4.0.3/glances/exports/glances_influxdb.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/exports/glances_influxdb2.py` & `Glances-3.4.0.3/glances/exports/glances_influxdb2.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/exports/glances_json.py` & `Glances-3.4.0.3/glances/exports/glances_json.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/exports/glances_kafka.py` & `Glances-3.4.0.3/glances/exports/glances_kafka.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/exports/glances_mongodb.py` & `Glances-3.4.0.3/glances/exports/glances_mongodb.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/exports/glances_mqtt.py` & `Glances-3.4.0.3/glances/exports/glances_mqtt.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/exports/glances_opentsdb.py` & `Glances-3.4.0.3/glances/exports/glances_opentsdb.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/exports/glances_prometheus.py` & `Glances-3.4.0.3/glances/exports/glances_prometheus.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/exports/glances_rabbitmq.py` & `Glances-3.4.0.3/glances/exports/glances_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/exports/glances_restful.py` & `Glances-3.4.0.3/glances/exports/glances_restful.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/exports/glances_riemann.py` & `Glances-3.4.0.3/glances/exports/glances_riemann.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/exports/glances_statsd.py` & `Glances-3.4.0.3/glances/exports/glances_statsd.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/exports/glances_zeromq.py` & `Glances-3.4.0.3/glances/exports/glances_zeromq.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/filter.py` & `Glances-3.4.0.3/glances/filter.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/folder_list.py` & `Glances-3.4.0.3/glances/folder_list.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/globals.py` & `Glances-3.4.0.3/glances/globals.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/history.py` & `Glances-3.4.0.3/glances/history.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/logger.py` & `Glances-3.4.0.3/glances/logger.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/main.py` & `Glances-3.4.0.3/glances/main.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outdated.py` & `Glances-3.4.0.3/glances/outdated.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/glances_bars.py` & `Glances-3.4.0.3/glances/outputs/glances_bars.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/glances_bottle.py` & `Glances-3.4.0.3/glances/outputs/glances_bottle.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/glances_curses.py` & `Glances-3.4.0.3/glances/outputs/glances_curses.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/glances_curses_browser.py` & `Glances-3.4.0.3/glances/outputs/glances_curses_browser.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/glances_sparklines.py` & `Glances-3.4.0.3/glances/outputs/glances_sparklines.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/glances_stdout.py` & `Glances-3.4.0.3/glances/outputs/glances_stdout.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/glances_stdout_apidoc.py` & `Glances-3.4.0.3/glances/outputs/glances_stdout_apidoc.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/glances_stdout_csv.py` & `Glances-3.4.0.3/glances/outputs/glances_stdout_csv.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/glances_stdout_issue.py` & `Glances-3.4.0.3/glances/outputs/glances_stdout_issue.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/glances_stdout_json.py` & `Glances-3.4.0.3/glances/outputs/glances_stdout_json.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/glances_unicode.py` & `Glances-3.4.0.3/glances/outputs/glances_unicode.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/README.md` & `Glances-3.4.0.3/glances/outputs/static/README.md`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/css/bootstrap.less` & `Glances-3.4.0.3/glances/outputs/static/css/bootstrap.less`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/css/style.scss` & `Glances-3.4.0.3/glances/outputs/static/css/style.scss`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/images/favicon.ico` & `Glances-3.4.0.3/glances/outputs/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/images/glances.png` & `Glances-3.4.0.3/glances/outputs/static/images/glances.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/js/App.vue` & `Glances-3.4.0.3/glances/outputs/static/js/App.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/js/components/help.vue` & `Glances-3.4.0.3/glances/outputs/static/js/components/help.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-alert.vue` & `Glances-3.4.0.3/glances/outputs/static/js/components/plugin-alert.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-amps.vue` & `Glances-3.4.0.3/glances/outputs/static/js/components/plugin-amps.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-cloud.vue` & `Glances-3.4.0.3/glances/outputs/static/js/components/plugin-cloud.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-connections.vue` & `Glances-3.4.0.3/glances/outputs/static/js/components/plugin-connections.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-containers.vue` & `Glances-3.4.0.3/glances/outputs/static/js/components/plugin-containers.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-cpu.vue` & `Glances-3.4.0.3/glances/outputs/static/js/components/plugin-cpu.vue`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <template>
     <section id="cpu" class="plugin">
         <div class="row">
             <div class="col-sm-24 col-md-12 col-lg-8">
                 <div class="table">
                     <div class="table-row">
                         <div class="table-cell text-left title">CPU</div>
-                        <div class="table-cell">{{ total }}%</div>
+                        <div class="table-cell" :class="getDecoration('total')">{{ total }}%</div>
                     </div>
                     <div class="table-row">
                         <div class="table-cell text-left">user:</div>
                         <div class="table-cell" :class="getDecoration('user')">{{ user }}%</div>
                     </div>
                     <div class="table-row">
                         <div class="table-cell text-left">system:</div>
```

### Comparing `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-diskio.vue` & `Glances-3.4.0.3/glances/outputs/static/js/components/plugin-diskio.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-folders.vue` & `Glances-3.4.0.3/glances/outputs/static/js/components/plugin-folders.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-fs.vue` & `Glances-3.4.0.3/glances/outputs/static/js/components/plugin-fs.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-gpu.vue` & `Glances-3.4.0.3/glances/outputs/static/js/components/plugin-gpu.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-ip.vue` & `Glances-3.4.0.3/glances/outputs/static/js/components/plugin-ip.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-irq.vue` & `Glances-3.4.0.3/glances/outputs/static/js/components/plugin-irq.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-load.vue` & `Glances-3.4.0.3/glances/outputs/static/js/components/plugin-load.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-mem-more.vue` & `Glances-3.4.0.3/glances/outputs/static/js/components/plugin-mem-more.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-mem.vue` & `Glances-3.4.0.3/glances/outputs/static/js/components/plugin-mem.vue`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <template>
     <section id="mem" class="plugin">
         <div class="table">
             <div class="table-row">
                 <div class="table-cell text-left title">MEM</div>
-                <div class="table-cell">{{ percent }}%</div>
+                <div class="table-cell" :class="getDecoration('percent')">{{ percent }}%</div>
             </div>
             <div class="table-row">
                 <div class="table-cell text-left">total:</div>
                 <div class="table-cell">{{ $filters.bytes(total) }}</div>
             </div>
             <div class="table-row">
                 <div class="table-cell text-left">used:</div>
```

### Comparing `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-memswap.vue` & `Glances-3.4.0.3/glances/outputs/static/js/components/plugin-memswap.vue`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <template>
     <section id="memswap" class="plugin">
         <div class="table">
             <div class="table-row">
                 <div class="table-cell text-left title">SWAP</div>
-                <div class="table-cell">{{ percent }}%</div>
+                <div class="table-cell" :class="getDecoration('percent')">{{ percent }}%</div>
             </div>
             <div class="table-row">
                 <div class="table-cell text-left">total:</div>
                 <div class="table-cell">{{ $filters.bytes(total) }}</div>
             </div>
             <div class="table-row">
                 <div class="table-cell text-left">used:</div>
```

### Comparing `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-network.vue` & `Glances-3.4.0.3/glances/outputs/static/js/components/plugin-network.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-percpu.vue` & `Glances-3.4.0.3/glances/outputs/static/js/components/plugin-percpu.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-ports.vue` & `Glances-3.4.0.3/glances/outputs/static/js/components/plugin-ports.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-process.vue` & `Glances-3.4.0.3/glances/outputs/static/js/components/plugin-process.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-processcount.vue` & `Glances-3.4.0.3/glances/outputs/static/js/components/plugin-processcount.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-processlist.vue` & `Glances-3.4.0.3/glances/outputs/static/js/components/plugin-processlist.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-quicklook.vue` & `Glances-3.4.0.3/glances/outputs/static/js/components/plugin-quicklook.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-raid.vue` & `Glances-3.4.0.3/glances/outputs/static/js/components/plugin-raid.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-sensors.vue` & `Glances-3.4.0.3/glances/outputs/static/js/components/plugin-sensors.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-system.vue` & `Glances-3.4.0.3/glances/outputs/static/js/components/plugin-system.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/js/components/plugin-wifi.vue` & `Glances-3.4.0.3/glances/outputs/static/js/components/plugin-wifi.vue`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/js/filters.js` & `Glances-3.4.0.3/glances/outputs/static/js/filters.js`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/js/services.js` & `Glances-3.4.0.3/glances/outputs/static/js/services.js`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/package-lock.json` & `Glances-3.4.0.3/glances/outputs/static/package-lock.json`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/package.json` & `Glances-3.4.0.3/glances/outputs/static/package.json`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/public/87708faeed9a66b0fcdb.png` & `Glances-3.4.0.3/glances/outputs/static/public/87708faeed9a66b0fcdb.png`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/public/favicon.ico` & `Glances-3.4.0.3/glances/outputs/static/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/outputs/static/public/glances.js` & `Glances-3.4.0.3/glances/outputs/static/public/glances.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -10768,24 +10768,24 @@
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, n.nmd = e => (e.paths = [], e.children || (e.children = []), e), n.p = "/", n.b = document.baseURI || self.location.href, n.nc = void 0, (() => {
         "use strict";
         var e = {};
         n.r(e), n.d(e, {
-            bits: () => zu,
-            bytes: () => Hu,
-            exclamation: () => Vu,
-            leftPad: () => Gu,
-            limitTo: () => Wu,
-            minSize: () => Zu,
-            nl2br: () => Ku,
-            number: () => Qu,
-            timedelta: () => Ju,
-            timemillis: () => Xu
+            bits: () => $u,
+            bytes: () => zu,
+            exclamation: () => Hu,
+            leftPad: () => Vu,
+            limitTo: () => Gu,
+            minSize: () => Wu,
+            nl2br: () => Zu,
+            number: () => Ku,
+            timedelta: () => Xu,
+            timemillis: () => Qu
         });
         var t = n(3379),
             r = n.n(t),
             i = n(7795),
             s = n.n(i),
             o = n(569),
             a = n.n(o),
@@ -15124,139 +15124,136 @@
             zc = {
                 class: "table-row"
             },
             Hc = wi("div", {
                 class: "table-cell text-left title"
             }, "CPU", -1),
             Vc = {
-                class: "table-cell"
-            },
-            Gc = {
                 class: "table-row"
             },
-            Wc = wi("div", {
+            Gc = wi("div", {
                 class: "table-cell text-left"
             }, "user:", -1),
-            Zc = {
+            Wc = {
                 class: "table-row"
             },
-            Kc = wi("div", {
+            Zc = wi("div", {
                 class: "table-cell text-left"
             }, "system:", -1),
-            Qc = {
+            Kc = {
                 class: "table-row"
             },
-            Xc = wi("div", {
+            Qc = wi("div", {
                 class: "table-cell text-left"
             }, "iowait:", -1),
-            Jc = {
+            Xc = {
                 class: "table-row"
             },
-            Yc = wi("div", {
+            Jc = wi("div", {
                 class: "table-cell text-left"
             }, "dpc:", -1),
-            eu = {
+            Yc = {
                 class: "hidden-xs hidden-sm col-md-12 col-lg-8"
             },
-            tu = {
+            eu = {
                 class: "table"
             },
-            nu = {
+            tu = {
                 class: "table-row"
             },
-            ru = wi("div", {
+            nu = wi("div", {
                 class: "table-cell text-left"
             }, "idle:", -1),
-            iu = {
+            ru = {
                 class: "table-cell"
             },
-            su = {
+            iu = {
                 class: "table-row"
             },
-            ou = wi("div", {
+            su = wi("div", {
                 class: "table-cell text-left"
             }, "irq:", -1),
-            au = {
+            ou = {
                 class: "table-cell"
             },
-            lu = {
+            au = {
                 class: "table-row"
             },
-            cu = wi("div", {
+            lu = wi("div", {
                 class: "table-cell text-left"
             }, "inter:", -1),
-            uu = {
+            cu = {
                 class: "table-cell"
             },
-            du = {
+            uu = {
                 class: "table-row"
             },
-            fu = wi("div", {
+            du = wi("div", {
                 class: "table-cell text-left"
             }, "nice:", -1),
-            pu = {
+            fu = {
                 class: "table-cell"
             },
-            hu = {
+            pu = {
                 key: 0,
                 class: "table-row"
             },
-            gu = wi("div", {
+            hu = wi("div", {
                 class: "table-cell text-left"
             }, "ctx_sw:", -1),
-            mu = {
+            gu = {
                 class: "table-row"
             },
-            bu = wi("div", {
+            mu = wi("div", {
                 class: "table-cell text-left"
             }, "steal:", -1),
-            vu = {
+            bu = {
                 key: 1,
                 class: "table-row"
             },
-            yu = wi("div", {
+            vu = wi("div", {
                 class: "table-cell text-left"
             }, "syscal:", -1),
-            wu = {
+            yu = {
                 class: "table-cell"
             },
-            xu = {
+            wu = {
                 class: "hidden-xs hidden-sm hidden-md col-lg-8"
             },
-            _u = {
+            xu = {
                 class: "table"
             },
-            ku = {
+            _u = {
                 key: 0,
                 class: "table-row"
             },
-            Su = wi("div", {
+            ku = wi("div", {
                 class: "table-cell text-left"
             }, "ctx_sw:", -1),
-            Cu = {
+            Su = {
                 key: 1,
                 class: "table-row"
             },
-            Tu = wi("div", {
+            Cu = wi("div", {
                 class: "table-cell text-left"
             }, "inter:", -1),
-            Au = {
+            Tu = {
                 class: "table-cell"
             },
-            Eu = {
+            Au = {
                 key: 2,
                 class: "table-row"
             },
-            Ou = wi("div", {
+            Eu = wi("div", {
                 class: "table-cell text-left"
             }, "sw_int:", -1),
-            Iu = {
+            Ou = {
                 class: "table-cell"
             };
-        const Pu = {
+        const Iu = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 computed: {
                     stats() {
@@ -15328,79 +15325,81 @@
                 },
                 methods: {
                     getDecoration(e) {
                         if (void 0 !== this.view[e]) return this.view[e].decoration.toLowerCase()
                     }
                 }
             },
-            Nu = (0, ec.Z)(Pu, [
+            Pu = (0, ec.Z)(Iu, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", Bc, [wi("div", Uc, [wi("div", Fc, [wi("div", $c, [wi("div", zc, [Hc, wi("div", Vc, pe(s.total) + "%", 1)]), wi("div", Gc, [Wc, wi("div", {
+                    return li(), pi("section", Bc, [wi("div", Uc, [wi("div", Fc, [wi("div", $c, [wi("div", zc, [Hc, wi("div", {
+                        class: ce(["table-cell", s.getDecoration("total")])
+                    }, pe(s.total) + "%", 3)]), wi("div", Vc, [Gc, wi("div", {
                         class: ce(["table-cell", s.getDecoration("user")])
-                    }, pe(s.user) + "%", 3)]), wi("div", Zc, [Kc, wi("div", {
+                    }, pe(s.user) + "%", 3)]), wi("div", Wc, [Zc, wi("div", {
                         class: ce(["table-cell", s.getDecoration("system")])
-                    }, pe(s.system) + "%", 3)]), On(wi("div", Qc, [Xc, wi("div", {
+                    }, pe(s.system) + "%", 3)]), On(wi("div", Kc, [Qc, wi("div", {
                         class: ce(["table-cell", s.getDecoration("iowait")])
                     }, pe(s.iowait) + "%", 3)], 512), [
                         [Ds, null != s.iowait]
-                    ]), On(wi("div", Jc, [Yc, wi("div", {
+                    ]), On(wi("div", Xc, [Jc, wi("div", {
                         class: ce(["table-cell", s.getDecoration("dpc")])
                     }, pe(s.dpc) + "%", 3)], 512), [
                         [Ds, null == s.iowait && null != s.dpc]
-                    ])])]), wi("div", eu, [wi("div", tu, [wi("div", nu, [ru, wi("div", iu, pe(s.idle) + "%", 1)]), On(wi("div", su, [ou, wi("div", au, pe(s.irq) + "%", 1)], 512), [
+                    ])])]), wi("div", Yc, [wi("div", eu, [wi("div", tu, [nu, wi("div", ru, pe(s.idle) + "%", 1)]), On(wi("div", iu, [su, wi("div", ou, pe(s.irq) + "%", 1)], 512), [
                         [Ds, null != s.irq]
-                    ]), Ti(" If no irq, display interrupts "), On(wi("div", lu, [cu, wi("div", uu, pe(s.interrupts), 1)], 512), [
+                    ]), Ti(" If no irq, display interrupts "), On(wi("div", au, [lu, wi("div", cu, pe(s.interrupts), 1)], 512), [
                         [Ds, null == s.irq]
-                    ]), On(wi("div", du, [fu, wi("div", pu, pe(s.nice) + "%", 1)], 512), [
+                    ]), On(wi("div", uu, [du, wi("div", fu, pe(s.nice) + "%", 1)], 512), [
                         [Ds, null != s.nice]
-                    ]), Ti(" If no nice, display ctx_switches "), null == s.nice && s.ctx_switches ? (li(), pi("div", hu, [gu, wi("div", {
+                    ]), Ti(" If no nice, display ctx_switches "), null == s.nice && s.ctx_switches ? (li(), pi("div", pu, [hu, wi("div", {
                         class: ce(["table-cell", s.getDecoration("ctx_switches")])
-                    }, pe(s.ctx_switches), 3)])) : Ti("v-if", !0), On(wi("div", mu, [bu, wi("div", {
+                    }, pe(s.ctx_switches), 3)])) : Ti("v-if", !0), On(wi("div", gu, [mu, wi("div", {
                         class: ce(["table-cell", s.getDecoration("steal")])
                     }, pe(s.steal) + "%", 3)], 512), [
                         [Ds, null != s.steal]
-                    ]), !s.isLinux && s.syscalls ? (li(), pi("div", vu, [yu, wi("div", wu, pe(s.syscalls), 1)])) : Ti("v-if", !0)])]), wi("div", xu, [wi("div", _u, [Ti(" If not already display instead of nice, then display ctx_switches "), null != s.nice && s.ctx_switches ? (li(), pi("div", ku, [Su, wi("div", {
+                    ]), !s.isLinux && s.syscalls ? (li(), pi("div", bu, [vu, wi("div", yu, pe(s.syscalls), 1)])) : Ti("v-if", !0)])]), wi("div", wu, [wi("div", xu, [Ti(" If not already display instead of nice, then display ctx_switches "), null != s.nice && s.ctx_switches ? (li(), pi("div", _u, [ku, wi("div", {
                         class: ce(["table-cell", s.getDecoration("ctx_switches")])
-                    }, pe(s.ctx_switches), 3)])) : Ti("v-if", !0), Ti(" If not already display instead of irq, then display interrupts "), null != s.irq && s.interrupts ? (li(), pi("div", Cu, [Tu, wi("div", Au, pe(s.interrupts), 1)])) : Ti("v-if", !0), s.isWindows || s.isSunOS || !s.soft_interrupts ? Ti("v-if", !0) : (li(), pi("div", Eu, [Ou, wi("div", Iu, pe(s.soft_interrupts), 1)]))])])])])
+                    }, pe(s.ctx_switches), 3)])) : Ti("v-if", !0), Ti(" If not already display instead of irq, then display interrupts "), null != s.irq && s.interrupts ? (li(), pi("div", Su, [Cu, wi("div", Tu, pe(s.interrupts), 1)])) : Ti("v-if", !0), s.isWindows || s.isSunOS || !s.soft_interrupts ? Ti("v-if", !0) : (li(), pi("div", Au, [Eu, wi("div", Ou, pe(s.soft_interrupts), 1)]))])])])])
                 }]
             ]),
-            Lu = {
+            Nu = {
                 class: "plugin",
                 id: "diskio"
             },
-            Du = {
+            Lu = {
                 key: 0,
                 class: "table-row"
             },
-            Mu = wi("div", {
+            Du = wi("div", {
                 class: "table-cell text-left title"
             }, "DISK I/O", -1),
+            Mu = {
+                class: "table-cell"
+            },
             ju = {
                 class: "table-cell"
             },
             Ru = {
                 class: "table-cell"
             },
             qu = {
                 class: "table-cell"
             },
             Bu = {
-                class: "table-cell"
-            },
-            Uu = {
                 class: "table-cell text-left"
             };
-        var Fu = n(1036),
-            $u = n.n(Fu);
+        var Uu = n(1036),
+            Fu = n.n(Uu);
 
-        function zu(e, t) {
-            return Hu(e = 8 * Math.round(e), t) + "b"
+        function $u(e, t) {
+            return zu(e = 8 * Math.round(e), t) + "b"
         }
 
-        function Hu(e, t) {
+        function zu(e, t) {
             if (t = t || !1, isNaN(parseFloat(e)) || !isFinite(e) || 0 == e) return e;
             const n = ["Y", "Z", "E", "P", "T", "G", "M", "K"],
                 r = {
                     Y: 12089258196146292e8,
                     Z: 11805916207174113e5,
                     E: 0x1000000000000000,
                     P: 0x4000000000000,
@@ -15416,63 +15415,63 @@
                     var a = 0;
                     return o < 10 ? a = 2 : o < 100 && (a = 1), t ? a = "MK" == s ? 0 : (0, cc.min)([1, a]) : "K" == s && (a = 0), parseFloat(o).toFixed(a) + s
                 }
             }
             return e.toFixed(0)
         }
 
-        function Vu(e) {
+        function Hu(e) {
             return void 0 === e || "" === e ? "?" : e
         }
 
-        function Gu(e, t, n) {
+        function Vu(e, t, n) {
             return t = t || 0, n = n || " ", String(e).padStart(t, n)
         }
 
-        function Wu(e, t) {
+        function Gu(e, t) {
             return "function" != typeof e.slice && (e = String(e)), e.slice(0, t)
         }
 
-        function Zu(e, t) {
+        function Wu(e, t) {
             return t = t || 8, e.length > t ? "_" + e.substring(e.length - t + 1) : e
         }
 
-        function Ku(e) {
+        function Zu(e) {
             if (void 0 === e) return e;
             var t = function(e) {
                     var t = document.createElement("div");
                     return t.innerText = e, t.innerHTML
                 }(e),
                 n = t.replace(/\n/g, "<br>");
-            return $u()(n)
+            return Fu()(n)
         }
 
-        function Qu(e, t) {
+        function Ku(e, t) {
             return new Intl.NumberFormat(void 0, "number" == typeof t ? {
                 maximumFractionDigits: t
             } : t).format(e)
         }
 
-        function Xu(e) {
+        function Qu(e) {
             for (var t = 0, n = 0; n < e.length; n++) t += 1e3 * e[n];
             return t
         }
 
-        function Ju(e) {
-            var t = Xu(e),
+        function Xu(e) {
+            var t = Qu(e),
                 n = new Date(t),
                 r = Math.floor((n - new Date(n.getFullYear(), 0, 0)) / 1e3 / 60 / 60 / 24);
             return {
                 hours: n.getUTCHours() + 24 * (r - 1),
                 minutes: n.getUTCMinutes(),
                 seconds: n.getUTCSeconds(),
                 milliseconds: parseInt("" + n.getUTCMilliseconds() / 10)
             }
         }
-        const Yu = {
+        const Ju = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 data: () => ({
                     store: qo
@@ -15486,42 +15485,42 @@
                     },
                     disks() {
                         const e = this.stats.map((e => {
                             const t = e.time_since_update;
                             return {
                                 name: e.disk_name,
                                 bitrate: {
-                                    txps: Hu(e.read_bytes / t),
-                                    rxps: Hu(e.write_bytes / t)
+                                    txps: zu(e.read_bytes / t),
+                                    rxps: zu(e.write_bytes / t)
                                 },
                                 count: {
-                                    txps: Hu(e.read_count / t),
-                                    rxps: Hu(e.write_count / t)
+                                    txps: zu(e.read_count / t),
+                                    rxps: zu(e.write_count / t)
                                 },
                                 alias: void 0 !== e.alias ? e.alias : null
                             }
                         }));
                         return (0, cc.orderBy)(e, ["name"])
                     }
                 }
             },
-            ed = (0, ec.Z)(Yu, [
+            Yu = (0, ec.Z)(Ju, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", Lu, [s.disks.length > 0 ? (li(), pi("div", Du, [Mu, On(wi("div", ju, "R/s", 512), [
+                    return li(), pi("section", Nu, [s.disks.length > 0 ? (li(), pi("div", Lu, [Du, On(wi("div", Mu, "R/s", 512), [
                         [Ds, !s.args.diskio_iops]
-                    ]), On(wi("div", Ru, "W/s", 512), [
+                    ]), On(wi("div", ju, "W/s", 512), [
                         [Ds, !s.args.diskio_iops]
-                    ]), On(wi("div", qu, "IOR/s", 512), [
+                    ]), On(wi("div", Ru, "IOR/s", 512), [
                         [Ds, s.args.diskio_iops]
-                    ]), On(wi("div", Bu, "IOW/s", 512), [
+                    ]), On(wi("div", qu, "IOW/s", 512), [
                         [Ds, s.args.diskio_iops]
                     ])])) : Ti("v-if", !0), (li(!0), pi(ni, null, pr(s.disks, ((t, n) => (li(), pi("div", {
                         class: "table-row",
                         key: n
-                    }, [wi("div", Uu, pe(e.$filters.minSize(t.alias ? t.alias : t.name, 32)), 1), On(wi("div", {
+                    }, [wi("div", Bu, pe(e.$filters.minSize(t.alias ? t.alias : t.name, 32)), 1), On(wi("div", {
                         class: "table-cell"
                     }, pe(t.bitrate.txps), 513), [
                         [Ds, !s.args.diskio_iops]
                     ]), On(wi("div", {
                         class: "table-cell"
                     }, pe(t.bitrate.rxps), 513), [
                         [Ds, !s.args.diskio_iops]
@@ -15532,49 +15531,52 @@
                     ]), On(wi("div", {
                         class: "table-cell"
                     }, pe(t.count.rxps), 513), [
                         [Ds, s.args.diskio_iops]
                     ])])))), 128))])
                 }]
             ]),
-            td = {
+            ed = {
                 key: 0,
                 id: "containers-plugin",
                 class: "plugin"
             },
-            nd = wi("span", {
+            td = wi("span", {
                 class: "title"
             }, "CONTAINERS", -1),
-            rd = {
+            nd = {
                 class: "table"
             },
-            id = {
+            rd = {
                 class: "table-row"
             },
-            sd = wi("div", {
+            id = wi("div", {
                 class: "table-cell text-left"
             }, "Engine", -1),
-            od = wi("div", {
+            sd = wi("div", {
                 class: "table-cell text-left"
             }, "Pod", -1),
-            ad = wi("div", {
+            od = wi("div", {
                 class: "table-cell"
             }, "Status", -1),
-            ld = wi("div", {
+            ad = wi("div", {
                 class: "table-cell"
             }, "Uptime", -1),
-            cd = Ci('<div class="table-cell">/MAX</div><div class="table-cell">IOR/s</div><div class="table-cell">IOW/s</div><div class="table-cell">RX/s</div><div class="table-cell">TX/s</div><div class="table-cell text-left">Command</div>', 6),
+            ld = Ci('<div class="table-cell">/MAX</div><div class="table-cell">IOR/s</div><div class="table-cell">IOW/s</div><div class="table-cell">RX/s</div><div class="table-cell">TX/s</div><div class="table-cell text-left">Command</div>', 6),
+            cd = {
+                class: "table-cell text-left"
+            },
             ud = {
                 class: "table-cell text-left"
             },
             dd = {
                 class: "table-cell text-left"
             },
             fd = {
-                class: "table-cell text-left"
+                class: "table-cell"
             },
             pd = {
                 class: "table-cell"
             },
             hd = {
                 class: "table-cell"
             },
@@ -15590,20 +15592,17 @@
             vd = {
                 class: "table-cell"
             },
             yd = {
                 class: "table-cell"
             },
             wd = {
-                class: "table-cell"
-            },
-            xd = {
                 class: "table-cell text-left"
             };
-        const _d = {
+        const xd = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 data: () => ({
                     store: qo,
@@ -15665,55 +15664,55 @@
                                     } [e] || e
                                 }
                             })
                         }
                     }
                 }
             },
-            kd = (0, ec.Z)(_d, [
+            _d = (0, ec.Z)(xd, [
                 ["render", function(e, t, n, r, i, s) {
-                    return s.containers.length ? (li(), pi("section", td, [nd, Si(" " + pe(s.containers.length) + " sorted by " + pe(i.sorter.getColumnLabel(i.sorter.column)) + " ", 1), wi("div", rd, [wi("div", id, [sd, od, wi("div", {
+                    return s.containers.length ? (li(), pi("section", ed, [td, Si(" " + pe(s.containers.length) + " sorted by " + pe(i.sorter.getColumnLabel(i.sorter.column)) + " ", 1), wi("div", nd, [wi("div", rd, [id, sd, wi("div", {
                         class: ce(["table-cell text-left", ["sortable", "name" === i.sorter.column && "sort"]]),
                         onClick: t[0] || (t[0] = e => s.args.sort_processes_key = "name")
-                    }, " Name ", 2), ad, ld, wi("div", {
+                    }, " Name ", 2), od, ad, wi("div", {
                         class: ce(["table-cell", ["sortable", "cpu_percent" === i.sorter.column && "sort"]]),
                         onClick: t[1] || (t[1] = e => s.args.sort_processes_key = "cpu_percent")
                     }, " CPU% ", 2), wi("div", {
                         class: ce(["table-cell", ["sortable", "memory_percent" === i.sorter.column && "sort"]]),
                         onClick: t[2] || (t[2] = e => s.args.sort_processes_key = "memory_percent")
-                    }, " MEM ", 2), cd]), (li(!0), pi(ni, null, pr(s.containers, ((t, n) => (li(), pi("div", {
+                    }, " MEM ", 2), ld]), (li(!0), pi(ni, null, pr(s.containers, ((t, n) => (li(), pi("div", {
                         class: "table-row",
                         key: n
-                    }, [wi("div", ud, pe(t.engine), 1), wi("div", dd, pe(t.pod_id || "-"), 1), wi("div", fd, pe(t.name), 1), wi("div", {
+                    }, [wi("div", cd, pe(t.engine), 1), wi("div", ud, pe(t.pod_id || "-"), 1), wi("div", dd, pe(t.name), 1), wi("div", {
                         class: ce(["table-cell", "Paused" == t.status ? "careful" : "ok"])
-                    }, pe(t.status), 3), wi("div", pd, pe(t.uptime), 1), wi("div", hd, pe(e.$filters.number(t.cpu_percent, 1)), 1), wi("div", gd, pe(e.$filters.bytes(t.memory_usage)), 1), wi("div", md, pe(e.$filters.bytes(t.limit)), 1), wi("div", bd, pe(e.$filters.bits(t.ior / t.io_time_since_update)), 1), wi("div", vd, pe(e.$filters.bits(t.iow / t.io_time_since_update)), 1), wi("div", yd, pe(e.$filters.bits(t.rx / t.net_time_since_update)), 1), wi("div", wd, pe(e.$filters.bits(t.tx / t.net_time_since_update)), 1), wi("div", xd, pe(t.command), 1)])))), 128))])])) : Ti("v-if", !0)
+                    }, pe(t.status), 3), wi("div", fd, pe(t.uptime), 1), wi("div", pd, pe(e.$filters.number(t.cpu_percent, 1)), 1), wi("div", hd, pe(e.$filters.bytes(t.memory_usage)), 1), wi("div", gd, pe(e.$filters.bytes(t.limit)), 1), wi("div", md, pe(e.$filters.bits(t.ior / t.io_time_since_update)), 1), wi("div", bd, pe(e.$filters.bits(t.iow / t.io_time_since_update)), 1), wi("div", vd, pe(e.$filters.bits(t.rx / t.net_time_since_update)), 1), wi("div", yd, pe(e.$filters.bits(t.tx / t.net_time_since_update)), 1), wi("div", wd, pe(t.command), 1)])))), 128))])])) : Ti("v-if", !0)
                 }]
             ]),
-            Sd = {
+            kd = {
                 class: "plugin",
                 id: "folders"
             },
-            Cd = {
+            Sd = {
                 key: 0,
                 class: "table-row"
             },
-            Td = [wi("div", {
+            Cd = [wi("div", {
                 class: "table-cell text-left title"
             }, "FOLDERS", -1), wi("div", {
                 class: "table-cell"
             }, null, -1), wi("div", {
                 class: "table-cell"
             }, "Size", -1)],
-            Ad = {
+            Td = {
                 class: "table-cell text-left"
             },
-            Ed = wi("div", {
+            Ad = wi("div", {
                 class: "table-cell"
             }, null, -1);
-        const Od = {
+        const Ed = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 computed: {
                     stats() {
@@ -15731,51 +15730,51 @@
                 },
                 methods: {
                     getDecoration(e) {
                         if (Number.isInteger(e.size)) return null !== e.critical && e.size > 1e6 * e.critical ? "critical" : null !== e.warning && e.size > 1e6 * e.warning ? "warning" : null !== e.careful && e.size > 1e6 * e.careful ? "careful" : "ok"
                     }
                 }
             },
-            Id = (0, ec.Z)(Od, [
+            Od = (0, ec.Z)(Ed, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", Sd, [s.folders.length > 0 ? (li(), pi("div", Cd, Td)) : Ti("v-if", !0), (li(!0), pi(ni, null, pr(s.folders, ((t, n) => (li(), pi("div", {
+                    return li(), pi("section", kd, [s.folders.length > 0 ? (li(), pi("div", Sd, Cd)) : Ti("v-if", !0), (li(!0), pi(ni, null, pr(s.folders, ((t, n) => (li(), pi("div", {
                         class: "table-row",
                         key: n
-                    }, [wi("div", Ad, pe(t.path), 1), Ed, wi("div", {
+                    }, [wi("div", Td, pe(t.path), 1), Ad, wi("div", {
                         class: ce(["table-cell", s.getDecoration(t)])
                     }, pe(e.$filters.bytes(t.size)), 3)])))), 128))])
                 }]
             ]),
-            Pd = {
+            Id = {
                 class: "plugin",
                 id: "fs"
             },
-            Nd = {
+            Pd = {
                 class: "table-row"
             },
-            Ld = wi("div", {
+            Nd = wi("div", {
                 class: "table-cell text-left title"
             }, "FILE SYS", -1),
-            Dd = {
+            Ld = {
                 class: "table-cell"
             },
-            Md = wi("div", {
+            Dd = wi("div", {
                 class: "table-cell"
             }, "Total", -1),
-            jd = {
+            Md = {
                 class: "table-cell text-left"
             },
-            Rd = {
+            jd = {
                 key: 0,
                 class: "visible-lg-inline"
             },
-            qd = {
+            Rd = {
                 class: "table-cell"
             };
-        const Bd = {
+        const qd = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 data: () => ({
                     store: qo
@@ -15808,88 +15807,88 @@
                 },
                 methods: {
                     getDecoration(e, t) {
                         if (null != this.view[e][t]) return this.view[e][t].decoration.toLowerCase()
                     }
                 }
             },
-            Ud = (0, ec.Z)(Bd, [
+            Bd = (0, ec.Z)(qd, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", Pd, [wi("div", Nd, [Ld, wi("div", Dd, [On(wi("span", null, "Used", 512), [
+                    return li(), pi("section", Id, [wi("div", Pd, [Nd, wi("div", Ld, [On(wi("span", null, "Used", 512), [
                         [Ds, !s.args.fs_free_space]
                     ]), On(wi("span", null, "Free", 512), [
                         [Ds, s.args.fs_free_space]
-                    ])]), Md]), (li(!0), pi(ni, null, pr(s.fileSystems, ((t, n) => (li(), pi("div", {
+                    ])]), Dd]), (li(!0), pi(ni, null, pr(s.fileSystems, ((t, n) => (li(), pi("div", {
                         class: "table-row",
                         key: n
-                    }, [wi("div", jd, [Si(pe(t.shortMountPoint) + " ", 1), t.shortMountPoint.length <= 12 ? (li(), pi("span", Rd, " (" + pe(t.name) + ") ", 1)) : Ti("v-if", !0)]), wi("div", {
+                    }, [wi("div", Md, [Si(pe(t.shortMountPoint) + " ", 1), t.shortMountPoint.length <= 12 ? (li(), pi("span", jd, " (" + pe(t.name) + ") ", 1)) : Ti("v-if", !0)]), wi("div", {
                         class: ce(["table-cell", s.getDecoration(t.mountPoint, "used")])
                     }, [On(wi("span", null, pe(e.$filters.bytes(t.used)), 513), [
                         [Ds, !s.args.fs_free_space]
                     ]), On(wi("span", null, pe(e.$filters.bytes(t.free)), 513), [
                         [Ds, s.args.fs_free_space]
-                    ])], 2), wi("div", qd, pe(e.$filters.bytes(t.size)), 1)])))), 128))])
+                    ])], 2), wi("div", Rd, pe(e.$filters.bytes(t.size)), 1)])))), 128))])
                 }]
             ]),
-            Fd = {
+            Ud = {
                 id: "gpu",
                 class: "plugin"
             },
-            $d = {
+            Fd = {
                 class: "gpu-name title"
             },
-            zd = {
+            $d = {
                 class: "table"
             },
-            Hd = {
+            zd = {
                 key: 0,
                 class: "table-row"
             },
-            Vd = wi("div", {
+            Hd = wi("div", {
                 class: "table-cell text-left"
             }, "proc:", -1),
-            Gd = {
+            Vd = {
                 key: 1,
                 class: "table-cell"
             },
-            Wd = {
+            Gd = {
                 key: 1,
                 class: "table-row"
             },
-            Zd = wi("div", {
+            Wd = wi("div", {
                 class: "table-cell text-left"
             }, "mem:", -1),
-            Kd = {
+            Zd = {
                 key: 1,
                 class: "table-cell"
             },
-            Qd = {
+            Kd = {
                 key: 2,
                 class: "table-row"
             },
-            Xd = wi("div", {
+            Qd = wi("div", {
                 class: "table-cell text-left"
             }, "temperature::", -1),
-            Jd = {
+            Xd = {
                 key: 1,
                 class: "table-cell"
             },
-            Yd = {
+            Jd = {
                 class: "table-cell text-left"
             },
-            ef = {
+            Yd = {
                 key: 1
             },
-            tf = {
+            ef = {
                 key: 3
             },
-            nf = {
+            tf = {
                 key: 5
             };
-        const rf = {
+        const nf = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 data: () => ({
                     store: qo
@@ -15933,65 +15932,65 @@
                         if (void 0 !== this.view[e][t]) return this.view[e][t].decoration.toLowerCase()
                     },
                     getMeanDecoration(e) {
                         return this.getDecoration(0, e)
                     }
                 }
             },
-            sf = (0, ec.Z)(rf, [
+            rf = (0, ec.Z)(nf, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", Fd, [wi("div", $d, pe(s.name), 1), wi("div", zd, [s.args.meangpu || 1 === s.gpus.length ? (li(), pi("div", Hd, [Vd, null != s.mean.proc ? (li(), pi("div", {
+                    return li(), pi("section", Ud, [wi("div", Fd, pe(s.name), 1), wi("div", $d, [s.args.meangpu || 1 === s.gpus.length ? (li(), pi("div", zd, [Hd, null != s.mean.proc ? (li(), pi("div", {
                         key: 0,
                         class: ce(["table-cell", s.getMeanDecoration("proc")])
-                    }, pe(e.$filters.number(s.mean.proc, 0)) + "% ", 3)) : Ti("v-if", !0), null == s.mean.proc ? (li(), pi("div", Gd, "N/A")) : Ti("v-if", !0)])) : Ti("v-if", !0), s.args.meangpu || 1 === s.gpus.length ? (li(), pi("div", Wd, [Zd, null != s.mean.mem ? (li(), pi("div", {
+                    }, pe(e.$filters.number(s.mean.proc, 0)) + "% ", 3)) : Ti("v-if", !0), null == s.mean.proc ? (li(), pi("div", Vd, "N/A")) : Ti("v-if", !0)])) : Ti("v-if", !0), s.args.meangpu || 1 === s.gpus.length ? (li(), pi("div", Gd, [Wd, null != s.mean.mem ? (li(), pi("div", {
                         key: 0,
                         class: ce(["table-cell", s.getMeanDecoration("mem")])
-                    }, pe(e.$filters.number(s.mean.mem, 0)) + "% ", 3)) : Ti("v-if", !0), null == s.mean.mem ? (li(), pi("div", Kd, "N/A")) : Ti("v-if", !0)])) : Ti("v-if", !0), s.args.meangpu || 1 === s.gpus.length ? (li(), pi("div", Qd, [Xd, null != s.mean.temperature ? (li(), pi("div", {
+                    }, pe(e.$filters.number(s.mean.mem, 0)) + "% ", 3)) : Ti("v-if", !0), null == s.mean.mem ? (li(), pi("div", Zd, "N/A")) : Ti("v-if", !0)])) : Ti("v-if", !0), s.args.meangpu || 1 === s.gpus.length ? (li(), pi("div", Kd, [Qd, null != s.mean.temperature ? (li(), pi("div", {
                         key: 0,
                         class: ce(["table-cell", s.getMeanDecoration("temperature")])
-                    }, pe(e.$filters.number(s.mean.temperature, 0)) + "° ", 3)) : Ti("v-if", !0), null == s.mean.temperature ? (li(), pi("div", Jd, "N/A")) : Ti("v-if", !0)])) : Ti("v-if", !0), !s.args.meangpu && s.gpus.length > 1 ? (li(!0), pi(ni, {
+                    }, pe(e.$filters.number(s.mean.temperature, 0)) + "° ", 3)) : Ti("v-if", !0), null == s.mean.temperature ? (li(), pi("div", Xd, "N/A")) : Ti("v-if", !0)])) : Ti("v-if", !0), !s.args.meangpu && s.gpus.length > 1 ? (li(!0), pi(ni, {
                         key: 3
                     }, pr(s.gpus, ((t, n) => (li(), pi("div", {
                         class: "table-row",
                         key: n
-                    }, [wi("div", Yd, [Si(pe(t.gpu_id) + ": ", 1), null != t.proc ? (li(), pi("span", {
+                    }, [wi("div", Jd, [Si(pe(t.gpu_id) + ": ", 1), null != t.proc ? (li(), pi("span", {
                         key: 0,
                         class: ce(s.getDecoration(t.gpu_id, "proc"))
-                    }, pe(e.$filters.number(t.proc, 0)) + "% ", 3)) : Ti("v-if", !0), null == t.proc ? (li(), pi("span", ef, "N/A")) : Ti("v-if", !0), Si(" mem: "), null != t.mem ? (li(), pi("span", {
+                    }, pe(e.$filters.number(t.proc, 0)) + "% ", 3)) : Ti("v-if", !0), null == t.proc ? (li(), pi("span", Yd, "N/A")) : Ti("v-if", !0), Si(" mem: "), null != t.mem ? (li(), pi("span", {
                         key: 2,
                         class: ce(s.getDecoration(t.gpu_id, "mem"))
-                    }, pe(e.$filters.number(t.mem, 0)) + "% ", 3)) : Ti("v-if", !0), null == t.mem ? (li(), pi("span", tf, "N/A")) : Ti("v-if", !0), Si(" temp: "), null != t.temperature ? (li(), pi("span", {
+                    }, pe(e.$filters.number(t.mem, 0)) + "% ", 3)) : Ti("v-if", !0), null == t.mem ? (li(), pi("span", ef, "N/A")) : Ti("v-if", !0), Si(" temp: "), null != t.temperature ? (li(), pi("span", {
                         key: 4,
                         class: ce(s.getDecoration(t.gpu_id, "temperature"))
-                    }, pe(e.$filters.number(t.temperature, 0)) + "C ", 3)) : Ti("v-if", !0), null == t.temperature ? (li(), pi("span", nf, "N/A")) : Ti("v-if", !0)])])))), 128)) : Ti("v-if", !0)])])
+                    }, pe(e.$filters.number(t.temperature, 0)) + "C ", 3)) : Ti("v-if", !0), null == t.temperature ? (li(), pi("span", tf, "N/A")) : Ti("v-if", !0)])])))), 128)) : Ti("v-if", !0)])])
                 }]
             ]),
-            of = {
+            sf = {
                 key: 0,
                 class: "plugin",
                 id: "ip"
             },
-            af = {
+            of = {
                 key: 0,
                 class: "title"
             },
-            lf = {
+            af = {
                 key: 1
             },
-            cf = {
+            lf = {
                 key: 2,
                 class: "title"
             },
-            uf = {
+            cf = {
                 key: 3
             },
-            df = {
+            uf = {
                 key: 4
             };
-        const ff = {
+        const df = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 computed: {
                     ipStats() {
@@ -16010,44 +16009,44 @@
                         return this.ipStats.public_address
                     },
                     publicInfo() {
                         return this.ipStats.public_info_human
                     }
                 }
             },
-            pf = (0, ec.Z)(ff, [
+            ff = (0, ec.Z)(df, [
                 ["render", function(e, t, n, r, i, s) {
-                    return null != s.address ? (li(), pi("section", of, [null != s.address ? (li(), pi("span", af, "IP")) : Ti("v-if", !0), null != s.address ? (li(), pi("span", lf, pe(s.address) + "/" + pe(s.maskCdir), 1)) : Ti("v-if", !0), null != s.publicAddress ? (li(), pi("span", cf, "Pub")) : Ti("v-if", !0), null != s.publicAddress ? (li(), pi("span", uf, pe(s.publicAddress), 1)) : Ti("v-if", !0), null != s.publicInfo ? (li(), pi("span", df, pe(s.publicInfo), 1)) : Ti("v-if", !0)])) : Ti("v-if", !0)
+                    return null != s.address ? (li(), pi("section", sf, [null != s.address ? (li(), pi("span", of, "IP")) : Ti("v-if", !0), null != s.address ? (li(), pi("span", af, pe(s.address) + "/" + pe(s.maskCdir), 1)) : Ti("v-if", !0), null != s.publicAddress ? (li(), pi("span", lf, "Pub")) : Ti("v-if", !0), null != s.publicAddress ? (li(), pi("span", cf, pe(s.publicAddress), 1)) : Ti("v-if", !0), null != s.publicInfo ? (li(), pi("span", uf, pe(s.publicInfo), 1)) : Ti("v-if", !0)])) : Ti("v-if", !0)
                 }]
             ]),
-            hf = {
+            pf = {
                 class: "plugin",
                 id: "irq"
             },
-            gf = {
+            hf = {
                 key: 0,
                 class: "table-row"
             },
-            mf = [wi("div", {
+            gf = [wi("div", {
                 class: "table-cell text-left title"
             }, "IRQ", -1), wi("div", {
                 class: "table-cell"
             }, null, -1), wi("div", {
                 class: "table-cell"
             }, "Rate/s", -1)],
-            bf = {
+            mf = {
                 class: "table-cell text-left"
             },
-            vf = wi("div", {
+            bf = wi("div", {
                 class: "table-cell"
             }, null, -1),
-            yf = {
+            vf = {
                 class: "table-cell"
             };
-        const wf = {
+        const yf = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 computed: {
                     stats() {
@@ -16057,61 +16056,61 @@
                         return this.stats.map((e => ({
                             irq_line: e.irq_line,
                             irq_rate: e.irq_rate
                         })))
                     }
                 }
             },
-            xf = (0, ec.Z)(wf, [
+            wf = (0, ec.Z)(yf, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", hf, [s.irqs.length > 0 ? (li(), pi("div", gf, mf)) : Ti("v-if", !0), (li(!0), pi(ni, null, pr(s.irqs, ((e, t) => (li(), pi("div", {
+                    return li(), pi("section", pf, [s.irqs.length > 0 ? (li(), pi("div", hf, gf)) : Ti("v-if", !0), (li(!0), pi(ni, null, pr(s.irqs, ((e, t) => (li(), pi("div", {
                         class: "table-row",
                         key: t
-                    }, [wi("div", bf, pe(e.irq_line), 1), vf, wi("div", yf, [wi("span", null, pe(e.irq_rate), 1)])])))), 128))])
+                    }, [wi("div", mf, pe(e.irq_line), 1), bf, wi("div", vf, [wi("span", null, pe(e.irq_rate), 1)])])))), 128))])
                 }]
             ]),
-            _f = {
+            xf = {
                 key: 0,
                 id: "load",
                 class: "plugin"
             },
-            kf = {
+            _f = {
                 class: "table"
             },
-            Sf = {
+            kf = {
                 class: "table-row"
             },
-            Cf = wi("div", {
+            Sf = wi("div", {
                 class: "table-cell text-left title"
             }, "LOAD", -1),
-            Tf = {
+            Cf = {
                 class: "table-cell"
             },
-            Af = {
+            Tf = {
                 class: "table-row"
             },
-            Ef = wi("div", {
+            Af = wi("div", {
                 class: "table-cell text-left"
             }, "1 min:", -1),
-            Of = {
+            Ef = {
                 class: "table-cell"
             },
-            If = {
+            Of = {
                 class: "table-row"
             },
-            Pf = wi("div", {
+            If = wi("div", {
                 class: "table-cell text-left"
             }, "5 min:", -1),
-            Nf = {
+            Pf = {
                 class: "table-row"
             },
-            Lf = wi("div", {
+            Nf = wi("div", {
                 class: "table-cell text-left"
             }, "15 min:", -1);
-        const Df = {
+        const Lf = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 computed: {
                     stats() {
@@ -16135,64 +16134,61 @@
                 },
                 methods: {
                     getDecoration(e) {
                         if (void 0 !== this.view[e]) return this.view[e].decoration.toLowerCase()
                     }
                 }
             },
-            Mf = (0, ec.Z)(Df, [
+            Df = (0, ec.Z)(Lf, [
                 ["render", function(e, t, n, r, i, s) {
-                    return null != s.cpucore ? (li(), pi("section", _f, [wi("div", kf, [wi("div", Sf, [Cf, wi("div", Tf, pe(s.cpucore) + "-core", 1)]), wi("div", Af, [Ef, wi("div", Of, pe(e.$filters.number(s.min1, 2)), 1)]), wi("div", If, [Pf, wi("div", {
+                    return null != s.cpucore ? (li(), pi("section", xf, [wi("div", _f, [wi("div", kf, [Sf, wi("div", Cf, pe(s.cpucore) + "-core", 1)]), wi("div", Tf, [Af, wi("div", Ef, pe(e.$filters.number(s.min1, 2)), 1)]), wi("div", Of, [If, wi("div", {
                         class: ce(["table-cell", s.getDecoration("min5")])
-                    }, pe(e.$filters.number(s.min5, 2)), 3)]), wi("div", Nf, [Lf, wi("div", {
+                    }, pe(e.$filters.number(s.min5, 2)), 3)]), wi("div", Pf, [Nf, wi("div", {
                         class: ce(["table-cell", s.getDecoration("min15")])
                     }, pe(e.$filters.number(s.min15, 2)), 3)])])])) : Ti("v-if", !0)
                 }]
             ]),
-            jf = {
+            Mf = {
                 id: "mem",
                 class: "plugin"
             },
-            Rf = {
+            jf = {
                 class: "table"
             },
-            qf = {
+            Rf = {
                 class: "table-row"
             },
-            Bf = wi("div", {
+            qf = wi("div", {
                 class: "table-cell text-left title"
             }, "MEM", -1),
-            Uf = {
-                class: "table-cell"
-            },
-            Ff = {
+            Bf = {
                 class: "table-row"
             },
-            $f = wi("div", {
+            Uf = wi("div", {
                 class: "table-cell text-left"
             }, "total:", -1),
-            zf = {
+            Ff = {
                 class: "table-cell"
             },
-            Hf = {
+            $f = {
                 class: "table-row"
             },
-            Vf = wi("div", {
+            zf = wi("div", {
                 class: "table-cell text-left"
             }, "used:", -1),
-            Gf = {
+            Hf = {
                 class: "table-row"
             },
-            Wf = wi("div", {
+            Vf = wi("div", {
                 class: "table-cell text-left"
             }, "free:", -1),
-            Zf = {
+            Gf = {
                 class: "table-cell"
             };
-        const Kf = {
+        const Wf = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 computed: {
                     stats() {
@@ -16216,65 +16212,67 @@
                 },
                 methods: {
                     getDecoration(e) {
                         if (void 0 !== this.view[e]) return this.view[e].decoration.toLowerCase()
                     }
                 }
             },
-            Qf = (0, ec.Z)(Kf, [
+            Zf = (0, ec.Z)(Wf, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", jf, [wi("div", Rf, [wi("div", qf, [Bf, wi("div", Uf, pe(s.percent) + "%", 1)]), wi("div", Ff, [$f, wi("div", zf, pe(e.$filters.bytes(s.total)), 1)]), wi("div", Hf, [Vf, wi("div", {
+                    return li(), pi("section", Mf, [wi("div", jf, [wi("div", Rf, [qf, wi("div", {
+                        class: ce(["table-cell", s.getDecoration("percent")])
+                    }, pe(s.percent) + "%", 3)]), wi("div", Bf, [Uf, wi("div", Ff, pe(e.$filters.bytes(s.total)), 1)]), wi("div", $f, [zf, wi("div", {
                         class: ce(["table-cell", s.getDecoration("used")])
-                    }, pe(e.$filters.bytes(s.used, 2)), 3)]), wi("div", Gf, [Wf, wi("div", Zf, pe(e.$filters.bytes(s.free)), 1)])])])
+                    }, pe(e.$filters.bytes(s.used, 2)), 3)]), wi("div", Hf, [Vf, wi("div", Gf, pe(e.$filters.bytes(s.free)), 1)])])])
                 }]
             ]),
-            Xf = {
+            Kf = {
                 id: "mem-more",
                 class: "plugin"
             },
-            Jf = {
+            Qf = {
                 class: "table"
             },
-            Yf = {
+            Xf = {
                 class: "table-row"
             },
-            ep = wi("div", {
+            Jf = wi("div", {
                 class: "table-cell text-left"
             }, "active:", -1),
-            tp = {
+            Yf = {
                 class: "table-cell"
             },
-            np = {
+            ep = {
                 class: "table-row"
             },
-            rp = wi("div", {
+            tp = wi("div", {
                 class: "table-cell text-left"
             }, "inactive:", -1),
-            ip = {
+            np = {
                 class: "table-cell"
             },
-            sp = {
+            rp = {
                 class: "table-row"
             },
-            op = wi("div", {
+            ip = wi("div", {
                 class: "table-cell text-left"
             }, "buffers:", -1),
-            ap = {
+            sp = {
                 class: "table-cell"
             },
-            lp = {
+            op = {
                 class: "table-row"
             },
-            cp = wi("div", {
+            ap = wi("div", {
                 class: "table-cell text-left"
             }, "cached:", -1),
-            up = {
+            lp = {
                 class: "table-cell"
             };
-        const dp = {
+        const cp = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 computed: {
                     stats() {
@@ -16290,68 +16288,65 @@
                         return this.stats.buffers
                     },
                     cached() {
                         return this.stats.cached
                     }
                 }
             },
-            fp = (0, ec.Z)(dp, [
+            up = (0, ec.Z)(cp, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", Xf, [wi("div", Jf, [On(wi("div", Yf, [ep, wi("div", tp, pe(e.$filters.bytes(s.active)), 1)], 512), [
+                    return li(), pi("section", Kf, [wi("div", Qf, [On(wi("div", Xf, [Jf, wi("div", Yf, pe(e.$filters.bytes(s.active)), 1)], 512), [
                         [Ds, null != s.active]
-                    ]), On(wi("div", np, [rp, wi("div", ip, pe(e.$filters.bytes(s.inactive)), 1)], 512), [
+                    ]), On(wi("div", ep, [tp, wi("div", np, pe(e.$filters.bytes(s.inactive)), 1)], 512), [
                         [Ds, null != s.inactive]
-                    ]), On(wi("div", sp, [op, wi("div", ap, pe(e.$filters.bytes(s.buffers)), 1)], 512), [
+                    ]), On(wi("div", rp, [ip, wi("div", sp, pe(e.$filters.bytes(s.buffers)), 1)], 512), [
                         [Ds, null != s.buffers]
-                    ]), On(wi("div", lp, [cp, wi("div", up, pe(e.$filters.bytes(s.cached)), 1)], 512), [
+                    ]), On(wi("div", op, [ap, wi("div", lp, pe(e.$filters.bytes(s.cached)), 1)], 512), [
                         [Ds, null != s.cached]
                     ])])])
                 }]
             ]),
-            pp = {
+            dp = {
                 id: "memswap",
                 class: "plugin"
             },
-            hp = {
+            fp = {
                 class: "table"
             },
-            gp = {
+            pp = {
                 class: "table-row"
             },
-            mp = wi("div", {
+            hp = wi("div", {
                 class: "table-cell text-left title"
             }, "SWAP", -1),
-            bp = {
-                class: "table-cell"
-            },
-            vp = {
+            gp = {
                 class: "table-row"
             },
-            yp = wi("div", {
+            mp = wi("div", {
                 class: "table-cell text-left"
             }, "total:", -1),
-            wp = {
+            bp = {
                 class: "table-cell"
             },
-            xp = {
+            vp = {
                 class: "table-row"
             },
-            _p = wi("div", {
+            yp = wi("div", {
                 class: "table-cell text-left"
             }, "used:", -1),
-            kp = {
+            wp = {
                 class: "table-row"
             },
-            Sp = wi("div", {
+            xp = wi("div", {
                 class: "table-cell text-left"
             }, "free:", -1),
-            Cp = {
+            _p = {
                 class: "table-cell"
             };
-        const Tp = {
+        const kp = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 computed: {
                     stats() {
@@ -16375,71 +16370,73 @@
                 },
                 methods: {
                     getDecoration(e) {
                         if (void 0 !== this.view[e]) return this.view[e].decoration.toLowerCase()
                     }
                 }
             },
-            Ap = (0, ec.Z)(Tp, [
+            Sp = (0, ec.Z)(kp, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", pp, [wi("div", hp, [wi("div", gp, [mp, wi("div", bp, pe(s.percent) + "%", 1)]), wi("div", vp, [yp, wi("div", wp, pe(e.$filters.bytes(s.total)), 1)]), wi("div", xp, [_p, wi("div", {
+                    return li(), pi("section", dp, [wi("div", fp, [wi("div", pp, [hp, wi("div", {
+                        class: ce(["table-cell", s.getDecoration("percent")])
+                    }, pe(s.percent) + "%", 3)]), wi("div", gp, [mp, wi("div", bp, pe(e.$filters.bytes(s.total)), 1)]), wi("div", vp, [yp, wi("div", {
                         class: ce(["table-cell", s.getDecoration("used")])
-                    }, pe(e.$filters.bytes(s.used)), 3)]), wi("div", kp, [Sp, wi("div", Cp, pe(e.$filters.bytes(s.free)), 1)])])])
+                    }, pe(e.$filters.bytes(s.used)), 3)]), wi("div", wp, [xp, wi("div", _p, pe(e.$filters.bytes(s.free)), 1)])])])
                 }]
             ]),
-            Ep = {
+            Cp = {
                 class: "plugin",
                 id: "network"
             },
-            Op = {
+            Tp = {
                 class: "table-row"
             },
-            Ip = wi("div", {
+            Ap = wi("div", {
                 class: "table-cell text-left title"
             }, "NETWORK", -1),
-            Pp = {
+            Ep = {
                 class: "table-cell"
             },
-            Np = {
+            Op = {
                 class: "table-cell"
             },
-            Lp = {
+            Ip = {
                 class: "table-cell"
             },
-            Dp = {
+            Pp = {
                 class: "table-cell"
             },
-            Mp = {
+            Np = {
                 class: "table-cell"
             },
-            jp = {
+            Lp = {
                 class: "table-cell"
             },
-            Rp = {
+            Dp = {
                 class: "table-cell"
             },
-            qp = {
+            Mp = {
                 class: "table-cell"
             },
-            Bp = {
+            jp = {
                 class: "table-cell text-left"
             },
-            Up = {
+            Rp = {
                 class: "visible-lg-inline"
             },
-            Fp = {
+            qp = {
                 class: "hidden-lg"
             },
-            $p = {
+            Bp = {
                 class: "table-cell"
             },
-            zp = {
+            Up = {
                 class: "table-cell"
             };
-        const Hp = {
+        const Fp = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 data: () => ({
                     store: qo
@@ -16466,133 +16463,133 @@
                                 cumulativeCx: e.cumulative_cx
                             }
                         }));
                         return (0, cc.orderBy)(e, ["interfaceName"])
                     }
                 }
             },
-            Vp = (0, ec.Z)(Hp, [
+            $p = (0, ec.Z)(Fp, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", Ep, [wi("div", Op, [Ip, On(wi("div", Pp, "Rx/s", 512), [
+                    return li(), pi("section", Cp, [wi("div", Tp, [Ap, On(wi("div", Ep, "Rx/s", 512), [
                         [Ds, !s.args.network_cumul && !s.args.network_sum]
-                    ]), On(wi("div", Np, "Tx/s", 512), [
+                    ]), On(wi("div", Op, "Tx/s", 512), [
                         [Ds, !s.args.network_cumul && !s.args.network_sum]
-                    ]), On(wi("div", Lp, null, 512), [
+                    ]), On(wi("div", Ip, null, 512), [
                         [Ds, !s.args.network_cumul && s.args.network_sum]
-                    ]), On(wi("div", Dp, "Rx+Tx/s", 512), [
+                    ]), On(wi("div", Pp, "Rx+Tx/s", 512), [
                         [Ds, !s.args.network_cumul && s.args.network_sum]
-                    ]), On(wi("div", Mp, "Rx", 512), [
+                    ]), On(wi("div", Np, "Rx", 512), [
                         [Ds, s.args.network_cumul && !s.args.network_sum]
-                    ]), On(wi("div", jp, "Tx", 512), [
+                    ]), On(wi("div", Lp, "Tx", 512), [
                         [Ds, s.args.network_cumul && !s.args.network_sum]
-                    ]), On(wi("div", Rp, null, 512), [
+                    ]), On(wi("div", Dp, null, 512), [
                         [Ds, s.args.network_cumul && s.args.network_sum]
-                    ]), On(wi("div", qp, "Rx+Tx", 512), [
+                    ]), On(wi("div", Mp, "Rx+Tx", 512), [
                         [Ds, s.args.network_cumul && s.args.network_sum]
                     ])]), (li(!0), pi(ni, null, pr(s.networks, ((t, n) => (li(), pi("div", {
                         class: "table-row",
                         key: n
-                    }, [wi("div", Bp, [wi("span", Up, pe(t.ifname), 1), wi("span", Fp, pe(e.$filters.minSize(t.ifname)), 1)]), On(wi("div", {
+                    }, [wi("div", jp, [wi("span", Rp, pe(t.ifname), 1), wi("span", qp, pe(e.$filters.minSize(t.ifname)), 1)]), On(wi("div", {
                         class: "table-cell"
                     }, pe(s.args.byte ? e.$filters.bytes(t.rx / t.time_since_update) : e.$filters.bits(t.rx / t.time_since_update)), 513), [
                         [Ds, !s.args.network_cumul && !s.args.network_sum]
                     ]), On(wi("div", {
                         class: "table-cell"
                     }, pe(s.args.byte ? e.$filters.bytes(t.tx / t.time_since_update) : e.$filters.bits(t.tx / t.time_since_update)), 513), [
                         [Ds, !s.args.network_cumul && !s.args.network_sum]
-                    ]), On(wi("div", $p, null, 512), [
+                    ]), On(wi("div", Bp, null, 512), [
                         [Ds, !s.args.network_cumul && s.args.network_sum]
                     ]), On(wi("div", {
                         class: "table-cell"
                     }, pe(s.args.byte ? e.$filters.bytes(t.cx / t.time_since_update) : e.$filters.bits(t.cx / t.time_since_update)), 513), [
                         [Ds, !s.args.network_cumul && s.args.network_sum]
                     ]), On(wi("div", {
                         class: "table-cell"
                     }, pe(s.args.byte ? e.$filters.bytes(t.cumulativeRx) : e.$filters.bits(t.cumulativeRx)), 513), [
                         [Ds, s.args.network_cumul && !s.args.network_sum]
                     ]), On(wi("div", {
                         class: "table-cell"
                     }, pe(s.args.byte ? e.$filters.bytes(t.cumulativeTx) : e.$filters.bits(t.cumulativeTx)), 513), [
                         [Ds, s.args.network_cumul && !s.args.network_sum]
-                    ]), On(wi("div", zp, null, 512), [
+                    ]), On(wi("div", Up, null, 512), [
                         [Ds, s.args.network_cumul && s.args.network_sum]
                     ]), On(wi("div", {
                         class: "table-cell"
                     }, pe(s.args.byte ? e.$filters.bytes(t.cumulativeCx) : e.$filters.bits(t.cumulativeCx)), 513), [
                         [Ds, s.args.network_cumul && s.args.network_sum]
                     ])])))), 128))])
                 }]
             ]),
-            Gp = {
+            zp = {
                 id: "now",
                 class: "plugin"
             };
-        const Wp = {
+        const Hp = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 computed: {
                     value() {
                         return this.data.stats.now
                     }
                 }
             },
-            Zp = (0, ec.Z)(Wp, [
+            Vp = (0, ec.Z)(Hp, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", Gp, [wi("span", null, pe(s.value), 1)])
+                    return li(), pi("section", zp, [wi("span", null, pe(s.value), 1)])
                 }]
             ]),
-            Kp = {
+            Gp = {
                 id: "percpu",
                 class: "plugin"
             },
-            Qp = {
+            Wp = {
                 class: "table-row"
             },
-            Xp = {
+            Zp = {
                 class: "table-cell text-left title"
             },
-            Jp = {
+            Kp = {
                 key: 0
             },
-            Yp = {
+            Qp = {
                 class: "table-row"
             },
-            eh = wi("div", {
+            Xp = wi("div", {
                 class: "table-cell text-left"
             }, "user:", -1),
-            th = {
+            Jp = {
                 class: "table-row"
             },
-            nh = wi("div", {
+            Yp = wi("div", {
                 class: "table-cell text-left"
             }, "system:", -1),
-            rh = {
+            eh = {
                 class: "table-row"
             },
-            ih = wi("div", {
+            th = wi("div", {
                 class: "table-cell text-left"
             }, "idle:", -1),
-            sh = {
+            nh = {
                 key: 0,
                 class: "table-row"
             },
-            oh = wi("div", {
+            rh = wi("div", {
                 class: "table-cell text-left"
             }, "iowait:", -1),
-            ah = {
+            ih = {
                 key: 1,
                 class: "table-row"
             },
-            lh = wi("div", {
+            sh = wi("div", {
                 class: "table-cell text-left"
             }, "steal:", -1);
-        const ch = {
+        const oh = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 computed: {
                     percpuStats() {
@@ -16612,72 +16609,72 @@
                     }
                 },
                 methods: {
                     getUserAlert: e => Fo.getAlert("percpu", "percpu_user_", e.user),
                     getSystemAlert: e => Fo.getAlert("percpu", "percpu_system_", e.system)
                 }
             },
-            uh = (0, ec.Z)(ch, [
+            ah = (0, ec.Z)(oh, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", Kp, [(li(!0), pi(ni, null, pr(s.cpusChunks, ((e, t) => (li(), pi("div", {
+                    return li(), pi("section", Gp, [(li(!0), pi(ni, null, pr(s.cpusChunks, ((e, t) => (li(), pi("div", {
                         class: "table",
                         key: t
-                    }, [wi("div", Qp, [wi("div", Xp, [0 === t ? (li(), pi("span", Jp, "PER CPU")) : Ti("v-if", !0)]), (li(!0), pi(ni, null, pr(e, ((e, t) => (li(), pi("div", {
+                    }, [wi("div", Wp, [wi("div", Zp, [0 === t ? (li(), pi("span", Kp, "PER CPU")) : Ti("v-if", !0)]), (li(!0), pi(ni, null, pr(e, ((e, t) => (li(), pi("div", {
                         class: "table-cell",
                         key: t
-                    }, pe(e.total) + "% ", 1)))), 128))]), wi("div", Yp, [eh, (li(!0), pi(ni, null, pr(e, ((e, t) => (li(), pi("div", {
+                    }, pe(e.total) + "% ", 1)))), 128))]), wi("div", Qp, [Xp, (li(!0), pi(ni, null, pr(e, ((e, t) => (li(), pi("div", {
                         class: ce(["table-cell", s.getUserAlert(e)]),
                         key: t
-                    }, pe(e.user) + "% ", 3)))), 128))]), wi("div", th, [nh, (li(!0), pi(ni, null, pr(e, ((e, t) => (li(), pi("div", {
+                    }, pe(e.user) + "% ", 3)))), 128))]), wi("div", Jp, [Yp, (li(!0), pi(ni, null, pr(e, ((e, t) => (li(), pi("div", {
                         class: ce(["table-cell", s.getSystemAlert(e)]),
                         key: t
-                    }, pe(e.system) + "% ", 3)))), 128))]), wi("div", rh, [ih, (li(!0), pi(ni, null, pr(e, ((e, t) => (li(), pi("div", {
+                    }, pe(e.system) + "% ", 3)))), 128))]), wi("div", eh, [th, (li(!0), pi(ni, null, pr(e, ((e, t) => (li(), pi("div", {
                         class: "table-cell",
                         key: t
-                    }, pe(e.idle) + "% ", 1)))), 128))]), e[0].iowait ? (li(), pi("div", sh, [oh, (li(!0), pi(ni, null, pr(e, ((e, t) => (li(), pi("div", {
+                    }, pe(e.idle) + "% ", 1)))), 128))]), e[0].iowait ? (li(), pi("div", nh, [rh, (li(!0), pi(ni, null, pr(e, ((e, t) => (li(), pi("div", {
                         class: ce(["table-cell", s.getSystemAlert(e)]),
                         key: t
-                    }, pe(e.iowait) + "% ", 3)))), 128))])) : Ti("v-if", !0), e[0].steal ? (li(), pi("div", ah, [lh, (li(!0), pi(ni, null, pr(e, ((e, t) => (li(), pi("div", {
+                    }, pe(e.iowait) + "% ", 3)))), 128))])) : Ti("v-if", !0), e[0].steal ? (li(), pi("div", ih, [sh, (li(!0), pi(ni, null, pr(e, ((e, t) => (li(), pi("div", {
                         class: ce(["table-cell", s.getSystemAlert(e)]),
                         key: t
                     }, pe(e.steal) + "% ", 3)))), 128))])) : Ti("v-if", !0)])))), 128))])
                 }]
             ]),
-            dh = {
+            lh = {
                 class: "plugin",
                 id: "ports"
             },
-            fh = {
+            ch = {
                 class: "table-cell text-left"
             },
-            ph = wi("div", {
+            uh = wi("div", {
                 class: "table-cell"
             }, null, -1),
-            hh = {
+            dh = {
                 key: 0
             },
-            gh = {
+            fh = {
                 key: 1
             },
-            mh = {
+            ph = {
                 key: 2
             },
-            bh = {
+            hh = {
                 key: 3
             },
-            vh = {
+            gh = {
                 key: 0
             },
-            yh = {
+            mh = {
                 key: 1
             },
-            wh = {
+            bh = {
                 key: 2
             };
-        const xh = {
+        const vh = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 computed: {
                     stats() {
@@ -16688,54 +16685,54 @@
                     }
                 },
                 methods: {
                     getPortDecoration: e => null === e.status ? "careful" : !1 === e.status ? "critical" : null !== e.rtt_warning && e.status > e.rtt_warning ? "warning" : "ok",
                     getWebDecoration: e => null === e.status ? "careful" : -1 === [200, 301, 302].indexOf(e.status) ? "critical" : null !== e.rtt_warning && e.elapsed > e.rtt_warning ? "warning" : "ok"
                 }
             },
-            _h = (0, ec.Z)(xh, [
+            yh = (0, ec.Z)(vh, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", dh, [(li(!0), pi(ni, null, pr(s.ports, ((t, n) => (li(), pi("div", {
+                    return li(), pi("section", lh, [(li(!0), pi(ni, null, pr(s.ports, ((t, n) => (li(), pi("div", {
                         class: "table-row",
                         key: n
-                    }, [wi("div", fh, [Ti(" prettier-ignore "), Si(" " + pe(e.$filters.minSize(t.description ? t.description : t.host + " " + t.port, 20)), 1)]), ph, t.host ? (li(), pi("div", {
+                    }, [wi("div", ch, [Ti(" prettier-ignore "), Si(" " + pe(e.$filters.minSize(t.description ? t.description : t.host + " " + t.port, 20)), 1)]), uh, t.host ? (li(), pi("div", {
                         key: 0,
                         class: ce([s.getPortDecoration(t), "table-cell"])
-                    }, ["null" == t.status ? (li(), pi("span", hh, "Scanning")) : "false" == t.status ? (li(), pi("span", gh, "Timeout")) : "true" == t.status ? (li(), pi("span", mh, "Open")) : (li(), pi("span", bh, pe(e.$filters.number(1e3 * t.status, 0)) + "ms", 1))], 2)) : Ti("v-if", !0), t.url ? (li(), pi("div", {
+                    }, ["null" == t.status ? (li(), pi("span", dh, "Scanning")) : "false" == t.status ? (li(), pi("span", fh, "Timeout")) : "true" == t.status ? (li(), pi("span", ph, "Open")) : (li(), pi("span", hh, pe(e.$filters.number(1e3 * t.status, 0)) + "ms", 1))], 2)) : Ti("v-if", !0), t.url ? (li(), pi("div", {
                         key: 1,
                         class: ce([s.getWebDecoration(t), "table-cell"])
-                    }, ["null" == t.status ? (li(), pi("span", vh, "Scanning")) : "Error" == t.status ? (li(), pi("span", yh, "Error")) : (li(), pi("span", wh, "Code " + pe(t.status), 1))], 2)) : Ti("v-if", !0)])))), 128))])
+                    }, ["null" == t.status ? (li(), pi("span", gh, "Scanning")) : "Error" == t.status ? (li(), pi("span", mh, "Error")) : (li(), pi("span", bh, "Code " + pe(t.status), 1))], 2)) : Ti("v-if", !0)])))), 128))])
                 }]
             ]),
-            kh = {
+            wh = {
                 key: 0
             },
-            Sh = {
+            xh = {
                 key: 1
             },
-            Ch = {
+            _h = {
                 key: 0,
                 class: "row"
             },
-            Th = {
+            kh = {
                 class: "col-lg-18"
             };
-        const Ah = {
+        const Sh = {
                 id: "amps",
                 class: "plugin"
             },
-            Eh = {
+            Ch = {
                 class: "table"
             },
-            Oh = {
+            Th = {
                 key: 0,
                 class: "table-cell text-left"
             },
-            Ih = ["innerHTML"];
-        const Ph = {
+            Ah = ["innerHTML"];
+        const Eh = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 computed: {
                     stats() {
@@ -16751,38 +16748,38 @@
                             n = e.countmin,
                             r = e.countmax;
                         let i = "ok";
                         return i = t > 0 ? (null === n || t >= n) && (null === r || t <= r) ? "ok" : "careful" : null === n ? "ok" : "critical", i
                     }
                 }
             },
-            Nh = (0, ec.Z)(Ph, [
+            Oh = (0, ec.Z)(Eh, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", Ah, [wi("div", Eh, [(li(!0), pi(ni, null, pr(s.processes, ((t, n) => (li(), pi("div", {
+                    return li(), pi("section", Sh, [wi("div", Ch, [(li(!0), pi(ni, null, pr(s.processes, ((t, n) => (li(), pi("div", {
                         class: "table-row",
                         key: n
                     }, [wi("div", {
                         class: ce(["table-cell text-left", s.getNameDecoration(t)])
-                    }, pe(t.name), 3), t.regex ? (li(), pi("div", Oh, pe(t.count), 1)) : Ti("v-if", !0), wi("div", {
+                    }, pe(t.name), 3), t.regex ? (li(), pi("div", Th, pe(t.count), 1)) : Ti("v-if", !0), wi("div", {
                         class: "table-cell text-left process-result",
                         innerHTML: e.$filters.nl2br(t.result)
-                    }, null, 8, Ih)])))), 128))])])
+                    }, null, 8, Ah)])))), 128))])])
                 }]
             ]),
-            Lh = {
+            Ih = {
                 id: "processcount",
                 class: "plugin"
             },
-            Dh = wi("span", {
+            Ph = wi("span", {
                 class: "title"
             }, "TASKS", -1),
-            Mh = {
+            Nh = {
                 class: "title"
             };
-        const jh = {
+        const Lh = {
                 props: {
                     data: {
                         type: Object
                     },
                     sorter: {
                         type: Object
                     }
@@ -16810,68 +16807,68 @@
                         return this.stats.stopped || 0
                     },
                     thread() {
                         return this.stats.thread || 0
                     }
                 }
             },
-            Rh = (0, ec.Z)(jh, [
+            Dh = (0, ec.Z)(Lh, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", Lh, [Dh, wi("span", null, pe(s.total) + " (" + pe(s.thread) + " thr),", 1), wi("span", null, pe(s.running) + " run,", 1), wi("span", null, pe(s.sleeping) + " slp,", 1), wi("span", null, pe(s.stopped) + " oth", 1), wi("span", null, pe(s.args.programs ? "Programs" : "Threads"), 1), wi("span", Mh, pe(n.sorter.auto ? "sorted automatically" : "sorted"), 1), wi("span", null, "by " + pe(n.sorter.getColumnLabel(n.sorter.column)), 1)])
+                    return li(), pi("section", Ih, [Ph, wi("span", null, pe(s.total) + " (" + pe(s.thread) + " thr),", 1), wi("span", null, pe(s.running) + " run,", 1), wi("span", null, pe(s.sleeping) + " slp,", 1), wi("span", null, pe(s.stopped) + " oth", 1), wi("span", null, pe(s.args.programs ? "Programs" : "Threads"), 1), wi("span", Nh, pe(n.sorter.auto ? "sorted automatically" : "sorted"), 1), wi("span", null, "by " + pe(n.sorter.getColumnLabel(n.sorter.column)), 1)])
                 }]
             ]),
-            qh = {
+            Mh = {
                 id: "processlist-plugin",
                 class: "plugin"
             },
-            Bh = {
+            jh = {
                 class: "table"
             },
-            Uh = {
+            Rh = {
                 class: "table-row"
             },
-            Fh = wi("div", {
+            qh = wi("div", {
                 class: "table-cell hidden-xs hidden-sm"
             }, "VIRT", -1),
-            $h = wi("div", {
+            Bh = wi("div", {
                 class: "table-cell hidden-xs hidden-sm"
             }, "RES", -1),
-            zh = wi("div", {
+            Uh = wi("div", {
                 class: "table-cell"
             }, "PID", -1),
-            Hh = wi("div", {
+            Fh = wi("div", {
                 class: "table-cell"
             }, "NI", -1),
-            Vh = wi("div", {
+            $h = wi("div", {
                 class: "table-cell"
             }, "S", -1),
-            Gh = {
+            zh = {
                 class: "table-cell hidden-xs hidden-sm"
             },
-            Wh = {
+            Hh = {
                 class: "table-cell hidden-xs hidden-sm"
             },
-            Zh = {
+            Vh = {
                 class: "table-cell"
             },
-            Kh = {
+            Gh = {
                 class: "table-cell text-left"
             },
-            Qh = {
+            Wh = {
                 key: 0,
                 class: "table-cell hidden-xs hidden-sm"
             },
-            Xh = {
+            Zh = {
                 key: 1,
                 class: "table-cell hidden-xs hidden-sm"
             },
-            Jh = {
+            Kh = {
                 class: "table-cell text-left hidden-xs hidden-sm"
             };
-        const Yh = {
+        const Qh = {
                 props: {
                     data: {
                         type: Object
                     },
                     sorter: {
                         type: Object
                     }
@@ -16888,15 +16885,15 @@
                     },
                     stats() {
                         return this.data.stats.processlist
                     },
                     processes() {
                         const {
                             sorter: e
-                        } = this, t = this.data.stats.isWindows, n = (this.stats || []).map((e => (e.memvirt = "?", e.memres = "?", e.memory_info && (e.memvirt = e.memory_info[1], e.memres = e.memory_info[0]), e.timeplus = "?", e.timemillis = "?", e.cpu_times && (e.timeplus = Ju(e.cpu_times), e.timemillis = Xu(e.cpu_times)), null === e.num_threads && (e.num_threads = -1), null === e.cpu_percent && (e.cpu_percent = -1), null === e.memory_percent && (e.memory_percent = -1), e.io_read = null, e.io_write = null, e.io_counters && (e.io_read = (e.io_counters[0] - e.io_counters[2]) / e.time_since_update, e.io_write = (e.io_counters[1] - e.io_counters[3]) / e.time_since_update), e.isNice = void 0 !== e.nice && (t && 32 != e.nice || !t && 0 != e.nice), Array.isArray(e.cmdline) && (e.cmdline = e.cmdline.join(" ").replace(/\n/g, " ")), null === e.cmdline && (e.cmdline = e.name), t && null !== e.username && (e.username = (0, cc.last)(e.username.split("\\"))), e)));
+                        } = this, t = this.data.stats.isWindows, n = (this.stats || []).map((e => (e.memvirt = "?", e.memres = "?", e.memory_info && (e.memvirt = e.memory_info[1], e.memres = e.memory_info[0]), e.timeplus = "?", e.timemillis = "?", e.cpu_times && (e.timeplus = Xu(e.cpu_times), e.timemillis = Qu(e.cpu_times)), null === e.num_threads && (e.num_threads = -1), null === e.cpu_percent && (e.cpu_percent = -1), null === e.memory_percent && (e.memory_percent = -1), e.io_read = null, e.io_write = null, e.io_counters && (e.io_read = (e.io_counters[0] - e.io_counters[2]) / e.time_since_update, e.io_write = (e.io_counters[1] - e.io_counters[3]) / e.time_since_update), e.isNice = void 0 !== e.nice && (t && 32 != e.nice || !t && 0 != e.nice), Array.isArray(e.cmdline) && (e.cmdline = e.cmdline.join(" ").replace(/\n/g, " ")), null === e.cmdline && (e.cmdline = e.name), t && null !== e.username && (e.username = (0, cc.last)(e.username.split("\\"))), e)));
                         return (0, cc.orderBy)(n, [e.column].reduce(((e, t) => ("io_counters" === t && (t = ["io_read", "io_write"]), e.concat(t))), []), [e.isReverseColumn(e.column) ? "desc" : "asc"]).slice(0, this.limit)
                     },
                     ioReadWritePresent() {
                         return (this.stats || []).some((({
                             io_counters: e
                         }) => e))
                     },
@@ -16905,36 +16902,36 @@
                     }
                 },
                 methods: {
                     getCpuPercentAlert: e => Fo.getAlert("processlist", "processlist_cpu_", e.cpu_percent),
                     getMemoryPercentAlert: e => Fo.getAlert("processlist", "processlist_mem_", e.cpu_percent)
                 }
             },
-            eg = {
+            Xh = {
                 components: {
-                    GlancesPluginAmps: Nh,
-                    GlancesPluginProcesscount: Rh,
-                    GlancesPluginProcesslist: (0, ec.Z)(Yh, [
+                    GlancesPluginAmps: Oh,
+                    GlancesPluginProcesscount: Dh,
+                    GlancesPluginProcesslist: (0, ec.Z)(Qh, [
                         ["render", function(e, t, n, r, i, s) {
-                            return li(), pi(ni, null, [Ti(" prettier-ignore "), wi("section", qh, [wi("div", Bh, [wi("div", Uh, [wi("div", {
+                            return li(), pi(ni, null, [Ti(" prettier-ignore "), wi("section", Mh, [wi("div", jh, [wi("div", Rh, [wi("div", {
                                 class: ce(["table-cell", ["sortable", "cpu_percent" === n.sorter.column && "sort"]]),
                                 onClick: t[0] || (t[0] = t => e.$emit("update:sorter", "cpu_percent"))
                             }, " CPU% ", 2), wi("div", {
                                 class: ce(["table-cell", ["sortable", "memory_percent" === n.sorter.column && "sort"]]),
                                 onClick: t[1] || (t[1] = t => e.$emit("update:sorter", "memory_percent"))
-                            }, " MEM% ", 2), Fh, $h, zh, wi("div", {
+                            }, " MEM% ", 2), qh, Bh, Uh, wi("div", {
                                 class: ce(["table-cell text-left", ["sortable", "username" === n.sorter.column && "sort"]]),
                                 onClick: t[2] || (t[2] = t => e.$emit("update:sorter", "username"))
                             }, " USER ", 2), wi("div", {
                                 class: ce(["table-cell hidden-xs hidden-sm", ["sortable", "timemillis" === n.sorter.column && "sort"]]),
                                 onClick: t[3] || (t[3] = t => e.$emit("update:sorter", "timemillis"))
                             }, " TIME+ ", 2), wi("div", {
                                 class: ce(["table-cell text-left hidden-xs hidden-sm", ["sortable", "num_threads" === n.sorter.column && "sort"]]),
                                 onClick: t[4] || (t[4] = t => e.$emit("update:sorter", "num_threads"))
-                            }, " THR ", 2), Hh, Vh, On(wi("div", {
+                            }, " THR ", 2), Fh, $h, On(wi("div", {
                                 class: ce(["table-cell hidden-xs hidden-sm", ["sortable", "io_counters" === n.sorter.column && "sort"]]),
                                 onClick: t[5] || (t[5] = t => e.$emit("update:sorter", "io_counters"))
                             }, " IOR/s ", 2), [
                                 [Ds, s.ioReadWritePresent]
                             ]), On(wi("div", {
                                 class: ce(["table-cell text-left hidden-xs hidden-sm", ["sortable", "io_counters" === n.sorter.column && "sort"]]),
                                 onClick: t[6] || (t[6] = t => e.$emit("update:sorter", "io_counters"))
@@ -16946,21 +16943,21 @@
                             }, " Command ", 2)]), (li(!0), pi(ni, null, pr(s.processes, ((t, n) => (li(), pi("div", {
                                 class: "table-row",
                                 key: n
                             }, [wi("div", {
                                 class: ce(["table-cell", s.getCpuPercentAlert(t)])
                             }, pe(-1 == t.cpu_percent ? "?" : e.$filters.number(t.cpu_percent, 1)), 3), wi("div", {
                                 class: ce(["table-cell", s.getMemoryPercentAlert(t)])
-                            }, pe(-1 == t.memory_percent ? "?" : e.$filters.number(t.memory_percent, 1)), 3), wi("div", Gh, pe(e.$filters.bytes(t.memvirt)), 1), wi("div", Wh, pe(e.$filters.bytes(t.memres)), 1), wi("div", Zh, pe(t.pid), 1), wi("div", Kh, pe(t.username), 1), "?" != t.timeplus ? (li(), pi("div", Qh, [On(wi("span", {
+                            }, pe(-1 == t.memory_percent ? "?" : e.$filters.number(t.memory_percent, 1)), 3), wi("div", zh, pe(e.$filters.bytes(t.memvirt)), 1), wi("div", Hh, pe(e.$filters.bytes(t.memres)), 1), wi("div", Vh, pe(t.pid), 1), wi("div", Gh, pe(t.username), 1), "?" != t.timeplus ? (li(), pi("div", Wh, [On(wi("span", {
                                 class: "highlight"
                             }, pe(t.timeplus.hours) + "h", 513), [
                                 [Ds, t.timeplus.hours > 0]
                             ]), Si(" " + pe(e.$filters.leftPad(t.timeplus.minutes, 2, "0")) + ":" + pe(e.$filters.leftPad(t.timeplus.seconds, 2, "0")) + " ", 1), On(wi("span", null, "." + pe(e.$filters.leftPad(t.timeplus.milliseconds, 2, "0")), 513), [
                                 [Ds, t.timeplus.hours <= 0]
-                            ])])) : Ti("v-if", !0), "?" == t.timeplus ? (li(), pi("div", Xh, "?")) : Ti("v-if", !0), wi("div", Jh, pe(-1 == t.num_threads ? "?" : t.num_threads), 1), wi("div", {
+                            ])])) : Ti("v-if", !0), "?" == t.timeplus ? (li(), pi("div", Zh, "?")) : Ti("v-if", !0), wi("div", Kh, pe(-1 == t.num_threads ? "?" : t.num_threads), 1), wi("div", {
                                 class: ce(["table-cell", {
                                     nice: t.isNice
                                 }])
                             }, pe(e.$filters.exclamation(t.nice)), 3), wi("div", {
                                 class: ce(["table-cell", {
                                     status: "R" == t.status
                                 }])
@@ -17024,104 +17021,104 @@
                                     } [e] || e
                                 }
                             })
                         }
                     }
                 }
             },
-            tg = (0, ec.Z)(eg, [
+            Jh = (0, ec.Z)(Xh, [
                 ["render", function(e, t, n, r, i, s) {
                     const o = cr("glances-plugin-processcount"),
                         a = cr("glances-plugin-amps"),
                         l = cr("glances-plugin-processlist");
-                    return s.args.disable_process ? (li(), pi("div", kh, "PROCESSES DISABLED (press 'z' to display)")) : (li(), pi("div", Sh, [xi(o, {
+                    return s.args.disable_process ? (li(), pi("div", wh, "PROCESSES DISABLED (press 'z' to display)")) : (li(), pi("div", xh, [xi(o, {
                         sorter: i.sorter,
                         data: n.data
-                    }, null, 8, ["sorter", "data"]), s.args.disable_amps ? Ti("v-if", !0) : (li(), pi("div", Ch, [wi("div", Th, [xi(a, {
+                    }, null, 8, ["sorter", "data"]), s.args.disable_amps ? Ti("v-if", !0) : (li(), pi("div", _h, [wi("div", kh, [xi(a, {
                         data: n.data
                     }, null, 8, ["data"])])])), xi(l, {
                         sorter: i.sorter,
                         data: n.data,
                         "onUpdate:sorter": t[0] || (t[0] = e => s.args.sort_processes_key = e)
                     }, null, 8, ["sorter", "data"])]))
                 }]
             ]),
-            ng = {
+            Yh = {
                 id: "quicklook",
                 class: "plugin"
             },
-            rg = {
+            eg = {
                 class: "cpu-name"
             },
-            ig = {
+            tg = {
                 class: "table"
             },
-            sg = {
+            ng = {
                 key: 0,
                 class: "table-row"
             },
-            og = wi("div", {
+            rg = wi("div", {
                 class: "table-cell text-left"
             }, "CPU", -1),
-            ag = {
+            ig = {
                 class: "table-cell"
             },
-            lg = {
+            sg = {
                 class: "progress"
             },
-            cg = ["aria-valuenow"],
-            ug = {
+            og = ["aria-valuenow"],
+            ag = {
                 class: "table-cell"
             },
-            dg = {
+            lg = {
                 class: "table-cell text-left"
             },
-            fg = {
+            cg = {
                 class: "table-cell"
             },
-            pg = {
+            ug = {
                 class: "progress"
             },
-            hg = ["aria-valuenow"],
-            gg = {
+            dg = ["aria-valuenow"],
+            fg = {
                 class: "table-cell"
             },
-            mg = {
+            pg = {
                 class: "table-row"
             },
-            bg = wi("div", {
+            hg = wi("div", {
                 class: "table-cell text-left"
             }, "MEM", -1),
-            vg = {
+            gg = {
                 class: "table-cell"
             },
-            yg = {
+            mg = {
                 class: "progress"
             },
-            wg = ["aria-valuenow"],
-            xg = {
+            bg = ["aria-valuenow"],
+            vg = {
                 class: "table-cell"
             },
-            _g = {
+            yg = {
                 class: "table-row"
             },
-            kg = wi("div", {
+            wg = wi("div", {
                 class: "table-cell text-left"
             }, "SWAP", -1),
-            Sg = {
+            xg = {
                 class: "table-cell"
             },
-            Cg = {
+            _g = {
                 class: "progress"
             },
-            Tg = ["aria-valuenow"],
-            Ag = {
+            kg = ["aria-valuenow"],
+            Sg = {
                 class: "table-cell"
             };
-        const Eg = {
+        const Cg = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 data: () => ({
                     store: qo
@@ -17166,74 +17163,74 @@
                 },
                 methods: {
                     getDecoration(e) {
                         if (void 0 !== this.view[e]) return this.view[e].decoration.toLowerCase()
                     }
                 }
             },
-            Og = (0, ec.Z)(Eg, [
+            Tg = (0, ec.Z)(Cg, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", ng, [wi("div", rg, pe(s.cpu_name), 1), wi("div", ig, [s.args.percpu ? Ti("v-if", !0) : (li(), pi("div", sg, [og, wi("div", ag, [wi("div", lg, [wi("div", {
+                    return li(), pi("section", Yh, [wi("div", eg, pe(s.cpu_name), 1), wi("div", tg, [s.args.percpu ? Ti("v-if", !0) : (li(), pi("div", ng, [rg, wi("div", ig, [wi("div", sg, [wi("div", {
                         class: ce(`progress-bar progress-bar-${s.getDecoration("cpu")}`),
                         role: "progressbar",
                         "aria-valuenow": s.cpu,
                         "aria-valuemin": "0",
                         "aria-valuemax": "100",
                         style: ie(`width: ${s.cpu}%;`)
-                    }, "   ", 14, cg)])]), wi("div", ug, pe(s.cpu) + "%", 1)])), s.args.percpu ? (li(!0), pi(ni, {
+                    }, "   ", 14, og)])]), wi("div", ag, pe(s.cpu) + "%", 1)])), s.args.percpu ? (li(!0), pi(ni, {
                         key: 1
                     }, pr(s.percpus, ((e, t) => (li(), pi("div", {
                         class: "table-row",
                         key: t
-                    }, [wi("div", dg, "CPU" + pe(e.number), 1), wi("div", fg, [wi("div", pg, [wi("div", {
+                    }, [wi("div", lg, "CPU" + pe(e.number), 1), wi("div", cg, [wi("div", ug, [wi("div", {
                         class: ce(`progress-bar progress-bar-${s.getDecoration("cpu")}`),
                         role: "progressbar",
                         "aria-valuenow": e.total,
                         "aria-valuemin": "0",
                         "aria-valuemax": "100",
                         style: ie(`width: ${e.total}%;`)
-                    }, "   ", 14, hg)])]), wi("div", gg, pe(e.total) + "%", 1)])))), 128)) : Ti("v-if", !0), wi("div", mg, [bg, wi("div", vg, [wi("div", yg, [wi("div", {
+                    }, "   ", 14, dg)])]), wi("div", fg, pe(e.total) + "%", 1)])))), 128)) : Ti("v-if", !0), wi("div", pg, [hg, wi("div", gg, [wi("div", mg, [wi("div", {
                         class: ce(`progress-bar progress-bar-${s.getDecoration("mem")}`),
                         role: "progressbar",
                         "aria-valuenow": s.mem,
                         "aria-valuemin": "0",
                         "aria-valuemax": "100",
                         style: ie(`width: ${s.mem}%;`)
-                    }, "   ", 14, wg)])]), wi("div", xg, pe(s.mem) + "%", 1)]), wi("div", _g, [kg, wi("div", Sg, [wi("div", Cg, [wi("div", {
+                    }, "   ", 14, bg)])]), wi("div", vg, pe(s.mem) + "%", 1)]), wi("div", yg, [wg, wi("div", xg, [wi("div", _g, [wi("div", {
                         class: ce(`progress-bar progress-bar-${s.getDecoration("swap")}`),
                         role: "progressbar",
                         "aria-valuenow": s.swap,
                         "aria-valuemin": "0",
                         "aria-valuemax": "100",
                         style: ie(`width: ${s.swap}%;`)
-                    }, "   ", 14, Tg)])]), wi("div", Ag, pe(s.swap) + "%", 1)])])])
+                    }, "   ", 14, kg)])]), wi("div", Sg, pe(s.swap) + "%", 1)])])])
                 }]
             ]),
-            Ig = {
+            Ag = {
                 class: "plugin",
                 id: "raid"
             },
-            Pg = {
+            Eg = {
                 key: 0,
                 class: "table-row"
             },
-            Ng = [wi("div", {
+            Og = [wi("div", {
                 class: "table-cell text-left title"
             }, "RAID disks", -1), wi("div", {
                 class: "table-cell"
             }, "Used", -1), wi("div", {
                 class: "table-cell"
             }, "Total", -1)],
-            Lg = {
+            Ig = {
                 class: "table-cell text-left"
             },
-            Dg = {
+            Pg = {
                 class: "warning"
             };
-        const Mg = {
+        const Ng = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 computed: {
                     stats() {
@@ -17263,20 +17260,20 @@
                         return this.disks.length > 0
                     }
                 },
                 methods: {
                     getAlert: e => e.inactive ? "critical" : e.degraded ? "warning" : "ok"
                 }
             },
-            jg = (0, ec.Z)(Mg, [
+            Lg = (0, ec.Z)(Ng, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", Ig, [s.hasDisks ? (li(), pi("div", Pg, Ng)) : Ti("v-if", !0), (li(!0), pi(ni, null, pr(s.disks, ((e, t) => (li(), pi("div", {
+                    return li(), pi("section", Ag, [s.hasDisks ? (li(), pi("div", Eg, Og)) : Ti("v-if", !0), (li(!0), pi(ni, null, pr(s.disks, ((e, t) => (li(), pi("div", {
                         class: "table-row",
                         key: t
-                    }, [wi("div", Lg, [Si(pe(e.type.toUppercase()) + " " + pe(e.name) + " ", 1), On(wi("div", Dg, "└─ Degraded mode", 512), [
+                    }, [wi("div", Ig, [Si(pe(e.type.toUppercase()) + " " + pe(e.name) + " ", 1), On(wi("div", Pg, "└─ Degraded mode", 512), [
                         [Ds, e.degraded]
                     ]), On(wi("div", null, "   └─ " + pe(e.config), 513), [
                         [Ds, e.degraded]
                     ]), On(wi("div", {
                         class: "critical"
                     }, "└─ Status " + pe(e.status), 513), [
                         [Ds, e.inactive]
@@ -17291,32 +17288,32 @@
                     ]), On(wi("div", {
                         class: ce(["table-cell", s.getAlert(e)])
                     }, pe(e.available), 3), [
                         [Ds, !e.inactive]
                     ])])))), 128))])
                 }]
             ]),
-            Rg = {
+            Dg = {
                 class: "plugin",
                 id: "sensors"
             },
-            qg = {
+            Mg = {
                 key: 0,
                 class: "table-row"
             },
-            Bg = [wi("div", {
+            jg = [wi("div", {
                 class: "table-cell text-left title"
             }, "SENSORS", -1)],
-            Ug = {
+            Rg = {
                 class: "table-cell text-left"
             },
-            Fg = {
+            qg = {
                 class: "table-cell"
             };
-        const $g = {
+        const Bg = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 data: () => ({
                     store: qo
@@ -17335,44 +17332,44 @@
                 methods: {
                     getAlert(e) {
                         const t = "battery" == e.type ? 100 - e.value : e.value;
                         return Fo.getAlert("sensors", "sensors_" + e.type + "_", t)
                     }
                 }
             },
-            zg = (0, ec.Z)($g, [
+            Ug = (0, ec.Z)(Bg, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", Rg, [s.sensors.length > 0 ? (li(), pi("div", qg, Bg)) : Ti("v-if", !0), (li(!0), pi(ni, null, pr(s.sensors, ((e, t) => (li(), pi("div", {
+                    return li(), pi("section", Dg, [s.sensors.length > 0 ? (li(), pi("div", Mg, jg)) : Ti("v-if", !0), (li(!0), pi(ni, null, pr(s.sensors, ((e, t) => (li(), pi("div", {
                         class: "table-row",
                         key: t
-                    }, [wi("div", Ug, pe(e.label), 1), wi("div", Fg, pe(e.unit), 1), wi("div", {
+                    }, [wi("div", Rg, pe(e.label), 1), wi("div", qg, pe(e.unit), 1), wi("div", {
                         class: ce(["table-cell", s.getAlert(e)])
                     }, pe(e.value), 3)])))), 128))])
                 }]
             ]),
-            Hg = {
+            Fg = {
                 class: "plugin",
                 id: "system"
             },
-            Vg = {
+            $g = {
                 key: 0,
                 class: "critical"
             },
-            Gg = {
+            zg = {
                 class: "title"
             },
-            Wg = {
+            Hg = {
                 key: 1,
                 class: "hidden-xs hidden-sm"
             },
-            Zg = {
+            Vg = {
                 key: 2,
                 class: "hidden-xs hidden-sm"
             };
-        const Kg = {
+        const Gg = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 data: () => ({
                     store: qo
@@ -17400,65 +17397,65 @@
                         return this.stats.hr_name
                     },
                     isDisconnected() {
                         return "FAILURE" === this.store.status
                     }
                 }
             },
-            Qg = (0, ec.Z)(Kg, [
+            Wg = (0, ec.Z)(Gg, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", Hg, [s.isDisconnected ? (li(), pi("span", Vg, "Disconnected from")) : Ti("v-if", !0), wi("span", Gg, pe(s.hostname), 1), s.isLinux ? (li(), pi("span", Wg, " (" + pe(s.humanReadableName) + " / " + pe(s.os.name) + " " + pe(s.os.version) + ") ", 1)) : Ti("v-if", !0), s.isLinux ? Ti("v-if", !0) : (li(), pi("span", Zg, " (" + pe(s.os.name) + " " + pe(s.os.version) + " " + pe(s.platform) + ") ", 1))])
+                    return li(), pi("section", Fg, [s.isDisconnected ? (li(), pi("span", $g, "Disconnected from")) : Ti("v-if", !0), wi("span", zg, pe(s.hostname), 1), s.isLinux ? (li(), pi("span", Hg, " (" + pe(s.humanReadableName) + " / " + pe(s.os.name) + " " + pe(s.os.version) + ") ", 1)) : Ti("v-if", !0), s.isLinux ? Ti("v-if", !0) : (li(), pi("span", Vg, " (" + pe(s.os.name) + " " + pe(s.os.version) + " " + pe(s.platform) + ") ", 1))])
                 }]
             ]),
-            Xg = {
+            Zg = {
                 class: "plugin",
                 id: "uptime"
             };
-        const Jg = {
+        const Kg = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 computed: {
                     value() {
                         return this.data.stats.uptime
                     }
                 }
             },
-            Yg = (0, ec.Z)(Jg, [
+            Qg = (0, ec.Z)(Kg, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", Xg, [wi("span", null, "Uptime: " + pe(s.value), 1)])
+                    return li(), pi("section", Zg, [wi("span", null, "Uptime: " + pe(s.value), 1)])
                 }]
             ]),
-            em = {
+            Xg = {
                 class: "plugin",
                 id: "wifi"
             },
-            tm = {
+            Jg = {
                 key: 0,
                 class: "table-row"
             },
-            nm = [wi("div", {
+            Yg = [wi("div", {
                 class: "table-cell text-left title"
             }, "WIFI", -1), wi("div", {
                 class: "table-cell"
             }, null, -1), wi("div", {
                 class: "table-cell"
             }, "dBm", -1)],
-            rm = {
+            em = {
                 class: "table-cell text-left"
             },
-            im = {
+            tm = {
                 key: 0
             },
-            sm = wi("div", {
+            nm = wi("div", {
                 class: "table-cell"
             }, null, -1);
-        const om = {
+        const rm = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 computed: {
                     stats() {
@@ -17481,48 +17478,48 @@
                 },
                 methods: {
                     getDecoration(e, t) {
                         if (void 0 !== this.view[e.ssid][t]) return this.view[e.ssid][t].decoration.toLowerCase()
                     }
                 }
             },
-            am = {
+            im = {
                 components: {
                     GlancesHelp: tc,
                     GlancesPluginAlert: dc,
                     GlancesPluginCloud: gc,
                     GlancesPluginConnections: qc,
-                    GlancesPluginCpu: Nu,
-                    GlancesPluginDiskio: ed,
-                    GlancesPluginContainers: kd,
-                    GlancesPluginFolders: Id,
-                    GlancesPluginFs: Ud,
-                    GlancesPluginGpu: sf,
-                    GlancesPluginIp: pf,
-                    GlancesPluginIrq: xf,
-                    GlancesPluginLoad: Mf,
-                    GlancesPluginMem: Qf,
-                    GlancesPluginMemMore: fp,
-                    GlancesPluginMemswap: Ap,
-                    GlancesPluginNetwork: Vp,
-                    GlancesPluginNow: Zp,
-                    GlancesPluginPercpu: uh,
-                    GlancesPluginPorts: _h,
-                    GlancesPluginProcess: tg,
-                    GlancesPluginQuicklook: Og,
-                    GlancesPluginRaid: jg,
-                    GlancesPluginSensors: zg,
-                    GlancesPluginSystem: Qg,
-                    GlancesPluginUptime: Yg,
-                    GlancesPluginWifi: (0, ec.Z)(om, [
+                    GlancesPluginCpu: Pu,
+                    GlancesPluginDiskio: Yu,
+                    GlancesPluginContainers: _d,
+                    GlancesPluginFolders: Od,
+                    GlancesPluginFs: Bd,
+                    GlancesPluginGpu: rf,
+                    GlancesPluginIp: ff,
+                    GlancesPluginIrq: wf,
+                    GlancesPluginLoad: Df,
+                    GlancesPluginMem: Zf,
+                    GlancesPluginMemMore: up,
+                    GlancesPluginMemswap: Sp,
+                    GlancesPluginNetwork: $p,
+                    GlancesPluginNow: Vp,
+                    GlancesPluginPercpu: ah,
+                    GlancesPluginPorts: yh,
+                    GlancesPluginProcess: Jh,
+                    GlancesPluginQuicklook: Tg,
+                    GlancesPluginRaid: Lg,
+                    GlancesPluginSensors: Ug,
+                    GlancesPluginSystem: Wg,
+                    GlancesPluginUptime: Qg,
+                    GlancesPluginWifi: (0, ec.Z)(rm, [
                         ["render", function(e, t, n, r, i, s) {
-                            return li(), pi("section", em, [s.hotspots.length > 0 ? (li(), pi("div", tm, nm)) : Ti("v-if", !0), (li(!0), pi(ni, null, pr(s.hotspots, ((t, n) => (li(), pi("div", {
+                            return li(), pi("section", Xg, [s.hotspots.length > 0 ? (li(), pi("div", Jg, Yg)) : Ti("v-if", !0), (li(!0), pi(ni, null, pr(s.hotspots, ((t, n) => (li(), pi("div", {
                                 class: "table-row",
                                 key: n
-                            }, [wi("div", rm, [Si(pe(e.$filters.limitTo(t.ssid, 20)) + " ", 1), t.encrypted ? (li(), pi("span", im, pe(t.encryption_type), 1)) : Ti("v-if", !0)]), sm, wi("div", {
+                            }, [wi("div", em, [Si(pe(e.$filters.limitTo(t.ssid, 20)) + " ", 1), t.encrypted ? (li(), pi("span", tm, pe(t.encryption_type), 1)) : Ti("v-if", !0)]), nm, wi("div", {
                                 class: ce(["table-cell", s.getDecoration(t, "signal")])
                             }, pe(t.signal), 3)])))), 128))])
                         }]
                     ])
                 },
                 data: () => ({
                     store: qo
@@ -17633,28 +17630,28 @@
                         t = isFinite(e["refresh-time"]) ? parseInt(e["refresh-time"], 10) : void 0;
                     $o.init(t), this.setupHotKeys()
                 },
                 beforeUnmount() {
                     Do.unbind()
                 }
             };
-        const lm = ((...e) => {
+        const sm = ((...e) => {
             const t = qs().createApp(...e);
             const {
                 mount: n
             } = t;
             return t.mount = e => {
                 const r = Bs(e);
                 if (!r) return;
                 const i = t._component;
                 L(i) || i.render || i.template || (i.template = r.innerHTML), r.innerHTML = "";
                 const s = n(r, !1, r instanceof SVGElement);
                 return r instanceof Element && (r.removeAttribute("v-cloak"), r.setAttribute("data-v-app", "")), s
             }, t
-        })((0, ec.Z)(am, [
+        })((0, ec.Z)(im, [
             ["render", function(e, t, n, r, i, s) {
                 const o = cr("glances-help"),
                     a = cr("glances-plugin-system"),
                     l = cr("glances-plugin-ip"),
                     c = cr("glances-plugin-uptime"),
                     u = cr("glances-plugin-cloud"),
                     d = cr("glances-plugin-quicklook"),
@@ -17764,10 +17761,10 @@
                     data: s.data
                 }, null, 8, ["data"]), s.args.disable_alert ? Ti("v-if", !0) : (li(), hi(N, {
                     key: 1,
                     data: s.data
                 }, null, 8, ["data"]))])])])])) : (li(), pi("div", Us, Fs))
             }]
         ]));
-        lm.config.globalProperties.$filters = e, lm.mount("#app")
+        sm.config.globalProperties.$filters = e, sm.mount("#app")
     })()
 })();
```

### Comparing `Glances-3.4.0.2/glances/outputs/static/webpack.config.js` & `Glances-3.4.0.3/glances/outputs/static/webpack.config.js`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/password.py` & `Glances-3.4.0.3/glances/password.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/password_list.py` & `Glances-3.4.0.3/glances/password_list.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/containers/glances_docker.py` & `Glances-3.4.0.3/glances/plugins/containers/glances_docker.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/containers/glances_podman.py` & `Glances-3.4.0.3/glances/plugins/containers/glances_podman.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/containers/stats_streamer.py` & `Glances-3.4.0.3/glances/plugins/containers/stats_streamer.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_alert.py` & `Glances-3.4.0.3/glances/plugins/glances_alert.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_amps.py` & `Glances-3.4.0.3/glances/plugins/glances_amps.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_cloud.py` & `Glances-3.4.0.3/glances/plugins/glances_cloud.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_connections.py` & `Glances-3.4.0.3/glances/plugins/glances_connections.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_containers.py` & `Glances-3.4.0.3/glances/plugins/glances_containers.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_core.py` & `Glances-3.4.0.3/glances/plugins/glances_core.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_cpu.py` & `Glances-3.4.0.3/glances/plugins/glances_cpu.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_diskio.py` & `Glances-3.4.0.3/glances/plugins/glances_diskio.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_folders.py` & `Glances-3.4.0.3/glances/plugins/glances_folders.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_fs.py` & `Glances-3.4.0.3/glances/plugins/glances_fs.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_gpu.py` & `Glances-3.4.0.3/glances/plugins/glances_gpu.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_help.py` & `Glances-3.4.0.3/glances/plugins/glances_help.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_ip.py` & `Glances-3.4.0.3/glances/plugins/glances_ip.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_irq.py` & `Glances-3.4.0.3/glances/plugins/glances_irq.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_load.py` & `Glances-3.4.0.3/glances/plugins/glances_load.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_mem.py` & `Glances-3.4.0.3/glances/plugins/glances_mem.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_memswap.py` & `Glances-3.4.0.3/glances/plugins/glances_memswap.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_network.py` & `Glances-3.4.0.3/glances/plugins/glances_network.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_now.py` & `Glances-3.4.0.3/glances/plugins/glances_now.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_percpu.py` & `Glances-3.4.0.3/glances/plugins/glances_percpu.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_plugin.py` & `Glances-3.4.0.3/glances/plugins/glances_plugin.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_ports.py` & `Glances-3.4.0.3/glances/plugins/glances_ports.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_processcount.py` & `Glances-3.4.0.3/glances/plugins/glances_processcount.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_processlist.py` & `Glances-3.4.0.3/glances/plugins/glances_processlist.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_psutilversion.py` & `Glances-3.4.0.3/glances/plugins/glances_psutilversion.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_quicklook.py` & `Glances-3.4.0.3/glances/plugins/glances_quicklook.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_raid.py` & `Glances-3.4.0.3/glances/plugins/glances_raid.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_sensors.py` & `Glances-3.4.0.3/glances/plugins/glances_sensors.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_smart.py` & `Glances-3.4.0.3/glances/plugins/glances_smart.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_system.py` & `Glances-3.4.0.3/glances/plugins/glances_system.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_uptime.py` & `Glances-3.4.0.3/glances/plugins/glances_uptime.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/glances_wifi.py` & `Glances-3.4.0.3/glances/plugins/glances_wifi.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/sensors/glances_batpercent.py` & `Glances-3.4.0.3/glances/plugins/sensors/glances_batpercent.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/plugins/sensors/glances_hddtemp.py` & `Glances-3.4.0.3/glances/plugins/sensors/glances_hddtemp.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/ports_list.py` & `Glances-3.4.0.3/glances/ports_list.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/processes.py` & `Glances-3.4.0.3/glances/processes.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/programs.py` & `Glances-3.4.0.3/glances/programs.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/secure.py` & `Glances-3.4.0.3/glances/secure.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/server.py` & `Glances-3.4.0.3/glances/server.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/snmp.py` & `Glances-3.4.0.3/glances/snmp.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/standalone.py` & `Glances-3.4.0.3/glances/standalone.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/static_list.py` & `Glances-3.4.0.3/glances/static_list.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/stats.py` & `Glances-3.4.0.3/glances/stats.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/stats_client.py` & `Glances-3.4.0.3/glances/stats_client.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/stats_client_snmp.py` & `Glances-3.4.0.3/glances/stats_client_snmp.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/stats_server.py` & `Glances-3.4.0.3/glances/stats_server.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/thresholds.py` & `Glances-3.4.0.3/glances/thresholds.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/timer.py` & `Glances-3.4.0.3/glances/timer.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/web_list.py` & `Glances-3.4.0.3/glances/web_list.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/glances/webserver.py` & `Glances-3.4.0.3/glances/webserver.py`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/pyproject.toml` & `Glances-3.4.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Glances-3.4.0.2/setup.py` & `Glances-3.4.0.3/setup.py`

 * *Files identical despite different names*

