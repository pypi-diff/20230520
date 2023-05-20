# Comparing `tmp/foliolib-0.3.4a1.tar.gz` & `tmp/foliolib-0.3.5a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foliolib-0.3.4a1.tar", last modified: Sun May  7 09:06:55 2023, max compression
+gzip compressed data, was "foliolib-0.3.5a1.tar", last modified: Sat May 20 15:30:27 2023, max compression
```

## Comparing `foliolib-0.3.4a1.tar` & `foliolib-0.3.5a1.tar`

### file list

```diff
@@ -1,128 +1,136 @@
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-07 09:06:55.405771 foliolib-0.3.4a1/
--rw-r--r--   0 tobi      (1000) tobi      (1000)    35146 2020-10-11 07:41:52.000000 foliolib-0.3.4a1/COPYING
--rw-r--r--   0 tobi      (1000) tobi      (1000)       43 2020-11-07 12:13:21.000000 foliolib-0.3.4a1/MANIFEST.in
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2459 2023-05-07 09:06:55.405771 foliolib-0.3.4a1/PKG-INFO
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1719 2023-02-21 11:23:02.000000 foliolib-0.3.4a1/README.rst
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-07 09:06:55.397771 foliolib-0.3.4a1/foliolib/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1031 2023-03-24 13:25:47.000000 foliolib-0.3.4a1/foliolib/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      396 2023-05-07 09:06:54.000000 foliolib-0.3.4a1/foliolib/__version__.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-07 09:06:55.397771 foliolib-0.3.4a1/foliolib/apiBuilder/
--rw-r--r--   0 tobi      (1000) tobi      (1000)      351 2022-10-11 12:37:16.000000 foliolib-0.3.4a1/foliolib/apiBuilder/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1288 2022-03-13 04:11:25.000000 foliolib-0.3.4a1/foliolib/apiBuilder/build_api.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1586 2022-05-04 20:18:39.000000 foliolib-0.3.4a1/foliolib/apiBuilder/cli.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-07 09:06:55.397771 foliolib-0.3.4a1/foliolib/cli/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3821 2023-04-21 06:17:59.000000 foliolib-0.3.4a1/foliolib/cli/__init__.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-07 09:06:55.397771 foliolib-0.3.4a1/foliolib/cli/folio/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1461 2022-05-09 17:53:56.000000 foliolib-0.3.4a1/foliolib/cli/folio/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      229 2022-04-05 13:20:51.000000 foliolib-0.3.4a1/foliolib/cli/folio/inventory.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      634 2022-02-21 04:57:32.000000 foliolib-0.3.4a1/foliolib/cli/main.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      374 2022-02-21 04:57:41.000000 foliolib-0.3.4a1/foliolib/cli/main_err.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      895 2022-02-21 04:57:36.000000 foliolib-0.3.4a1/foliolib/cli/main_noauth.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4591 2023-04-15 04:58:38.000000 foliolib-0.3.4a1/foliolib/cli/module.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3495 2023-04-01 07:43:09.000000 foliolib-0.3.4a1/foliolib/cli/okapi.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      446 2022-02-21 04:57:17.000000 foliolib-0.3.4a1/foliolib/cli/orderedGroup.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3680 2023-02-15 15:06:27.000000 foliolib-0.3.4a1/foliolib/cli/platform.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2759 2023-04-21 05:25:46.000000 foliolib-0.3.4a1/foliolib/cli/server.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    12868 2022-10-06 05:29:03.000000 foliolib-0.3.4a1/foliolib/cli/tenant.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    12088 2023-04-21 06:26:30.000000 foliolib-0.3.4a1/foliolib/config.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      801 2022-05-09 17:52:49.000000 foliolib-0.3.4a1/foliolib/exceptions.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-07 09:06:55.401771 foliolib-0.3.4a1/foliolib/folio/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1870 2022-10-06 05:35:01.000000 foliolib-0.3.4a1/foliolib/folio/__init__.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-07 09:06:55.405771 foliolib-0.3.4a1/foliolib/folio/api/
--rw-r--r--   0 tobi      (1000) tobi      (1000)        0 2021-11-15 08:23:39.000000 foliolib-0.3.4a1/foliolib/folio/api/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     9675 2023-04-16 06:50:57.000000 foliolib-0.3.4a1/foliolib/folio/api/audit.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     6883 2023-04-16 06:50:57.000000 foliolib-0.3.4a1/foliolib/folio/api/bulkOperations.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      173 2023-04-16 06:50:57.000000 foliolib-0.3.4a1/foliolib/folio/api/calendar.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    40174 2023-04-16 06:50:57.000000 foliolib-0.3.4a1/foliolib/folio/api/circulation.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    73691 2023-04-16 06:50:57.000000 foliolib-0.3.4a1/foliolib/folio/api/circulationStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     6506 2023-04-16 06:50:57.000000 foliolib-0.3.4a1/foliolib/folio/api/configuration.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4913 2023-04-16 06:50:57.000000 foliolib-0.3.4a1/foliolib/folio/api/copycat.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    54009 2023-04-16 06:50:58.000000 foliolib-0.3.4a1/foliolib/folio/api/courses.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    19883 2023-04-16 06:50:58.000000 foliolib-0.3.4a1/foliolib/folio/api/dataExport.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     6764 2023-04-16 06:50:58.000000 foliolib-0.3.4a1/foliolib/folio/api/dataExportSpring.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     5642 2023-04-16 06:50:58.000000 foliolib-0.3.4a1/foliolib/folio/api/dataExportWorker.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    13485 2023-04-16 06:50:58.000000 foliolib-0.3.4a1/foliolib/folio/api/dataImport.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    37645 2023-04-16 06:50:58.000000 foliolib-0.3.4a1/foliolib/folio/api/dataImportConverterStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2268 2023-04-16 06:50:58.000000 foliolib-0.3.4a1/foliolib/folio/api/ebsconet.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     7884 2023-04-16 06:50:58.000000 foliolib-0.3.4a1/foliolib/folio/api/email.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4399 2023-04-16 06:50:58.000000 foliolib-0.3.4a1/foliolib/folio/api/entitiesLinks.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    25152 2023-04-16 06:50:58.000000 foliolib-0.3.4a1/foliolib/folio/api/ermUsage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4482 2023-04-16 06:50:58.000000 foliolib-0.3.4a1/foliolib/folio/api/ermUsageHarvester.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4273 2023-04-16 06:50:58.000000 foliolib-0.3.4a1/foliolib/folio/api/eventConfig.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    80620 2023-04-16 06:50:59.000000 foliolib-0.3.4a1/foliolib/folio/api/feesfines.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    76479 2023-04-16 06:50:59.000000 foliolib-0.3.4a1/foliolib/folio/api/finance.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    79172 2023-04-16 06:50:59.000000 foliolib-0.3.4a1/foliolib/folio/api/financeStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    51717 2023-04-16 06:50:59.000000 foliolib-0.3.4a1/foliolib/folio/api/fincConfig.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8283 2023-04-16 06:51:00.000000 foliolib-0.3.4a1/foliolib/folio/api/gobi.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    76551 2023-04-16 06:51:02.000000 foliolib-0.3.4a1/foliolib/folio/api/innReach.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    22929 2023-04-16 06:51:02.000000 foliolib-0.3.4a1/foliolib/folio/api/inventory.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)   217418 2023-04-16 06:51:03.000000 foliolib-0.3.4a1/foliolib/folio/api/inventoryStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     6001 2023-04-16 06:51:03.000000 foliolib-0.3.4a1/foliolib/folio/api/inventoryUpdate.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    45051 2023-04-16 06:51:03.000000 foliolib-0.3.4a1/foliolib/folio/api/invoice.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    47143 2023-04-16 06:51:03.000000 foliolib-0.3.4a1/foliolib/folio/api/invoiceStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    54294 2023-04-16 06:51:03.000000 foliolib-0.3.4a1/foliolib/folio/api/kbEbscoJava.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3051 2023-04-16 06:51:03.000000 foliolib-0.3.4a1/foliolib/folio/api/ldp.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1332 2023-04-16 06:51:03.000000 foliolib-0.3.4a1/foliolib/folio/api/licenses.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8538 2023-04-16 06:51:03.000000 foliolib-0.3.4a1/foliolib/folio/api/login.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4260 2023-04-16 06:51:03.000000 foliolib-0.3.4a1/foliolib/folio/api/loginSaml.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    17932 2023-04-16 06:51:03.000000 foliolib-0.3.4a1/foliolib/folio/api/marccat.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    20392 2023-04-16 06:51:04.000000 foliolib-0.3.4a1/foliolib/folio/api/metaStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      171 2023-04-16 06:51:04.000000 foliolib-0.3.4a1/foliolib/folio/api/notes.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8870 2023-04-16 06:51:04.000000 foliolib-0.3.4a1/foliolib/folio/api/notify.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    12105 2023-04-16 06:51:04.000000 foliolib-0.3.4a1/foliolib/folio/api/oaiPmh.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    63105 2023-04-16 06:51:04.000000 foliolib-0.3.4a1/foliolib/folio/api/orders.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    78262 2023-04-16 06:51:04.000000 foliolib-0.3.4a1/foliolib/folio/api/ordersStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4978 2023-04-16 06:51:04.000000 foliolib-0.3.4a1/foliolib/folio/api/organizations.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    45825 2023-04-16 06:51:04.000000 foliolib-0.3.4a1/foliolib/folio/api/organizationsStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3678 2023-04-16 06:51:04.000000 foliolib-0.3.4a1/foliolib/folio/api/passwordValidator.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     5893 2023-04-16 06:51:04.000000 foliolib-0.3.4a1/foliolib/folio/api/patron.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    15601 2023-04-16 06:51:04.000000 foliolib-0.3.4a1/foliolib/folio/api/patronBlocks.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    14392 2023-04-16 06:51:04.000000 foliolib-0.3.4a1/foliolib/folio/api/permissions.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     9093 2023-04-16 06:51:04.000000 foliolib-0.3.4a1/foliolib/folio/api/pubsub.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4445 2023-04-16 06:51:05.000000 foliolib-0.3.4a1/foliolib/folio/api/quickMarc.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    17286 2023-04-16 06:51:05.000000 foliolib-0.3.4a1/foliolib/folio/api/remoteStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    21589 2023-04-16 06:51:05.000000 foliolib-0.3.4a1/foliolib/folio/api/reservoir.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1928 2023-04-16 06:51:05.000000 foliolib-0.3.4a1/foliolib/folio/api/rtac.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    17486 2023-04-16 06:51:05.000000 foliolib-0.3.4a1/foliolib/folio/api/search.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      732 2023-04-16 06:51:05.000000 foliolib-0.3.4a1/foliolib/folio/api/sender.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     5425 2023-04-16 06:51:05.000000 foliolib-0.3.4a1/foliolib/folio/api/settings.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    11154 2023-04-16 06:51:05.000000 foliolib-0.3.4a1/foliolib/folio/api/sharedIndex.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    21352 2023-04-16 06:51:05.000000 foliolib-0.3.4a1/foliolib/folio/api/sourceRecordManager.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    24923 2023-04-16 06:51:05.000000 foliolib-0.3.4a1/foliolib/folio/api/sourceRecordStorage.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      170 2023-04-16 06:51:05.000000 foliolib-0.3.4a1/foliolib/folio/api/tags.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     4091 2023-04-16 06:51:05.000000 foliolib-0.3.4a1/foliolib/folio/api/templateEngine.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      870 2023-04-16 06:51:05.000000 foliolib-0.3.4a1/foliolib/folio/api/userImport.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    22806 2023-04-16 06:51:05.000000 foliolib-0.3.4a1/foliolib/folio/api/users.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    11127 2023-04-16 06:51:05.000000 foliolib-0.3.4a1/foliolib/folio/api/usersBl.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     5803 2022-05-31 09:32:11.000000 foliolib-0.3.4a1/foliolib/folio/config.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     8495 2021-02-25 09:49:29.000000 foliolib-0.3.4a1/foliolib/folio/dataImport.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      436 2022-03-17 02:39:17.000000 foliolib-0.3.4a1/foliolib/folio/exceptions.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      945 2022-04-08 08:56:47.000000 foliolib-0.3.4a1/foliolib/folio/inventory.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    24056 2022-09-15 02:29:53.000000 foliolib-0.3.4a1/foliolib/folio/inventoryReferenceData.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     9488 2022-06-03 04:45:10.000000 foliolib-0.3.4a1/foliolib/folio/users.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-07 09:06:55.405771 foliolib-0.3.4a1/foliolib/helper/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1207 2023-04-21 05:23:46.000000 foliolib-0.3.4a1/foliolib/helper/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     9311 2023-04-21 05:23:46.000000 foliolib-0.3.4a1/foliolib/helper/database.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3636 2022-10-11 03:50:00.000000 foliolib-0.3.4a1/foliolib/helper/folio.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3055 2023-02-09 19:10:16.000000 foliolib-0.3.4a1/foliolib/helper/modules.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3935 2023-04-01 06:20:04.000000 foliolib-0.3.4a1/foliolib/helper/okapi.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     5714 2023-02-18 17:54:00.000000 foliolib-0.3.4a1/foliolib/helper/platform.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1517 2022-10-11 03:48:54.000000 foliolib-0.3.4a1/foliolib/helper/tenant.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-07 09:06:55.405771 foliolib-0.3.4a1/foliolib/okapi/
--rw-r--r--   0 tobi      (1000) tobi      (1000)    14520 2022-10-13 08:48:51.000000 foliolib-0.3.4a1/foliolib/okapi/__init__.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2399 2022-07-24 04:45:10.000000 foliolib-0.3.4a1/foliolib/okapi/exceptions.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    16267 2023-04-21 05:23:46.000000 foliolib-0.3.4a1/foliolib/okapi/kubeClient.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)      542 2022-03-22 15:04:58.000000 foliolib-0.3.4a1/foliolib/okapi/misc.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    38800 2023-04-21 05:23:46.000000 foliolib-0.3.4a1/foliolib/okapi/okapiClient.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    10030 2023-02-02 10:53:21.000000 foliolib-0.3.4a1/foliolib/okapi/okapiModule.py
--rw-r--r--   0 tobi      (1000) tobi      (1000)    17121 2023-04-21 05:23:46.000000 foliolib-0.3.4a1/foliolib/okapi/okapiModuleKubernetes.py
-drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-07 09:06:55.397771 foliolib-0.3.4a1/foliolib.egg-info/
--rw-r--r--   0 tobi      (1000) tobi      (1000)     2459 2023-05-07 09:06:55.000000 foliolib-0.3.4a1/foliolib.egg-info/PKG-INFO
--rw-r--r--   0 tobi      (1000) tobi      (1000)     3502 2023-05-07 09:06:55.000000 foliolib-0.3.4a1/foliolib.egg-info/SOURCES.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)        1 2023-05-07 09:06:55.000000 foliolib-0.3.4a1/foliolib.egg-info/dependency_links.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)       88 2023-05-07 09:06:55.000000 foliolib-0.3.4a1/foliolib.egg-info/entry_points.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)      130 2023-05-07 09:06:55.000000 foliolib-0.3.4a1/foliolib.egg-info/requires.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)      126 2023-05-07 09:06:55.000000 foliolib-0.3.4a1/foliolib.egg-info/top_level.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)      305 2023-02-21 08:41:56.000000 foliolib-0.3.4a1/requirements.txt
--rw-r--r--   0 tobi      (1000) tobi      (1000)     1225 2023-05-07 09:06:55.405771 foliolib-0.3.4a1/setup.cfg
--rw-r--r--   0 tobi      (1000) tobi      (1000)      117 2022-10-11 12:39:31.000000 foliolib-0.3.4a1/setup.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-20 15:30:27.142341 foliolib-0.3.5a1/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    35146 2020-10-11 07:41:52.000000 foliolib-0.3.5a1/COPYING
+-rw-r--r--   0 tobi      (1000) tobi      (1000)       43 2020-11-07 12:13:21.000000 foliolib-0.3.5a1/MANIFEST.in
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2459 2023-05-20 15:30:27.142341 foliolib-0.3.5a1/PKG-INFO
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1719 2023-02-21 11:23:02.000000 foliolib-0.3.5a1/README.rst
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-20 15:30:27.134341 foliolib-0.3.5a1/foliolib/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1031 2023-03-24 13:25:47.000000 foliolib-0.3.5a1/foliolib/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      396 2023-05-20 15:30:26.000000 foliolib-0.3.5a1/foliolib/__version__.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-20 15:30:27.134341 foliolib-0.3.5a1/foliolib/apiBuilder/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      351 2022-10-11 12:37:16.000000 foliolib-0.3.5a1/foliolib/apiBuilder/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1288 2022-03-13 04:11:25.000000 foliolib-0.3.5a1/foliolib/apiBuilder/build_api.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1586 2022-05-04 20:18:39.000000 foliolib-0.3.5a1/foliolib/apiBuilder/cli.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-20 15:30:27.134341 foliolib-0.3.5a1/foliolib/cli/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3821 2023-04-21 06:17:59.000000 foliolib-0.3.5a1/foliolib/cli/__init__.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-20 15:30:27.134341 foliolib-0.3.5a1/foliolib/cli/folio/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1461 2022-05-09 17:53:56.000000 foliolib-0.3.5a1/foliolib/cli/folio/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      229 2022-04-05 13:20:51.000000 foliolib-0.3.5a1/foliolib/cli/folio/inventory.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      634 2022-02-21 04:57:32.000000 foliolib-0.3.5a1/foliolib/cli/main.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      374 2022-02-21 04:57:41.000000 foliolib-0.3.5a1/foliolib/cli/main_err.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      895 2022-02-21 04:57:36.000000 foliolib-0.3.5a1/foliolib/cli/main_noauth.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4591 2023-04-15 04:58:38.000000 foliolib-0.3.5a1/foliolib/cli/module.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3495 2023-04-01 07:43:09.000000 foliolib-0.3.5a1/foliolib/cli/okapi.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      446 2022-02-21 04:57:17.000000 foliolib-0.3.5a1/foliolib/cli/orderedGroup.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3680 2023-02-15 15:06:27.000000 foliolib-0.3.5a1/foliolib/cli/platform.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2759 2023-04-21 05:25:46.000000 foliolib-0.3.5a1/foliolib/cli/server.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    12868 2022-10-06 05:29:03.000000 foliolib-0.3.5a1/foliolib/cli/tenant.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    12406 2023-05-20 05:12:45.000000 foliolib-0.3.5a1/foliolib/config.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      801 2022-05-09 17:52:49.000000 foliolib-0.3.5a1/foliolib/exceptions.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-20 15:30:27.134341 foliolib-0.3.5a1/foliolib/folio/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1870 2022-10-06 05:35:01.000000 foliolib-0.3.5a1/foliolib/folio/__init__.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-20 15:30:27.142341 foliolib-0.3.5a1/foliolib/folio/api/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)        0 2021-11-15 08:23:39.000000 foliolib-0.3.5a1/foliolib/folio/api/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     9675 2023-05-20 04:20:08.000000 foliolib-0.3.5a1/foliolib/folio/api/audit.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2643 2023-05-20 04:20:08.000000 foliolib-0.3.5a1/foliolib/folio/api/authtoken.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     6783 2023-05-20 04:20:08.000000 foliolib-0.3.5a1/foliolib/folio/api/bulkOperations.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8152 2023-05-20 04:20:08.000000 foliolib-0.3.5a1/foliolib/folio/api/calendar.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    40174 2023-05-20 04:20:08.000000 foliolib-0.3.5a1/foliolib/folio/api/circulation.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    73691 2023-05-20 04:20:08.000000 foliolib-0.3.5a1/foliolib/folio/api/circulationStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     6506 2023-05-20 04:20:08.000000 foliolib-0.3.5a1/foliolib/folio/api/configuration.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    10526 2023-05-20 04:20:08.000000 foliolib-0.3.5a1/foliolib/folio/api/consortia.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4913 2023-05-20 04:20:08.000000 foliolib-0.3.5a1/foliolib/folio/api/copycat.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    54009 2023-05-20 04:20:08.000000 foliolib-0.3.5a1/foliolib/folio/api/courses.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    19883 2023-05-20 04:20:09.000000 foliolib-0.3.5a1/foliolib/folio/api/dataExport.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     6349 2023-05-20 04:20:09.000000 foliolib-0.3.5a1/foliolib/folio/api/dataExportSpring.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    10066 2023-05-20 04:20:09.000000 foliolib-0.3.5a1/foliolib/folio/api/dataExportWorker.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    13485 2023-05-20 04:20:09.000000 foliolib-0.3.5a1/foliolib/folio/api/dataImport.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    37645 2023-05-20 04:20:09.000000 foliolib-0.3.5a1/foliolib/folio/api/dataImportConverterStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    41060 2023-05-20 04:20:09.000000 foliolib-0.3.5a1/foliolib/folio/api/diConverterStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2213 2023-05-20 04:20:09.000000 foliolib-0.3.5a1/foliolib/folio/api/ebsconet.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     7884 2023-05-20 04:20:09.000000 foliolib-0.3.5a1/foliolib/folio/api/email.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4984 2023-05-20 04:20:09.000000 foliolib-0.3.5a1/foliolib/folio/api/entitiesLinks.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    25152 2023-05-20 04:20:09.000000 foliolib-0.3.5a1/foliolib/folio/api/ermUsage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4482 2023-05-20 04:20:09.000000 foliolib-0.3.5a1/foliolib/folio/api/ermUsageHarvester.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8498 2023-05-20 04:20:09.000000 foliolib-0.3.5a1/foliolib/folio/api/eusageReports.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4273 2023-05-20 04:20:09.000000 foliolib-0.3.5a1/foliolib/folio/api/eventConfig.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    80620 2023-05-20 04:20:09.000000 foliolib-0.3.5a1/foliolib/folio/api/feesfines.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    76479 2023-05-20 04:20:10.000000 foliolib-0.3.5a1/foliolib/folio/api/finance.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    79172 2023-05-20 04:20:10.000000 foliolib-0.3.5a1/foliolib/folio/api/financeStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    51717 2023-05-20 04:20:10.000000 foliolib-0.3.5a1/foliolib/folio/api/fincConfig.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     6999 2023-05-20 04:20:08.000000 foliolib-0.3.5a1/foliolib/folio/api/folioCustomFields.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1342 2023-05-20 04:20:08.000000 foliolib-0.3.5a1/foliolib/folio/api/folioSpringBase.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1787 2023-05-20 04:20:08.000000 foliolib-0.3.5a1/foliolib/folio/api/folioVertxLib.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8283 2023-05-20 04:20:10.000000 foliolib-0.3.5a1/foliolib/folio/api/gobi.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     7801 2023-05-20 04:20:10.000000 foliolib-0.3.5a1/foliolib/folio/api/idmConnect.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    74110 2023-05-20 04:20:28.000000 foliolib-0.3.5a1/foliolib/folio/api/innReach.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    22929 2023-05-20 04:20:28.000000 foliolib-0.3.5a1/foliolib/folio/api/inventory.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)   220610 2023-05-20 04:20:29.000000 foliolib-0.3.5a1/foliolib/folio/api/inventoryStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     6001 2023-05-20 04:20:29.000000 foliolib-0.3.5a1/foliolib/folio/api/inventoryUpdate.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    45051 2023-05-20 04:20:29.000000 foliolib-0.3.5a1/foliolib/folio/api/invoice.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    47143 2023-05-20 04:20:29.000000 foliolib-0.3.5a1/foliolib/folio/api/invoiceStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    54294 2023-05-20 04:20:29.000000 foliolib-0.3.5a1/foliolib/folio/api/kbEbscoJava.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3051 2023-05-20 04:20:29.000000 foliolib-0.3.5a1/foliolib/folio/api/ldp.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1332 2023-05-20 04:20:29.000000 foliolib-0.3.5a1/foliolib/folio/api/licenses.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8538 2023-05-20 04:20:29.000000 foliolib-0.3.5a1/foliolib/folio/api/login.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4260 2023-05-20 04:20:29.000000 foliolib-0.3.5a1/foliolib/folio/api/loginSaml.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    17932 2023-05-20 04:20:29.000000 foliolib-0.3.5a1/foliolib/folio/api/marccat.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    20533 2023-05-20 04:20:30.000000 foliolib-0.3.5a1/foliolib/folio/api/metaStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8754 2023-05-20 04:20:30.000000 foliolib-0.3.5a1/foliolib/folio/api/notes.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8870 2023-05-20 04:20:30.000000 foliolib-0.3.5a1/foliolib/folio/api/notify.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    12105 2023-05-20 04:20:30.000000 foliolib-0.3.5a1/foliolib/folio/api/oaiPmh.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    63105 2023-05-20 04:20:30.000000 foliolib-0.3.5a1/foliolib/folio/api/orders.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    78262 2023-05-20 04:20:30.000000 foliolib-0.3.5a1/foliolib/folio/api/ordersStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4978 2023-05-20 04:20:30.000000 foliolib-0.3.5a1/foliolib/folio/api/organizations.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    45825 2023-05-20 04:20:30.000000 foliolib-0.3.5a1/foliolib/folio/api/organizationsStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3632 2023-05-20 04:20:30.000000 foliolib-0.3.5a1/foliolib/folio/api/passwordValidator.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     5893 2023-05-20 04:20:30.000000 foliolib-0.3.5a1/foliolib/folio/api/patron.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    15601 2023-05-20 04:20:30.000000 foliolib-0.3.5a1/foliolib/folio/api/patronBlocks.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    14392 2023-05-20 04:20:30.000000 foliolib-0.3.5a1/foliolib/folio/api/permissions.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     9093 2023-05-20 04:20:30.000000 foliolib-0.3.5a1/foliolib/folio/api/pubsub.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4214 2023-05-20 04:20:30.000000 foliolib-0.3.5a1/foliolib/folio/api/quickMarc.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    17165 2023-05-20 04:20:31.000000 foliolib-0.3.5a1/foliolib/folio/api/remoteStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    21731 2023-05-20 04:20:31.000000 foliolib-0.3.5a1/foliolib/folio/api/reservoir.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1928 2023-05-20 04:20:31.000000 foliolib-0.3.5a1/foliolib/folio/api/rtac.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    17672 2023-05-20 04:20:31.000000 foliolib-0.3.5a1/foliolib/folio/api/search.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      732 2023-05-20 04:20:31.000000 foliolib-0.3.5a1/foliolib/folio/api/sender.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     5419 2023-05-20 04:20:31.000000 foliolib-0.3.5a1/foliolib/folio/api/settings.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    11215 2023-05-20 04:20:31.000000 foliolib-0.3.5a1/foliolib/folio/api/sharedIndex.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    23625 2023-05-20 04:20:31.000000 foliolib-0.3.5a1/foliolib/folio/api/sourceRecordManager.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    28052 2023-05-20 04:20:31.000000 foliolib-0.3.5a1/foliolib/folio/api/sourceRecordStorage.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3187 2023-05-20 04:20:31.000000 foliolib-0.3.5a1/foliolib/folio/api/tags.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     4091 2023-05-20 04:20:31.000000 foliolib-0.3.5a1/foliolib/folio/api/templateEngine.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      870 2023-05-20 04:20:31.000000 foliolib-0.3.5a1/foliolib/folio/api/userImport.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    24002 2023-05-20 04:20:31.000000 foliolib-0.3.5a1/foliolib/folio/api/users.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    11127 2023-05-20 04:20:31.000000 foliolib-0.3.5a1/foliolib/folio/api/usersBl.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     5803 2022-05-31 09:32:11.000000 foliolib-0.3.5a1/foliolib/folio/config.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     8495 2021-02-25 09:49:29.000000 foliolib-0.3.5a1/foliolib/folio/dataImport.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      436 2022-03-17 02:39:17.000000 foliolib-0.3.5a1/foliolib/folio/exceptions.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      945 2022-04-08 08:56:47.000000 foliolib-0.3.5a1/foliolib/folio/inventory.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    24355 2023-05-09 16:17:52.000000 foliolib-0.3.5a1/foliolib/folio/inventoryReferenceData.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     9397 2023-05-20 07:12:08.000000 foliolib-0.3.5a1/foliolib/folio/users.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-20 15:30:27.142341 foliolib-0.3.5a1/foliolib/helper/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1207 2023-04-21 05:23:46.000000 foliolib-0.3.5a1/foliolib/helper/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     9311 2023-04-21 05:23:46.000000 foliolib-0.3.5a1/foliolib/helper/database.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3636 2022-10-11 03:50:00.000000 foliolib-0.3.5a1/foliolib/helper/folio.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3055 2023-02-09 19:10:16.000000 foliolib-0.3.5a1/foliolib/helper/modules.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3935 2023-04-01 06:20:04.000000 foliolib-0.3.5a1/foliolib/helper/okapi.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     5714 2023-02-18 17:54:00.000000 foliolib-0.3.5a1/foliolib/helper/platform.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1517 2022-10-11 03:48:54.000000 foliolib-0.3.5a1/foliolib/helper/tenant.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-20 15:30:27.142341 foliolib-0.3.5a1/foliolib/okapi/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    14520 2022-10-13 08:48:51.000000 foliolib-0.3.5a1/foliolib/okapi/__init__.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2399 2022-07-24 04:45:10.000000 foliolib-0.3.5a1/foliolib/okapi/exceptions.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    16267 2023-04-21 05:23:46.000000 foliolib-0.3.5a1/foliolib/okapi/kubeClient.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      542 2022-03-22 15:04:58.000000 foliolib-0.3.5a1/foliolib/okapi/misc.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    38800 2023-04-21 05:23:46.000000 foliolib-0.3.5a1/foliolib/okapi/okapiClient.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    10030 2023-02-02 10:53:21.000000 foliolib-0.3.5a1/foliolib/okapi/okapiModule.py
+-rw-r--r--   0 tobi      (1000) tobi      (1000)    17121 2023-04-21 05:23:46.000000 foliolib-0.3.5a1/foliolib/okapi/okapiModuleKubernetes.py
+drwxr-xr-x   0 tobi      (1000) tobi      (1000)        0 2023-05-20 15:30:27.134341 foliolib-0.3.5a1/foliolib.egg-info/
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     2459 2023-05-20 15:30:27.000000 foliolib-0.3.5a1/foliolib.egg-info/PKG-INFO
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     3790 2023-05-20 15:30:27.000000 foliolib-0.3.5a1/foliolib.egg-info/SOURCES.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)        1 2023-05-20 15:30:27.000000 foliolib-0.3.5a1/foliolib.egg-info/dependency_links.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)       46 2023-05-20 15:30:27.000000 foliolib-0.3.5a1/foliolib.egg-info/entry_points.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      130 2023-05-20 15:30:27.000000 foliolib-0.3.5a1/foliolib.egg-info/requires.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      126 2023-05-20 15:30:27.000000 foliolib-0.3.5a1/foliolib.egg-info/top_level.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      305 2023-02-21 08:41:56.000000 foliolib-0.3.5a1/requirements.txt
+-rw-r--r--   0 tobi      (1000) tobi      (1000)     1182 2023-05-20 15:30:27.142341 foliolib-0.3.5a1/setup.cfg
+-rw-r--r--   0 tobi      (1000) tobi      (1000)      117 2022-10-11 12:39:31.000000 foliolib-0.3.5a1/setup.py
```

### Comparing `foliolib-0.3.4a1/COPYING` & `foliolib-0.3.5a1/COPYING`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/PKG-INFO` & `foliolib-0.3.5a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foliolib
-Version: 0.3.4a1
+Version: 0.3.5a1
 Summary: Okapi/Folio Manager and Library
 Home-page: https://github.com/tobi-weber/foliolib
 Author: Tobias Weber
 Author-email: tobi-weber@gmx.de
 License: GPL-3.0 License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `foliolib-0.3.4a1/README.rst` & `foliolib-0.3.5a1/README.rst`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib/__init__.py` & `foliolib-0.3.5a1/foliolib/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib/apiBuilder/build_api.py` & `foliolib-0.3.5a1/foliolib/apiBuilder/build_api.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib/apiBuilder/cli.py` & `foliolib-0.3.5a1/foliolib/apiBuilder/cli.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib/cli/__init__.py` & `foliolib-0.3.5a1/foliolib/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib/cli/folio/__init__.py` & `foliolib-0.3.5a1/foliolib/cli/folio/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib/cli/main.py` & `foliolib-0.3.5a1/foliolib/cli/main.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib/cli/main_noauth.py` & `foliolib-0.3.5a1/foliolib/cli/main_noauth.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib/cli/module.py` & `foliolib-0.3.5a1/foliolib/cli/module.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib/cli/okapi.py` & `foliolib-0.3.5a1/foliolib/cli/okapi.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib/cli/platform.py` & `foliolib-0.3.5a1/foliolib/cli/platform.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib/cli/server.py` & `foliolib-0.3.5a1/foliolib/cli/server.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib/cli/tenant.py` & `foliolib-0.3.5a1/foliolib/cli/tenant.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib/config.py` & `foliolib-0.3.5a1/foliolib/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,14 +103,16 @@
             bool: Wether kubernets is enabled.
         """
         return self.__servercfg.get("Kubernetes", "enable", fallback=False)
 
     def get_kube_config(self):
         kube_config = os.path.join(self.get_confdir(),
                                    self.get_server(), "kube_config")
+        kube_config = self.__servercfg.get(
+            "Kubernetes", "kube_config", fallback=kube_config)
         if os.path.exists(kube_config):
             return kube_config
         else:
             raise FileNotFoundError("%s not found" % kube_config)
 
     def get_servers(self):
         """Get all available server configs.
@@ -344,12 +346,18 @@
         # Load server.conf
         sdir = os.path.join(self.get_confdir(), self.get_server())
         fpath = os.path.join(sdir, "server.conf")
         log.debug("Load config from %s", fpath)
         self.__servercfg.read(fpath)
 
 
-def server(name, logging_level="INFO"):
+def server(name: str, logging_level: str = "INFO"):
+    """ Load server sonfig for given name.
+
+    Args:
+        name (str): Name of the server config.
+        logging_level (str, optional): INFO, WARNING, ERROR or DEBUG. Defaults to "INFO".
+    """
     from foliolib import set_logging
     set_logging(level=logging_level)
     Config().set_server(name)
     print("Server is %s" % name)
```

### Comparing `foliolib-0.3.4a1/foliolib/exceptions.py` & `foliolib-0.3.5a1/foliolib/exceptions.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib/folio/__init__.py` & `foliolib-0.3.5a1/foliolib/folio/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/audit.py` & `foliolib-0.3.5a1/foliolib/folio/api/audit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.audit")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/bulkOperations.py` & `foliolib-0.3.5a1/foliolib/folio/api/bulkOperations.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.bulkOperations")
 
 
 
-class BulkoperationsAdmin(FolioAdminApi):
+class Bulkoperations(FolioApi):
     """Bulk operations API
-    Administration
 
     Bulk operations API
     """
 
-    def uploadCsvFile(self, filePath, **kwargs):
+    def uploadcsvfile(self, filePath, **kwargs):
         """Upload csv file with identifiers list (barcodes, UUIDs, HRIDs, etc.) or csv-file with already updated entities
 
         ``POST /bulk-operations/upload``
 
         Args:
             filePath (str): Path of file to upload.
 
@@ -35,28 +34,28 @@
 
         Raises:
             OkapiRequestError: Bad Request
             OkapiFatalError: Internal server errors, e.g. due to misconfiguration
 
         Schema:
 
-            .. literalinclude:: ../files/Bulkoperations_uploadCsvFile_response.schema
+            .. literalinclude:: ../files/Bulkoperations_uploadcsvfile_response.schema
         """
         import os
         headers = {}
         headers["Content-Type"] = "application/octet-stream"
         headers["Content-length"] = str(os.path.getsize(filePath))
         headers["Content-Disposition"] = "attachment; filename=%s" % os.path.basename(
             filePath)
         with open(filePath, 'rb') as f:
             data = f.read()
         
-        return self.call("POST", "/bulk-operations/upload", data=data, query=kwargs)
+        return self.call("POST", f"/bulk-operations/upload", data=data, query=kwargs)
 
-    def postContentUpdates(self, operationId, bulkOperationRuleCollection):
+    def postcontentupdates(self, operationId, bulkOperationRuleCollection):
         """Upload content updates
 
         ``POST /bulk-operations/{operationId}/content-update``
 
         Args:
             operationId (str): UUID of the Bulk Operation (format: uuid)
             bulkOperationRuleCollection (dict): See Schema below.
@@ -67,19 +66,19 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not found
             OkapiFatalError: Internal server errors, e.g. due to misconfiguration
 
         Schema:
 
-            .. literalinclude:: ../files/Bulkoperations_postContentUpdates_request.schema
+            .. literalinclude:: ../files/Bulkoperations_postcontentupdates_request.schema
         """
-        return self.call("POST", "/bulk-operations/{operationId}/content-update", operationId, bulkOperationRuleCollection)
+        return self.call("POST", f"/bulk-operations/{operationId}/content-update", bulkOperationRuleCollection)
 
-    def getPreviewByOperationId(self, operationId, **kwargs):
+    def getpreviewbyoperationid(self, operationId, **kwargs):
         """Get preview
 
         ``GET /bulk-operations/{operationId}/preview``
 
         Args:
             operationId (str): UUID of the Bulk Operation (format: uuid)
 
@@ -94,19 +93,19 @@
         Raises:
             OkapiRequestError: Bad Request
             OkapiRequestNotFound: Not found
             OkapiFatalError: Internal server errors, e.g. due to misconfiguration
 
         Schema:
 
-            .. literalinclude:: ../files/Bulkoperations_getPreviewByOperationId_response.schema
+            .. literalinclude:: ../files/Bulkoperations_getpreviewbyoperationid_response.schema
         """
-        return self.call("GET", "/bulk-operations/{operationId}/preview", operationId, query=kwargs)
+        return self.call("GET", f"/bulk-operations/{operationId}/preview", query=kwargs)
 
-    def startBulkOperation(self, operationId, bulkOperationStart):
+    def startbulkoperation(self, operationId, bulkOperationStart):
         """Start Bulk Operation
 
         ``POST /bulk-operations/{operationId}/start``
 
         Args:
             operationId (str): UUID of the Bulk Operation (format: uuid)
             bulkOperationStart (dict): See Schema below.
@@ -117,20 +116,20 @@
         Raises:
             OkapiRequestError: Bad Request
             OkapiRequestNotFound: Bad Request
             OkapiFatalError: Internal server errors, e.g. due to misconfiguration
 
         Schema:
 
-            .. literalinclude:: ../files/Bulkoperations_startBulkOperation_request.schema
-            .. literalinclude:: ../files/Bulkoperations_startBulkOperation_request.schema_response.schema
+            .. literalinclude:: ../files/Bulkoperations_startbulkoperation_request.schema
+            .. literalinclude:: ../files/Bulkoperations_startbulkoperation_request.schema_response.schema
         """
-        return self.call("POST", "/bulk-operations/{operationId}/start", operationId, bulkOperationStart)
+        return self.call("POST", f"/bulk-operations/{operationId}/start", bulkOperationStart)
 
-    def getErrorsPreviewByOperationId(self, operationId, **kwargs):
+    def geterrorspreviewbyoperationid(self, operationId, **kwargs):
         """Get a list of errors for preview
 
         ``GET /bulk-operations/{operationId}/errors``
 
         Args:
             operationId (str): UUID of the Bulk Operation (format: uuid)
 
@@ -142,19 +141,19 @@
 
         Raises:
             OkapiRequestNotFound: No found
             OkapiFatalError: Internal server errors, e.g. due to misconfiguration
 
         Schema:
 
-            .. literalinclude:: ../files/Bulkoperations_getErrorsPreviewByOperationId_response.schema
+            .. literalinclude:: ../files/Bulkoperations_geterrorspreviewbyoperationid_response.schema
         """
-        return self.call("GET", "/bulk-operations/{operationId}/errors", operationId, query=kwargs)
+        return self.call("GET", f"/bulk-operations/{operationId}/errors", query=kwargs)
 
-    def getBulkOperationCollection(self, **kwargs):
+    def getbulkoperationcollection(self, **kwargs):
         """Get a list of operations
 
         ``GET /bulk-operations``
 
         Keyword Args:
             query (str): Request query
             offset (int): Query offset
@@ -164,19 +163,19 @@
             dict: See Schema below.
 
         Raises:
             OkapiFatalError: Internal server errors, e.g. due to misconfiguration
 
         Schema:
 
-            .. literalinclude:: ../files/Bulkoperations_getBulkOperationCollection_response.schema
+            .. literalinclude:: ../files/Bulkoperations_getbulkoperationcollection_response.schema
         """
         return self.call("GET", "/bulk-operations", query=kwargs)
 
-    def downloadFileByOperationId(self, operationId, **kwargs):
+    def downloadfilebyoperationid(self, operationId, **kwargs):
         """Download file by operation id
 
         ``GET /bulk-operations/{operationId}/download``
 
         Args:
             operationId (str): UUID of the Bulk Operation (format: uuid)
 
@@ -184,17 +183,17 @@
             fileContentType (str): The file content type
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not found
             OkapiFatalError: Internal server errors, e.g. due to misconfiguration
         """
-        return self.call("GET", "/bulk-operations/{operationId}/download", operationId, query=kwargs)
+        return self.call("GET", f"/bulk-operations/{operationId}/download", query=kwargs)
 
-    def getBulkOperationById(self, operationId):
+    def getbulkoperationbyid(self, operationId):
         """Get bulk operation by id
 
         ``GET /bulk-operations/{operationId}``
 
         Args:
             operationId (str): UUID of the Bulk Operation (format: uuid)
 
@@ -203,10 +202,10 @@
 
         Raises:
             OkapiRequestNotFound: Not found
             OkapiFatalError: Internal server errors, e.g. due to misconfiguration
 
         Schema:
 
-            .. literalinclude:: ../files/Bulkoperations_getBulkOperationById_response.schema
+            .. literalinclude:: ../files/Bulkoperations_getbulkoperationbyid_response.schema
         """
-        return self.call("GET", "/bulk-operations/{operationId}", operationId)
+        return self.call("GET", f"/bulk-operations/{operationId}")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/circulation.py` & `foliolib-0.3.5a1/foliolib/folio/api/circulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.circulation")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/circulationStorage.py` & `foliolib-0.3.5a1/foliolib/folio/api/circulationStorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.circulationStorage")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/configuration.py` & `foliolib-0.3.5a1/foliolib/folio/api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.configuration")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/copycat.py` & `foliolib-0.3.5a1/foliolib/folio/api/copycat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.copycat")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/courses.py` & `foliolib-0.3.5a1/foliolib/folio/api/courses.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.courses")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/dataExport.py` & `foliolib-0.3.5a1/foliolib/folio/api/dataExport.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.dataExport")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/dataExportSpring.py` & `foliolib-0.3.5a1/foliolib/folio/api/dataExportSpring.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.dataExportSpring")
 
 
 
-class JobsAdmin(FolioAdminApi):
+class Jobs(FolioApi):
     """Data Export Spring Jobs
-    Administration
 
     
     """
 
-    def getJobs(self, **kwargs):
+    def getjobs(self, **kwargs):
         """Get jobs fy filter
 
         ``GET /data-export-spring/jobs``
 
         Keyword Args:
             offset (int): Skip over a number of elements by specifying an offset value for the query (default: 0, minimum: 0, maximum: 2147483647)
             limit (int): Limit the number of elements returned in the response (default: 10, minimum: 0, maximum: 2147483647)
@@ -31,20 +30,20 @@
 
         Raises:
             OkapiRequestError: Bad request, e.g. malformed request body or query parameter. Details of the errors (e.g. name of the parameter or line/character number with malformed data) provided in the response.
             OkapiFatalError: Internal server errors, e.g. due to misconfiguration
 
         Schema:
 
-            .. literalinclude:: ../files/Jobs_getJobs_response.schema
+            .. literalinclude:: ../files/Jobs_getjobs_response.schema
         """
         return self.call("GET", "/data-export-spring/jobs", query=kwargs)
 
 		
-    def upsertJob(self, job):
+    def upsertjob(self, job):
         """Create or update a job
 
         ``POST /data-export-spring/jobs``
 
         Args:
             job (dict): See Schema below.
 
@@ -53,75 +52,65 @@
 
         Raises:
             OkapiRequestError: Bad Request
             OkapiFatalError: Internal server errors, e.g. due to misconfiguration
 
         Schema:
 
-            .. literalinclude:: ../files/Jobs_upsertJob_request.schema
+            .. literalinclude:: ../files/Jobs_upsertjob_request.schema
         """
-        return self.call("POST", "/data-export-spring/jobs", job)
+        return self.call("POST", f"/data-export-spring/jobs", job)
 
-    def getJobById(self, id_):
+    def getjobbyid(self, id_):
         """Get a job by the job ID
 
         ``GET /data-export-spring/jobs/{id}``
 
-        Args:
-            id_ (str): UUID of the job (format: uuid)
-
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request, e.g. malformed request body or query parameter. Details of the errors (e.g. name of the parameter or line/character number with malformed data) provided in the response.
             OkapiRequestNotFound: Job with a given ID not found
             OkapiFatalError: Internal server errors, e.g. due to misconfiguration
 
         Schema:
 
-            .. literalinclude:: ../files/Jobs_getJobById_response.schema
+            .. literalinclude:: ../files/Jobs_getjobbyid_response.schema
         """
-        return self.call("GET", "/data-export-spring/jobs/{id}", id_)
+        return self.call("GET", f"/data-export-spring/jobs/{id_}")
 
-    def resendExportedFile(self, id_):
+    def resendexportedfile(self, id_):
         """resend exported file by the job ID
 
         ``POST /data-export-spring/jobs/{id}/resend``
 
-        Args:
-            id_ (str): UUID of the job (format: uuid)
-
         Raises:
             OkapiRequestError: Bad Request
             OkapiRequestNotFound: ExportFile with a given Job ID not found
             OkapiFatalError: Internal server errors
         """
-        return self.call("POST", "/data-export-spring/jobs/{id}/resend", id_)
+        return self.call("POST", f"/data-export-spring/jobs/{id_}/resend")
 
-    def downloadExportedFileByJobId(self, id_):
+    def downloadexportedfilebyjobid(self, id_):
         """Download exported file by the job ID
 
         ``GET /data-export-spring/jobs/{id}/download``
-
-        Args:
-            id_ (str): UUID of the job (format: uuid)
         """
-        return self.call("GET", "/data-export-spring/jobs/{id}/download", id_)
+        return self.call("GET", f"/data-export-spring/jobs/{id_}/download")
 
 
 
-class ExportconfigsAdmin(FolioAdminApi):
+class Exportconfigs(FolioApi):
     """Data Export Spring Configurations
-    Administration
 
     
     """
 
-    def getExportConfigs(self, **kwargs):
+    def getexportconfigs(self, **kwargs):
         """Get a list of data export configurations
 
         ``GET /data-export-spring/configs``
 
         Keyword Args:
             query (str): A query string to filter rules based on matching criteria in fields.
             limit (int): Limit the number of elements returned in the response (default: 10)
@@ -130,88 +119,81 @@
             dict: See Schema below.
 
         Raises:
             OkapiFatalError: Internal server errors, e.g. due to misconfiguration
 
         Schema:
 
-            .. literalinclude:: ../files/Exportconfigs_getExportConfigs_response.schema
+            .. literalinclude:: ../files/Exportconfigs_getexportconfigs_response.schema
         """
         return self.call("GET", "/data-export-spring/configs", query=kwargs)
 
 		
-    def postExportConfig(self, exportConfig):
+    def postexportconfig(self, exportConfig):
         """Add an export configuration
 
         ``POST /data-export-spring/configs``
 
         Args:
             exportConfig (dict): See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal server errors, e.g. due to misconfiguration
 
         Schema:
 
-            .. literalinclude:: ../files/Exportconfigs_postExportConfig_request.schema
+            .. literalinclude:: ../files/Exportconfigs_postexportconfig_request.schema
         """
-        return self.call("POST", "/data-export-spring/configs", exportConfig)
+        return self.call("POST", f"/data-export-spring/configs", exportConfig)
 
-    def getConfigById(self, id_):
+    def getconfigbyid(self, id_):
         """Get a export configuration by the export configuration ID
 
         ``GET /data-export-spring/configs/{id}``
 
-        Args:
-            id_ (str): UUID of the export configuration
-
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request, e.g. malformed request body or query parameter. Details of the errors (e.g. name of the parameter or line/character number with malformed data) provided in the response.
             OkapiRequestNotFound: Export configuration with a given ID not found
             OkapiFatalError: Internal server errors, e.g. due to misconfiguration
 
         Schema:
 
-            .. literalinclude:: ../files/Exportconfigs_getConfigById_response.schema
+            .. literalinclude:: ../files/Exportconfigs_getconfigbyid_response.schema
         """
-        return self.call("GET", "/data-export-spring/configs/{id}", id_)
+        return self.call("GET", f"/data-export-spring/configs/{id_}")
 
 		
-    def putExportConfig(self, id_, exportConfig):
+    def putexportconfig(self, exportConfig, id_):
         """Change an export configuration
 
         ``PUT /data-export-spring/configs/{id}``
 
         Args:
-            id_ (str): 
             exportConfig (dict): See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Export config not found
             OkapiFatalError: Internal server errors, e.g. due to misconfiguration
 
         Schema:
 
-            .. literalinclude:: ../files/Exportconfigs_putExportConfig_request.schema
+            .. literalinclude:: ../files/Exportconfigs_putexportconfig_request.schema
         """
-        return self.call("PUT", "/data-export-spring/configs/{id}", id_, exportConfig)
+        return self.call("PUT", f"/data-export-spring/configs/{id_}", exportConfig)
 
 		
-    def deleteExportConfigById(self, id_):
+    def deleteexportconfigbyid(self, id_):
         """Delete export configuration by UUID
 
         ``DELETE /data-export-spring/configs/{id}``
 
-        Args:
-            id_ (str): 
-
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Export config not found
             OkapiFatalError: Internal server errors, e.g. due to misconfiguration
         """
-        return self.call("DELETE", "/data-export-spring/configs/{id}", id_)
+        return self.call("DELETE", f"/data-export-spring/configs/{id_}")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/dataImport.py` & `foliolib-0.3.5a1/foliolib/folio/api/dataImport.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.dataImport")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/dataImportConverterStorage.py` & `foliolib-0.3.5a1/foliolib/folio/api/dataImportConverterStorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.dataImportConverterStorage")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/ebsconet.py` & `foliolib-0.3.5a1/foliolib/folio/api/ebsconet.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.ebsconet")
 
 
 
-class EbsconetAdmin(FolioAdminApi):
+class Ebsconet(FolioApi):
     """Ebsconet integration API
-    Administration
 
     Ebsconet integration API
     """
 
-    def getValidation(self):
+    def getvalidation(self):
         """
 
         ``GET /ebsconet/validate``
 
         Returns:
             dict: See Schema below.
 
         Schema:
 
-            .. literalinclude:: ../files/Ebsconet_getValidation_response.schema
+            .. literalinclude:: ../files/Ebsconet_getvalidation_response.schema
         """
         return self.call("GET", "/ebsconet/validate")
 
-    def getEbsconetOrderLine(self, poLineNumber):
+    def getebsconetorderline(self, poLineNumber):
         """
 
         ``GET /ebsconet/orders/order-lines/{poLineNumber}``
 
         Args:
             poLineNumber (str): product order line number
 
@@ -44,30 +43,30 @@
         Raises:
             OkapiRequestError: Bad request, e.g. malformed request body or query parameter. Details of the error (e.g. name of the parameter or line/character number with malformed data) provided in the response.
             OkapiRequestNotFound: Purchase order line with a given number not found
             OkapiFatalError: Internal server error, e.g. due to misconfiguration
 
         Schema:
 
-            .. literalinclude:: ../files/Ebsconet_getEbsconetOrderLine_response.schema
+            .. literalinclude:: ../files/Ebsconet_getebsconetorderline_response.schema
         """
-        return self.call("GET", "/ebsconet/orders/order-lines/{poLineNumber}", poLineNumber)
+        return self.call("GET", f"/ebsconet/orders/order-lines/{poLineNumber}")
 
 		
-    def putEbsconetOrderLine(self, poLineNumber, ebsconetOrderLine):
+    def putebsconetorderline(self, poLineNumber, ebsconetOrderLine):
         """
 
         ``PUT /ebsconet/orders/order-lines/{poLineNumber}``
 
         Args:
             poLineNumber (str): product order line number
             ebsconetOrderLine (dict): See Schema below.
 
         Raises:
             OkapiRequestError: Bad request, e.g. malformed request body or query parameter. Details of the error (e.g. name of the parameter or line/character number with malformed data) provided in the response.
             OkapiFatalError: Internal server error, e.g. due to misconfiguration
 
         Schema:
 
-            .. literalinclude:: ../files/Ebsconet_putEbsconetOrderLine_request.schema
+            .. literalinclude:: ../files/Ebsconet_putebsconetorderline_request.schema
         """
-        return self.call("PUT", "/ebsconet/orders/order-lines/{poLineNumber}", poLineNumber, ebsconetOrderLine)
+        return self.call("PUT", f"/ebsconet/orders/order-lines/{poLineNumber}", ebsconetOrderLine)
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/email.py` & `foliolib-0.3.5a1/foliolib/folio/api/email.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.email")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/entitiesLinks.py` & `foliolib-0.3.5a1/foliolib/folio/api/entitiesLinks.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.entitiesLinks")
 
 
 
-class EntitieslinksAdmin(FolioAdminApi):
+class Entitieslinks(FolioApi):
     """Entities Links API
-    Administration
 
     Entity Links API
     """
 
-    def updateInstanceLinks(self, instanceId, instanceLinkDtoCollection):
+    def updateinstancelinks(self, instanceId, instanceLinkDtoCollection):
         """Update links collection related to Instance
 
         ``PUT /links/instances/{instanceId}``
 
         Args:
             instanceId (str): UUID of the Instance that is related to the MARC record (format: uuid)
             instanceLinkDtoCollection (dict): See Schema below.
@@ -28,20 +27,20 @@
         Raises:
             OkapiRequestError: Validation errors.
             OkapiRequestUnprocessableEntity: Validation error for the request.
             OkapiFatalError: Internal server error.
 
         Schema:
 
-            .. literalinclude:: ../files/Entitieslinks_updateInstanceLinks_request.schema
+            .. literalinclude:: ../files/Entitieslinks_updateinstancelinks_request.schema
         """
-        return self.call("PUT", "/links/instances/{instanceId}", instanceId, instanceLinkDtoCollection)
+        return self.call("PUT", f"/links/instances/{instanceId}", instanceLinkDtoCollection)
 
 		
-    def getInstanceLinks(self, instanceId):
+    def getinstancelinks(self, instanceId):
         """Get links collection related to Instance
 
         ``GET /links/instances/{instanceId}``
 
         Args:
             instanceId (str): UUID of the Instance that is related to the MARC record (format: uuid)
 
@@ -50,19 +49,19 @@
 
         Raises:
             OkapiRequestError: Validation errors.
             OkapiFatalError: Internal server error.
 
         Schema:
 
-            .. literalinclude:: ../files/Entitieslinks_getInstanceLinks_response.schema
+            .. literalinclude:: ../files/Entitieslinks_getinstancelinks_response.schema
         """
-        return self.call("GET", "/links/instances/{instanceId}", instanceId)
+        return self.call("GET", f"/links/instances/{instanceId}")
 
-    def countLinksByAuthorityIds(self, uuidCollection):
+    def countlinksbyauthorityids(self, uuidCollection):
         """Retrieve number of links by authority IDs
 
         ``POST /links/authorities/bulk/count``
 
         Args:
             uuidCollection (dict): See Schema below.
 
@@ -71,31 +70,50 @@
 
         Raises:
             OkapiRequestError: Validation errors.
             OkapiFatalError: Internal server error.
 
         Schema:
 
-            .. literalinclude:: ../files/Entitieslinks_countLinksByAuthorityIds_request.schema
-            .. literalinclude:: ../files/Entitieslinks_countLinksByAuthorityIds_request.schema_response.schema
+            .. literalinclude:: ../files/Entitieslinks_countlinksbyauthorityids_request.schema
+            .. literalinclude:: ../files/Entitieslinks_countlinksbyauthorityids_request.schema_response.schema
         """
-        return self.call("POST", "/links/authorities/bulk/count", uuidCollection)
+        return self.call("POST", f"/links/authorities/bulk/count", uuidCollection)
 
-    def getInstanceAuthorityLinkingRules(self):
+    def getinstanceauthoritylinkingrules(self):
         """Retrieve instance-authority linking rules
 
         ``GET /linking-rules/instance-authority``
 
         Raises:
             OkapiRequestError: Validation errors.
             OkapiFatalError: Internal server error.
         """
         return self.call("GET", "/linking-rules/instance-authority")
 
-    def getAuthorityLinksStats(self, **kwargs):
+    def getinstanceauthoritylinkingrulebyid(self, ruleId):
+        """Retrieve instance-authority linking rule by ID
+
+        ``GET /linking-rules/instance-authority/{ruleId}``
+
+        Returns:
+            dict: See Schema below.
+
+        Raises:
+            OkapiRequestError: Validation errors.
+            OkapiRequestNotFound: Validation error for the request.
+            OkapiFatalError: Internal server error.
+
+        Schema:
+
+            .. literalinclude:: ../files/Entitieslinks_getinstanceauthoritylinkingrulebyid_response.schema
+        """
+        return self.call("GET", f"/linking-rules/instance-authority/{ruleId}")
+
+    def getauthoritylinksstats(self, **kwargs):
         """Retrieve authority updates (related to links) statistics
 
         ``GET /links/stats/authority``
 
         Keyword Args:
             fromDate (str): Start date to seek from (format: date-time)
             toDate (str): End date to seek from (format: date-time)
@@ -107,19 +125,19 @@
 
         Raises:
             OkapiRequestError: Validation errors.
             OkapiFatalError: Internal server error.
 
         Schema:
 
-            .. literalinclude:: ../files/Entitieslinks_getAuthorityLinksStats_response.schema
+            .. literalinclude:: ../files/Entitieslinks_getauthoritylinksstats_response.schema
         """
         return self.call("GET", "/links/stats/authority", query=kwargs)
 
-    def getLinkedBibUpdateStats(self, **kwargs):
+    def getlinkedbibupdatestats(self, **kwargs):
         """Retrieve linked bib update statistics
 
         ``GET /links/stats/instance``
 
         Keyword Args:
             fromDate (str): Start date to seek from (format: date-time)
             toDate (str): End date to seek to (format: date-time)
@@ -131,10 +149,10 @@
 
         Raises:
             OkapiRequestError: Validation errors.
             OkapiFatalError: Internal server error.
 
         Schema:
 
-            .. literalinclude:: ../files/Entitieslinks_getLinkedBibUpdateStats_response.schema
+            .. literalinclude:: ../files/Entitieslinks_getlinkedbibupdatestats_response.schema
         """
         return self.call("GET", "/links/stats/instance", query=kwargs)
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/ermUsage.py` & `foliolib-0.3.5a1/foliolib/folio/api/ermUsage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.ermUsage")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/ermUsageHarvester.py` & `foliolib-0.3.5a1/foliolib/folio/api/ermUsageHarvester.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.ermUsageHarvester")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/eventConfig.py` & `foliolib-0.3.5a1/foliolib/folio/api/eventConfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.eventConfig")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/feesfines.py` & `foliolib-0.3.5a1/foliolib/folio/api/feesfines.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.feesfines")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/finance.py` & `foliolib-0.3.5a1/foliolib/folio/api/finance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.finance")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/financeStorage.py` & `foliolib-0.3.5a1/foliolib/folio/api/financeStorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.financeStorage")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/fincConfig.py` & `foliolib-0.3.5a1/foliolib/folio/api/fincConfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.fincConfig")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/gobi.py` & `foliolib-0.3.5a1/foliolib/folio/api/gobi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.gobi")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/innReach.py` & `foliolib-0.3.5a1/foliolib/folio/api/innReach.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.innReach")
 
 
 
-class ContributionAdmin(FolioAdminApi):
+class Contribution(FolioApi):
     """INN-Reach Contribution API
-    Administration
 
     
     """
 
-    def getCurrentContributionByServerId(self, centralServerId):
+    def getcurrentcontributionbyserverid(self, centralServerId):
         """Get current INN-Reach contribution for the given central server
 
         ``GET /inn-reach/central-servers/{centralServerId}/contributions/current``
 
         Args:
             centralServerId (str):  (format: uuid)
 
@@ -29,34 +28,34 @@
 
         Raises:
             OkapiRequestError: Bad request, e.g. malformed query parameter.
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Contribution_getCurrentContributionByServerId_response.schema
+            .. literalinclude:: ../files/Contribution_getcurrentcontributionbyserverid_response.schema
         """
-        return self.call("GET", "/inn-reach/central-servers/{centralServerId}/contributions/current", centralServerId)
+        return self.call("GET", f"/inn-reach/central-servers/{centralServerId}/contributions/current")
 
 		
-    def cancelCurrentContributionByServerId(self, centralServerId):
+    def cancelcurrentcontributionbyserverid(self, centralServerId):
         """Cancel current INN-Reach contribution for the given central server
 
         ``DELETE /inn-reach/central-servers/{centralServerId}/contributions/current``
 
         Args:
             centralServerId (str):  (format: uuid)
 
         Raises:
             OkapiRequestError: Bad request, e.g. malformed query parameter.
             OkapiFatalError: Internal server error
         """
-        return self.call("DELETE", "/inn-reach/central-servers/{centralServerId}/contributions/current", centralServerId)
+        return self.call("DELETE", f"/inn-reach/central-servers/{centralServerId}/contributions/current")
 
-    def getContributionHistoryByServerId(self, centralServerId, **kwargs):
+    def getcontributionhistorybyserverid(self, centralServerId, **kwargs):
         """Get a list of Inn-Reach contributions for the given central server
 
         ``GET /inn-reach/central-servers/{centralServerId}/contributions/history``
 
         Args:
             centralServerId (str):  (format: uuid)
 
@@ -69,42 +68,41 @@
 
         Raises:
             OkapiRequestError: Bad request, e.g. malformed query parameter.
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Contribution_getContributionHistoryByServerId_response.schema
+            .. literalinclude:: ../files/Contribution_getcontributionhistorybyserverid_response.schema
         """
-        return self.call("GET", "/inn-reach/central-servers/{centralServerId}/contributions/history", centralServerId, query=kwargs)
+        return self.call("GET", f"/inn-reach/central-servers/{centralServerId}/contributions/history", query=kwargs)
 
-    def startInitialContribution(self, centralServerId):
+    def startinitialcontribution(self, centralServerId):
         """Start initial contribution process
 
         ``POST /inn-reach/central-servers/{centralServerId}/contributions``
 
         Args:
             centralServerId (str):  (format: uuid)
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal server error
         """
-        return self.call("POST", "/inn-reach/central-servers/{centralServerId}/contributions", centralServerId)
+        return self.call("POST", f"/inn-reach/central-servers/{centralServerId}/contributions")
 
 
 
-class SettingsAdmin(FolioAdminApi):
+class Settings(FolioApi):
     """INN-Reach Settings API
-    Administration
 
     
     """
 
-    def postCentralServer(self, centralServerDTO):
+    def postcentralserver(self, centralServerDTO):
         """Add new central server
 
         ``POST /inn-reach/central-servers``
 
         Args:
             centralServerDTO (dict): See Schema below.
 
@@ -114,20 +112,20 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestConflict: Item state conflict
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_postCentralServer_request.schema
+            .. literalinclude:: ../files/Settings_postcentralserver_request.schema
         """
-        return self.call("POST", "/inn-reach/central-servers", centralServerDTO)
+        return self.call("POST", f"/inn-reach/central-servers", centralServerDTO)
 
 		
-    def getCentralServers(self, **kwargs):
+    def getcentralservers(self, **kwargs):
         """Get a list of central servers
 
         ``GET /inn-reach/central-servers``
 
         Keyword Args:
             offset (int): Skip over a number of elements by specifying an offset value for the query (default: 0, minimum: 0, maximum: 2147483647)
             limit (int): Limit the number of elements returned in the response (default: 10, minimum: 0, maximum: 2147483647)
@@ -136,76 +134,69 @@
             dict: See Schema below.
 
         Raises:
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_getCentralServers_response.schema
+            .. literalinclude:: ../files/Settings_getcentralservers_response.schema
         """
         return self.call("GET", "/inn-reach/central-servers", query=kwargs)
 
-    def getCentralServerById(self, id_):
+    def getcentralserverbyid(self, centralServerId):
         """Get central server by id
 
         ``GET /inn-reach/central-servers/{centralServerId}``
 
-        Args:
-            id_ (str):  (format: uuid)
-
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_getCentralServerById_response.schema
+            .. literalinclude:: ../files/Settings_getcentralserverbyid_response.schema
         """
-        return self.call("GET", "/inn-reach/central-servers/{centralServerId}", id_)
+        return self.call("GET", f"/inn-reach/central-servers/{centralServerId}")
 
 		
-    def updateCentralServer(self, id_, centralServerDTO):
+    def updatecentralserver(self, centralServerDTO, centralServerId):
         """Update central server
 
         ``PUT /inn-reach/central-servers/{centralServerId}``
 
         Args:
-            id_ (str):  (format: uuid)
             centralServerDTO (dict): See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_updateCentralServer_request.schema
+            .. literalinclude:: ../files/Settings_updatecentralserver_request.schema
         """
-        return self.call("PUT", "/inn-reach/central-servers/{centralServerId}", id_, centralServerDTO)
+        return self.call("PUT", f"/inn-reach/central-servers/{centralServerId}", centralServerDTO)
 
 		
-    def deleteCentralServer(self, id_):
+    def deletecentralserver(self, centralServerId):
         """Delete central server
 
         ``DELETE /inn-reach/central-servers/{centralServerId}``
 
-        Args:
-            id_ (str):  (format: uuid)
-
         Raises:
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
         """
-        return self.call("DELETE", "/inn-reach/central-servers/{centralServerId}", id_)
+        return self.call("DELETE", f"/inn-reach/central-servers/{centralServerId}")
 
-    def getMaterialTypeMappingsByServerId(self, centralServerId, **kwargs):
+    def getmaterialtypemappingsbyserverid(self, centralServerId, **kwargs):
         """Get a list of material type mappings for the given central server
 
         ``GET /inn-reach/central-servers/{centralServerId}/material-type-mappings``
 
         Args:
             centralServerId (str):  (format: uuid)
 
@@ -218,20 +209,20 @@
 
         Raises:
             OkapiRequestError: Bad request, e.g. malformed query parameter.
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_getMaterialTypeMappingsByServerId_response.schema
+            .. literalinclude:: ../files/Settings_getmaterialtypemappingsbyserverid_response.schema
         """
-        return self.call("GET", "/inn-reach/central-servers/{centralServerId}/material-type-mappings", centralServerId, query=kwargs)
+        return self.call("GET", f"/inn-reach/central-servers/{centralServerId}/material-type-mappings", query=kwargs)
 
 		
-    def postMaterialTypeMapping(self, centralServerId, materialTypeMappingDTO):
+    def postmaterialtypemapping(self, centralServerId, materialTypeMappingDTO):
         """Add new material type mapping associated with the central server
 
         ``POST /inn-reach/central-servers/{centralServerId}/material-type-mappings``
 
         Args:
             centralServerId (str):  (format: uuid)
             materialTypeMappingDTO (dict): See Schema below.
@@ -242,20 +233,20 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestConflict: Item state conflict
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_postMaterialTypeMapping_request.schema
+            .. literalinclude:: ../files/Settings_postmaterialtypemapping_request.schema
         """
-        return self.call("POST", "/inn-reach/central-servers/{centralServerId}/material-type-mappings", centralServerId, materialTypeMappingDTO)
+        return self.call("POST", f"/inn-reach/central-servers/{centralServerId}/material-type-mappings", materialTypeMappingDTO)
 
 		
-    def updateMaterialTypeMappings(self, centralServerId, materialTypeMappingsDTO):
+    def updatematerialtypemappings(self, centralServerId, materialTypeMappingsDTO):
         """Update (replace) the entire collection of material type mappings associated with the central server
 
         ``PUT /inn-reach/central-servers/{centralServerId}/material-type-mappings``
 
         Args:
             centralServerId (str):  (format: uuid)
             materialTypeMappingsDTO (dict): See Schema below.
@@ -263,79 +254,76 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestConflict: Item state conflict
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_updateMaterialTypeMappings_request.schema
+            .. literalinclude:: ../files/Settings_updatematerialtypemappings_request.schema
         """
-        return self.call("PUT", "/inn-reach/central-servers/{centralServerId}/material-type-mappings", centralServerId, materialTypeMappingsDTO)
+        return self.call("PUT", f"/inn-reach/central-servers/{centralServerId}/material-type-mappings", materialTypeMappingsDTO)
 
-    def getMaterialTypeMappingById(self, centralServerId, id_):
+    def getmaterialtypemappingbyid(self, centralServerId, id_):
         """Get material type mapping by id
 
         ``GET /inn-reach/central-servers/{centralServerId}/material-type-mappings/{id}``
 
         Args:
             centralServerId (str):  (format: uuid)
-            id_ (str):  (format: uuid)
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_getMaterialTypeMappingById_response.schema
+            .. literalinclude:: ../files/Settings_getmaterialtypemappingbyid_response.schema
         """
-        return self.call("GET", "/inn-reach/central-servers/{centralServerId}/material-type-mappings/{id}", centralServerId, id_)
+        return self.call("GET", f"/inn-reach/central-servers/{centralServerId}/material-type-mappings/{id_}")
 
 		
-    def updateMaterialTypeMapping(self, centralServerId, id_, materialTypeMappingDTO):
+    def updatematerialtypemapping(self, centralServerId, materialTypeMappingDTO, id_):
         """Update material type mapping
 
         ``PUT /inn-reach/central-servers/{centralServerId}/material-type-mappings/{id}``
 
         Args:
             centralServerId (str):  (format: uuid)
-            id_ (str):  (format: uuid)
             materialTypeMappingDTO (dict): See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_updateMaterialTypeMapping_request.schema
+            .. literalinclude:: ../files/Settings_updatematerialtypemapping_request.schema
         """
-        return self.call("PUT", "/inn-reach/central-servers/{centralServerId}/material-type-mappings/{id}", centralServerId, id_, materialTypeMappingDTO)
+        return self.call("PUT", f"/inn-reach/central-servers/{centralServerId}/material-type-mappings/{id_}", materialTypeMappingDTO)
 
 		
-    def deleteMaterialTypeMapping(self, centralServerId, id_):
+    def deletematerialtypemapping(self, centralServerId, id_):
         """Delete material type mapping
 
         ``DELETE /inn-reach/central-servers/{centralServerId}/material-type-mappings/{id}``
 
         Args:
             centralServerId (str):  (format: uuid)
-            id_ (str):  (format: uuid)
 
         Raises:
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
         """
-        return self.call("DELETE", "/inn-reach/central-servers/{centralServerId}/material-type-mappings/{id}", centralServerId, id_)
+        return self.call("DELETE", f"/inn-reach/central-servers/{centralServerId}/material-type-mappings/{id_}")
 
-    def postInnReachLocation(self, innReachLocationDTO):
+    def postinnreachlocation(self, innReachLocationDTO):
         """Add new InnReach location
 
         ``POST /inn-reach/locations``
 
         Args:
             innReachLocationDTO (dict): See Schema below.
 
@@ -344,20 +332,20 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_postInnReachLocation_request.schema
+            .. literalinclude:: ../files/Settings_postinnreachlocation_request.schema
         """
-        return self.call("POST", "/inn-reach/locations", innReachLocationDTO)
+        return self.call("POST", f"/inn-reach/locations", innReachLocationDTO)
 
 		
-    def getLocations(self, **kwargs):
+    def getlocations(self, **kwargs):
         """Get a list of InnReach locations
 
         ``GET /inn-reach/locations``
 
         Keyword Args:
             offset (int): Skip over a number of elements by specifying an offset value for the query (default: 0, minimum: 0, maximum: 2147483647)
             limit (int): Limit the number of elements returned in the response (default: 10, minimum: 0, maximum: 2147483647)
@@ -366,76 +354,69 @@
             dict: See Schema below.
 
         Raises:
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_getLocations_response.schema
+            .. literalinclude:: ../files/Settings_getlocations_response.schema
         """
         return self.call("GET", "/inn-reach/locations", query=kwargs)
 
-    def getLocationById(self, id_):
+    def getlocationbyid(self, locationId):
         """Get InnReach location by id
 
         ``GET /inn-reach/locations/{locationId}``
 
-        Args:
-            id_ (str):  (format: uuid)
-
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_getLocationById_response.schema
+            .. literalinclude:: ../files/Settings_getlocationbyid_response.schema
         """
-        return self.call("GET", "/inn-reach/locations/{locationId}", id_)
+        return self.call("GET", f"/inn-reach/locations/{locationId}")
 
 		
-    def updateLocation(self, id_, innReachLocationDTO):
+    def updatelocation(self, innReachLocationDTO, locationId):
         """Update InnReach location
 
         ``PUT /inn-reach/locations/{locationId}``
 
         Args:
-            id_ (str):  (format: uuid)
             innReachLocationDTO (dict): See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_updateLocation_request.schema
+            .. literalinclude:: ../files/Settings_updatelocation_request.schema
         """
-        return self.call("PUT", "/inn-reach/locations/{locationId}", id_, innReachLocationDTO)
+        return self.call("PUT", f"/inn-reach/locations/{locationId}", innReachLocationDTO)
 
 		
-    def deleteLocation(self, id_):
+    def deletelocation(self, locationId):
         """Delete InnReach location
 
         ``DELETE /inn-reach/locations/{locationId}``
 
-        Args:
-            id_ (str):  (format: uuid)
-
         Raises:
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
         """
-        return self.call("DELETE", "/inn-reach/locations/{locationId}", id_)
+        return self.call("DELETE", f"/inn-reach/locations/{locationId}")
 
-    def getLibraryMappingsByServerId(self, centralServerId, **kwargs):
+    def getlibrarymappingsbyserverid(self, centralServerId, **kwargs):
         """Get a list of library to Inn-Reach location mappings for the given central server
 
         ``GET /inn-reach/central-servers/{centralServerId}/libraries/location-mappings``
 
         Args:
             centralServerId (str):  (format: uuid)
 
@@ -448,20 +429,20 @@
 
         Raises:
             OkapiRequestError: Bad request, e.g. malformed query parameter.
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_getLibraryMappingsByServerId_response.schema
+            .. literalinclude:: ../files/Settings_getlibrarymappingsbyserverid_response.schema
         """
-        return self.call("GET", "/inn-reach/central-servers/{centralServerId}/libraries/location-mappings", centralServerId, query=kwargs)
+        return self.call("GET", f"/inn-reach/central-servers/{centralServerId}/libraries/location-mappings", query=kwargs)
 
 		
-    def putLibraryMappings(self, centralServerId, libraryMappingsDTO):
+    def putlibrarymappings(self, centralServerId, libraryMappingsDTO):
         """Update (replace) the entire collection of library to Inn-Reach location mappings associated with the central server
 
         ``PUT /inn-reach/central-servers/{centralServerId}/libraries/location-mappings``
 
         Args:
             centralServerId (str):  (format: uuid)
             libraryMappingsDTO (dict): See Schema below.
@@ -469,19 +450,19 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestConflict: Item state conflict
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_putLibraryMappings_request.schema
+            .. literalinclude:: ../files/Settings_putlibrarymappings_request.schema
         """
-        return self.call("PUT", "/inn-reach/central-servers/{centralServerId}/libraries/location-mappings", centralServerId, libraryMappingsDTO)
+        return self.call("PUT", f"/inn-reach/central-servers/{centralServerId}/libraries/location-mappings", libraryMappingsDTO)
 
-    def getLocationMappingsByServerId(self, centralServerId, libraryId, **kwargs):
+    def getlocationmappingsbyserverid(self, centralServerId, libraryId, **kwargs):
         """Get a list of library location to Inn-Reach location mappings for the given central server
 
         ``GET /inn-reach/central-servers/{centralServerId}/libraries/{libraryId}/locations/location-mappings``
 
         Args:
             centralServerId (str):  (format: uuid)
             libraryId (str):  (format: uuid)
@@ -495,20 +476,20 @@
 
         Raises:
             OkapiRequestError: Bad request, e.g. malformed query parameter.
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_getLocationMappingsByServerId_response.schema
+            .. literalinclude:: ../files/Settings_getlocationmappingsbyserverid_response.schema
         """
-        return self.call("GET", "/inn-reach/central-servers/{centralServerId}/libraries/{libraryId}/locations/location-mappings", centralServerId, libraryId, query=kwargs)
+        return self.call("GET", f"/inn-reach/central-servers/{centralServerId}/libraries/{libraryId}/locations/location-mappings", query=kwargs)
 
 		
-    def putLocationMappings(self, centralServerId, libraryId, locationMappingsDTO):
+    def putlocationmappings(self, centralServerId, libraryId, locationMappingsDTO):
         """Update (replace) the entire collection of library location to Inn-Reach location mappings associated with the central server
 
         ``PUT /inn-reach/central-servers/{centralServerId}/libraries/{libraryId}/locations/location-mappings``
 
         Args:
             centralServerId (str):  (format: uuid)
             libraryId (str):  (format: uuid)
@@ -517,33 +498,33 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestConflict: Item state conflict
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_putLocationMappings_request.schema
+            .. literalinclude:: ../files/Settings_putlocationmappings_request.schema
         """
-        return self.call("PUT", "/inn-reach/central-servers/{centralServerId}/libraries/{libraryId}/locations/location-mappings", centralServerId, libraryId, locationMappingsDTO)
+        return self.call("PUT", f"/inn-reach/central-servers/{centralServerId}/libraries/{libraryId}/locations/location-mappings", locationMappingsDTO)
 
-    def getLocationMappingsForAllLibrariesByServerId(self, centralServerId):
+    def getlocationmappingsforalllibrariesbyserverid(self, centralServerId):
         """Get a list of libraries locations to Inn-Reach location mappings for the given central server
 
         ``GET /inn-reach/central-servers/{centralServerId}/libraries/locations/location-mappings``
 
         Args:
             centralServerId (str):  (format: uuid)
 
         Raises:
             OkapiRequestError: Bad request, e.g. malformed query parameter.
             OkapiFatalError: Internal server error
         """
-        return self.call("GET", "/inn-reach/central-servers/{centralServerId}/libraries/locations/location-mappings", centralServerId)
+        return self.call("GET", f"/inn-reach/central-servers/{centralServerId}/libraries/locations/location-mappings")
 
-    def getCriteriaByServerId(self, centralServerId):
+    def getcriteriabyserverid(self, centralServerId):
         """Get Contribution Criteria by Central Server id
 
         ``GET /inn-reach/central-servers/{centralServerId}/contribution-criteria``
 
         Args:
             centralServerId (str):  (format: uuid)
 
@@ -552,20 +533,20 @@
 
         Raises:
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_getCriteriaByServerId_response.schema
+            .. literalinclude:: ../files/Settings_getcriteriabyserverid_response.schema
         """
-        return self.call("GET", "/inn-reach/central-servers/{centralServerId}/contribution-criteria", centralServerId)
+        return self.call("GET", f"/inn-reach/central-servers/{centralServerId}/contribution-criteria")
 
 		
-    def postContributionCriteria(self, centralServerId, contributionCriteriaDTO):
+    def postcontributioncriteria(self, centralServerId, contributionCriteriaDTO):
         """Create new contribution criteria for Central Server
 
         ``POST /inn-reach/central-servers/{centralServerId}/contribution-criteria``
 
         Args:
             centralServerId (str):  (format: uuid)
             contributionCriteriaDTO (dict): See Schema below.
@@ -576,35 +557,35 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestConflict: Item state conflict
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_postContributionCriteria_request.schema
+            .. literalinclude:: ../files/Settings_postcontributioncriteria_request.schema
         """
-        return self.call("POST", "/inn-reach/central-servers/{centralServerId}/contribution-criteria", centralServerId, contributionCriteriaDTO)
+        return self.call("POST", f"/inn-reach/central-servers/{centralServerId}/contribution-criteria", contributionCriteriaDTO)
 
 		
-    def deleteCriteria(self, centralServerId):
+    def deletecriteria(self, centralServerId):
         """Delete Contribution Criteria Configuration
 
         ``DELETE /inn-reach/central-servers/{centralServerId}/contribution-criteria``
 
         Args:
             centralServerId (str):  (format: uuid)
 
         Raises:
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
         """
-        return self.call("DELETE", "/inn-reach/central-servers/{centralServerId}/contribution-criteria", centralServerId)
+        return self.call("DELETE", f"/inn-reach/central-servers/{centralServerId}/contribution-criteria")
 
 		
-    def updateCriteria(self, centralServerId, contributionCriteriaDTO):
+    def updatecriteria(self, centralServerId, contributionCriteriaDTO):
         """Update Contribution Criteria Configuration
 
         ``PUT /inn-reach/central-servers/{centralServerId}/contribution-criteria``
 
         Args:
             centralServerId (str):  (format: uuid)
             contributionCriteriaDTO (dict): See Schema below.
@@ -613,38 +594,38 @@
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Item not found
             OkapiRequestConflict: Item state conflict
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_updateCriteria_request.schema
+            .. literalinclude:: ../files/Settings_updatecriteria_request.schema
         """
-        return self.call("PUT", "/inn-reach/central-servers/{centralServerId}/contribution-criteria", centralServerId, contributionCriteriaDTO)
+        return self.call("PUT", f"/inn-reach/central-servers/{centralServerId}/contribution-criteria", contributionCriteriaDTO)
 
-    def authenticateLocalServerKeySecret(self, authenticationRequest):
+    def authenticatelocalserverkeysecret(self, authenticationRequest):
         """Authenticate InnReach local server key/secret pair
 
         ``POST /inn-reach/authentication``
 
         Args:
             authenticationRequest (dict): See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestUnauthorized: Unauthorized
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_authenticateLocalServerKeySecret_request.schema
+            .. literalinclude:: ../files/Settings_authenticatelocalserverkeysecret_request.schema
         """
-        return self.call("POST", "/inn-reach/authentication", authenticationRequest)
+        return self.call("POST", f"/inn-reach/authentication", authenticationRequest)
 
-    def getItemContributionOptionsConfigurationById(self, centralServerId):
+    def getitemcontributionoptionsconfigurationbyid(self, centralServerId):
         """Get Item Contribution Options Configuration by id
 
         ``GET /inn-reach/central-servers/{centralServerId}/item-contribution-options``
 
         Args:
             centralServerId (str):  (format: uuid)
 
@@ -653,20 +634,20 @@
 
         Raises:
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_getItemContributionOptionsConfigurationById_response.schema
+            .. literalinclude:: ../files/Settings_getitemcontributionoptionsconfigurationbyid_response.schema
         """
-        return self.call("GET", "/inn-reach/central-servers/{centralServerId}/item-contribution-options", centralServerId)
+        return self.call("GET", f"/inn-reach/central-servers/{centralServerId}/item-contribution-options")
 
 		
-    def updateItemContributionOptionsConfiguration(self, centralServerId, itemContributionOptionsConfigurationDTO):
+    def updateitemcontributionoptionsconfiguration(self, centralServerId, itemContributionOptionsConfigurationDTO):
         """Update Item Contribution Options Configuration
 
         ``PUT /inn-reach/central-servers/{centralServerId}/item-contribution-options``
 
         Args:
             centralServerId (str):  (format: uuid)
             itemContributionOptionsConfigurationDTO (dict): See Schema below.
@@ -674,20 +655,20 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_updateItemContributionOptionsConfiguration_request.schema
+            .. literalinclude:: ../files/Settings_updateitemcontributionoptionsconfiguration_request.schema
         """
-        return self.call("PUT", "/inn-reach/central-servers/{centralServerId}/item-contribution-options", centralServerId, itemContributionOptionsConfigurationDTO)
+        return self.call("PUT", f"/inn-reach/central-servers/{centralServerId}/item-contribution-options", itemContributionOptionsConfigurationDTO)
 
 		
-    def createItemContributionOptionsConfiguration(self, centralServerId, itemContributionOptionsConfigurationDTO):
+    def createitemcontributionoptionsconfiguration(self, centralServerId, itemContributionOptionsConfigurationDTO):
         """Add new item contribution options configuration associated with the central server
 
         ``POST /inn-reach/central-servers/{centralServerId}/item-contribution-options``
 
         Args:
             centralServerId (str):  (format: uuid)
             itemContributionOptionsConfigurationDTO (dict): See Schema below.
@@ -697,19 +678,19 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_createItemContributionOptionsConfiguration_request.schema
+            .. literalinclude:: ../files/Settings_createitemcontributionoptionsconfiguration_request.schema
         """
-        return self.call("POST", "/inn-reach/central-servers/{centralServerId}/item-contribution-options", centralServerId, itemContributionOptionsConfigurationDTO)
+        return self.call("POST", f"/inn-reach/central-servers/{centralServerId}/item-contribution-options", itemContributionOptionsConfigurationDTO)
 
-    def getAgencyMappingsByServerId(self, centralServerId):
+    def getagencymappingsbyserverid(self, centralServerId):
         """Get a list of Inn-Reach Agency to FOLIO location mappings for the given central server
 
         ``GET /inn-reach/central-servers/{centralServerId}/agency-mappings``
 
         Args:
             centralServerId (str):  (format: uuid)
 
@@ -718,20 +699,20 @@
 
         Raises:
             OkapiRequestError: Bad request, e.g. malformed query parameter.
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_getAgencyMappingsByServerId_response.schema
+            .. literalinclude:: ../files/Settings_getagencymappingsbyserverid_response.schema
         """
-        return self.call("GET", "/inn-reach/central-servers/{centralServerId}/agency-mappings", centralServerId)
+        return self.call("GET", f"/inn-reach/central-servers/{centralServerId}/agency-mappings")
 
 		
-    def putAgencyMappings(self, centralServerId, agencyLocationMappingDTO):
+    def putagencymappings(self, centralServerId, agencyLocationMappingDTO):
         """Update (add) INN-Reach Agency to FOLIO location mappings associated with the central server
 
         ``PUT /inn-reach/central-servers/{centralServerId}/agency-mappings``
 
         Args:
             centralServerId (str):  (format: uuid)
             agencyLocationMappingDTO (dict): See Schema below.
@@ -739,19 +720,19 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestConflict: Item state conflict
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_putAgencyMappings_request.schema
+            .. literalinclude:: ../files/Settings_putagencymappings_request.schema
         """
-        return self.call("PUT", "/inn-reach/central-servers/{centralServerId}/agency-mappings", centralServerId, agencyLocationMappingDTO)
+        return self.call("PUT", f"/inn-reach/central-servers/{centralServerId}/agency-mappings", agencyLocationMappingDTO)
 
-    def getMARCTransformationOptionsSettingsById(self, centralServerId):
+    def getmarctransformationoptionssettingsbyid(self, centralServerId):
         """Get MARC Transformation Options Settings by id
 
         ``GET /inn-reach/central-servers/{centralServerId}/marc-transformation-options``
 
         Args:
             centralServerId (str):  (format: uuid)
 
@@ -760,78 +741,78 @@
 
         Raises:
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_getMARCTransformationOptionsSettingsById_response.schema
+            .. literalinclude:: ../files/Settings_getmarctransformationoptionssettingsbyid_response.schema
         """
-        return self.call("GET", "/inn-reach/central-servers/{centralServerId}/marc-transformation-options", centralServerId)
+        return self.call("GET", f"/inn-reach/central-servers/{centralServerId}/marc-transformation-options")
 
 		
-    def updateMARCTransformationOptionsSettings(self, centralServerId, MARCTransformationOptionsSettingsDTO):
+    def updatemarctransformationoptionssettings(self, centralServerId, mARCTransformationOptionsSettingsDTO):
         """Update MARC Transformation Options Settings
 
         ``PUT /inn-reach/central-servers/{centralServerId}/marc-transformation-options``
 
         Args:
             centralServerId (str):  (format: uuid)
-            MARCTransformationOptionsSettingsDTO (dict): See Schema below.
+            mARCTransformationOptionsSettingsDTO (dict): See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_updateMARCTransformationOptionsSettings_request.schema
+            .. literalinclude:: ../files/Settings_updatemarctransformationoptionssettings_request.schema
         """
-        return self.call("PUT", "/inn-reach/central-servers/{centralServerId}/marc-transformation-options", centralServerId, MARCTransformationOptionsSettingsDTO)
+        return self.call("PUT", f"/inn-reach/central-servers/{centralServerId}/marc-transformation-options", mARCTransformationOptionsSettingsDTO)
 
 		
-    def createMARCTransformationOptionsSettings(self, centralServerId, MARCTransformationOptionsSettingsDTO):
+    def createmarctransformationoptionssettings(self, centralServerId, mARCTransformationOptionsSettingsDTO):
         """Add new MARC Transformation Options Settings associated with the central server
 
         ``POST /inn-reach/central-servers/{centralServerId}/marc-transformation-options``
 
         Args:
             centralServerId (str):  (format: uuid)
-            MARCTransformationOptionsSettingsDTO (dict): See Schema below.
+            mARCTransformationOptionsSettingsDTO (dict): See Schema below.
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_createMARCTransformationOptionsSettings_request.schema
+            .. literalinclude:: ../files/Settings_createmarctransformationoptionssettings_request.schema
         """
-        return self.call("POST", "/inn-reach/central-servers/{centralServerId}/marc-transformation-options", centralServerId, MARCTransformationOptionsSettingsDTO)
+        return self.call("POST", f"/inn-reach/central-servers/{centralServerId}/marc-transformation-options", mARCTransformationOptionsSettingsDTO)
 
 		
-    def deleteMARCTransformationOptionsSettings(self, centralServerId):
+    def deletemarctransformationoptionssettings(self, centralServerId):
         """Delete Marc Transformation Options Settings
 
         ``DELETE /inn-reach/central-servers/{centralServerId}/marc-transformation-options``
 
         Args:
             centralServerId (str):  (format: uuid)
 
         Raises:
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
         """
-        return self.call("DELETE", "/inn-reach/central-servers/{centralServerId}/marc-transformation-options", centralServerId)
+        return self.call("DELETE", f"/inn-reach/central-servers/{centralServerId}/marc-transformation-options")
 
-    def getAllMARCTransformationOptionsSettings(self, **kwargs):
+    def getallmarctransformationoptionssettings(self, **kwargs):
         """Get a list of Marc Transformation Options Settings
 
         ``GET /inn-reach/central-servers/marc-transformation-options``
 
         Keyword Args:
             offset (int): Skip over a number of elements by specifying an offset value for the query (default: 0, minimum: 0, maximum: 2147483647)
             limit (int): Limit the number of elements returned in the response (default: 10, minimum: 0, maximum: 2147483647)
@@ -840,19 +821,19 @@
             dict: See Schema below.
 
         Raises:
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_getAllMARCTransformationOptionsSettings_response.schema
+            .. literalinclude:: ../files/Settings_getallmarctransformationoptionssettings_response.schema
         """
         return self.call("GET", "/inn-reach/central-servers/marc-transformation-options", query=kwargs)
 
-    def getPatronTypeMappingsByServerId(self, centralServerId, **kwargs):
+    def getpatrontypemappingsbyserverid(self, centralServerId, **kwargs):
         """Get a list of Patron Type Mappings
 
         ``GET /inn-reach/central-servers/{centralServerId}/patron-type-mappings``
 
         Args:
             centralServerId (str):  (format: uuid)
 
@@ -864,20 +845,20 @@
             dict: See Schema below.
 
         Raises:
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_getPatronTypeMappingsByServerId_response.schema
+            .. literalinclude:: ../files/Settings_getpatrontypemappingsbyserverid_response.schema
         """
-        return self.call("GET", "/inn-reach/central-servers/{centralServerId}/patron-type-mappings", centralServerId, query=kwargs)
+        return self.call("GET", f"/inn-reach/central-servers/{centralServerId}/patron-type-mappings", query=kwargs)
 
 		
-    def updatePatronTypeMappings(self, centralServerId, patronTypeMappingsDTO):
+    def updatepatrontypemappings(self, centralServerId, patronTypeMappingsDTO):
         """Update Patron Type Mappings
 
         ``PUT /inn-reach/central-servers/{centralServerId}/patron-type-mappings``
 
         Args:
             centralServerId (str):  (format: uuid)
             patronTypeMappingsDTO (dict): See Schema below.
@@ -885,19 +866,19 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_updatePatronTypeMappings_request.schema
+            .. literalinclude:: ../files/Settings_updatepatrontypemappings_request.schema
         """
-        return self.call("PUT", "/inn-reach/central-servers/{centralServerId}/patron-type-mappings", centralServerId, patronTypeMappingsDTO)
+        return self.call("PUT", f"/inn-reach/central-servers/{centralServerId}/patron-type-mappings", patronTypeMappingsDTO)
 
-    def transformMARCRecord(self, centralServerId, inventoryInstanceId):
+    def transformmarcrecord(self, centralServerId, inventoryInstanceId):
         """Transform MARC record by Id according to CentralServer settings
 
         ``GET /inn-reach/central-servers/{centralServerId}/marc-record-transformation/{inventoryInstanceId}``
 
         Args:
             centralServerId (str):  (format: uuid)
             inventoryInstanceId (str):  (format: uuid)
@@ -907,19 +888,19 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_transformMARCRecord_response.schema
+            .. literalinclude:: ../files/Settings_transformmarcrecord_response.schema
         """
-        return self.call("GET", "/inn-reach/central-servers/{centralServerId}/marc-record-transformation/{inventoryInstanceId}", centralServerId, inventoryInstanceId)
+        return self.call("GET", f"/inn-reach/central-servers/{centralServerId}/marc-record-transformation/{inventoryInstanceId}")
 
-    def getItemTypeMappingsByServerId(self, centralServerId, **kwargs):
+    def getitemtypemappingsbyserverid(self, centralServerId, **kwargs):
         """Get a list of Item Type Mappings
 
         ``GET /inn-reach/central-servers/{centralServerId}/item-type-mappings``
 
         Args:
             centralServerId (str):  (format: uuid)
 
@@ -931,20 +912,20 @@
             dict: See Schema below.
 
         Raises:
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_getItemTypeMappingsByServerId_response.schema
+            .. literalinclude:: ../files/Settings_getitemtypemappingsbyserverid_response.schema
         """
-        return self.call("GET", "/inn-reach/central-servers/{centralServerId}/item-type-mappings", centralServerId, query=kwargs)
+        return self.call("GET", f"/inn-reach/central-servers/{centralServerId}/item-type-mappings", query=kwargs)
 
 		
-    def updateItemTypeMappings(self, centralServerId, itemTypeMappingsDTO):
+    def updateitemtypemappings(self, centralServerId, itemTypeMappingsDTO):
         """Update Item Type Mappings
 
         ``PUT /inn-reach/central-servers/{centralServerId}/item-type-mappings``
 
         Args:
             centralServerId (str):  (format: uuid)
             itemTypeMappingsDTO (dict): See Schema below.
@@ -952,19 +933,19 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_updateItemTypeMappings_request.schema
+            .. literalinclude:: ../files/Settings_updateitemtypemappings_request.schema
         """
-        return self.call("PUT", "/inn-reach/central-servers/{centralServerId}/item-type-mappings", centralServerId, itemTypeMappingsDTO)
+        return self.call("PUT", f"/inn-reach/central-servers/{centralServerId}/item-type-mappings", itemTypeMappingsDTO)
 
-    def getUserCustomFieldMapping(self, centralServerId):
+    def getusercustomfieldmapping(self, centralServerId):
         """Get a User Custom Field Mapping
 
         ``GET /inn-reach/central-servers/{centralServerId}/user-custom-field-mappings``
 
         Args:
             centralServerId (str):  (format: uuid)
 
@@ -972,20 +953,20 @@
             dict: See Schema below.
 
         Raises:
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_getUserCustomFieldMapping_response.schema
+            .. literalinclude:: ../files/Settings_getusercustomfieldmapping_response.schema
         """
-        return self.call("GET", "/inn-reach/central-servers/{centralServerId}/user-custom-field-mappings", centralServerId)
+        return self.call("GET", f"/inn-reach/central-servers/{centralServerId}/user-custom-field-mappings")
 
 		
-    def updateUserCustomFieldMapping(self, centralServerId, userCustomFieldMappingDTO):
+    def updateusercustomfieldmapping(self, centralServerId, userCustomFieldMappingDTO):
         """Update User Custom Field Mapping
 
         ``PUT /inn-reach/central-servers/{centralServerId}/user-custom-field-mappings``
 
         Args:
             centralServerId (str):  (format: uuid)
             userCustomFieldMappingDTO (dict): See Schema below.
@@ -993,20 +974,20 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_updateUserCustomFieldMapping_request.schema
+            .. literalinclude:: ../files/Settings_updateusercustomfieldmapping_request.schema
         """
-        return self.call("PUT", "/inn-reach/central-servers/{centralServerId}/user-custom-field-mappings", centralServerId, userCustomFieldMappingDTO)
+        return self.call("PUT", f"/inn-reach/central-servers/{centralServerId}/user-custom-field-mappings", userCustomFieldMappingDTO)
 
 		
-    def createUserCustomFieldMapping(self, centralServerId, userCustomFieldMappingDTO):
+    def createusercustomfieldmapping(self, centralServerId, userCustomFieldMappingDTO):
         """Add new User Custom Field Mapping associated with the central server
 
         ``POST /inn-reach/central-servers/{centralServerId}/user-custom-field-mappings``
 
         Args:
             centralServerId (str):  (format: uuid)
             userCustomFieldMappingDTO (dict): See Schema below.
@@ -1016,19 +997,19 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_createUserCustomFieldMapping_request.schema
+            .. literalinclude:: ../files/Settings_createusercustomfieldmapping_request.schema
         """
-        return self.call("POST", "/inn-reach/central-servers/{centralServerId}/user-custom-field-mappings", centralServerId, userCustomFieldMappingDTO)
+        return self.call("POST", f"/inn-reach/central-servers/{centralServerId}/user-custom-field-mappings", userCustomFieldMappingDTO)
 
-    def getCentralPatronTypeMappings(self, centralServerId, **kwargs):
+    def getcentralpatrontypemappings(self, centralServerId, **kwargs):
         """Get a list of Central Patron Type Mappings
 
         ``GET /inn-reach/central-servers/{centralServerId}/central-patron-type-mappings``
 
         Args:
             centralServerId (str):  (format: uuid)
 
@@ -1040,20 +1021,20 @@
             dict: See Schema below.
 
         Raises:
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_getCentralPatronTypeMappings_response.schema
+            .. literalinclude:: ../files/Settings_getcentralpatrontypemappings_response.schema
         """
-        return self.call("GET", "/inn-reach/central-servers/{centralServerId}/central-patron-type-mappings", centralServerId, query=kwargs)
+        return self.call("GET", f"/inn-reach/central-servers/{centralServerId}/central-patron-type-mappings", query=kwargs)
 
 		
-    def updateCentralPatronTypeMappings(self, centralServerId, centralPatronTypeMappingsDTO):
+    def updatecentralpatrontypemappings(self, centralServerId, centralPatronTypeMappingsDTO):
         """Update Central Patron Type Mappings
 
         ``PUT /inn-reach/central-servers/{centralServerId}/central-patron-type-mappings``
 
         Args:
             centralServerId (str):  (format: uuid)
             centralPatronTypeMappingsDTO (dict): See Schema below.
@@ -1061,19 +1042,19 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_updateCentralPatronTypeMappings_request.schema
+            .. literalinclude:: ../files/Settings_updatecentralpatrontypemappings_request.schema
         """
-        return self.call("PUT", "/inn-reach/central-servers/{centralServerId}/central-patron-type-mappings", centralServerId, centralPatronTypeMappingsDTO)
+        return self.call("PUT", f"/inn-reach/central-servers/{centralServerId}/central-patron-type-mappings", centralPatronTypeMappingsDTO)
 
-    def saveInnReachRecallUser(self, centralServerId, innReachRecallUserDTO):
+    def saveinnreachrecalluser(self, centralServerId, innReachRecallUserDTO):
         """Add new Inn-Reach recall user to central server
 
         ``POST /inn-reach/central-servers/{centralServerId}/inn-reach-recall-user``
 
         Args:
             centralServerId (str):  (format: uuid)
             innReachRecallUserDTO (dict): See Schema below.
@@ -1083,20 +1064,20 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_saveInnReachRecallUser_request.schema
+            .. literalinclude:: ../files/Settings_saveinnreachrecalluser_request.schema
         """
-        return self.call("POST", "/inn-reach/central-servers/{centralServerId}/inn-reach-recall-user", centralServerId, innReachRecallUserDTO)
+        return self.call("POST", f"/inn-reach/central-servers/{centralServerId}/inn-reach-recall-user", innReachRecallUserDTO)
 
 		
-    def getCentralServerRecallUser(self, centralServerId):
+    def getcentralserverrecalluser(self, centralServerId):
         """Get Inn-Reach Central server recall user
 
         ``GET /inn-reach/central-servers/{centralServerId}/inn-reach-recall-user``
 
         Args:
             centralServerId (str):  (format: uuid)
 
@@ -1104,20 +1085,20 @@
             dict: See Schema below.
 
         Raises:
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_getCentralServerRecallUser_response.schema
+            .. literalinclude:: ../files/Settings_getcentralserverrecalluser_response.schema
         """
-        return self.call("GET", "/inn-reach/central-servers/{centralServerId}/inn-reach-recall-user", centralServerId)
+        return self.call("GET", f"/inn-reach/central-servers/{centralServerId}/inn-reach-recall-user")
 
 		
-    def updateCentralServerRecallUser(self, centralServerId, innReachRecallUserDTO):
+    def updatecentralserverrecalluser(self, centralServerId, innReachRecallUserDTO):
         """Update Inn-Reach Central server recall user
 
         ``PUT /inn-reach/central-servers/{centralServerId}/inn-reach-recall-user``
 
         Args:
             centralServerId (str):  (format: uuid)
             innReachRecallUserDTO (dict): See Schema below.
@@ -1125,19 +1106,19 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_updateCentralServerRecallUser_request.schema
+            .. literalinclude:: ../files/Settings_updatecentralserverrecalluser_request.schema
         """
-        return self.call("PUT", "/inn-reach/central-servers/{centralServerId}/inn-reach-recall-user", centralServerId, innReachRecallUserDTO)
+        return self.call("PUT", f"/inn-reach/central-servers/{centralServerId}/inn-reach-recall-user", innReachRecallUserDTO)
 
-    def getConfigurationByCentralServerId(self, centralServerId):
+    def getconfigurationbycentralserverid(self, centralServerId):
         """Get Visible Patron Field Configuration by Central Server id
 
         ``GET /inn-reach/central-servers/{centralServerId}/visible-patron-field-configuration``
 
         Args:
             centralServerId (str):  (format: uuid)
 
@@ -1146,20 +1127,20 @@
 
         Raises:
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_getConfigurationByCentralServerId_response.schema
+            .. literalinclude:: ../files/Settings_getconfigurationbycentralserverid_response.schema
         """
-        return self.call("GET", "/inn-reach/central-servers/{centralServerId}/visible-patron-field-configuration", centralServerId)
+        return self.call("GET", f"/inn-reach/central-servers/{centralServerId}/visible-patron-field-configuration")
 
 		
-    def updateConfiguration(self, centralServerId, visiblePatronFieldConfigurationDTO):
+    def updateconfiguration(self, centralServerId, visiblePatronFieldConfigurationDTO):
         """Update Visible Patron Field Configuration
 
         ``PUT /inn-reach/central-servers/{centralServerId}/visible-patron-field-configuration``
 
         Args:
             centralServerId (str):  (format: uuid)
             visiblePatronFieldConfigurationDTO (dict): See Schema below.
@@ -1167,20 +1148,20 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_updateConfiguration_request.schema
+            .. literalinclude:: ../files/Settings_updateconfiguration_request.schema
         """
-        return self.call("PUT", "/inn-reach/central-servers/{centralServerId}/visible-patron-field-configuration", centralServerId, visiblePatronFieldConfigurationDTO)
+        return self.call("PUT", f"/inn-reach/central-servers/{centralServerId}/visible-patron-field-configuration", visiblePatronFieldConfigurationDTO)
 
 		
-    def createConfiguration(self, centralServerId, visiblePatronFieldConfigurationDTO):
+    def createconfiguration(self, centralServerId, visiblePatronFieldConfigurationDTO):
         """Add new Visible Patron Field Configuration associated with the central server
 
         ``POST /inn-reach/central-servers/{centralServerId}/visible-patron-field-configuration``
 
         Args:
             centralServerId (str):  (format: uuid)
             visiblePatronFieldConfigurationDTO (dict): See Schema below.
@@ -1190,19 +1171,19 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_createConfiguration_request.schema
+            .. literalinclude:: ../files/Settings_createconfiguration_request.schema
         """
-        return self.call("POST", "/inn-reach/central-servers/{centralServerId}/visible-patron-field-configuration", centralServerId, visiblePatronFieldConfigurationDTO)
+        return self.call("POST", f"/inn-reach/central-servers/{centralServerId}/visible-patron-field-configuration", visiblePatronFieldConfigurationDTO)
 
-    def getPagingSlipTemplate(self, centralServerId):
+    def getpagingsliptemplate(self, centralServerId):
         """Get Paging Slip Template
 
         ``GET /inn-reach/central-servers/{centralServerId}/paging-slip-template``
 
         Args:
             centralServerId (str):  (format: uuid)
 
@@ -1211,20 +1192,20 @@
 
         Raises:
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_getPagingSlipTemplate_response.schema
+            .. literalinclude:: ../files/Settings_getpagingsliptemplate_response.schema
         """
-        return self.call("GET", "/inn-reach/central-servers/{centralServerId}/paging-slip-template", centralServerId)
+        return self.call("GET", f"/inn-reach/central-servers/{centralServerId}/paging-slip-template")
 
 		
-    def updatePagingSlipTemplate(self, centralServerId, pagingSlipTemplateDTO):
+    def updatepagingsliptemplate(self, centralServerId, pagingSlipTemplateDTO):
         """Update Paging Slip Template
 
         ``PUT /inn-reach/central-servers/{centralServerId}/paging-slip-template``
 
         Args:
             centralServerId (str):  (format: uuid)
             pagingSlipTemplateDTO (dict): See Schema below.
@@ -1232,98 +1213,97 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_updatePagingSlipTemplate_request.schema
+            .. literalinclude:: ../files/Settings_updatepagingsliptemplate_request.schema
         """
-        return self.call("PUT", "/inn-reach/central-servers/{centralServerId}/paging-slip-template", centralServerId, pagingSlipTemplateDTO)
+        return self.call("PUT", f"/inn-reach/central-servers/{centralServerId}/paging-slip-template", pagingSlipTemplateDTO)
 
-    def getAllPagingSlipTemplates(self):
+    def getallpagingsliptemplates(self):
         """Get list of Paging Slip Templates
 
         ``GET /inn-reach/central-servers/paging-slip-template``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_getAllPagingSlipTemplates_response.schema
+            .. literalinclude:: ../files/Settings_getallpagingsliptemplates_response.schema
         """
         return self.call("GET", "/inn-reach/central-servers/paging-slip-template")
 
 
 
 
-class CirculationAdmin(FolioAdminApi):
+class Circulation(FolioApi):
     """INN-Reach Circulation API
-    Administration
 
     
     """
 
-    def getCentralServerAgencies(self):
+    def getcentralserveragencies(self):
         """Get a combined list of agencies available from all configured central servers
 
         ``GET /inn-reach/central-servers/agencies``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_getCentralServerAgencies_response.schema
+            .. literalinclude:: ../files/Circulation_getcentralserveragencies_response.schema
         """
         return self.call("GET", "/inn-reach/central-servers/agencies")
 
-    def getCentralServerItemTypes(self):
+    def getcentralserveritemtypes(self):
         """Get a combined list of item types available from all configured central servers
 
         ``GET /inn-reach/central-servers/item-types``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_getCentralServerItemTypes_response.schema
+            .. literalinclude:: ../files/Circulation_getcentralserveritemtypes_response.schema
         """
         return self.call("GET", "/inn-reach/central-servers/item-types")
 
-    def getCentralServerPatronTypes(self):
+    def getcentralserverpatrontypes(self):
         """Get a combined list of patron types available from all configured central servers
 
         ``GET /inn-reach/central-servers/patron-types``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_getCentralServerPatronTypes_response.schema
+            .. literalinclude:: ../files/Circulation_getcentralserverpatrontypes_response.schema
         """
         return self.call("GET", "/inn-reach/central-servers/patron-types")
 
-    def getBibRecord(self, bibId, centralCode):
+    def getbibrecord(self, bibId, centralCode):
         """Handles D2IR request from central server for an already-contributed Bib record.
 
         ``POST /inn-reach/d2ir/getbibrecord/{bibId}/{centralCode}``
 
         Args:
             bibId (str): 32-character, alphanumeric id corresponding to a FOLIO instance record HRID
             centralCode (str): Unique code that identifies the central server (match against value stored in Central Server settings, used to determine contribution status) (pattern: [a-z,0-9]{3,5})
@@ -1332,19 +1312,19 @@
             dict: See Schema below.
 
         Raises:
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_getBibRecord_response.schema
+            .. literalinclude:: ../files/Circulation_getbibrecord_response.schema
         """
-        return self.call("POST", "/inn-reach/d2ir/getbibrecord/{bibId}/{centralCode}", bibId, centralCode)
+        return self.call("POST", f"/inn-reach/d2ir/getbibrecord/{bibId}/{centralCode}")
 
-    def createInnReachTransactionItemHold(self, trackingId, centralCode, transactionHoldDTO):
+    def createinnreachtransactionitemhold(self, trackingId, centralCode, transactionHoldDTO):
         """Originates an item hold at the owning site
 
         ``POST /inn-reach/d2ir/circ/itemhold/{trackingId}/{centralCode}``
 
         Args:
             trackingId (str): 
             centralCode (str): Unique code that identifies the central server (match against value stored in Central Server settings, used to determine contribution status) (pattern: [a-z,0-9]{3,5})
@@ -1355,20 +1335,20 @@
 
         Raises:
             OkapiRequestError: An error occurred during creation of transaction record
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_createInnReachTransactionItemHold_request.schema
-            .. literalinclude:: ../files/Circulation_createInnReachTransactionItemHold_request.schema_response.schema
+            .. literalinclude:: ../files/Circulation_createinnreachtransactionitemhold_request.schema
+            .. literalinclude:: ../files/Circulation_createinnreachtransactionitemhold_request.schema_response.schema
         """
-        return self.call("POST", "/inn-reach/d2ir/circ/itemhold/{trackingId}/{centralCode}", trackingId, centralCode, transactionHoldDTO)
+        return self.call("POST", f"/inn-reach/d2ir/circ/itemhold/{trackingId}/{centralCode}", transactionHoldDTO)
 
-    def getAllTransactions(self, **kwargs):
+    def getalltransactions(self, **kwargs):
         """Get a list of transactions for the given central server
 
         ``GET /inn-reach/transactions``
 
         Keyword Args:
             offset (int): Skip over a number of elements by specifying an offset value for the query (default: 0, minimum: 0, maximum: 2147483647)
             limit (int): Limit the number of elements returned in the response (default: 10, minimum: 0, maximum: 2147483647)
@@ -1379,179 +1359,169 @@
 
         Raises:
             OkapiRequestError: Bad request, e.g. malformed query parameter.
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_getAllTransactions_response.schema
+            .. literalinclude:: ../files/Circulation_getalltransactions_response.schema
         """
         return self.call("GET", "/inn-reach/transactions", query=kwargs)
 
-    def getInnReachTransaction(self, id_):
+    def getinnreachtransaction(self, id_):
         """get inn-reach transaction by id
 
         ``GET /inn-reach/transactions/{id}``
 
-        Args:
-            id_ (str):  (format: uuid)
-
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_getInnReachTransaction_response.schema
+            .. literalinclude:: ../files/Circulation_getinnreachtransaction_response.schema
         """
-        return self.call("GET", "/inn-reach/transactions/{id}", id_)
+        return self.call("GET", f"/inn-reach/transactions/{id_}")
 
 		
-    def updateInnReachTransaction(self, id_, innReachTransactionDTO):
+    def updateinnreachtransaction(self, innReachTransactionDTO, id_):
         """update inn-reach transaction by id
 
         ``PUT /inn-reach/transactions/{id}``
 
         Args:
-            id_ (str):  (format: uuid)
             innReachTransactionDTO (dict): See Schema below.
 
         Raises:
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_updateInnReachTransaction_request.schema
+            .. literalinclude:: ../files/Circulation_updateinnreachtransaction_request.schema
         """
-        return self.call("PUT", "/inn-reach/transactions/{id}", id_, innReachTransactionDTO)
+        return self.call("PUT", f"/inn-reach/transactions/{id_}", innReachTransactionDTO)
 
-    def checkInPatronHoldItem(self, id_, servicePointId):
+    def checkinpatronholditem(self, servicePointId, id_):
         """receive item for patron hold transaction
 
         ``POST /inn-reach/transactions/{id}/receive-item/{servicePointId}``
 
         Args:
-            id_ (str):  (format: uuid)
             servicePointId (str):  (format: uuid)
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_checkInPatronHoldItem_response.schema
+            .. literalinclude:: ../files/Circulation_checkinpatronholditem_response.schema
         """
-        return self.call("POST", "/inn-reach/transactions/{id}/receive-item/{servicePointId}", id_, servicePointId)
+        return self.call("POST", f"/inn-reach/transactions/{id_}/receive-item/{servicePointId}")
 
-    def checkInPatronHoldUnshippedItem(self, id_, servicePointId, itemBarcode):
+    def checkinpatronholdunshippeditem(self, servicePointId, itemBarcode, id_):
         """receive un-shipped/unannounced item for patron hold transaction
 
         ``POST /inn-reach/transactions/{id}/receive-unshipped-item/{servicePointId}/{itemBarcode}``
 
         Args:
-            id_ (str):  (format: uuid)
             servicePointId (str):  (format: uuid)
             itemBarcode (str): Barcode of the item
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_checkInPatronHoldUnshippedItem_response.schema
+            .. literalinclude:: ../files/Circulation_checkinpatronholdunshippeditem_response.schema
         """
-        return self.call("POST", "/inn-reach/transactions/{id}/receive-unshipped-item/{servicePointId}/{itemBarcode}", id_, servicePointId, itemBarcode)
+        return self.call("POST", f"/inn-reach/transactions/{id_}/receive-unshipped-item/{servicePointId}/{itemBarcode}")
 
-    def finalCheckInItemHold(self, id_, servicePointId):
+    def finalcheckinitemhold(self, servicePointId, id_):
         """Final check-in of an item loaned through INN-Reach
 
         ``POST /inn-reach/transactions/{id}/itemhold/finalcheckin/{servicePointId}``
 
         Args:
-            id_ (str):  (format: uuid)
             servicePointId (str):  (format: uuid)
 
         Raises:
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
         """
-        return self.call("POST", "/inn-reach/transactions/{id}/itemhold/finalcheckin/{servicePointId}", id_, servicePointId)
+        return self.call("POST", f"/inn-reach/transactions/{id_}/itemhold/finalcheckin/{servicePointId}")
 
-    def transferItemHold(self, id_, itemId):
+    def transferitemhold(self, itemId, id_):
         """Transfer item hold to another item
 
         ``POST /inn-reach/transactions/{id}/itemhold/transfer-item/{itemId}``
 
         Args:
-            id_ (str):  (format: uuid)
             itemId (str):  (format: uuid)
 
         Raises:
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
         """
-        return self.call("POST", "/inn-reach/transactions/{id}/itemhold/transfer-item/{itemId}", id_, itemId)
+        return self.call("POST", f"/inn-reach/transactions/{id_}/itemhold/transfer-item/{itemId}")
 
-    def checkOutPatronHoldItem(self, id_, servicePointId):
+    def checkoutpatronholditem(self, servicePointId, id_):
         """Checks out to requesting patron
 
         ``POST /inn-reach/transactions/{id}/patronhold/check-out-item/{servicePointId}``
 
         Args:
-            id_ (str):  (format: uuid)
             servicePointId (str):  (format: uuid)
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_checkOutPatronHoldItem_response.schema
+            .. literalinclude:: ../files/Circulation_checkoutpatronholditem_response.schema
         """
-        return self.call("POST", "/inn-reach/transactions/{id}/patronhold/check-out-item/{servicePointId}", id_, servicePointId)
+        return self.call("POST", f"/inn-reach/transactions/{id_}/patronhold/check-out-item/{servicePointId}")
 
-    def checkOutLocalHoldItem(self, id_, servicePointId):
+    def checkoutlocalholditem(self, servicePointId, id_):
         """Checks out Local Hold item to requesting patron
 
         ``POST /inn-reach/transactions/{id}/localhold/check-out-item/{servicePointId}``
 
         Args:
-            id_ (str):  (format: uuid)
             servicePointId (str):  (format: uuid)
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_checkOutLocalHoldItem_response.schema
+            .. literalinclude:: ../files/Circulation_checkoutlocalholditem_response.schema
         """
-        return self.call("POST", "/inn-reach/transactions/{id}/localhold/check-out-item/{servicePointId}", id_, servicePointId)
+        return self.call("POST", f"/inn-reach/transactions/{id_}/localhold/check-out-item/{servicePointId}")
 
-    def checkOutItemHoldItem(self, itemBarcode, servicePointId):
+    def checkoutitemholditem(self, itemBarcode, servicePointId):
         """checks out an item from the owning site to the borrowing site for an Item Hold transaction
 
         ``PUT /inn-reach/transactions/{itemBarcode}/check-out-item/{servicePointId}``
 
         Args:
             itemBarcode (str): Barcode of the item
             servicePointId (str):  (format: uuid)
@@ -1561,113 +1531,106 @@
 
         Raises:
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_checkOutItemHoldItem_response.schema
+            .. literalinclude:: ../files/Circulation_checkoutitemholditem_response.schema
         """
-        return self.call("PUT", "/inn-reach/transactions/{itemBarcode}/check-out-item/{servicePointId}", itemBarcode, servicePointId)
+        return self.call("PUT", f"/inn-reach/transactions/{itemBarcode}/check-out-item/{servicePointId}")
 
-    def cancelPatronHoldTransaction(self, id_, cancelTransactionHoldDTO):
+    def cancelpatronholdtransaction(self, cancelTransactionHoldDTO, id_):
         """Cancel patron hold transaction with the reason provided
 
         ``POST /inn-reach/transactions/{id}/patronhold/cancel``
 
         Args:
-            id_ (str):  (format: uuid)
             cancelTransactionHoldDTO (dict): See Schema below.
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_cancelPatronHoldTransaction_request.schema
-            .. literalinclude:: ../files/Circulation_cancelPatronHoldTransaction_request.schema_response.schema
+            .. literalinclude:: ../files/Circulation_cancelpatronholdtransaction_request.schema
+            .. literalinclude:: ../files/Circulation_cancelpatronholdtransaction_request.schema_response.schema
         """
-        return self.call("POST", "/inn-reach/transactions/{id}/patronhold/cancel", id_, cancelTransactionHoldDTO)
+        return self.call("POST", f"/inn-reach/transactions/{id_}/patronhold/cancel", cancelTransactionHoldDTO)
 
-    def recallItemHoldTransaction(self, id_):
+    def recallitemholdtransaction(self, id_):
         """Recall item hold transaction
 
         ``POST /inn-reach/transactions/{id}/itemhold/recall``
 
-        Args:
-            id_ (str):  (format: uuid)
-
         Raises:
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
         """
-        return self.call("POST", "/inn-reach/transactions/{id}/itemhold/recall", id_)
+        return self.call("POST", f"/inn-reach/transactions/{id_}/itemhold/recall")
 
-    def returnPatronHoldItem(self, id_, servicePointId):
+    def returnpatronholditem(self, servicePointId, id_):
         """Returns Patron Hold item
 
         ``POST /inn-reach/transactions/{id}/patronhold/return-item/{servicePointId}``
 
         Args:
-            id_ (str):  (format: uuid)
             servicePointId (str):  (format: uuid)
 
         Raises:
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
         """
-        return self.call("POST", "/inn-reach/transactions/{id}/patronhold/return-item/{servicePointId}", id_, servicePointId)
+        return self.call("POST", f"/inn-reach/transactions/{id_}/patronhold/return-item/{servicePointId}")
 
-    def cancelItemHoldTransaction(self, id_, cancelTransactionHoldDTO):
+    def cancelitemholdtransaction(self, cancelTransactionHoldDTO, id_):
         """Cancel item hold transaction with the reason provided
 
         ``POST /inn-reach/transactions/{id}/itemhold/cancel``
 
         Args:
-            id_ (str):  (format: uuid)
             cancelTransactionHoldDTO (dict): See Schema below.
 
         Raises:
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_cancelItemHoldTransaction_request.schema
+            .. literalinclude:: ../files/Circulation_cancelitemholdtransaction_request.schema
         """
-        return self.call("POST", "/inn-reach/transactions/{id}/itemhold/cancel", id_, cancelTransactionHoldDTO)
+        return self.call("POST", f"/inn-reach/transactions/{id_}/itemhold/cancel", cancelTransactionHoldDTO)
 
-    def cancelLocalHoldTransaction(self, id_, cancelTransactionHoldDTO):
+    def cancellocalholdtransaction(self, cancelTransactionHoldDTO, id_):
         """Cancel local hold transaction with the reason provided
 
         ``POST /inn-reach/transactions/{id}/localhold/cancel``
 
         Args:
-            id_ (str):  (format: uuid)
             cancelTransactionHoldDTO (dict): See Schema below.
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_cancelLocalHoldTransaction_request.schema
-            .. literalinclude:: ../files/Circulation_cancelLocalHoldTransaction_request.schema_response.schema
+            .. literalinclude:: ../files/Circulation_cancellocalholdtransaction_request.schema
+            .. literalinclude:: ../files/Circulation_cancellocalholdtransaction_request.schema_response.schema
         """
-        return self.call("POST", "/inn-reach/transactions/{id}/localhold/cancel", id_, cancelTransactionHoldDTO)
+        return self.call("POST", f"/inn-reach/transactions/{id_}/localhold/cancel", cancelTransactionHoldDTO)
 
-    def verifyPatron(self, patronInfoRequestDTO):
+    def verifypatron(self, patronInfoRequestDTO):
         """Handles D2IR request from central server for patron verification.
 
         ``POST /inn-reach/d2ir/circ/verifypatron``
 
         Args:
             patronInfoRequestDTO (dict): See Schema below.
 
@@ -1675,20 +1638,20 @@
             dict: See Schema below.
 
         Raises:
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_verifyPatron_request.schema
-            .. literalinclude:: ../files/Circulation_verifyPatron_request.schema_response.schema
+            .. literalinclude:: ../files/Circulation_verifypatron_request.schema
+            .. literalinclude:: ../files/Circulation_verifypatron_request.schema_response.schema
         """
-        return self.call("POST", "/inn-reach/d2ir/circ/verifypatron", patronInfoRequestDTO)
+        return self.call("POST", f"/inn-reach/d2ir/circ/verifypatron", patronInfoRequestDTO)
 
-    def patronHold(self, trackingId, centralCode, patronHoldDTO):
+    def patronhold(self, trackingId, centralCode, patronHoldDTO):
         """Originate a patron hold
 
         ``POST /inn-reach/d2ir/circ/patronhold/{trackingId}/{centralCode}``
 
         Args:
             trackingId (str): 
             centralCode (str): Unique code that identifies the central server (match against value stored in Central Server settings, used to determine contribution status) (pattern: [a-z,0-9]{3,5})
@@ -1699,20 +1662,20 @@
 
         Raises:
             OkapiRequestError: An error occurred during processing the request
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_patronHold_request.schema
-            .. literalinclude:: ../files/Circulation_patronHold_request.schema_response.schema
+            .. literalinclude:: ../files/Circulation_patronhold_request.schema
+            .. literalinclude:: ../files/Circulation_patronhold_request.schema_response.schema
         """
-        return self.call("POST", "/inn-reach/d2ir/circ/patronhold/{trackingId}/{centralCode}", trackingId, centralCode, patronHoldDTO)
+        return self.call("POST", f"/inn-reach/d2ir/circ/patronhold/{trackingId}/{centralCode}", patronHoldDTO)
 
-    def itemShipped(self, trackingId, centralCode, itemShippedDTO):
+    def itemshipped(self, trackingId, centralCode, itemShippedDTO):
         """Process shipped item
 
         ``PUT /inn-reach/d2ir/circ/itemshipped/{trackingId}/{centralCode}``
 
         Args:
             trackingId (str): 
             centralCode (str): Unique code that identifies the central server (match against value stored in Central Server settings, used to determine contribution status) (pattern: [a-z,0-9]{3,5})
@@ -1723,20 +1686,20 @@
 
         Raises:
             OkapiRequestError: An error occurred during processing the request
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_itemShipped_request.schema
-            .. literalinclude:: ../files/Circulation_itemShipped_request.schema_response.schema
+            .. literalinclude:: ../files/Circulation_itemshipped_request.schema
+            .. literalinclude:: ../files/Circulation_itemshipped_request.schema_response.schema
         """
-        return self.call("PUT", "/inn-reach/d2ir/circ/itemshipped/{trackingId}/{centralCode}", trackingId, centralCode, itemShippedDTO)
+        return self.call("PUT", f"/inn-reach/d2ir/circ/itemshipped/{trackingId}/{centralCode}", itemShippedDTO)
 
-    def cancelPatronHold(self, trackingId, centralCode, cancelRequestDTO):
+    def cancelpatronhold(self, trackingId, centralCode, cancelRequestDTO):
         """Cancel Patron Hold transaction
 
         ``PUT /inn-reach/d2ir/circ/cancelrequest/{trackingId}/{centralCode}``
 
         Args:
             trackingId (str): 
             centralCode (str): Unique code that identifies the central server (match against value stored in Central Server settings, used to determine contribution status) (pattern: [a-z,0-9]{3,5})
@@ -1747,20 +1710,20 @@
 
         Raises:
             OkapiRequestError: An error occurred during processing the request
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_cancelPatronHold_request.schema
-            .. literalinclude:: ../files/Circulation_cancelPatronHold_request.schema_response.schema
+            .. literalinclude:: ../files/Circulation_cancelpatronhold_request.schema
+            .. literalinclude:: ../files/Circulation_cancelpatronhold_request.schema_response.schema
         """
-        return self.call("PUT", "/inn-reach/d2ir/circ/cancelrequest/{trackingId}/{centralCode}", trackingId, centralCode, cancelRequestDTO)
+        return self.call("PUT", f"/inn-reach/d2ir/circ/cancelrequest/{trackingId}/{centralCode}", cancelRequestDTO)
 
-    def transferRequest(self, trackingId, centralCode, transferRequestDTO):
+    def transferrequest(self, trackingId, centralCode, transferRequestDTO):
         """Put transfer request
 
         ``PUT /inn-reach/d2ir/circ/transferrequest/{trackingId}/{centralCode}``
 
         Args:
             trackingId (str): 
             centralCode (str): Unique code that identifies the central server (match against value stored in Central Server settings, used to determine contribution status) (pattern: [a-z,0-9]{3,5})
@@ -1771,20 +1734,20 @@
 
         Raises:
             OkapiRequestError: An error occurred during processing the request
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_transferRequest_request.schema
-            .. literalinclude:: ../files/Circulation_transferRequest_request.schema_response.schema
+            .. literalinclude:: ../files/Circulation_transferrequest_request.schema
+            .. literalinclude:: ../files/Circulation_transferrequest_request.schema_response.schema
         """
-        return self.call("PUT", "/inn-reach/d2ir/circ/transferrequest/{trackingId}/{centralCode}", trackingId, centralCode, transferRequestDTO)
+        return self.call("PUT", f"/inn-reach/d2ir/circ/transferrequest/{trackingId}/{centralCode}", transferRequestDTO)
 
-    def cancelItemHold(self, trackingId, centralCode, baseCircRequestDTO):
+    def cancelitemhold(self, trackingId, centralCode, baseCircRequestDTO):
         """Cancel an item request
 
         ``PUT /inn-reach/d2ir/circ/cancelitemhold/{trackingId}/{centralCode}``
 
         Args:
             trackingId (str): 
             centralCode (str): Unique code that identifies the central server (match against value stored in Central Server settings, used to determine contribution status) (pattern: [a-z,0-9]{3,5})
@@ -1795,20 +1758,20 @@
 
         Raises:
             OkapiRequestError: An error occurred during processing the request
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_cancelItemHold_request.schema
-            .. literalinclude:: ../files/Circulation_cancelItemHold_request.schema_response.schema
+            .. literalinclude:: ../files/Circulation_cancelitemhold_request.schema
+            .. literalinclude:: ../files/Circulation_cancelitemhold_request.schema_response.schema
         """
-        return self.call("PUT", "/inn-reach/d2ir/circ/cancelitemhold/{trackingId}/{centralCode}", trackingId, centralCode, baseCircRequestDTO)
+        return self.call("PUT", f"/inn-reach/d2ir/circ/cancelitemhold/{trackingId}/{centralCode}", baseCircRequestDTO)
 
-    def receiveUnshipped(self, trackingId, centralCode, baseCircRequestDTO):
+    def receiveunshipped(self, trackingId, centralCode, baseCircRequestDTO):
         """Report unshipped item received to owning site for item hold
 
         ``PUT /inn-reach/d2ir/circ/receiveunshipped/{trackingId}/{centralCode}``
 
         Args:
             trackingId (str): 
             centralCode (str): Unique code that identifies the central server (match against value stored in Central Server settings, used to determine contribution status) (pattern: [a-z,0-9]{3,5})
@@ -1818,20 +1781,20 @@
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: An error occurred during processing the request
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_receiveUnshipped_request.schema
-            .. literalinclude:: ../files/Circulation_receiveUnshipped_request.schema_response.schema
+            .. literalinclude:: ../files/Circulation_receiveunshipped_request.schema
+            .. literalinclude:: ../files/Circulation_receiveunshipped_request.schema_response.schema
         """
-        return self.call("PUT", "/inn-reach/d2ir/circ/receiveunshipped/{trackingId}/{centralCode}", trackingId, centralCode, baseCircRequestDTO)
+        return self.call("PUT", f"/inn-reach/d2ir/circ/receiveunshipped/{trackingId}/{centralCode}", baseCircRequestDTO)
 
-    def itemInTransit(self, trackingId, centralCode, baseCircRequestDTO):
+    def itemintransit(self, trackingId, centralCode, baseCircRequestDTO):
         """Receives message from central server to owning site indicating that a loaned item is being returned after being loaned to the borrowing patron.
 
         ``PUT /inn-reach/d2ir/circ/intransit/{trackingId}/{centralCode}``
 
         Args:
             trackingId (str): 
             centralCode (str): Unique code that identifies the central server (match against value stored in Central Server settings, used to determine contribution status) (pattern: [a-z,0-9]{3,5})
@@ -1842,20 +1805,20 @@
 
         Raises:
             OkapiRequestError: An error occurred during processing the request
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_itemInTransit_request.schema
-            .. literalinclude:: ../files/Circulation_itemInTransit_request.schema_response.schema
+            .. literalinclude:: ../files/Circulation_itemintransit_request.schema
+            .. literalinclude:: ../files/Circulation_itemintransit_request.schema_response.schema
         """
-        return self.call("PUT", "/inn-reach/d2ir/circ/intransit/{trackingId}/{centralCode}", trackingId, centralCode, baseCircRequestDTO)
+        return self.call("PUT", f"/inn-reach/d2ir/circ/intransit/{trackingId}/{centralCode}", baseCircRequestDTO)
 
-    def returnUncirculated(self, trackingId, centralCode, returnUncirculatedDTO):
+    def returnuncirculated(self, trackingId, centralCode, returnUncirculatedDTO):
         """Return uncirculated message for item hold
 
         ``PUT /inn-reach/d2ir/circ/returnuncirculated/{trackingId}/{centralCode}``
 
         Args:
             trackingId (str): 
             centralCode (str): Unique code that identifies the central server (match against value stored in Central Server settings, used to determine contribution status) (pattern: [a-z,0-9]{3,5})
@@ -1866,20 +1829,20 @@
 
         Raises:
             OkapiRequestError: An error occurred during processing the request
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_returnUncirculated_request.schema
-            .. literalinclude:: ../files/Circulation_returnUncirculated_request.schema_response.schema
+            .. literalinclude:: ../files/Circulation_returnuncirculated_request.schema
+            .. literalinclude:: ../files/Circulation_returnuncirculated_request.schema_response.schema
         """
-        return self.call("PUT", "/inn-reach/d2ir/circ/returnuncirculated/{trackingId}/{centralCode}", trackingId, centralCode, returnUncirculatedDTO)
+        return self.call("PUT", f"/inn-reach/d2ir/circ/returnuncirculated/{trackingId}/{centralCode}", returnUncirculatedDTO)
 
-    def createLocalHold(self, trackingId, centralCode, localHoldDTO):
+    def createlocalhold(self, trackingId, centralCode, localHoldDTO):
         """Create Local Hold - Central server to owning site when a local patron of that site requests an item through central.
 
         ``PUT /inn-reach/d2ir/circ/localhold/{trackingId}/{centralCode}``
 
         Args:
             trackingId (str): 
             centralCode (str): Unique code that identifies the central server (match against value stored in Central Server settings, used to determine contribution status) (pattern: [a-z,0-9]{3,5})
@@ -1890,20 +1853,20 @@
 
         Raises:
             OkapiRequestError: An error occurred during processing the request
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_createLocalHold_request.schema
-            .. literalinclude:: ../files/Circulation_createLocalHold_request.schema_response.schema
+            .. literalinclude:: ../files/Circulation_createlocalhold_request.schema
+            .. literalinclude:: ../files/Circulation_createlocalhold_request.schema_response.schema
         """
-        return self.call("PUT", "/inn-reach/d2ir/circ/localhold/{trackingId}/{centralCode}", trackingId, centralCode, localHoldDTO)
+        return self.call("PUT", f"/inn-reach/d2ir/circ/localhold/{trackingId}/{centralCode}", localHoldDTO)
 
-    def itemReceived(self, trackingId, centralCode, itemReceivedDTO):
+    def itemreceived(self, trackingId, centralCode, itemReceivedDTO):
         """Shipped item has been received
 
         ``PUT /inn-reach/d2ir/circ/itemreceived/{trackingId}/{centralCode}``
 
         Args:
             trackingId (str): 
             centralCode (str): Unique code that identifies the central server (match against value stored in Central Server settings, used to determine contribution status) (pattern: [a-z,0-9]{3,5})
@@ -1914,18 +1877,18 @@
 
         Raises:
             OkapiRequestError: An error occurred during processing the request
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_itemReceived_request.schema
-            .. literalinclude:: ../files/Circulation_itemReceived_request.schema_response.schema
+            .. literalinclude:: ../files/Circulation_itemreceived_request.schema
+            .. literalinclude:: ../files/Circulation_itemreceived_request.schema_response.schema
         """
-        return self.call("PUT", "/inn-reach/d2ir/circ/itemreceived/{trackingId}/{centralCode}", trackingId, centralCode, itemReceivedDTO)
+        return self.call("PUT", f"/inn-reach/d2ir/circ/itemreceived/{trackingId}/{centralCode}", itemReceivedDTO)
 
     def recall(self, trackingId, centralCode, recallDTO):
         """Item has been recalled
 
         ``PUT /inn-reach/d2ir/circ/recall/{trackingId}/{centralCode}``
 
         Args:
@@ -1941,17 +1904,17 @@
             OkapiFatalError: Internal server error
 
         Schema:
 
             .. literalinclude:: ../files/Circulation_recall_request.schema
             .. literalinclude:: ../files/Circulation_recall_request.schema_response.schema
         """
-        return self.call("PUT", "/inn-reach/d2ir/circ/recall/{trackingId}/{centralCode}", trackingId, centralCode, recallDTO)
+        return self.call("PUT", f"/inn-reach/d2ir/circ/recall/{trackingId}/{centralCode}", recallDTO)
 
-    def borrowerRenew(self, trackingId, centralCode, renewLoanDTO):
+    def borrowerrenew(self, trackingId, centralCode, renewLoanDTO):
         """Borrower Renew Message for Item Hold
 
         ``PUT /inn-reach/d2ir/circ/borrowerrenew/{trackingId}/{centralCode}``
 
         Args:
             trackingId (str): 
             centralCode (str): Unique code that identifies the central server (match against value stored in Central Server settings, used to determine contribution status) (pattern: [a-z,0-9]{3,5})
@@ -1962,20 +1925,20 @@
 
         Raises:
             OkapiRequestError: An error occurred during processing the request
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_borrowerRenew_request.schema
-            .. literalinclude:: ../files/Circulation_borrowerRenew_request.schema_response.schema
+            .. literalinclude:: ../files/Circulation_borrowerrenew_request.schema
+            .. literalinclude:: ../files/Circulation_borrowerrenew_request.schema_response.schema
         """
-        return self.call("PUT", "/inn-reach/d2ir/circ/borrowerrenew/{trackingId}/{centralCode}", trackingId, centralCode, renewLoanDTO)
+        return self.call("PUT", f"/inn-reach/d2ir/circ/borrowerrenew/{trackingId}/{centralCode}", renewLoanDTO)
 
-    def finalCheckIn(self, trackingId, centralCode, baseCircRequestDTO):
+    def finalcheckin(self, trackingId, centralCode, baseCircRequestDTO):
         """Indicating that a returned item has been received by its owning site. This is a terminating transaction.
 
         ``PUT /inn-reach/d2ir/circ/finalcheckin/{trackingId}/{centralCode}``
 
         Args:
             trackingId (str): 
             centralCode (str): Unique code that identifies the central server (match against value stored in Central Server settings, used to determine contribution status) (pattern: [a-z,0-9]{3,5})
@@ -1986,20 +1949,20 @@
 
         Raises:
             OkapiRequestError: An error occurred during processing the request
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_finalCheckIn_request.schema
-            .. literalinclude:: ../files/Circulation_finalCheckIn_request.schema_response.schema
+            .. literalinclude:: ../files/Circulation_finalcheckin_request.schema
+            .. literalinclude:: ../files/Circulation_finalcheckin_request.schema_response.schema
         """
-        return self.call("PUT", "/inn-reach/d2ir/circ/finalcheckin/{trackingId}/{centralCode}", trackingId, centralCode, baseCircRequestDTO)
+        return self.call("PUT", f"/inn-reach/d2ir/circ/finalcheckin/{trackingId}/{centralCode}", baseCircRequestDTO)
 
-    def ownerRenew(self, trackingId, centralCode, renewLoanDTO):
+    def ownerrenew(self, trackingId, centralCode, renewLoanDTO):
         """Owner Renew loan
 
         ``PUT /inn-reach/d2ir/circ/ownerrenew/{trackingId}/{centralCode}``
 
         Args:
             trackingId (str): 
             centralCode (str): Unique code that identifies the central server (match against value stored in Central Server settings, used to determine contribution status) (pattern: [a-z,0-9]{3,5})
@@ -2010,20 +1973,20 @@
 
         Raises:
             OkapiRequestError: An error occurred during processing the request
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_ownerRenew_request.schema
-            .. literalinclude:: ../files/Circulation_ownerRenew_request.schema_response.schema
+            .. literalinclude:: ../files/Circulation_ownerrenew_request.schema
+            .. literalinclude:: ../files/Circulation_ownerrenew_request.schema_response.schema
         """
-        return self.call("PUT", "/inn-reach/d2ir/circ/ownerrenew/{trackingId}/{centralCode}", trackingId, centralCode, renewLoanDTO)
+        return self.call("PUT", f"/inn-reach/d2ir/circ/ownerrenew/{trackingId}/{centralCode}", renewLoanDTO)
 
-    def claimsReturned(self, trackingId, centralCode, claimsItemReturnedDTO):
+    def claimsreturned(self, trackingId, centralCode, claimsItemReturnedDTO):
         """Borrower claims item returned
 
         ``PUT /inn-reach/d2ir/circ/claimsreturned/{trackingId}/{centralCode}``
 
         Args:
             trackingId (str): 
             centralCode (str): Unique code that identifies the central server (match against value stored in Central Server settings, used to determine contribution status) (pattern: [a-z,0-9]{3,5})
@@ -2034,42 +1997,41 @@
 
         Raises:
             OkapiRequestError: An error occurred during processing the request
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_claimsReturned_request.schema
-            .. literalinclude:: ../files/Circulation_claimsReturned_request.schema_response.schema
+            .. literalinclude:: ../files/Circulation_claimsreturned_request.schema
+            .. literalinclude:: ../files/Circulation_claimsreturned_request.schema_response.schema
         """
-        return self.call("PUT", "/inn-reach/d2ir/circ/claimsreturned/{trackingId}/{centralCode}", trackingId, centralCode, claimsItemReturnedDTO)
+        return self.call("PUT", f"/inn-reach/d2ir/circ/claimsreturned/{trackingId}/{centralCode}", claimsItemReturnedDTO)
 
-    def transferLocalHold(self, id_, itemId):
+    def transferlocalhold(self, itemId, id_):
         """Transfer local hold to another item
 
         ``POST /inn-reach/transactions/{id}/localhold/transfer-item/{itemId}``
 
         Args:
-            id_ (str):  (format: uuid)
             itemId (str):  (format: uuid)
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_transferLocalHold_response.schema
+            .. literalinclude:: ../files/Circulation_transferlocalhold_response.schema
         """
-        return self.call("POST", "/inn-reach/transactions/{id}/localhold/transfer-item/{itemId}", id_, itemId)
+        return self.call("POST", f"/inn-reach/transactions/{id_}/localhold/transfer-item/{itemId}")
 
-    def getPagingSlips(self, servicePointId):
+    def getpagingslips(self, servicePointId):
         """Get a list of available tokens for INN-Reach paging slips
 
         ``GET /inn-reach/paging-slips/{servicePointId}``
 
         Args:
             servicePointId (str):  (format: uuid)
 
@@ -2078,10 +2040,10 @@
 
         Raises:
             OkapiRequestNotFound: Item not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Circulation_getPagingSlips_response.schema
+            .. literalinclude:: ../files/Circulation_getpagingslips_response.schema
         """
-        return self.call("GET", "/inn-reach/paging-slips/{servicePointId}", servicePointId)
+        return self.call("GET", f"/inn-reach/paging-slips/{servicePointId}")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/inventory.py` & `foliolib-0.3.5a1/foliolib/folio/api/inventory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.inventory")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/inventoryStorage.py` & `foliolib-0.3.5a1/foliolib/folio/api/inventoryStorage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.inventoryStorage")
 
@@ -1122,28 +1122,67 @@
 
 class AuthoritiesReindex(FolioApi):
     """Authority reindex
 
     Reindex authorities by generating domain events for them
     """
 
-    def set_reindex(self):
-        """Submit a reindex job
+    def get_reindices(self, **kwargs):
+        """Get all reindex jobs
 
-        ``POST /authority-storage/reindex``
+        ``GET /authority-storage/reindex``
+
+        Args:
+            **kwargs (properties): Keyword Arguments
+
+        Keyword Args:
+            query (str):  A query expressed as a CQL string
+                    (see [dev.folio.org/reference/glossary#cql](https://dev.folio.org/reference/glossary#cql))
+                    using valid searchable fields.
+                    The first example below shows the general form of a full CQL query,
+                    but those fields might not be relevant in this context.
+                    
+                    with valid searchable fields
+                    
+                    
+                    Example:
+                    
+                     - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
+                    
+                     - name=aaa
+            offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
+                    
+                    Example:
+                    
+                     - 0
+            limit (int): (default=10) Limit the number of elements returned in the response
+                    
+                    Example:
+                    
+                     - 10
 
         Returns:
             dict: See Schema below
 
         Raises:
+            OkapiRequestError: Bad Request
+            OkapiRequestUnauthorized: Authentication is required
+            OkapiRequestNotFound: Not Found
             OkapiFatalError: Server Error
 
         Schema:
 
-            .. literalinclude:: ../files/AuthoritiesReindex_set_reindex_return.schema 
+            .. literalinclude:: ../files/AuthoritiesReindex_get_reindices_return.schema 
+        """
+        return self.call("GET", "/authority-storage/reindex", query=kwargs)
+
+    def set_reindex(self):
+        """
+
+        ``POST /authority-storage/reindex``
         """
         return self.call("POST", "/authority-storage/reindex")
 
     def get_reindex(self, reindexId: str):
         """Get reindex job by id
 
         ``GET /authority-storage/reindex/{reindexId}``
@@ -2971,28 +3010,67 @@
 
 class InstanceReindex(FolioApi):
     """Instance reindex
 
     Reindex instances by generating domain events for them
     """
 
-    def set_reindex(self):
-        """Submit a reindex job
+    def get_reindices(self, **kwargs):
+        """Get all reindex jobs
 
-        ``POST /instance-storage/reindex``
+        ``GET /instance-storage/reindex``
+
+        Args:
+            **kwargs (properties): Keyword Arguments
+
+        Keyword Args:
+            query (str):  A query expressed as a CQL string
+                    (see [dev.folio.org/reference/glossary#cql](https://dev.folio.org/reference/glossary#cql))
+                    using valid searchable fields.
+                    The first example below shows the general form of a full CQL query,
+                    but those fields might not be relevant in this context.
+                    
+                    with valid searchable fields
+                    
+                    
+                    Example:
+                    
+                     - (username=="ab*" or personal.firstName=="ab*" or personal.lastName=="ab*") and active=="true" sortby personal.lastName personal.firstName barcode
+                    
+                     - name=aaa
+            offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
+                    
+                    Example:
+                    
+                     - 0
+            limit (int): (default=10) Limit the number of elements returned in the response
+                    
+                    Example:
+                    
+                     - 10
 
         Returns:
             dict: See Schema below
 
         Raises:
+            OkapiRequestError: Bad Request
+            OkapiRequestUnauthorized: Authentication is required
+            OkapiRequestNotFound: Not Found
             OkapiFatalError: Server Error
 
         Schema:
 
-            .. literalinclude:: ../files/InstanceReindex_set_reindex_return.schema 
+            .. literalinclude:: ../files/InstanceReindex_get_reindices_return.schema 
+        """
+        return self.call("GET", "/instance-storage/reindex", query=kwargs)
+
+    def set_reindex(self):
+        """
+
+        ``POST /instance-storage/reindex``
         """
         return self.call("POST", "/instance-storage/reindex")
 
     def get_reindex(self, reindexId: str):
         """Get reindex job by id
 
         ``GET /instance-storage/reindex/{reindexId}``
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/inventoryUpdate.py` & `foliolib-0.3.5a1/foliolib/folio/api/inventoryUpdate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.inventoryUpdate")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/invoice.py` & `foliolib-0.3.5a1/foliolib/folio/api/invoice.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.invoice")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/invoiceStorage.py` & `foliolib-0.3.5a1/foliolib/folio/api/invoiceStorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.invoiceStorage")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/kbEbscoJava.py` & `foliolib-0.3.5a1/foliolib/folio/api/kbEbscoJava.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.kbEbscoJava")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/ldp.py` & `foliolib-0.3.5a1/foliolib/folio/api/ldp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.ldp")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/licenses.py` & `foliolib-0.3.5a1/foliolib/folio/api/licenses.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.licenses")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/login.py` & `foliolib-0.3.5a1/foliolib/folio/api/login.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.login")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/loginSaml.py` & `foliolib-0.3.5a1/foliolib/folio/api/loginSaml.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.loginSaml")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/marccat.py` & `foliolib-0.3.5a1/foliolib/folio/api/marccat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.marccat")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/metaStorage.py` & `foliolib-0.3.5a1/foliolib/folio/api/metaStorage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,77 +1,76 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.metaStorage")
 
 
 
-class MetastorageAdmin(FolioAdminApi):
+class Metastorage(FolioApi):
     """Meta Storage
-    Administration
 
     
     """
 
-    def getOaiConfig(self):
+    def getoaiconfig(self):
         """Get OAI configuration
 
         ``GET /meta-storage/config/oai``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Metastorage_getOaiConfig_response.schema
+            .. literalinclude:: ../files/Metastorage_getoaiconfig_response.schema
         """
         return self.call("GET", "/meta-storage/config/oai")
 
 		
-    def putOaiConfig(self, oaiConfig):
+    def putoaiconfig(self, oaiConfig):
         """Update OAI configuration.
 
         ``PUT /meta-storage/config/oai``
 
         Args:
             oaiConfig (dict): See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Metastorage_putOaiConfig_request.schema
+            .. literalinclude:: ../files/Metastorage_putoaiconfig_request.schema
         """
-        return self.call("PUT", "/meta-storage/config/oai", oaiConfig)
+        return self.call("PUT", f"/meta-storage/config/oai", oaiConfig)
 
 		
-    def deleteOaiConfig(self):
+    def deleteoaiconfig(self):
         """Update OAI configuration.
 
         ``DELETE /meta-storage/config/oai``
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
         """
         return self.call("DELETE", "/meta-storage/config/oai")
 
-    def postConfigMatchKey(self, matchKey):
+    def postconfigmatchkey(self, matchKey):
         """Create match key
 
         ``POST /meta-storage/config/matchkeys``
 
         Args:
             matchKey (dict): See Schema below.
 
@@ -80,20 +79,20 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Metastorage_postConfigMatchKey_request.schema
+            .. literalinclude:: ../files/Metastorage_postconfigmatchkey_request.schema
         """
-        return self.call("POST", "/meta-storage/config/matchkeys", matchKey)
+        return self.call("POST", f"/meta-storage/config/matchkeys", matchKey)
 
 		
-    def getConfigMatchKeys(self, **kwargs):
+    def getconfigmatchkeys(self, **kwargs):
         """Get match key configurations
 
         ``GET /meta-storage/config/matchkeys``
 
         Keyword Args:
             count (str): control of counting in queries (default: none, enum: ['exact', 'none'])
             limit (int): Limit the number of elements returned in the response (default: 10, minimum: 0)
@@ -105,109 +104,109 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Metastorage_getConfigMatchKeys_response.schema
+            .. literalinclude:: ../files/Metastorage_getconfigmatchkeys_response.schema
         """
         return self.call("GET", "/meta-storage/config/matchkeys", query=kwargs)
 
-    def getConfigMatchKey(self):
+    def getconfigmatchkey(self, id_):
         """Get match key configuration
 
         ``GET /meta-storage/config/matchkeys/{id}``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Metastorage_getConfigMatchKey_response.schema
+            .. literalinclude:: ../files/Metastorage_getconfigmatchkey_response.schema
         """
-        return self.call("GET", "/meta-storage/config/matchkeys/{id}")
+        return self.call("GET", f"/meta-storage/config/matchkeys/{id_}")
 
 		
-    def deleteConfigMatchKey(self):
+    def deleteconfigmatchkey(self, id_):
         """Delete match key configuration
 
         ``DELETE /meta-storage/config/matchkeys/{id}``
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
         """
-        return self.call("DELETE", "/meta-storage/config/matchkeys/{id}")
+        return self.call("DELETE", f"/meta-storage/config/matchkeys/{id_}")
 
 		
-    def putConfigMatchKey(self, matchKey):
+    def putconfigmatchkey(self, matchKey, id_):
         """Update match key configuration.
 
         ``PUT /meta-storage/config/matchkeys/{id}``
 
         Args:
             matchKey (dict): See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Metastorage_putConfigMatchKey_request.schema
+            .. literalinclude:: ../files/Metastorage_putconfigmatchkey_request.schema
         """
-        return self.call("PUT", "/meta-storage/config/matchkeys/{id}", matchKey)
+        return self.call("PUT", f"/meta-storage/config/matchkeys/{id_}", matchKey)
 
-    def initializeMatchKey(self):
+    def initializematchkey(self, id_):
         """Recalculate match key across all records.
 
         ``PUT /meta-storage/config/matchkeys/{id}/initialize``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Metastorage_initializeMatchKey_response.schema
+            .. literalinclude:: ../files/Metastorage_initializematchkey_response.schema
         """
-        return self.call("PUT", "/meta-storage/config/matchkeys/{id}/initialize")
+        return self.call("PUT", f"/meta-storage/config/matchkeys/{id_}/initialize")
 
-    def statsMatchKey(self):
+    def statsmatchkey(self, id_):
         """Get statistics for match key configuration
 
         ``GET /meta-storage/config/matchkeys/{id}/stats``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Metastorage_statsMatchKey_response.schema
+            .. literalinclude:: ../files/Metastorage_statsmatchkey_response.schema
         """
-        return self.call("GET", "/meta-storage/config/matchkeys/{id}/stats")
+        return self.call("GET", f"/meta-storage/config/matchkeys/{id_}/stats")
 
-    def postCodeModule(self, codeModule):
+    def postcodemodule(self, codeModule):
         """Create a new code module
 
         ``POST /meta-storage/config/modules``
 
         Args:
             codeModule (dict): See Schema below.
 
@@ -216,20 +215,20 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Metastorage_postCodeModule_request.schema
+            .. literalinclude:: ../files/Metastorage_postcodemodule_request.schema
         """
-        return self.call("POST", "/meta-storage/config/modules", codeModule)
+        return self.call("POST", f"/meta-storage/config/modules", codeModule)
 
 		
-    def getCodeModules(self, **kwargs):
+    def getcodemodules(self, **kwargs):
         """Retrieve all code modules
 
         ``GET /meta-storage/config/modules``
 
         Keyword Args:
             count (str): control of counting in queries (default: none, enum: ['exact', 'none'])
             limit (int): Limit the number of elements returned in the response (default: 10, minimum: 0)
@@ -241,83 +240,83 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Metastorage_getCodeModules_response.schema
+            .. literalinclude:: ../files/Metastorage_getcodemodules_response.schema
         """
         return self.call("GET", "/meta-storage/config/modules", query=kwargs)
 
-    def getCodeModule(self):
+    def getcodemodule(self, id_):
         """Retrieve a code module by id
 
         ``GET /meta-storage/config/modules/{id}``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Metastorage_getCodeModule_response.schema
+            .. literalinclude:: ../files/Metastorage_getcodemodule_response.schema
         """
-        return self.call("GET", "/meta-storage/config/modules/{id}")
+        return self.call("GET", f"/meta-storage/config/modules/{id_}")
 
 		
-    def putCodeModule(self, codeModule):
+    def putcodemodule(self, codeModule, id_):
         """Update code module by id
 
         ``PUT /meta-storage/config/modules/{id}``
 
         Args:
             codeModule (dict): See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Metastorage_putCodeModule_request.schema
+            .. literalinclude:: ../files/Metastorage_putcodemodule_request.schema
         """
-        return self.call("PUT", "/meta-storage/config/modules/{id}", codeModule)
+        return self.call("PUT", f"/meta-storage/config/modules/{id_}", codeModule)
 
 		
-    def deleteCodeModule(self):
+    def deletecodemodule(self, id_):
         """Delete code module by id
 
         ``DELETE /meta-storage/config/modules/{id}``
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
         """
-        return self.call("DELETE", "/meta-storage/config/modules/{id}")
+        return self.call("DELETE", f"/meta-storage/config/modules/{id_}")
 
-    def reloadCodeModule(self):
+    def reloadcodemodule(self, id_):
         """Force module to be reloaded
 
         ``PUT /meta-storage/config/modules/{id}/reload``
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
         """
-        return self.call("PUT", "/meta-storage/config/modules/{id}/reload")
+        return self.call("PUT", f"/meta-storage/config/modules/{id_}/reload")
 
-    def postSource(self, source):
+    def postsource(self, source):
         """Create source.
 
         ``POST /meta-storage/sources``
 
         Args:
             source (dict): See Schema below.
 
@@ -326,20 +325,20 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Metastorage_postSource_request.schema
+            .. literalinclude:: ../files/Metastorage_postsource_request.schema
         """
-        return self.call("POST", "/meta-storage/sources", source)
+        return self.call("POST", f"/meta-storage/sources", source)
 
 		
-    def getSources(self, **kwargs):
+    def getsources(self, **kwargs):
         """Get sources.
 
         ``GET /meta-storage/sources``
 
         Keyword Args:
             limit (int): Limit the number of elements returned in the response (default: 10, minimum: 0)
             query (str): CQL query
@@ -350,51 +349,51 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Metastorage_getSources_response.schema
+            .. literalinclude:: ../files/Metastorage_getsources_response.schema
         """
         return self.call("GET", "/meta-storage/sources", query=kwargs)
 
-    def getSource(self):
+    def getsource(self, id_):
         """Get source.
 
         ``GET /meta-storage/config/sources/{id}``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Metastorage_getSource_response.schema
+            .. literalinclude:: ../files/Metastorage_getsource_response.schema
         """
-        return self.call("GET", "/meta-storage/config/sources/{id}")
+        return self.call("GET", f"/meta-storage/config/sources/{id_}")
 
 		
-    def deleteSource(self):
+    def deletesource(self, id_):
         """Delete source.
 
         ``DELETE /meta-storage/config/sources/{id}``
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
         """
-        return self.call("DELETE", "/meta-storage/config/sources/{id}")
+        return self.call("DELETE", f"/meta-storage/config/sources/{id_}")
 
-    def postIngestJob(self, ingestJobRequest):
+    def postingestjob(self, ingestJobRequest):
         """Create ingest job
 
         ``POST /meta-storage/ingest-jobs``
 
         Args:
             ingestJobRequest (dict): See Schema below.
 
@@ -403,19 +402,19 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Metastorage_postIngestJob_request.schema
+            .. literalinclude:: ../files/Metastorage_postingestjob_request.schema
         """
-        return self.call("POST", "/meta-storage/ingest-jobs", ingestJobRequest)
+        return self.call("POST", f"/meta-storage/ingest-jobs", ingestJobRequest)
 
-    def ingestJobRecord(self, ingestRecordChunk):
+    def ingestjobrecord(self, ingestRecordChunk, id_):
         """Put records for job.
 
         ``PUT /meta-storage/ingest-jobs/{id}``
 
         Args:
             ingestRecordChunk (dict): See Schema below.
 
@@ -425,56 +424,56 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Metastorage_ingestJobRecord_request.schema
-            .. literalinclude:: ../files/Metastorage_ingestJobRecord_request.schema_response.schema
+            .. literalinclude:: ../files/Metastorage_ingestjobrecord_request.schema
+            .. literalinclude:: ../files/Metastorage_ingestjobrecord_request.schema_response.schema
         """
-        return self.call("PUT", "/meta-storage/ingest-jobs/{id}", ingestRecordChunk)
+        return self.call("PUT", f"/meta-storage/ingest-jobs/{id_}", ingestRecordChunk)
 
 		
-    def ingestJobInfo(self):
+    def ingestjobinfo(self, id_):
         """Get ingest job information.
 
         ``GET /meta-storage/ingest-jobs/{id}``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Metastorage_ingestJobInfo_response.schema
+            .. literalinclude:: ../files/Metastorage_ingestjobinfo_response.schema
         """
-        return self.call("GET", "/meta-storage/ingest-jobs/{id}")
+        return self.call("GET", f"/meta-storage/ingest-jobs/{id_}")
 
 		
-    def ingestJobFinish(self, **kwargs):
+    def ingestjobfinish(self, id_, **kwargs):
         """Finish ingest job with either rollback of commit.
 
         ``DELETE /meta-storage/ingest-jobs/{id}``
 
         Keyword Args:
             commit (bool): whether to commit (default: False)
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
         """
-        return self.call("DELETE", "/meta-storage/ingest-jobs/{id}", query=kwargs)
+        return self.call("DELETE", f"/meta-storage/ingest-jobs/{id_}", query=kwargs)
 
-    def getGlobalRecords(self, **kwargs):
+    def getglobalrecords(self, **kwargs):
         """Get records that satisfy CQL query with fields localId, sourceId, globalId.
 
         ``GET /meta-storage/records``
 
         Keyword Args:
             count (str): control of counting in queries (default: none, enum: ['exact', 'none'])
             limit (int): Limit the number of elements returned in the response (default: 10, minimum: 0)
@@ -486,20 +485,20 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Metastorage_getGlobalRecords_response.schema
+            .. literalinclude:: ../files/Metastorage_getglobalrecords_response.schema
         """
         return self.call("GET", "/meta-storage/records", query=kwargs)
 
 		
-    def putGlobalRecords(self, ingestRecordRequest):
+    def putglobalrecords(self, ingestRecordRequest):
         """Create or update records.
 
         ``PUT /meta-storage/records``
 
         Args:
             ingestRecordRequest (dict): See Schema below.
 
@@ -508,103 +507,103 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Metastorage_putGlobalRecords_request.schema
-            .. literalinclude:: ../files/Metastorage_putGlobalRecords_request.schema_response.schema
+            .. literalinclude:: ../files/Metastorage_putglobalrecords_request.schema
+            .. literalinclude:: ../files/Metastorage_putglobalrecords_request.schema_response.schema
         """
-        return self.call("PUT", "/meta-storage/records", ingestRecordRequest)
+        return self.call("PUT", f"/meta-storage/records", ingestRecordRequest)
 
 		
-    def deleteGlobalRecords(self, **kwargs):
+    def deleteglobalrecords(self, **kwargs):
         """Delete global records.
 
         ``DELETE /meta-storage/records``
 
         Keyword Args:
             query (str): CQL query
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
         """
         return self.call("DELETE", "/meta-storage/records", query=kwargs)
 
-    def getGlobalRecord(self):
+    def getglobalrecord(self, globalId):
         """Get record with global identifier.
 
         ``GET /meta-storage/records/{globalId}``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Metastorage_getGlobalRecord_response.schema
+            .. literalinclude:: ../files/Metastorage_getglobalrecord_response.schema
         """
-        return self.call("GET", "/meta-storage/records/{globalId}")
+        return self.call("GET", f"/meta-storage/records/{globalId}")
 
-    def getClusters(self):
+    def getclusters(self):
         """Get clusters with matchkeyid. CQL query with matchValue, clusterId fields
 
         ``GET /meta-storage/clusters``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Metastorage_getClusters_response.schema
+            .. literalinclude:: ../files/Metastorage_getclusters_response.schema
         """
         return self.call("GET", "/meta-storage/clusters")
 
-    def getCluster(self):
+    def getcluster(self, clusterId):
         """Get cluster by identifier
 
         ``GET /meta-storage/clusters/{clusterId}``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Metastorage_getCluster_response.schema
+            .. literalinclude:: ../files/Metastorage_getcluster_response.schema
         """
-        return self.call("GET", "/meta-storage/clusters/{clusterId}")
+        return self.call("GET", f"/meta-storage/clusters/{clusterId}")
 
-    def oaiService(self):
+    def oaiservice(self):
         """OAI service
 
         ``GET /meta-storage/oai``
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
         """
         return self.call("GET", "/meta-storage/oai")
 
-    def postOaiPmhClient(self, oai_pmh_client):
+    def postoaipmhclient(self, oai_pmh_client):
         """Create OAI PMH client job
 
         ``POST /meta-storage/pmh-clients``
 
         Args:
             oai-pmh-client (dict): See Schema below.
 
@@ -613,131 +612,131 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Metastorage_postOaiPmhClient_request.schema
+            .. literalinclude:: ../files/Metastorage_postoaipmhclient_request.schema
         """
-        return self.call("POST", "/meta-storage/pmh-clients", oai_pmh_client)
+        return self.call("POST", f"/meta-storage/pmh-clients", oai_pmh_client)
 
 		
-    def getCollectionOaiPmhClient(self):
+    def getcollectionoaipmhclient(self):
         """Get all OAI PMH client jobs
 
         ``GET /meta-storage/pmh-clients``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Metastorage_getCollectionOaiPmhClient_response.schema
+            .. literalinclude:: ../files/Metastorage_getcollectionoaipmhclient_response.schema
         """
         return self.call("GET", "/meta-storage/pmh-clients")
 
-    def getOaiPmhClient(self):
+    def getoaipmhclient(self, id_):
         """Get OAI-PMH client
 
         ``GET /meta-storage/pmh-clients/{id}``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Metastorage_getOaiPmhClient_response.schema
+            .. literalinclude:: ../files/Metastorage_getoaipmhclient_response.schema
         """
-        return self.call("GET", "/meta-storage/pmh-clients/{id}")
+        return self.call("GET", f"/meta-storage/pmh-clients/{id_}")
 
 		
-    def putOaiPmhClient(self, oai_pmh_client):
+    def putoaipmhclient(self, oai_pmh_client, id_):
         """Update OAI-PMH client
 
         ``PUT /meta-storage/pmh-clients/{id}``
 
         Args:
             oai-pmh-client (dict): See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Metastorage_putOaiPmhClient_request.schema
+            .. literalinclude:: ../files/Metastorage_putoaipmhclient_request.schema
         """
-        return self.call("PUT", "/meta-storage/pmh-clients/{id}", oai_pmh_client)
+        return self.call("PUT", f"/meta-storage/pmh-clients/{id_}", oai_pmh_client)
 
 		
-    def deleteOaiPmhClient(self):
+    def deleteoaipmhclient(self, id_):
         """Delete OAI-PMH client
 
         ``DELETE /meta-storage/pmh-clients/{id}``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Metastorage_deleteOaiPmhClient_response.schema
+            .. literalinclude:: ../files/Metastorage_deleteoaipmhclient_response.schema
         """
-        return self.call("DELETE", "/meta-storage/pmh-clients/{id}")
+        return self.call("DELETE", f"/meta-storage/pmh-clients/{id_}")
 
-    def startOaiPmhClient(self):
+    def startoaipmhclient(self, id_):
         """Start OAI PMH client job
 
         ``POST /meta-storage/pmh-clients/{id}/start``
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
         """
-        return self.call("POST", "/meta-storage/pmh-clients/{id}/start")
+        return self.call("POST", f"/meta-storage/pmh-clients/{id_}/start")
 
-    def stopOaiPmhClient(self):
+    def stopoaipmhclient(self, id_):
         """Stop OAI PMH client job
 
         ``POST /meta-storage/pmh-clients/{id}/stop``
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
         """
-        return self.call("POST", "/meta-storage/pmh-clients/{id}/stop")
+        return self.call("POST", f"/meta-storage/pmh-clients/{id_}/stop")
 
-    def statusOaiPmhClient(self):
+    def statusoaipmhclient(self, id_):
         """Get OAI PMH client status
 
         ``GET /meta-storage/pmh-clients/{id}/status``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Metastorage_statusOaiPmhClient_response.schema
+            .. literalinclude:: ../files/Metastorage_statusoaipmhclient_response.schema
         """
-        return self.call("GET", "/meta-storage/pmh-clients/{id}/status")
+        return self.call("GET", f"/meta-storage/pmh-clients/{id_}/status")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/notify.py` & `foliolib-0.3.5a1/foliolib/folio/api/notify.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.notify")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/oaiPmh.py` & `foliolib-0.3.5a1/foliolib/folio/api/oaiPmh.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.oaiPmh")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/orders.py` & `foliolib-0.3.5a1/foliolib/folio/api/orders.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.orders")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/ordersStorage.py` & `foliolib-0.3.5a1/foliolib/folio/api/ordersStorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.ordersStorage")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/organizations.py` & `foliolib-0.3.5a1/foliolib/folio/api/organizations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.organizations")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/organizationsStorage.py` & `foliolib-0.3.5a1/foliolib/folio/api/organizationsStorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.organizationsStorage")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/passwordValidator.py` & `foliolib-0.3.5a1/foliolib/folio/api/passwordValidator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.passwordValidator")
 
 
 
-class PasswordvalidatorAdmin(FolioAdminApi):
+class Passwordvalidator(FolioApi):
     """Password validator module
-    Administration
 
     
     """
 
-    def validatePassword(self, password):
+    def validatepassword(self, password):
         """Validate password
 
         ``POST /tenant/password/validate``
 
         Args:
             password (dict): See Schema below.
 
@@ -31,29 +30,28 @@
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not found error
             OkapiRequestUnprocessableEntity: Validation errors
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Passwordvalidator_validatePassword_request.schema
-            .. literalinclude:: ../files/Passwordvalidator_validatePassword_request.schema_response.schema
+            .. literalinclude:: ../files/Passwordvalidator_validatepassword_request.schema
+            .. literalinclude:: ../files/Passwordvalidator_validatepassword_request.schema_response.schema
         """
-        return self.call("POST", "/tenant/password/validate", password)
+        return self.call("POST", f"/tenant/password/validate", password)
 
 
 
-class ValidatorregistryAdmin(FolioAdminApi):
+class Validatorregistry(FolioApi):
     """Validator Registry
-    Administration
 
     
     """
 
-    def getTenantRules(self, **kwargs):
+    def gettenantrules(self, **kwargs):
         """Get a list of existing validation rules for a tenant
 
         ``GET /tenant/rules``
 
         Keyword Args:
             offset (int): Skip over a number of elements by specifying an offset value for the query (default: 0, minimum: 0, maximum: 2147483647)
             limit (int): Limit the number of elements returned in the response (default: 10, minimum: 0, maximum: 2147483647)
@@ -64,20 +62,20 @@
 
         Raises:
             OkapiRequestUnprocessableEntity: Validation errors
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Validatorregistry_getTenantRules_response.schema
+            .. literalinclude:: ../files/Validatorregistry_gettenantrules_response.schema
         """
         return self.call("GET", "/tenant/rules", query=kwargs)
 
 		
-    def postTenantRules(self, validationRule):
+    def posttenantrules(self, validationRule):
         """Add a rule to a tenant
 
         ``POST /tenant/rules``
 
         Args:
             validationRule (dict): See Schema below.
 
@@ -87,20 +85,20 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestUnprocessableEntity: Validation errors
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Validatorregistry_postTenantRules_request.schema
+            .. literalinclude:: ../files/Validatorregistry_posttenantrules_request.schema
         """
-        return self.call("POST", "/tenant/rules", validationRule)
+        return self.call("POST", f"/tenant/rules", validationRule)
 
 		
-    def putTenantRule(self, validationRule):
+    def puttenantrule(self, validationRule):
         """Enable/disable/change the rule
 
         ``PUT /tenant/rules``
 
         Args:
             validationRule (dict): See Schema below.
 
@@ -110,28 +108,28 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Rule not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Validatorregistry_putTenantRule_request.schema
+            .. literalinclude:: ../files/Validatorregistry_puttenantrule_request.schema
         """
-        return self.call("PUT", "/tenant/rules", validationRule)
+        return self.call("PUT", f"/tenant/rules", validationRule)
 
-    def getTenantRuleById(self):
+    def gettenantrulebyid(self, ruleId):
         """
 
         ``GET /tenant/rules/{ruleId}``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestNotFound: Rule not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Validatorregistry_getTenantRuleById_response.schema
+            .. literalinclude:: ../files/Validatorregistry_gettenantrulebyid_response.schema
         """
-        return self.call("GET", "/tenant/rules/{ruleId}")
+        return self.call("GET", f"/tenant/rules/{ruleId}")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/patron.py` & `foliolib-0.3.5a1/foliolib/folio/api/patron.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.patron")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/patronBlocks.py` & `foliolib-0.3.5a1/foliolib/folio/api/patronBlocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.patronBlocks")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/permissions.py` & `foliolib-0.3.5a1/foliolib/folio/api/permissions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.permissions")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/pubsub.py` & `foliolib-0.3.5a1/foliolib/folio/api/pubsub.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.pubsub")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/quickMarc.py` & `foliolib-0.3.5a1/foliolib/folio/api/quickMarc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,130 +1,124 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.quickMarc")
 
 
 
-class RecordseditorAdmin(FolioAdminApi):
+class Recordseditor(FolioApi):
     """quickMARC Record Editor
-    Administration
 
     
     """
 
-    def getRecordByExternalId(self, **kwargs):
+    def getrecordbyexternalid(self, **kwargs):
         """Get MARC record by externalId
 
         ``GET /records-editor/records``
 
         Keyword Args:
-            externalId (str): UUID of the external that is related to the MARC record (format: uuid)
+            externalId (str): UUID of the external that is related to the MARC record
             lang (str): Requested language. Optional. [lang=en] (pattern: [a-zA-Z]{2}, default: en)
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request, e.g. malformed request body or query parameter. Details of the error (e.g. name of the parameter or line/character number with malformed data) provided in the response.
             OkapiRequestNotFound: MARC record with a given ID not found
             OkapiFatalError: Internal server error, e.g. due to misconfiguration
 
         Schema:
 
-            .. literalinclude:: ../files/Recordseditor_getRecordByExternalId_response.schema
+            .. literalinclude:: ../files/Recordseditor_getrecordbyexternalid_response.schema
         """
         return self.call("GET", "/records-editor/records", query=kwargs)
 
 		
-    def records(self, quickMarc):
+    def records(self, quickMarcCreate):
         """
 
         ``POST /records-editor/records``
 
         Args:
-            quickMarc (dict): See Schema below.
+            quickMarcCreate (dict): See Schema below.
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad Request
             OkapiFatalError: Internal server error, e.g. due to misconfiguration
 
         Schema:
 
             .. literalinclude:: ../files/Recordseditor_records_request.schema
             .. literalinclude:: ../files/Recordseditor_records_request.schema_response.schema
         """
-        return self.call("POST", "/records-editor/records", quickMarc)
+        return self.call("POST", f"/records-editor/records", quickMarcCreate)
 
-    def getRecordCreationStatus(self, **kwargs):
+    def getrecordcreationstatus(self, **kwargs):
         """Get status of MARC bibliographic record creation
 
         ``GET /records-editor/records/status``
 
         Keyword Args:
-            qmRecordId (str): UUID of ParsedRecord to be created (format: uuid)
+            qmRecordId (str): UUID of ParsedRecord to be created
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request, e.g. malformed request body or query parameter. Details of the error (e.g. name of the parameter or line/character number with malformed data) provided in the response.
             OkapiRequestNotFound: MARC record with a given ID not found
             OkapiFatalError: Internal server error, e.g. due to misconfiguration
 
         Schema:
 
-            .. literalinclude:: ../files/Recordseditor_getRecordCreationStatus_response.schema
+            .. literalinclude:: ../files/Recordseditor_getrecordcreationstatus_response.schema
         """
         return self.call("GET", "/records-editor/records/status", query=kwargs)
 
 
 
-class RecordseditorasyncAdmin(FolioAdminApi):
+class Recordseditorasync(FolioApi):
     """quickMARC Record Editor
-    Administration
 
     
     """
 
-    def putRecord(self, id_, quickMarc):
+    def putrecord(self, quickMarcEdit, id_):
         """Edit MARC record
 
         ``PUT /records-editor/records/{id}``
 
         Args:
-            id_ (str): The UUID of a record (format: uuid)
-            quickMarc (dict): See Schema below.
+            quickMarcEdit (dict): See Schema below.
 
         Raises:
             OkapiRequestError: Bad request, e.g. malformed request body or query parameter. Details of the error (e.g. name of the parameter or line/character number with malformed data) provided in the response.
             OkapiRequestConflict: Update failed due to optimistic locking
             OkapiFatalError: Internal server error, e.g. due to misconfiguration
 
         Schema:
 
-            .. literalinclude:: ../files/Recordseditorasync_putRecord_request.schema
+            .. literalinclude:: ../files/Recordseditorasync_putrecord_request.schema
         """
-        return self.call("PUT", "/records-editor/records/{id}", id_, quickMarc)
+        return self.call("PUT", f"/records-editor/records/{id_}", quickMarcEdit)
 
 		
-    def deleteRecordByExternalId(self, id_):
+    def deleterecordbyexternalid(self, id_):
         """Delete MARC record by externalId
 
         ``DELETE /records-editor/records/{id}``
 
-        Args:
-            id_ (str): UUID of the external that is related to the MARC record (format: uuid)
-
         Raises:
             OkapiRequestError: Bad request, e.g. malformed request body or query parameter. Details of the error (e.g. name of the parameter or line/character number with malformed data) provided in the response.
             OkapiRequestNotFound: MARC record with a given ID not found
             OkapiFatalError: Internal server error, e.g. due to misconfiguration
         """
-        return self.call("DELETE", "/records-editor/records/{id}", id_)
+        return self.call("DELETE", f"/records-editor/records/{id_}")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/remoteStorage.py` & `foliolib-0.3.5a1/foliolib/folio/api/remoteStorage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.remoteStorage")
 
 
 
-class RemotestorageAdmin(FolioAdminApi):
+class Remotestorage(FolioApi):
     """Remote storages API
-    Administration
 
     
     """
 
-    def getConfigurations(self, **kwargs):
+    def getconfigurations(self, **kwargs):
         """Get a list of remote storage configurations
 
         ``GET /remote-storage/configurations``
 
         Keyword Args:
             offset (int): Skip over a number of elements by specifying an offset value for the query (default: 0, minimum: 0, maximum: 2147483647)
             limit (int): Limit the number of elements returned in the response (default: 10, minimum: 0, maximum: 2147483647)
@@ -30,20 +29,20 @@
             dict: See Schema below.
 
         Raises:
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Remotestorage_getConfigurations_response.schema
+            .. literalinclude:: ../files/Remotestorage_getconfigurations_response.schema
         """
         return self.call("GET", "/remote-storage/configurations", query=kwargs)
 
 		
-    def postConfiguration(self, storageConfiguration):
+    def postconfiguration(self, storageConfiguration):
         """Add new remote storage configuration
 
         ``POST /remote-storage/configurations``
 
         Args:
             storageConfiguration (dict): See Schema below.
 
@@ -53,69 +52,69 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestUnprocessableEntity: Validation errors
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Remotestorage_postConfiguration_request.schema
+            .. literalinclude:: ../files/Remotestorage_postconfiguration_request.schema
         """
-        return self.call("POST", "/remote-storage/configurations", storageConfiguration)
+        return self.call("POST", f"/remote-storage/configurations", storageConfiguration)
 
-    def getConfigurationById(self):
+    def getconfigurationbyid(self, configId):
         """
 
         ``GET /remote-storage/configurations/{configId}``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestNotFound: Configuration not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Remotestorage_getConfigurationById_response.schema
+            .. literalinclude:: ../files/Remotestorage_getconfigurationbyid_response.schema
         """
-        return self.call("GET", "/remote-storage/configurations/{configId}")
+        return self.call("GET", f"/remote-storage/configurations/{configId}")
 
 		
-    def putConfiguration(self, storageConfiguration):
+    def putconfiguration(self, storageConfiguration, configId):
         """Change the remote storage configuration
 
         ``PUT /remote-storage/configurations/{configId}``
 
         Args:
             storageConfiguration (dict): See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Configuration not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Remotestorage_putConfiguration_request.schema
+            .. literalinclude:: ../files/Remotestorage_putconfiguration_request.schema
         """
-        return self.call("PUT", "/remote-storage/configurations/{configId}", storageConfiguration)
+        return self.call("PUT", f"/remote-storage/configurations/{configId}", storageConfiguration)
 
 		
-    def deleteConfigurationById(self):
+    def deleteconfigurationbyid(self, configId):
         """
 
         ``DELETE /remote-storage/configurations/{configId}``
 
         Raises:
             OkapiRequestNotFound: Configuration not found
             OkapiFatalError: Internal server error
         """
-        return self.call("DELETE", "/remote-storage/configurations/{configId}")
+        return self.call("DELETE", f"/remote-storage/configurations/{configId}")
 
-    def postMapping(self, remoteLocationConfigurationMapping):
+    def postmapping(self, remoteLocationConfigurationMapping):
         """Add/update a mapping between remote and Folio locations
 
         ``POST /remote-storage/mappings``
 
         Args:
             remoteLocationConfigurationMapping (dict): See Schema below.
 
@@ -125,20 +124,20 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestUnprocessableEntity: Validation errors
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Remotestorage_postMapping_request.schema
+            .. literalinclude:: ../files/Remotestorage_postmapping_request.schema
         """
-        return self.call("POST", "/remote-storage/mappings", remoteLocationConfigurationMapping)
+        return self.call("POST", f"/remote-storage/mappings", remoteLocationConfigurationMapping)
 
 		
-    def getMappings(self, **kwargs):
+    def getmappings(self, **kwargs):
         """Get a list of location mappings
 
         ``GET /remote-storage/mappings``
 
         Keyword Args:
             finalLocationId (str): Final location id
             remoteStorageConfigurationId (str): Remote storage configuration id
@@ -149,49 +148,49 @@
             dict: See Schema below.
 
         Raises:
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Remotestorage_getMappings_response.schema
+            .. literalinclude:: ../files/Remotestorage_getmappings_response.schema
         """
         return self.call("GET", "/remote-storage/mappings", query=kwargs)
 
-    def getMappingById(self):
+    def getmappingbyid(self, folioLocationId):
         """
 
         ``GET /remote-storage/mappings/{folioLocationId}``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestNotFound: Mapping not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Remotestorage_getMappingById_response.schema
+            .. literalinclude:: ../files/Remotestorage_getmappingbyid_response.schema
         """
-        return self.call("GET", "/remote-storage/mappings/{folioLocationId}")
+        return self.call("GET", f"/remote-storage/mappings/{folioLocationId}")
 
 		
-    def deleteMappingById(self):
+    def deletemappingbyid(self, folioLocationId):
         """
 
         ``DELETE /remote-storage/mappings/{folioLocationId}``
 
         Raises:
             OkapiRequestNotFound: Mapping not found
             OkapiFatalError: Internal server error
         """
-        return self.call("DELETE", "/remote-storage/mappings/{folioLocationId}")
+        return self.call("DELETE", f"/remote-storage/mappings/{folioLocationId}")
 
-    def postExtendedRemoteLocationConfigurationMapping(self, extendedRemoteLocationConfigurationMapping):
+    def postextendedremotelocationconfigurationmapping(self, extendedRemoteLocationConfigurationMapping):
         """Add/update a mapping between remote and Folio locations
 
         ``POST /remote-storage/extended-mappings``
 
         Args:
             extendedRemoteLocationConfigurationMapping (dict): See Schema below.
 
@@ -201,20 +200,20 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestUnprocessableEntity: Validation errors
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Remotestorage_postExtendedRemoteLocationConfigurationMapping_request.schema
+            .. literalinclude:: ../files/Remotestorage_postextendedremotelocationconfigurationmapping_request.schema
         """
-        return self.call("POST", "/remote-storage/extended-mappings", extendedRemoteLocationConfigurationMapping)
+        return self.call("POST", f"/remote-storage/extended-mappings", extendedRemoteLocationConfigurationMapping)
 
 		
-    def getExtendedRemoteLocationConfigurationMappings(self, **kwargs):
+    def getextendedremotelocationconfigurationmappings(self, **kwargs):
         """Get a list of location mappings
 
         ``GET /remote-storage/extended-mappings``
 
         Keyword Args:
             finalLocationId (str): Final location id
             remoteStorageConfigurationId (str): Remote storage configuration id
@@ -226,52 +225,52 @@
             dict: See Schema below.
 
         Raises:
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Remotestorage_getExtendedRemoteLocationConfigurationMappings_response.schema
+            .. literalinclude:: ../files/Remotestorage_getextendedremotelocationconfigurationmappings_response.schema
         """
         return self.call("GET", "/remote-storage/extended-mappings", query=kwargs)
 
-    def getExtendedRemoteLocationConfigurationMappingsById(self):
+    def getextendedremotelocationconfigurationmappingsbyid(self, finalLocationId):
         """
 
         ``GET /remote-storage/extended-mappings/{finalLocationId}``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestNotFound: Mapping not found
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Remotestorage_getExtendedRemoteLocationConfigurationMappingsById_response.schema
+            .. literalinclude:: ../files/Remotestorage_getextendedremotelocationconfigurationmappingsbyid_response.schema
         """
-        return self.call("GET", "/remote-storage/extended-mappings/{finalLocationId}")
+        return self.call("GET", f"/remote-storage/extended-mappings/{finalLocationId}")
 
-    def deleteOriginalLocationByRemoteStorageConfigurationIdAndOriginalLocationId(self, remoteStorageConfigurationId, originalLocationId):
+    def deleteoriginallocationbyremotestorageconfigurationidandoriginallocationid(self, remoteStorageConfigurationId, originalLocationId):
         """
 
         ``DELETE /remote-storage/extended-mappings/{remoteStorageConfigurationId}/{originalLocationId}``
 
         Args:
             remoteStorageConfigurationId (str): uuid
             originalLocationId (str): uuid
 
         Raises:
             OkapiRequestNotFound: Mapping not found
             OkapiFatalError: Internal server error
         """
-        return self.call("DELETE", "/remote-storage/extended-mappings/{remoteStorageConfigurationId}/{originalLocationId}", remoteStorageConfigurationId, originalLocationId)
+        return self.call("DELETE", f"/remote-storage/extended-mappings/{remoteStorageConfigurationId}/{originalLocationId}")
 
-    def getExtendedRemoteLocationConfigurationMappingsLocations(self, **kwargs):
+    def getextendedremotelocationconfigurationmappingslocations(self, **kwargs):
         """Get a list of location mappings
 
         ``GET /remote-storage/extended-mappings/locations``
 
         Keyword Args:
             remoteStorageConfigurationId (str): Remote storage configuration id
             offset (int): Skip over a number of elements by specifying an offset value for the query (default: 0, minimum: 0, maximum: 2147483647)
@@ -281,36 +280,36 @@
             dict: See Schema below.
 
         Raises:
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Remotestorage_getExtendedRemoteLocationConfigurationMappingsLocations_response.schema
+            .. literalinclude:: ../files/Remotestorage_getextendedremotelocationconfigurationmappingslocations_response.schema
         """
         return self.call("GET", "/remote-storage/extended-mappings/locations", query=kwargs)
 
-    def getProviders(self):
+    def getproviders(self):
         """Get a list of providers
 
         ``GET /remote-storage/providers``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Remotestorage_getProviders_response.schema
+            .. literalinclude:: ../files/Remotestorage_getproviders_response.schema
         """
         return self.call("GET", "/remote-storage/providers")
 
-    def postAccession(self, accessionRequest):
+    def postaccession(self, accessionRequest):
         """Perform remote storage initiated accession
 
         ``POST /remote-storage/accessions``
 
         Args:
             accessionRequest (dict): See Schema below.
 
@@ -320,21 +319,21 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestUnprocessableEntity: Validation errors
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Remotestorage_postAccession_request.schema
-            .. literalinclude:: ../files/Remotestorage_postAccession_request.schema_response.schema
+            .. literalinclude:: ../files/Remotestorage_postaccession_request.schema
+            .. literalinclude:: ../files/Remotestorage_postaccession_request.schema_response.schema
         """
-        return self.call("POST", "/remote-storage/accessions", accessionRequest)
+        return self.call("POST", f"/remote-storage/accessions", accessionRequest)
 
 		
-    def getAccessions(self, **kwargs):
+    def getaccessions(self, **kwargs):
         """Get a list of accession records
 
         ``GET /remote-storage/accessions``
 
         Keyword Args:
             accessioned (bool): Flag to indicate, that accession queue record was accessioned and has accesion date
             storageId (str): Remote storage id
@@ -346,53 +345,53 @@
             dict: See Schema below.
 
         Raises:
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Remotestorage_getAccessions_response.schema
+            .. literalinclude:: ../files/Remotestorage_getaccessions_response.schema
         """
         return self.call("GET", "/remote-storage/accessions", query=kwargs)
 
-    def setAccessionedById(self, accessionId):
+    def setaccessionedbyid(self, accessionId):
         """Set accessioned date by accession queue id
 
         ``PUT /remote-storage/accessions/id/{accessionId}``
 
         Args:
             accessionId (str): uuid
         """
-        return self.call("PUT", "/remote-storage/accessions/id/{accessionId}", accessionId)
+        return self.call("PUT", f"/remote-storage/accessions/id/{accessionId}")
 
-    def setAccessionedByBarcode(self, barcode):
+    def setaccessionedbybarcode(self, barcode):
         """Set accessioned date by item barcode
 
         ``PUT /remote-storage/accessions/barcode/{barcode}``
 
         Args:
             barcode (str): 
         """
-        return self.call("PUT", "/remote-storage/accessions/barcode/{barcode}", barcode)
+        return self.call("PUT", f"/remote-storage/accessions/barcode/{barcode}")
 
-    def logRecordEvent(self, pubSubEvent):
+    def logrecordevent(self, pubSubEvent):
         """
 
         ``POST /remote-storage/pub-sub-handlers/log-record-event``
 
         Args:
             pubSubEvent (dict): See Schema below.
 
         Schema:
 
-            .. literalinclude:: ../files/Remotestorage_logRecordEvent_request.schema
+            .. literalinclude:: ../files/Remotestorage_logrecordevent_request.schema
         """
-        return self.call("POST", "/remote-storage/pub-sub-handlers/log-record-event", pubSubEvent)
+        return self.call("POST", f"/remote-storage/pub-sub-handlers/log-record-event", pubSubEvent)
 
-    def getRetrievals(self, **kwargs):
+    def getretrievals(self, **kwargs):
         """Get a list of retrieval records
 
         ``GET /remote-storage/retrievals``
 
         Keyword Args:
             retrieved (bool): Flag to indicate, that retrievals queue record was retrieved and has retrievals date
             storageId (str): Remote storage id
@@ -404,39 +403,39 @@
             dict: See Schema below.
 
         Raises:
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Remotestorage_getRetrievals_response.schema
+            .. literalinclude:: ../files/Remotestorage_getretrievals_response.schema
         """
         return self.call("GET", "/remote-storage/retrievals", query=kwargs)
 
-    def setRetrievedById(self, retrievalId):
+    def setretrievedbyid(self, retrievalId):
         """Set retrieval date by retrieval queue id
 
         ``PUT /remote-storage/retrievals/id/{retrievalId}``
 
         Args:
             retrievalId (str): uuid
         """
-        return self.call("PUT", "/remote-storage/retrievals/id/{retrievalId}", retrievalId)
+        return self.call("PUT", f"/remote-storage/retrievals/id/{retrievalId}")
 
-    def setRetrievedByBarcode(self, barcode):
+    def setretrievedbybarcode(self, barcode):
         """Set retrieved date by item barcode
 
         ``PUT /remote-storage/retrievals/barcode/{barcode}``
 
         Args:
             barcode (str): 
         """
-        return self.call("PUT", "/remote-storage/retrievals/barcode/{barcode}", barcode)
+        return self.call("PUT", f"/remote-storage/retrievals/barcode/{barcode}")
 
-    def checkInItemByBarcodeWithRemoteStorageConfigurationId(self, remoteStorageConfigurationId, checkInItem):
+    def checkinitembybarcodewithremotestorageconfigurationid(self, remoteStorageConfigurationId, checkInItem):
         """Check-in the item in the primary service by barcode value
 
         ``POST /remote-storage/retrieve/{remoteStorageConfigurationId}/checkInItem``
 
         Args:
             remoteStorageConfigurationId (str): uuid
             checkInItem (dict): See Schema below.
@@ -444,19 +443,19 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestUnprocessableEntity: Validation errors
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Remotestorage_checkInItemByBarcodeWithRemoteStorageConfigurationId_request.schema
+            .. literalinclude:: ../files/Remotestorage_checkinitembybarcodewithremotestorageconfigurationid_request.schema
         """
-        return self.call("POST", "/remote-storage/retrieve/{remoteStorageConfigurationId}/checkInItem", remoteStorageConfigurationId, checkInItem)
+        return self.call("POST", f"/remote-storage/retrieve/{remoteStorageConfigurationId}/checkInItem", checkInItem)
 
-    def checkInItemByHoldIdWithRemoteStorageConfigurationId(self, remoteStorageConfigurationId, checkInItemByHoldId):
+    def checkinitembyholdidwithremotestorageconfigurationid(self, remoteStorageConfigurationId, checkInItemByHoldId):
         """Check-in the item in the primary service by barcode value
 
         ``POST /remote-storage/retrieve/{remoteStorageConfigurationId}/checkInItemByHoldId``
 
         Args:
             remoteStorageConfigurationId (str): 
             checkInItemByHoldId (dict): See Schema below.
@@ -464,19 +463,19 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestUnprocessableEntity: Validation errors
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Remotestorage_checkInItemByHoldIdWithRemoteStorageConfigurationId_request.schema
+            .. literalinclude:: ../files/Remotestorage_checkinitembyholdidwithremotestorageconfigurationid_request.schema
         """
-        return self.call("POST", "/remote-storage/retrieve/{remoteStorageConfigurationId}/checkInItemByHoldId", remoteStorageConfigurationId, checkInItemByHoldId)
+        return self.call("POST", f"/remote-storage/retrieve/{remoteStorageConfigurationId}/checkInItemByHoldId", checkInItemByHoldId)
 
-    def returnItemByBarcode(self, remoteStorageConfigurationId, checkInItem):
+    def returnitembybarcode(self, remoteStorageConfigurationId, checkInItem):
         """Return the item by barcode
 
         ``POST /remote-storage/return/{remoteStorageConfigurationId}``
 
         Args:
             remoteStorageConfigurationId (str): 
             checkInItem (dict): See Schema below.
@@ -485,25 +484,25 @@
             dict: See Schema below.
 
         Raises:
             OkapiFatalError: Internal server error
 
         Schema:
 
-            .. literalinclude:: ../files/Remotestorage_returnItemByBarcode_request.schema
-            .. literalinclude:: ../files/Remotestorage_returnItemByBarcode_request.schema_response.schema
+            .. literalinclude:: ../files/Remotestorage_returnitembybarcode_request.schema
+            .. literalinclude:: ../files/Remotestorage_returnitembybarcode_request.schema_response.schema
         """
-        return self.call("POST", "/remote-storage/return/{remoteStorageConfigurationId}", remoteStorageConfigurationId, checkInItem)
+        return self.call("POST", f"/remote-storage/return/{remoteStorageConfigurationId}", checkInItem)
 
-    def markItemAsMissingByBarcode(self, barcode):
+    def markitemasmissingbybarcode(self, barcode):
         """Mark item as missing
 
         ``POST /remote-storage/items/barcode/{barcode}/markAsMissing``
 
         Args:
             barcode (str): 
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal server error
         """
-        return self.call("POST", "/remote-storage/items/barcode/{barcode}/markAsMissing", barcode)
+        return self.call("POST", f"/remote-storage/items/barcode/{barcode}/markAsMissing")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/reservoir.py` & `foliolib-0.3.5a1/foliolib/folio/api/reservoir.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,77 +1,76 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.reservoir")
 
 
 
-class ReservoirAdmin(FolioAdminApi):
+class Reservoir(FolioApi):
     """Reservoir
-    Administration
 
     
     """
 
-    def getOaiConfig(self):
+    def getoaiconfig(self):
         """Get OAI configuration
 
         ``GET /reservoir/config/oai``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Reservoir_getOaiConfig_response.schema
+            .. literalinclude:: ../files/Reservoir_getoaiconfig_response.schema
         """
         return self.call("GET", "/reservoir/config/oai")
 
 		
-    def putOaiConfig(self, oaiConfig):
+    def putoaiconfig(self, oaiConfig):
         """Update OAI configuration.
 
         ``PUT /reservoir/config/oai``
 
         Args:
             oaiConfig (dict): See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Reservoir_putOaiConfig_request.schema
+            .. literalinclude:: ../files/Reservoir_putoaiconfig_request.schema
         """
-        return self.call("PUT", "/reservoir/config/oai", oaiConfig)
+        return self.call("PUT", f"/reservoir/config/oai", oaiConfig)
 
 		
-    def deleteOaiConfig(self):
+    def deleteoaiconfig(self):
         """Update OAI configuration.
 
         ``DELETE /reservoir/config/oai``
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
         """
         return self.call("DELETE", "/reservoir/config/oai")
 
-    def postConfigMatchKey(self, matchKey):
+    def postconfigmatchkey(self, matchKey):
         """Create match key
 
         ``POST /reservoir/config/matchkeys``
 
         Args:
             matchKey (dict): See Schema below.
 
@@ -80,20 +79,20 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Reservoir_postConfigMatchKey_request.schema
+            .. literalinclude:: ../files/Reservoir_postconfigmatchkey_request.schema
         """
-        return self.call("POST", "/reservoir/config/matchkeys", matchKey)
+        return self.call("POST", f"/reservoir/config/matchkeys", matchKey)
 
 		
-    def getConfigMatchKeys(self, **kwargs):
+    def getconfigmatchkeys(self, **kwargs):
         """Get match key configurations
 
         ``GET /reservoir/config/matchkeys``
 
         Keyword Args:
             count (str): control of counting in queries (default: none, enum: ['exact', 'none'])
             limit (int): Limit the number of elements returned in the response (default: 10, minimum: 0)
@@ -105,109 +104,109 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Reservoir_getConfigMatchKeys_response.schema
+            .. literalinclude:: ../files/Reservoir_getconfigmatchkeys_response.schema
         """
         return self.call("GET", "/reservoir/config/matchkeys", query=kwargs)
 
-    def getConfigMatchKey(self):
+    def getconfigmatchkey(self, id_):
         """Get match key configuration
 
         ``GET /reservoir/config/matchkeys/{id}``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Reservoir_getConfigMatchKey_response.schema
+            .. literalinclude:: ../files/Reservoir_getconfigmatchkey_response.schema
         """
-        return self.call("GET", "/reservoir/config/matchkeys/{id}")
+        return self.call("GET", f"/reservoir/config/matchkeys/{id_}")
 
 		
-    def deleteConfigMatchKey(self):
+    def deleteconfigmatchkey(self, id_):
         """Delete match key configuration
 
         ``DELETE /reservoir/config/matchkeys/{id}``
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
         """
-        return self.call("DELETE", "/reservoir/config/matchkeys/{id}")
+        return self.call("DELETE", f"/reservoir/config/matchkeys/{id_}")
 
 		
-    def putConfigMatchKey(self, matchKey):
+    def putconfigmatchkey(self, matchKey, id_):
         """Update match key configuration.
 
         ``PUT /reservoir/config/matchkeys/{id}``
 
         Args:
             matchKey (dict): See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Reservoir_putConfigMatchKey_request.schema
+            .. literalinclude:: ../files/Reservoir_putconfigmatchkey_request.schema
         """
-        return self.call("PUT", "/reservoir/config/matchkeys/{id}", matchKey)
+        return self.call("PUT", f"/reservoir/config/matchkeys/{id_}", matchKey)
 
-    def initializeMatchKey(self):
+    def initializematchkey(self, id_):
         """Recalculate match key across all records.
 
         ``PUT /reservoir/config/matchkeys/{id}/initialize``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Reservoir_initializeMatchKey_response.schema
+            .. literalinclude:: ../files/Reservoir_initializematchkey_response.schema
         """
-        return self.call("PUT", "/reservoir/config/matchkeys/{id}/initialize")
+        return self.call("PUT", f"/reservoir/config/matchkeys/{id_}/initialize")
 
-    def statsMatchKey(self):
+    def statsmatchkey(self, id_):
         """Get statistics for match key configuration
 
         ``GET /reservoir/config/matchkeys/{id}/stats``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Reservoir_statsMatchKey_response.schema
+            .. literalinclude:: ../files/Reservoir_statsmatchkey_response.schema
         """
-        return self.call("GET", "/reservoir/config/matchkeys/{id}/stats")
+        return self.call("GET", f"/reservoir/config/matchkeys/{id_}/stats")
 
-    def postCodeModule(self, codeModule):
+    def postcodemodule(self, codeModule):
         """Create a new code module
 
         ``POST /reservoir/config/modules``
 
         Args:
             codeModule (dict): See Schema below.
 
@@ -216,20 +215,20 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Reservoir_postCodeModule_request.schema
+            .. literalinclude:: ../files/Reservoir_postcodemodule_request.schema
         """
-        return self.call("POST", "/reservoir/config/modules", codeModule)
+        return self.call("POST", f"/reservoir/config/modules", codeModule)
 
 		
-    def getCodeModules(self, **kwargs):
+    def getcodemodules(self, **kwargs):
         """Retrieve all code modules
 
         ``GET /reservoir/config/modules``
 
         Keyword Args:
             count (str): control of counting in queries (default: none, enum: ['exact', 'none'])
             limit (int): Limit the number of elements returned in the response (default: 10, minimum: 0)
@@ -241,83 +240,83 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Reservoir_getCodeModules_response.schema
+            .. literalinclude:: ../files/Reservoir_getcodemodules_response.schema
         """
         return self.call("GET", "/reservoir/config/modules", query=kwargs)
 
-    def getCodeModule(self):
+    def getcodemodule(self, id_):
         """Retrieve a code module by id
 
         ``GET /reservoir/config/modules/{id}``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Reservoir_getCodeModule_response.schema
+            .. literalinclude:: ../files/Reservoir_getcodemodule_response.schema
         """
-        return self.call("GET", "/reservoir/config/modules/{id}")
+        return self.call("GET", f"/reservoir/config/modules/{id_}")
 
 		
-    def putCodeModule(self, codeModule):
+    def putcodemodule(self, codeModule, id_):
         """Update code module by id
 
         ``PUT /reservoir/config/modules/{id}``
 
         Args:
             codeModule (dict): See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Reservoir_putCodeModule_request.schema
+            .. literalinclude:: ../files/Reservoir_putcodemodule_request.schema
         """
-        return self.call("PUT", "/reservoir/config/modules/{id}", codeModule)
+        return self.call("PUT", f"/reservoir/config/modules/{id_}", codeModule)
 
 		
-    def deleteCodeModule(self):
+    def deletecodemodule(self, id_):
         """Delete code module by id
 
         ``DELETE /reservoir/config/modules/{id}``
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
         """
-        return self.call("DELETE", "/reservoir/config/modules/{id}")
+        return self.call("DELETE", f"/reservoir/config/modules/{id_}")
 
-    def reloadCodeModule(self):
+    def reloadcodemodule(self, id_):
         """Force module to be reloaded
 
         ``PUT /reservoir/config/modules/{id}/reload``
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
         """
-        return self.call("PUT", "/reservoir/config/modules/{id}/reload")
+        return self.call("PUT", f"/reservoir/config/modules/{id_}/reload")
 
-    def postSource(self, source):
+    def postsource(self, source):
         """Create source.
 
         ``POST /reservoir/sources``
 
         Args:
             source (dict): See Schema below.
 
@@ -326,20 +325,20 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Reservoir_postSource_request.schema
+            .. literalinclude:: ../files/Reservoir_postsource_request.schema
         """
-        return self.call("POST", "/reservoir/sources", source)
+        return self.call("POST", f"/reservoir/sources", source)
 
 		
-    def getSources(self, **kwargs):
+    def getsources(self, **kwargs):
         """Get sources.
 
         ``GET /reservoir/sources``
 
         Keyword Args:
             limit (int): Limit the number of elements returned in the response (default: 10, minimum: 0)
             query (str): CQL query
@@ -350,51 +349,51 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Reservoir_getSources_response.schema
+            .. literalinclude:: ../files/Reservoir_getsources_response.schema
         """
         return self.call("GET", "/reservoir/sources", query=kwargs)
 
-    def getSource(self):
+    def getsource(self, id_):
         """Get source.
 
         ``GET /reservoir/config/sources/{id}``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Reservoir_getSource_response.schema
+            .. literalinclude:: ../files/Reservoir_getsource_response.schema
         """
-        return self.call("GET", "/reservoir/config/sources/{id}")
+        return self.call("GET", f"/reservoir/config/sources/{id_}")
 
 		
-    def deleteSource(self):
+    def deletesource(self, id_):
         """Delete source.
 
         ``DELETE /reservoir/config/sources/{id}``
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
         """
-        return self.call("DELETE", "/reservoir/config/sources/{id}")
+        return self.call("DELETE", f"/reservoir/config/sources/{id_}")
 
-    def postIngestJob(self, ingestJobRequest):
+    def postingestjob(self, ingestJobRequest):
         """Create ingest job
 
         ``POST /reservoir/ingest-jobs``
 
         Args:
             ingestJobRequest (dict): See Schema below.
 
@@ -403,19 +402,19 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Reservoir_postIngestJob_request.schema
+            .. literalinclude:: ../files/Reservoir_postingestjob_request.schema
         """
-        return self.call("POST", "/reservoir/ingest-jobs", ingestJobRequest)
+        return self.call("POST", f"/reservoir/ingest-jobs", ingestJobRequest)
 
-    def ingestJobRecord(self, ingestRecordChunk):
+    def ingestjobrecord(self, ingestRecordChunk, id_):
         """Put records for job.
 
         ``PUT /reservoir/ingest-jobs/{id}``
 
         Args:
             ingestRecordChunk (dict): See Schema below.
 
@@ -425,56 +424,56 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Reservoir_ingestJobRecord_request.schema
-            .. literalinclude:: ../files/Reservoir_ingestJobRecord_request.schema_response.schema
+            .. literalinclude:: ../files/Reservoir_ingestjobrecord_request.schema
+            .. literalinclude:: ../files/Reservoir_ingestjobrecord_request.schema_response.schema
         """
-        return self.call("PUT", "/reservoir/ingest-jobs/{id}", ingestRecordChunk)
+        return self.call("PUT", f"/reservoir/ingest-jobs/{id_}", ingestRecordChunk)
 
 		
-    def ingestJobInfo(self):
+    def ingestjobinfo(self, id_):
         """Get ingest job information.
 
         ``GET /reservoir/ingest-jobs/{id}``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Reservoir_ingestJobInfo_response.schema
+            .. literalinclude:: ../files/Reservoir_ingestjobinfo_response.schema
         """
-        return self.call("GET", "/reservoir/ingest-jobs/{id}")
+        return self.call("GET", f"/reservoir/ingest-jobs/{id_}")
 
 		
-    def ingestJobFinish(self, **kwargs):
+    def ingestjobfinish(self, id_, **kwargs):
         """Finish ingest job with either rollback of commit.
 
         ``DELETE /reservoir/ingest-jobs/{id}``
 
         Keyword Args:
             commit (bool): whether to commit (default: False)
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
         """
-        return self.call("DELETE", "/reservoir/ingest-jobs/{id}", query=kwargs)
+        return self.call("DELETE", f"/reservoir/ingest-jobs/{id_}", query=kwargs)
 
-    def uploadRecords(self, filePath):
+    def uploadrecords(self, filePath):
         """Upload MARC binary and MARCXML records.
 
         ``POST /reservoir/upload``
 
         Args:
             filePath (str): Path of file to upload.
 
@@ -484,28 +483,28 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestForbidden: Forbidden
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Reservoir_uploadRecords_response.schema
+            .. literalinclude:: ../files/Reservoir_uploadrecords_response.schema
         """
         import os
         headers = {}
         headers["Content-Type"] = "application/octet-stream"
         headers["Content-length"] = str(os.path.getsize(filePath))
         headers["Content-Disposition"] = "attachment; filename=%s" % os.path.basename(
             filePath)
         with open(filePath, 'rb') as f:
             data = f.read()
         
-        return self.call("POST", "/reservoir/upload", data=data)
+        return self.call("POST", f"/reservoir/upload", data=data)
 
-    def getGlobalRecords(self, **kwargs):
+    def getglobalrecords(self, **kwargs):
         """Get records that satisfy CQL query with fields localId, sourceId, globalId.
 
         ``GET /reservoir/records``
 
         Keyword Args:
             count (str): control of counting in queries (default: none, enum: ['exact', 'none'])
             limit (int): Limit the number of elements returned in the response (default: 10, minimum: 0)
@@ -517,20 +516,20 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Reservoir_getGlobalRecords_response.schema
+            .. literalinclude:: ../files/Reservoir_getglobalrecords_response.schema
         """
         return self.call("GET", "/reservoir/records", query=kwargs)
 
 		
-    def putGlobalRecords(self, ingestRecordRequest):
+    def putglobalrecords(self, ingestRecordRequest):
         """Create or update records.
 
         ``PUT /reservoir/records``
 
         Args:
             ingestRecordRequest (dict): See Schema below.
 
@@ -539,54 +538,54 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Reservoir_putGlobalRecords_request.schema
-            .. literalinclude:: ../files/Reservoir_putGlobalRecords_request.schema_response.schema
+            .. literalinclude:: ../files/Reservoir_putglobalrecords_request.schema
+            .. literalinclude:: ../files/Reservoir_putglobalrecords_request.schema_response.schema
         """
-        return self.call("PUT", "/reservoir/records", ingestRecordRequest)
+        return self.call("PUT", f"/reservoir/records", ingestRecordRequest)
 
 		
-    def deleteGlobalRecords(self, **kwargs):
+    def deleteglobalrecords(self, **kwargs):
         """Delete global records.
 
         ``DELETE /reservoir/records``
 
         Keyword Args:
             query (str): CQL query
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
         """
         return self.call("DELETE", "/reservoir/records", query=kwargs)
 
-    def getGlobalRecord(self):
+    def getglobalrecord(self, globalId):
         """Get record with global identifier.
 
         ``GET /reservoir/records/{globalId}``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Reservoir_getGlobalRecord_response.schema
+            .. literalinclude:: ../files/Reservoir_getglobalrecord_response.schema
         """
-        return self.call("GET", "/reservoir/records/{globalId}")
+        return self.call("GET", f"/reservoir/records/{globalId}")
 
-    def getClusters(self):
+    def getclusters(self):
         """Get clusters based on matchkeyid. Query is CQL with the following fields supported: matchValue, clusterId, globalId, localId, sourceId, sourceVersion.
 
 
         ``GET /reservoir/clusters``
 
         Returns:
             dict: See Schema below.
@@ -594,19 +593,19 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Reservoir_getClusters_response.schema
+            .. literalinclude:: ../files/Reservoir_getclusters_response.schema
         """
         return self.call("GET", "/reservoir/clusters")
 
-    def touchClusters(self, **kwargs):
+    def touchclusters(self, **kwargs):
         """Update cluster timestamps. CQL must specify at least matchkeyId and sourceId. The sourceVersion and clusterId are optional.
 
         ``POST /reservoir/clusters/touch``
 
         Keyword Args:
             query (str): CQL query
 
@@ -616,49 +615,49 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Reservoir_touchClusters_response.schema
+            .. literalinclude:: ../files/Reservoir_touchclusters_response.schema
         """
         return self.call("POST", "/reservoir/clusters/touch", query=kwargs)
 
-    def getCluster(self):
+    def getcluster(self, clusterId):
         """Get cluster by identifier
 
         ``GET /reservoir/clusters/{clusterId}``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Reservoir_getCluster_response.schema
+            .. literalinclude:: ../files/Reservoir_getcluster_response.schema
         """
-        return self.call("GET", "/reservoir/clusters/{clusterId}")
+        return self.call("GET", f"/reservoir/clusters/{clusterId}")
 
-    def oaiService(self):
+    def oaiservice(self):
         """OAI service
 
         ``GET /reservoir/oai``
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
         """
         return self.call("GET", "/reservoir/oai")
 
-    def postOaiPmhClient(self, oaiPmhClient):
+    def postoaipmhclient(self, oaiPmhClient):
         """Create OAI PMH client job
 
         ``POST /reservoir/pmh-clients``
 
         Args:
             oaiPmhClient (dict): See Schema below.
 
@@ -667,124 +666,124 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Reservoir_postOaiPmhClient_request.schema
+            .. literalinclude:: ../files/Reservoir_postoaipmhclient_request.schema
         """
-        return self.call("POST", "/reservoir/pmh-clients", oaiPmhClient)
+        return self.call("POST", f"/reservoir/pmh-clients", oaiPmhClient)
 
 		
-    def getCollectionOaiPmhClient(self):
+    def getcollectionoaipmhclient(self):
         """Get all OAI PMH client jobs
 
         ``GET /reservoir/pmh-clients``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Reservoir_getCollectionOaiPmhClient_response.schema
+            .. literalinclude:: ../files/Reservoir_getcollectionoaipmhclient_response.schema
         """
         return self.call("GET", "/reservoir/pmh-clients")
 
-    def getOaiPmhClient(self):
+    def getoaipmhclient(self, id_):
         """Get OAI-PMH client
 
         ``GET /reservoir/pmh-clients/{id}``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Reservoir_getOaiPmhClient_response.schema
+            .. literalinclude:: ../files/Reservoir_getoaipmhclient_response.schema
         """
-        return self.call("GET", "/reservoir/pmh-clients/{id}")
+        return self.call("GET", f"/reservoir/pmh-clients/{id_}")
 
 		
-    def putOaiPmhClient(self, oaiPmhClient):
+    def putoaipmhclient(self, oaiPmhClient, id_):
         """Update OAI-PMH client
 
         ``PUT /reservoir/pmh-clients/{id}``
 
         Args:
             oaiPmhClient (dict): See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Reservoir_putOaiPmhClient_request.schema
+            .. literalinclude:: ../files/Reservoir_putoaipmhclient_request.schema
         """
-        return self.call("PUT", "/reservoir/pmh-clients/{id}", oaiPmhClient)
+        return self.call("PUT", f"/reservoir/pmh-clients/{id_}", oaiPmhClient)
 
 		
-    def deleteOaiPmhClient(self):
+    def deleteoaipmhclient(self, id_):
         """Delete OAI-PMH client
 
         ``DELETE /reservoir/pmh-clients/{id}``
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
         """
-        return self.call("DELETE", "/reservoir/pmh-clients/{id}")
+        return self.call("DELETE", f"/reservoir/pmh-clients/{id_}")
 
-    def startOaiPmhClient(self):
+    def startoaipmhclient(self, id_):
         """Start OAI PMH client job
 
         ``POST /reservoir/pmh-clients/{id}/start``
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
         """
-        return self.call("POST", "/reservoir/pmh-clients/{id}/start")
+        return self.call("POST", f"/reservoir/pmh-clients/{id_}/start")
 
-    def stopOaiPmhClient(self):
+    def stopoaipmhclient(self, id_):
         """Stop OAI PMH client job
 
         ``POST /reservoir/pmh-clients/{id}/stop``
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
         """
-        return self.call("POST", "/reservoir/pmh-clients/{id}/stop")
+        return self.call("POST", f"/reservoir/pmh-clients/{id_}/stop")
 
-    def statusOaiPmhClient(self):
+    def statusoaipmhclient(self, id_):
         """Get OAI PMH client status
 
         ``GET /reservoir/pmh-clients/{id}/status``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Reservoir_statusOaiPmhClient_response.schema
+            .. literalinclude:: ../files/Reservoir_statusoaipmhclient_response.schema
         """
-        return self.call("GET", "/reservoir/pmh-clients/{id}/status")
+        return self.call("GET", f"/reservoir/pmh-clients/{id_}/status")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/rtac.py` & `foliolib-0.3.5a1/foliolib/folio/api/rtac.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.rtac")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/search.py` & `foliolib-0.3.5a1/foliolib/folio/api/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.search")
 
@@ -11,15 +11,15 @@
 
 class Search(FolioApi):
     """Search API
 
     Search API
     """
 
-    def searchInstances(self, **kwargs):
+    def searchinstances(self, **kwargs):
         """Get a list of instances for CQL query
 
         ``GET /search/instances``
 
         Keyword Args:
             query (str): A CQL query string with search conditions.
             limit (int): Limit the number of elements returned in the response. (minimum: 0, maximum: 500, default: 100)
@@ -31,47 +31,47 @@
 
         Raises:
             OkapiRequestError: Validation errors
             OkapiFatalError: When unhandled exception occurred during code execution, e.g. NullPointerException
 
         Schema:
 
-            .. literalinclude:: ../files/Search_searchInstances_response.schema
+            .. literalinclude:: ../files/Search_searchinstances_response.schema
         """
         return self.call("GET", "/search/instances", query=kwargs)
 
-    def getInstanceIds(self, **kwargs):
+    def getinstanceids(self, **kwargs):
         """Get a list of instance ids for CQL query
 
         ``GET /search/instances/ids``
 
         Keyword Args:
             query (str): A CQL query string with search conditions.
 
         Raises:
             OkapiRequestError: Validation errors
             OkapiFatalError: When unhandled exception occurred during code execution, e.g. NullPointerException
         """
         return self.call("GET", "/search/instances/ids", query=kwargs)
 
-    def getHoldingIds(self, **kwargs):
+    def getholdingids(self, **kwargs):
         """Get a list of holding ids linked to instances found by the CQL query
 
         ``GET /search/holdings/ids``
 
         Keyword Args:
             query (str): A CQL query string with search conditions.
 
         Raises:
             OkapiRequestError: Validation errors
             OkapiFatalError: When unhandled exception occurred during code execution, e.g. NullPointerException
         """
         return self.call("GET", "/search/holdings/ids", query=kwargs)
 
-    def getFacets(self, recordType, **kwargs):
+    def getfacets(self, recordType, **kwargs):
         """Provides list of facets for the record type
 
         ``GET /search/{recordType}/facets``
 
         Args:
             recordType (str):  (enum: ['instances', 'authorities', 'contributors'])
 
@@ -84,43 +84,44 @@
 
         Raises:
             OkapiRequestError: Validation errors
             OkapiFatalError: When unhandled exception occurred during code execution, e.g. NullPointerException
 
         Schema:
 
-            .. literalinclude:: ../files/Search_getFacets_response.schema
+            .. literalinclude:: ../files/Search_getfacets_response.schema
         """
-        return self.call("GET", "/search/{recordType}/facets", recordType, query=kwargs)
+        return self.call("GET", f"/search/{recordType}/facets", query=kwargs)
 
-    def searchAuthorities(self, **kwargs):
+    def searchauthorities(self, **kwargs):
         """Get a list of authorities for CQL query
 
         ``GET /search/authorities``
 
         Keyword Args:
             query (str): A CQL query string with search conditions.
             limit (int): Limit the number of elements returned in the response. (minimum: 0, maximum: 500, default: 100)
             offset (int): Skip over a number of elements by specifying an offset value for the query. (minimum: 0, maximum: 9999, default: 0)
             expandAll (bool): Whether to return only basic properties or entire instance. (default: False)
+            includeNumberOfTitles (bool): Whether to perform a search for a number of linked instances. (default: True)
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Validation errors
             OkapiFatalError: When unhandled exception occurred during code execution, e.g. NullPointerException
 
         Schema:
 
-            .. literalinclude:: ../files/Search_searchAuthorities_response.schema
+            .. literalinclude:: ../files/Search_searchauthorities_response.schema
         """
         return self.call("GET", "/search/authorities", query=kwargs)
 
-    def getIdsJob(self, jobId):
+    def getidsjob(self, jobId):
         """Get a job for the stream of resource ids.
 
         ``GET /search/resources/jobs/{jobId}``
 
         Args:
             jobId (str): UUID of the job to get
 
@@ -129,19 +130,19 @@
 
         Raises:
             OkapiRequestError: Validation errors
             OkapiFatalError: When unhandled exception occurred during code execution, e.g. NullPointerException
 
         Schema:
 
-            .. literalinclude:: ../files/Search_getIdsJob_response.schema
+            .. literalinclude:: ../files/Search_getidsjob_response.schema
         """
-        return self.call("GET", "/search/resources/jobs/{jobId}", jobId)
+        return self.call("GET", f"/search/resources/jobs/{jobId}")
 
-    def submitIdsJob(self, resourceIdsJob):
+    def submitidsjob(self, resourceIdsJob):
         """Creates a job for the stream of resource ids.
 
         ``POST /search/resources/jobs``
 
         Args:
             resourceIdsJob (dict): See Schema below.
 
@@ -150,58 +151,59 @@
 
         Raises:
             OkapiRequestError: Validation errors
             OkapiFatalError: When unhandled exception occurred during code execution, e.g. NullPointerException
 
         Schema:
 
-            .. literalinclude:: ../files/Search_submitIdsJob_request.schema
+            .. literalinclude:: ../files/Search_submitidsjob_request.schema
         """
-        return self.call("POST", "/search/resources/jobs", resourceIdsJob)
+        return self.call("POST", f"/search/resources/jobs", resourceIdsJob)
 
-    def getResourceIds(self, jobId):
+    def getresourceids(self, jobId):
         """Get a list of resource ids by job id
 
         ``GET /search/resources/jobs/{jobId}/ids``
 
         Args:
             jobId (str): UUID of the job to get
 
         Raises:
             OkapiRequestError: Validation errors
             OkapiFatalError: When unhandled exception occurred during code execution, e.g. NullPointerException
         """
-        return self.call("GET", "/search/resources/jobs/{jobId}/ids", jobId)
+        return self.call("GET", f"/search/resources/jobs/{jobId}/ids")
 
-    def browseInstancesByCallNumber(self, **kwargs):
+    def browseinstancesbycallnumber(self, **kwargs):
         """Provides list of instances for browsing by call number
 
         ``GET /search/browse/call-numbers/instances``
 
         Keyword Args:
             query (str): A CQL query string with search conditions.
             limit (int): Limit the number of elements returned in the browse response. (minimum: 0, maximum: 100, default: 100)
             expandAll (bool): Whether to return only basic properties or entire instance. (default: False)
             highlightMatch (bool): Whether to highlight matched resource by query input or not. (default: True)
             precedingRecordsCount (int): Number of preceding records for browsing around and around-including options (minimum: 1, maximum: 100)
+            callNumberType (str): Type of call number (enum: ['lc', 'dewey', 'nlm', 'sudoc', 'other', 'local'])
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Validation errors
             OkapiFatalError: When unhandled exception occurred during code execution, e.g. NullPointerException
 
         Schema:
 
-            .. literalinclude:: ../files/Search_browseInstancesByCallNumber_response.schema
+            .. literalinclude:: ../files/Search_browseinstancesbycallnumber_response.schema
         """
         return self.call("GET", "/search/browse/call-numbers/instances", query=kwargs)
 
-    def browseInstancesBySubject(self, **kwargs):
+    def browseinstancesbysubject(self, **kwargs):
         """Provides list of instances for browsing by subject
 
         ``GET /search/browse/subjects/instances``
 
         Keyword Args:
             query (str): A CQL query string with search conditions.
             limit (int): Limit the number of elements returned in the response. (minimum: 0, maximum: 500, default: 100)
@@ -213,19 +215,19 @@
 
         Raises:
             OkapiRequestError: Validation errors
             OkapiFatalError: When unhandled exception occurred during code execution, e.g. NullPointerException
 
         Schema:
 
-            .. literalinclude:: ../files/Search_browseInstancesBySubject_response.schema
+            .. literalinclude:: ../files/Search_browseinstancesbysubject_response.schema
         """
         return self.call("GET", "/search/browse/subjects/instances", query=kwargs)
 
-    def browseInstancesByContributor(self, **kwargs):
+    def browseinstancesbycontributor(self, **kwargs):
         """Provides list of instances for browsing by contributor
 
         ``GET /search/browse/contributors/instances``
 
         Keyword Args:
             query (str): A CQL query string with search conditions.
             limit (int): Limit the number of elements returned in the response. (minimum: 0, maximum: 500, default: 100)
@@ -237,19 +239,19 @@
 
         Raises:
             OkapiRequestError: Validation errors
             OkapiFatalError: When unhandled exception occurred during code execution, e.g. NullPointerException
 
         Schema:
 
-            .. literalinclude:: ../files/Search_browseInstancesByContributor_response.schema
+            .. literalinclude:: ../files/Search_browseinstancesbycontributor_response.schema
         """
         return self.call("GET", "/search/browse/contributors/instances", query=kwargs)
 
-    def browseAuthorities(self, **kwargs):
+    def browseauthorities(self, **kwargs):
         """Provides list of authorities by headingRef
 
         ``GET /search/browse/authorities``
 
         Keyword Args:
             query (str): A CQL query string with search conditions.
             limit (int): Limit the number of elements returned in the response. (minimum: 0, maximum: 500, default: 100)
@@ -262,19 +264,19 @@
 
         Raises:
             OkapiRequestError: Validation errors
             OkapiFatalError: When unhandled exception occurred during code execution, e.g. NullPointerException
 
         Schema:
 
-            .. literalinclude:: ../files/Search_browseAuthorities_response.schema
+            .. literalinclude:: ../files/Search_browseauthorities_response.schema
         """
         return self.call("GET", "/search/browse/authorities", query=kwargs)
 
-    def createIndices(self, createIndexRequest):
+    def createindices(self, createIndexRequest):
         """Creates indices for passed resource name and tenant id in request header.
 
         ``POST /search/index/indices``
 
         Args:
             createIndexRequest (dict): See Schema below.
 
@@ -283,20 +285,20 @@
 
         Raises:
             OkapiRequestError: Validation errors
             OkapiFatalError: When unhandled exception occurred during code execution, e.g. NullPointerException
 
         Schema:
 
-            .. literalinclude:: ../files/Search_createIndices_request.schema
-            .. literalinclude:: ../files/Search_createIndices_request.schema_response.schema
+            .. literalinclude:: ../files/Search_createindices_request.schema
+            .. literalinclude:: ../files/Search_createindices_request.schema_response.schema
         """
-        return self.call("POST", "/search/index/indices", createIndexRequest)
+        return self.call("POST", f"/search/index/indices", createIndexRequest)
 
-    def updateMappings(self, updateMappingsRequest):
+    def updatemappings(self, updateMappingsRequest):
         """Creates mappings for passed resource name and tenant id in request header.
 
         ``POST /search/index/mappings``
 
         Args:
             updateMappingsRequest (dict): See Schema below.
 
@@ -304,20 +306,20 @@
             dict: See Schema below.
 
         Raises:
             OkapiFatalError: When unhandled exception occurred during code execution, e.g. NullPointerException
 
         Schema:
 
-            .. literalinclude:: ../files/Search_updateMappings_request.schema
-            .. literalinclude:: ../files/Search_updateMappings_request.schema_response.schema
+            .. literalinclude:: ../files/Search_updatemappings_request.schema
+            .. literalinclude:: ../files/Search_updatemappings_request.schema_response.schema
         """
-        return self.call("POST", "/search/index/mappings", updateMappingsRequest)
+        return self.call("POST", f"/search/index/mappings", updateMappingsRequest)
 
-    def reindexInventoryRecords(self, reindexRequest):
+    def reindexinventoryrecords(self, reindexRequest):
         """Initiates reindex for the inventory records
 
         ``POST /search/index/inventory/reindex``
 
         Args:
             reindexRequest (dict): See Schema below.
 
@@ -325,28 +327,28 @@
             dict: See Schema below.
 
         Raises:
             OkapiFatalError: When unhandled exception occurred during code execution, e.g. NullPointerException
 
         Schema:
 
-            .. literalinclude:: ../files/Search_reindexInventoryRecords_request.schema
-            .. literalinclude:: ../files/Search_reindexInventoryRecords_request.schema_response.schema
+            .. literalinclude:: ../files/Search_reindexinventoryrecords_request.schema
+            .. literalinclude:: ../files/Search_reindexinventoryrecords_request.schema_response.schema
         """
-        return self.call("POST", "/search/index/inventory/reindex", reindexRequest)
+        return self.call("POST", f"/search/index/inventory/reindex", reindexRequest)
 
 
 class SearchAdmin(FolioAdminApi):
     """Search API
     Administration
 
     Search API
     """
 
-    def indexRecords(self, indexRecordRequest):
+    def indexrecords(self, indexRecordRequest):
         """Indexes the records into elasticsearch.
 
         ``POST /search/index/records``
 
         Args:
             indexRecordRequest (dict): See Schema below.
 
@@ -354,20 +356,20 @@
             dict: See Schema below.
 
         Raises:
             OkapiFatalError: When unhandled exception occurred during code execution, e.g. NullPointerException
 
         Schema:
 
-            .. literalinclude:: ../files/Search_indexRecords_request.schema
-            .. literalinclude:: ../files/Search_indexRecords_request.schema_response.schema
+            .. literalinclude:: ../files/Search_indexrecords_request.schema
+            .. literalinclude:: ../files/Search_indexrecords_request.schema_response.schema
         """
-        return self.call("POST", "/search/index/records", indexRecordRequest)
+        return self.call("POST", f"/search/index/records", indexRecordRequest)
 
-    def createLanguageConfig(self, languageConfig):
+    def createlanguageconfig(self, languageConfig):
         """Save languages that will be used for analyzers
 
         ``POST /search/config/languages``
 
         Args:
             languageConfig (dict): See Schema below.
 
@@ -375,34 +377,34 @@
             dict: See Schema below.
 
         Raises:
             OkapiRequestUnprocessableEntity: Validation error for the request.
 
         Schema:
 
-            .. literalinclude:: ../files/Search_createLanguageConfig_request.schema
+            .. literalinclude:: ../files/Search_createlanguageconfig_request.schema
         """
-        return self.call("POST", "/search/config/languages", languageConfig)
+        return self.call("POST", f"/search/config/languages", languageConfig)
 
 		
-    def getAllLanguageConfigs(self):
+    def getalllanguageconfigs(self):
         """Get all supported languages
 
         ``GET /search/config/languages``
 
         Returns:
             dict: See Schema below.
 
         Schema:
 
-            .. literalinclude:: ../files/Search_getAllLanguageConfigs_response.schema
+            .. literalinclude:: ../files/Search_getalllanguageconfigs_response.schema
         """
         return self.call("GET", "/search/config/languages")
 
-    def updateLanguageConfig(self, code, languageConfig):
+    def updatelanguageconfig(self, code, languageConfig):
         """Update language config settings
 
         ``PUT /search/config/languages/{code}``
 
         Args:
             code (str): Language code (pattern: [a-zA-Z]{3})
             languageConfig (dict): See Schema below.
@@ -411,33 +413,33 @@
             dict: See Schema below.
 
         Raises:
             OkapiRequestUnprocessableEntity: Validation error for the request.
 
         Schema:
 
-            .. literalinclude:: ../files/Search_updateLanguageConfig_request.schema
+            .. literalinclude:: ../files/Search_updatelanguageconfig_request.schema
         """
-        return self.call("PUT", "/search/config/languages/{code}", code, languageConfig)
+        return self.call("PUT", f"/search/config/languages/{code}", languageConfig)
 
 		
-    def deleteLanguageConfig(self, code):
+    def deletelanguageconfig(self, code):
         """Delete all supported languages
 
         ``DELETE /search/config/languages/{code}``
 
         Args:
             code (str): Language code (pattern: [a-zA-Z]{3})
 
         Raises:
             OkapiRequestNotFound: No language support is found
         """
-        return self.call("DELETE", "/search/config/languages/{code}", code)
+        return self.call("DELETE", f"/search/config/languages/{code}")
 
-    def saveFeatureConfiguration(self, featureConfig):
+    def savefeatureconfiguration(self, featureConfig):
         """Save feature configuration (enables or disables pre-defined optional search options)
 
         ``POST /search/config/features``
 
         Args:
             featureConfig (dict): See Schema below.
 
@@ -446,34 +448,34 @@
 
         Raises:
             OkapiRequestError: Validation errors
             OkapiRequestUnprocessableEntity: Validation error for the request.
 
         Schema:
 
-            .. literalinclude:: ../files/Search_saveFeatureConfiguration_request.schema
+            .. literalinclude:: ../files/Search_savefeatureconfiguration_request.schema
         """
-        return self.call("POST", "/search/config/features", featureConfig)
+        return self.call("POST", f"/search/config/features", featureConfig)
 
 		
-    def getAllFeatures(self):
+    def getallfeatures(self):
         """Get all feature configurations per tenant
 
         ``GET /search/config/features``
 
         Returns:
             dict: See Schema below.
 
         Schema:
 
-            .. literalinclude:: ../files/Search_getAllFeatures_response.schema
+            .. literalinclude:: ../files/Search_getallfeatures_response.schema
         """
         return self.call("GET", "/search/config/features")
 
-    def updateFeatureConfiguration(self, featureId, featureConfig):
+    def updatefeatureconfiguration(self, featureId, featureConfig):
         """Update feature configuration settings
 
         ``PUT /search/config/features/{featureId}``
 
         Args:
             featureId (str): Feature id (name) (enum: ['search.all.fields', 'browse.cn.intermediate.values', 'browse.cn.intermediate.remove.duplicates'])
             featureConfig (dict): See Schema below.
@@ -483,24 +485,24 @@
 
         Raises:
             OkapiRequestError: Validation errors
             OkapiRequestUnprocessableEntity: Validation error for the request.
 
         Schema:
 
-            .. literalinclude:: ../files/Search_updateFeatureConfiguration_request.schema
+            .. literalinclude:: ../files/Search_updatefeatureconfiguration_request.schema
         """
-        return self.call("PUT", "/search/config/features/{featureId}", featureId, featureConfig)
+        return self.call("PUT", f"/search/config/features/{featureId}", featureConfig)
 
 		
-    def deleteFeatureConfigurationById(self, featureId):
+    def deletefeatureconfigurationbyid(self, featureId):
         """Delete feature configuration by id
 
         ``DELETE /search/config/features/{featureId}``
 
         Args:
             featureId (str): Feature id (name) (enum: ['search.all.fields', 'browse.cn.intermediate.values', 'browse.cn.intermediate.remove.duplicates'])
 
         Raises:
             OkapiRequestNotFound: No feature configuration is found by id
         """
-        return self.call("DELETE", "/search/config/features/{featureId}", featureId)
+        return self.call("DELETE", f"/search/config/features/{featureId}")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/sender.py` & `foliolib-0.3.5a1/foliolib/folio/api/sender.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.sender")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/settings.py` & `foliolib-0.3.5a1/foliolib/folio/api/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.settings")
 
 
 
-class SettingsAdmin(FolioAdminApi):
+class Settings(FolioApi):
     """Settings
-    Administration
 
     
     """
 
-    def getSettings(self):
+    def getsettings(self):
         """Get settings with optional CQL query. If X-Okapi-Permissions includes settings.global.read then settings without a userId are returned. If X-Okapi-Permissions includes settings.users.read then settings with a userId are returned. If X-Okapi-Permissions includes settings.owner.read then settings with userId = current-user are returned.
 
 
         ``GET /settings/entries``
 
         Returns:
             dict: See Schema below.
@@ -28,20 +27,20 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_getSettings_response.schema
+            .. literalinclude:: ../files/Settings_getsettings_response.schema
         """
         return self.call("GET", "/settings/entries")
 
 		
-    def postSetting(self, entry):
+    def postsetting(self, entry):
         """Create setting entry. If X-Okapi-Permissions includes settings.global.write, then a setting without a userId may be created. If X-Okapi-Permissions includes settings.users.write, then a setting with a userId may be created. If X-Okapi-Permissions includes settings.owner.write, then a setting with userId = current-user may be created.
 
 
         ``POST /settings/entries``
 
         Args:
             entry (dict): See Schema below.
@@ -50,19 +49,19 @@
             OkapiRequestError: Bad request
             OkapiRequestForbidden: Forbidden
             OkapiRequestPayloadToLarge: Payload Too Large
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_postSetting_request.schema
+            .. literalinclude:: ../files/Settings_postsetting_request.schema
         """
-        return self.call("POST", "/settings/entries", entry)
+        return self.call("POST", f"/settings/entries", entry)
 
-    def getSetting(self):
+    def getsetting(self, id_):
         """Get setting. If X-Okapi-Permissions includes settings.global.read, then a setting without a userId may be retrieved. If X-Okapi-Permissions includes settings.users.read, then a setting with a userId may be retrieved. If X-Okapi-Permissions includes settings.owner.read, then a setting with userId = current-user may be retrieved.
 
 
         ``GET /settings/entries/{id}``
 
         Returns:
             dict: See Schema below.
@@ -71,20 +70,20 @@
             OkapiRequestError: Bad request
             OkapiRequestForbidden: Forbidden
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_getSetting_response.schema
+            .. literalinclude:: ../files/Settings_getsetting_response.schema
         """
-        return self.call("GET", "/settings/entries/{id}")
+        return self.call("GET", f"/settings/entries/{id_}")
 
 		
-    def putSetting(self, entry):
+    def putsetting(self, entry, id_):
         """Update setting. If X-Okapi-Permissions includes settings.global.write, then a setting without a userId may be updated. If X-Okapi-Permissions includes settings.users.write, then a setting with a userId may be updated. If X-Okapi-Permissions includes settings.owner.write, then a setting with userId = current-user may be updated.
 
 
         ``PUT /settings/entries/{id}``
 
         Args:
             entry (dict): See Schema below.
@@ -94,33 +93,33 @@
             OkapiRequestForbidden: Forbidden
             OkapiRequestNotFound: Not Found
             OkapiRequestPayloadToLarge: Payload Too Large
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_putSetting_request.schema
+            .. literalinclude:: ../files/Settings_putsetting_request.schema
         """
-        return self.call("PUT", "/settings/entries/{id}", entry)
+        return self.call("PUT", f"/settings/entries/{id_}", entry)
 
 		
-    def deleteSetting(self):
+    def deletesetting(self, id_):
         """Delete setting. If X-Okapi-Permissions includes settings.global.write, then a setting without a userId may be deleted. If X-Okapi-Permissions includes settings.users.write, then a setting with a userId may be deleted. If X-Okapi-Permissions includes settings.owner.write, then a setting with userId = current-user may be deleted.
 
 
         ``DELETE /settings/entries/{id}``
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
         """
-        return self.call("DELETE", "/settings/entries/{id}")
+        return self.call("DELETE", f"/settings/entries/{id_}")
 
-    def uploadSettings(self, uploadRequest):
+    def uploadsettings(self, uploadRequest):
         """Upload settings. The entries are inserted or updated depending on whether key, scope, userId already. Each entry gets a unique identifier assigned if it's a new setting. The id must not be supplied. If X-Okapi-Permissions includes settings.global.write, then a setting without a userId may be created/updated. If X-Okapi-Permissions includes settings.users.write, then a setting with a userId may be created/updated. If X-Okapi-Permissions includes settings.owner.write, then a setting with userId = current-user may be created/updated.
 
 
         ``PUT /settings/upload``
 
         Args:
             uploadRequest (dict): See Schema below.
@@ -131,11 +130,11 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestForbidden: Forbidden
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Settings_uploadSettings_request.schema
-            .. literalinclude:: ../files/Settings_uploadSettings_request.schema_response.schema
+            .. literalinclude:: ../files/Settings_uploadsettings_request.schema
+            .. literalinclude:: ../files/Settings_uploadsettings_request.schema_response.schema
         """
-        return self.call("PUT", "/settings/upload", uploadRequest)
+        return self.call("PUT", f"/settings/upload", uploadRequest)
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/sharedIndex.py` & `foliolib-0.3.5a1/foliolib/folio/api/sharedIndex.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("foliolib.folio.api.sharedIndex")
 
 
 
-class SharedindexAdmin(FolioAdminApi):
+class Sharedindex(FolioApi):
     """Shared Index
-    Administration
 
     
     """
 
-    def postConfigMatchKey(self, matchKey):
+    def postconfigmatchkey(self, matchKey):
         """Create match key
 
         ``POST /shared-index/config/matchkeys``
 
         Args:
             matchKey (dict): See Schema below.
 
@@ -29,20 +28,20 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Sharedindex_postConfigMatchKey_request.schema
+            .. literalinclude:: ../files/Sharedindex_postconfigmatchkey_request.schema
         """
-        return self.call("POST", "/shared-index/config/matchkeys", matchKey)
+        return self.call("POST", f"/shared-index/config/matchkeys", matchKey)
 
 		
-    def getConfigMatchKeys(self, **kwargs):
+    def getconfigmatchkeys(self, **kwargs):
         """Get match key configurations
 
         ``GET /shared-index/config/matchkeys``
 
         Keyword Args:
             limit (int): Limit the number of elements returned in the response (default: 10, minimum: 0)
             query (str): CQL query
@@ -53,90 +52,90 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Sharedindex_getConfigMatchKeys_response.schema
+            .. literalinclude:: ../files/Sharedindex_getconfigmatchkeys_response.schema
         """
         return self.call("GET", "/shared-index/config/matchkeys", query=kwargs)
 
-    def getConfigMatchKey(self):
+    def getconfigmatchkey(self, id_):
         """Get match key configuration
 
         ``GET /shared-index/config/matchkeys/{id}``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Sharedindex_getConfigMatchKey_response.schema
+            .. literalinclude:: ../files/Sharedindex_getconfigmatchkey_response.schema
         """
-        return self.call("GET", "/shared-index/config/matchkeys/{id}")
+        return self.call("GET", f"/shared-index/config/matchkeys/{id_}")
 
 		
-    def putConfigMatchKey(self, matchKey):
+    def putconfigmatchkey(self, matchKey, id_):
         """Update match key configuration.
 
         ``PUT /shared-index/config/matchkeys/{id}``
 
         Args:
             matchKey (dict): See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Sharedindex_putConfigMatchKey_request.schema
+            .. literalinclude:: ../files/Sharedindex_putconfigmatchkey_request.schema
         """
-        return self.call("PUT", "/shared-index/config/matchkeys/{id}", matchKey)
+        return self.call("PUT", f"/shared-index/config/matchkeys/{id_}", matchKey)
 
 		
-    def deleteConfigMatchKey(self):
+    def deleteconfigmatchkey(self, id_):
         """Delete match key configuration
 
         ``DELETE /shared-index/config/matchkeys/{id}``
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
         """
-        return self.call("DELETE", "/shared-index/config/matchkeys/{id}")
+        return self.call("DELETE", f"/shared-index/config/matchkeys/{id_}")
 
-    def initializeMatchKey(self):
+    def initializematchkey(self, id_):
         """Recalculate match key across all records.
 
         ``PUT /shared-index/config/matchkeys/{id}/initialize``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Sharedindex_initializeMatchKey_response.schema
+            .. literalinclude:: ../files/Sharedindex_initializematchkey_response.schema
         """
-        return self.call("PUT", "/shared-index/config/matchkeys/{id}/initialize")
+        return self.call("PUT", f"/shared-index/config/matchkeys/{id_}/initialize")
 
-    def postSource(self, source):
+    def postsource(self, source):
         """Create source.
 
         ``POST /shared-index/sources``
 
         Args:
             source (dict): See Schema below.
 
@@ -145,20 +144,20 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Sharedindex_postSource_request.schema
+            .. literalinclude:: ../files/Sharedindex_postsource_request.schema
         """
-        return self.call("POST", "/shared-index/sources", source)
+        return self.call("POST", f"/shared-index/sources", source)
 
 		
-    def getSources(self, **kwargs):
+    def getsources(self, **kwargs):
         """Get sources.
 
         ``GET /shared-index/sources``
 
         Keyword Args:
             limit (int): Limit the number of elements returned in the response (default: 10, minimum: 0)
             query (str): CQL query
@@ -169,51 +168,51 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Sharedindex_getSources_response.schema
+            .. literalinclude:: ../files/Sharedindex_getsources_response.schema
         """
         return self.call("GET", "/shared-index/sources", query=kwargs)
 
-    def getSource(self):
+    def getsource(self, id_):
         """Get source.
 
         ``GET /shared-index/config/sources/{id}``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Sharedindex_getSource_response.schema
+            .. literalinclude:: ../files/Sharedindex_getsource_response.schema
         """
-        return self.call("GET", "/shared-index/config/sources/{id}")
+        return self.call("GET", f"/shared-index/config/sources/{id_}")
 
 		
-    def deleteSource(self):
+    def deletesource(self, id_):
         """Delete source.
 
         ``DELETE /shared-index/config/sources/{id}``
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
         """
-        return self.call("DELETE", "/shared-index/config/sources/{id}")
+        return self.call("DELETE", f"/shared-index/config/sources/{id_}")
 
-    def postIngestJob(self, ingestJobRequest):
+    def postingestjob(self, ingestJobRequest):
         """Create ingest job
 
         ``POST /shared-index/shared-index/ingest-jobs``
 
         Args:
             ingestJobRequest (dict): See Schema below.
 
@@ -222,19 +221,19 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Sharedindex_postIngestJob_request.schema
+            .. literalinclude:: ../files/Sharedindex_postingestjob_request.schema
         """
-        return self.call("POST", "/shared-index/shared-index/ingest-jobs", ingestJobRequest)
+        return self.call("POST", f"/shared-index/shared-index/ingest-jobs", ingestJobRequest)
 
-    def ingestJobRecord(self, ingestRecordChunk):
+    def ingestjobrecord(self, ingestRecordChunk, id_):
         """Put records for job.
 
         ``PUT /shared-index/shared-index/ingest-jobs/{id}``
 
         Args:
             ingestRecordChunk (dict): See Schema below.
 
@@ -244,75 +243,75 @@
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Sharedindex_ingestJobRecord_request.schema
-            .. literalinclude:: ../files/Sharedindex_ingestJobRecord_request.schema_response.schema
+            .. literalinclude:: ../files/Sharedindex_ingestjobrecord_request.schema
+            .. literalinclude:: ../files/Sharedindex_ingestjobrecord_request.schema_response.schema
         """
-        return self.call("PUT", "/shared-index/shared-index/ingest-jobs/{id}", ingestRecordChunk)
+        return self.call("PUT", f"/shared-index/shared-index/ingest-jobs/{id_}", ingestRecordChunk)
 
 		
-    def ingestJobInfo(self):
+    def ingestjobinfo(self, id_):
         """Get ingest job information.
 
         ``GET /shared-index/shared-index/ingest-jobs/{id}``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Sharedindex_ingestJobInfo_response.schema
+            .. literalinclude:: ../files/Sharedindex_ingestjobinfo_response.schema
         """
-        return self.call("GET", "/shared-index/shared-index/ingest-jobs/{id}")
+        return self.call("GET", f"/shared-index/shared-index/ingest-jobs/{id_}")
 
 		
-    def ingestJobFinish(self, **kwargs):
+    def ingestjobfinish(self, id_, **kwargs):
         """Finish ingest job with either rollback of commit.
 
         ``DELETE /shared-index/shared-index/ingest-jobs/{id}``
 
         Keyword Args:
             commit (bool): whether to commit (default: False)
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
         """
-        return self.call("DELETE", "/shared-index/shared-index/ingest-jobs/{id}", query=kwargs)
+        return self.call("DELETE", f"/shared-index/shared-index/ingest-jobs/{id_}", query=kwargs)
 
-    def getGlobalRecords(self):
+    def getglobalrecords(self):
         """Get records that satisfy CQL query with fields localId, sourceId, globalId.
 
         ``GET /shared-index/records``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Sharedindex_getGlobalRecords_response.schema
+            .. literalinclude:: ../files/Sharedindex_getglobalrecords_response.schema
         """
         return self.call("GET", "/shared-index/records")
 
 		
-    def putGlobalRecords(self, ingestRecordRequest):
+    def putglobalrecords(self, ingestRecordRequest):
         """Create or update records.
 
         ``PUT /shared-index/records``
 
         Args:
             ingestRecordRequest (dict): See Schema below.
 
@@ -321,89 +320,89 @@
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Sharedindex_putGlobalRecords_request.schema
-            .. literalinclude:: ../files/Sharedindex_putGlobalRecords_request.schema_response.schema
+            .. literalinclude:: ../files/Sharedindex_putglobalrecords_request.schema
+            .. literalinclude:: ../files/Sharedindex_putglobalrecords_request.schema_response.schema
         """
-        return self.call("PUT", "/shared-index/records", ingestRecordRequest)
+        return self.call("PUT", f"/shared-index/records", ingestRecordRequest)
 
 		
-    def deleteGlobalRecords(self):
+    def deleteglobalrecords(self):
         """Delete global records.
 
         ``DELETE /shared-index/records``
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
         """
         return self.call("DELETE", "/shared-index/records")
 
-    def getGlobalRecord(self):
+    def getglobalrecord(self, globalId):
         """Get record with global identifier.
 
         ``GET /shared-index/records/{globalId}``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Sharedindex_getGlobalRecord_response.schema
+            .. literalinclude:: ../files/Sharedindex_getglobalrecord_response.schema
         """
-        return self.call("GET", "/shared-index/records/{globalId}")
+        return self.call("GET", f"/shared-index/records/{globalId}")
 
-    def getClusters(self):
+    def getclusters(self):
         """Get clusters with matchkeyid. CQL query with matchValue, clusterId fields
 
         ``GET /shared-index/clusters``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Sharedindex_getClusters_response.schema
+            .. literalinclude:: ../files/Sharedindex_getclusters_response.schema
         """
         return self.call("GET", "/shared-index/clusters")
 
-    def getCluster(self):
+    def getcluster(self, clusterId):
         """Get cluster by identifier
 
         ``GET /shared-index/clusters/{clusterId}``
 
         Returns:
             dict: See Schema below.
 
         Raises:
             OkapiRequestError: Bad request
             OkapiRequestNotFound: Not Found
             OkapiFatalError: Internal error
 
         Schema:
 
-            .. literalinclude:: ../files/Sharedindex_getCluster_response.schema
+            .. literalinclude:: ../files/Sharedindex_getcluster_response.schema
         """
-        return self.call("GET", "/shared-index/clusters/{clusterId}")
+        return self.call("GET", f"/shared-index/clusters/{clusterId}")
 
-    def oaiService(self):
+    def oaiservice(self):
         """OAI service
 
         ``GET /shared-index/oai``
 
         Raises:
             OkapiRequestError: Bad request
             OkapiFatalError: Internal error
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/sourceRecordManager.py` & `foliolib-0.3.5a1/foliolib/folio/api/sourceRecordManager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.sourceRecordManager")
 
@@ -146,14 +146,15 @@
         Args:
             jobExecutionsId (str)
             jobExecution (dict): See Schema below
 
         Raises:
             OkapiRequestNotFound: Not Found
             OkapiRequestError: Bad Request
+            OkapiRequestConflict: Conflict
             OkapiFatalError: Server Error
             OkapiRequestUnprocessableEntity: Unprocessable Entity
 
         Schema:
 
             .. literalinclude:: ../files/ChangeManager_modify_jobExecution_request.schema
         """
@@ -170,14 +171,19 @@
 
         Keyword Args:
             limit (int): (default=10) Limit the number of elements returned in the response
                     
                     Example:
                     
                      - 10
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
 
         Returns:
@@ -388,14 +394,19 @@
             completedAfter (datetime):  Start date to filter after, inclusive
             completedBefore (datetime):  End date to filter before, inclusive
             sortBy (list): (default=['completed_date,asc']) Sorting jobExecutions by field: completed_date, progress_total, file_name, status, job_profile_name, hrid, job_user_first_name, job_user_last_name
                     
                     Example:
                     
                      - ['completed_date,asc']
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -475,14 +486,19 @@
                     
                      - True
             entityType (str (MARC|INSTANCE|HOLDINGS|AUTHORITY|ITEM|ORDER|INVOICE|ALL):): (default=ALL) Filter by entity type: MARC, INSTANCE, HOLDINGS, AUTHORITY, ITEM, ORDER, INVOICE
                     
                     Example:
                     
                      - MARC
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -549,14 +565,19 @@
 
         ``GET /metadata-provider/jobExecutions/jobProfiles``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -581,14 +602,19 @@
 
         ``GET /metadata-provider/jobExecutions/users``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/sourceRecordStorage.py` & `foliolib-0.3.5a1/foliolib/folio/api/sourceRecordStorage.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.sourceRecordStorage")
 
@@ -86,14 +86,19 @@
             updatedAfter (datetime):  Start date to filter after, inclusive
             updatedBefore (datetime):  End date to filter before, inclusive
             orderBy (list):  Sort records
                     
                     Example:
                     
                      - ['order,ASC']
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -265,14 +270,38 @@
         Schema:
 
             .. literalinclude:: ../files/SourceRecordStorageBatch_modify_parsedRecord_request.schema
             .. literalinclude:: ../files/SourceRecordStorageBatch_modify_parsedRecord_return.schema 
         """
         return self.call("PUT", "/source-storage/batch/parsed-records", data=parsedRecord)
 
+    def set_fetch(self, fetch: dict):
+        """Fetch exact fields of parsed records by external IDs.
+
+        ``POST /source-storage/batch/parsed-records/fetch``
+
+        Args:
+            fetch (dict): See Schema below
+
+        Returns:
+            dict: See Schema below
+
+        Raises:
+            OkapiRequestError: Bad Request
+            OkapiRequestUnprocessableEntity: Unprocessable Entity
+            OkapiFatalError: Server Error
+            OkapiRequestUnprocessableEntity: Unprocessable Entity
+
+        Schema:
+
+            .. literalinclude:: ../files/SourceRecordStorageBatch_set_fetch_request.schema
+            .. literalinclude:: ../files/SourceRecordStorageBatch_set_fetch_return.schema 
+        """
+        return self.call("POST", "/source-storage/batch/parsed-records/fetch", data=fetch)
+
 
 class SourceRecordStorageTestRecords(FolioApi):
     """Source Record Storage Test Record API
 
     API for managing test records
     """
 
@@ -328,14 +357,19 @@
                     
                      - ACTUAL
             orderBy (list):  Sort Records
                     
                     Example:
                     
                      - ['order,ASC']
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -420,14 +454,19 @@
             updatedAfter (datetime):  Start date to filter after, inclusive
             updatedBefore (datetime):  End date to filter before, inclusive
             orderBy (list):  Sort records
                     
                     Example:
                     
                      - ['order,ASC']
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -471,14 +510,19 @@
 
         ``GET /source-storage/records``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -568,14 +612,15 @@
         Args:
             recordsId (str)
             record (dict): See Schema below
 
         Raises:
             OkapiRequestNotFound: Not Found
             OkapiRequestError: Bad Request
+            OkapiRequestConflict: Conflict
             OkapiFatalError: Server Error
             OkapiRequestUnprocessableEntity: Unprocessable Entity
 
         Schema:
 
             .. literalinclude:: ../files/SourceRecordStorageRecords_modify_record_request.schema
         """
@@ -651,14 +696,19 @@
 
         ``GET /source-storage/snapshots``
 
         Args:
             **kwargs (properties): Keyword Arguments
 
         Keyword Args:
+            totalRecords (str): (default=auto) How to calculate the totalRecords property. "exact" for the correct number, "estimated" for an estimation, "auto" to automatically select "exact" or "estimated", "none" for suppressing the totalRecords property. For details see https://github.com/folio-org/raml-module-builder#estimated-totalrecords
+                    
+                    Example:
+                    
+                     - none
             offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
                     
                     Example:
                     
                      - 0
             limit (int): (default=10) Limit the number of elements returned in the response
                     
@@ -748,14 +798,15 @@
         Args:
             jobExecutionId (str)
             snapshot (dict): See Schema below
 
         Raises:
             OkapiRequestNotFound: Not Found
             OkapiRequestError: Bad Request
+            OkapiRequestConflict: Conflict
             OkapiFatalError: Server Error
             OkapiRequestUnprocessableEntity: Unprocessable Entity
 
         Schema:
 
             .. literalinclude:: ../files/SourceRecordStorageSnapshots_modify_snapshot_request.schema
         """
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/templateEngine.py` & `foliolib-0.3.5a1/foliolib/folio/api/templateEngine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.templateEngine")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/userImport.py` & `foliolib-0.3.5a1/foliolib/folio/api/userImport.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.userImport")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/users.py` & `foliolib-0.3.5a1/foliolib/folio/api/users.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.users")
 
@@ -703,14 +703,56 @@
         Schema:
 
             .. literalinclude:: ../files/Groups_modify_group_request.schema
         """
         return self.call("PUT", f"/groups/{groupId}", data=group)
 
 
+class UserTenants(FolioApi):
+    """mod-users User tenants API
+
+    Records that show the primary tenant for a user when doing single-sign-on
+    """
+
+    def get_userTenants(self, **kwargs):
+        """Return a list of user tenants
+
+        ``GET /user-tenants``
+
+        Args:
+            **kwargs (properties): Keyword Arguments
+
+        Keyword Args:
+            offset (int): (default=0) Skip over a number of elements by specifying an offset value for the query
+                    
+                    Example:
+                    
+                     - 0
+            limit (int): (default=10) Limit the number of elements returned in the response
+                    
+                    Example:
+                    
+                     - 10
+
+        Returns:
+            dict: See Schema below
+
+        Raises:
+            OkapiRequestError: Bad Request
+            OkapiRequestUnauthorized: Authentication is required
+            OkapiRequestNotFound: Not Found
+            OkapiFatalError: Server Error
+
+        Schema:
+
+            .. literalinclude:: ../files/UserTenants_get_userTenants_return.schema 
+        """
+        return self.call("GET", "/user-tenants", query=kwargs)
+
+
 class Patronpin(FolioApi):
     """patron-pins API
 
     This documents the API calls that can be made to set and verify patron pins
     """
 
     def set_patronPin(self, patronPin: dict):
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/api/usersBl.py` & `foliolib-0.3.5a1/foliolib/folio/api/usersBl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Generated at 2023-04-16
+# Generated at 2023-05-20
 
 import logging
 
 from foliolib.folio import FolioApi, FolioAdminApi
 
 log = logging.getLogger("oliolib.folio.api.usersBl")
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/config.py` & `foliolib-0.3.5a1/foliolib/folio/config.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib/folio/dataImport.py` & `foliolib-0.3.5a1/foliolib/folio/dataImport.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib/folio/inventory.py` & `foliolib-0.3.5a1/foliolib/folio/inventory.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib/folio/inventoryReferenceData.py` & `foliolib-0.3.5a1/foliolib/folio/inventoryReferenceData.py`

 * *Files 1% similar despite different names*

```diff
@@ -463,16 +463,22 @@
             add = getattr(self, "set_%s" %
                           singularize(baseMethodName))
             fullpath = os.path.join(path, refpath)
             if os.path.exists(fullpath):
                 for fname in os.listdir(fullpath):
                     if fname.endswith((".json")):
                         fpath = os.path.join(fullpath, fname)
-                        with open(fpath, encoding="utf-8") as f:
-                            data = json.load(f)
+                        log.info("Load json %s", fpath)
+                        try:
+                            with open(fpath, encoding="utf-8") as f:
+                                data = json.load(f)
+                        except:
+                            with open(fpath, encoding="utf-8") as f:
+                                log.error("Json error:\n%s", f.read())
+                            raise
                         add(data, replace)
                         count += 1
         log.info("%i files processed", count)
         return count
 
     def dump_reference_data(self, path):
         for refpath in DIRS:
```

### Comparing `foliolib-0.3.4a1/foliolib/folio/users.py` & `foliolib-0.3.5a1/foliolib/folio/users.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,19 +13,14 @@
 from foliolib.okapi.exceptions import OkapiRequestNotFound
 
 log = logging.getLogger("foliolib.folio.users")
 
 
 class Users(FolioService):
     """
-    Requirements:
-
-        - mod-login
-        - mod-users
-        - mod-inventory-storage
     """
 
     def __init__(self, tenant: str) -> None:
         """
         Args:
             tenant (str): Tenant id
         """
```

### Comparing `foliolib-0.3.4a1/foliolib/helper/__init__.py` & `foliolib-0.3.5a1/foliolib/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib/helper/database.py` & `foliolib-0.3.5a1/foliolib/helper/database.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib/helper/folio.py` & `foliolib-0.3.5a1/foliolib/helper/folio.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib/helper/modules.py` & `foliolib-0.3.5a1/foliolib/helper/modules.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib/helper/okapi.py` & `foliolib-0.3.5a1/foliolib/helper/okapi.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib/helper/platform.py` & `foliolib-0.3.5a1/foliolib/helper/platform.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib/helper/tenant.py` & `foliolib-0.3.5a1/foliolib/helper/tenant.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib/okapi/__init__.py` & `foliolib-0.3.5a1/foliolib/okapi/__init__.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib/okapi/exceptions.py` & `foliolib-0.3.5a1/foliolib/okapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib/okapi/kubeClient.py` & `foliolib-0.3.5a1/foliolib/okapi/kubeClient.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib/okapi/misc.py` & `foliolib-0.3.5a1/foliolib/okapi/misc.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib/okapi/okapiClient.py` & `foliolib-0.3.5a1/foliolib/okapi/okapiClient.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib/okapi/okapiModule.py` & `foliolib-0.3.5a1/foliolib/okapi/okapiModule.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib/okapi/okapiModuleKubernetes.py` & `foliolib-0.3.5a1/foliolib/okapi/okapiModuleKubernetes.py`

 * *Files identical despite different names*

### Comparing `foliolib-0.3.4a1/foliolib.egg-info/PKG-INFO` & `foliolib-0.3.5a1/foliolib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foliolib
-Version: 0.3.4a1
+Version: 0.3.5a1
 Summary: Okapi/Folio Manager and Library
 Home-page: https://github.com/tobi-weber/foliolib
 Author: Tobias Weber
 Author-email: tobi-weber@gmx.de
 License: GPL-3.0 License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `foliolib-0.3.4a1/foliolib.egg-info/SOURCES.txt` & `foliolib-0.3.5a1/foliolib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,37 +34,45 @@
 foliolib/folio/dataImport.py
 foliolib/folio/exceptions.py
 foliolib/folio/inventory.py
 foliolib/folio/inventoryReferenceData.py
 foliolib/folio/users.py
 foliolib/folio/api/__init__.py
 foliolib/folio/api/audit.py
+foliolib/folio/api/authtoken.py
 foliolib/folio/api/bulkOperations.py
 foliolib/folio/api/calendar.py
 foliolib/folio/api/circulation.py
 foliolib/folio/api/circulationStorage.py
 foliolib/folio/api/configuration.py
+foliolib/folio/api/consortia.py
 foliolib/folio/api/copycat.py
 foliolib/folio/api/courses.py
 foliolib/folio/api/dataExport.py
 foliolib/folio/api/dataExportSpring.py
 foliolib/folio/api/dataExportWorker.py
 foliolib/folio/api/dataImport.py
 foliolib/folio/api/dataImportConverterStorage.py
+foliolib/folio/api/diConverterStorage.py
 foliolib/folio/api/ebsconet.py
 foliolib/folio/api/email.py
 foliolib/folio/api/entitiesLinks.py
 foliolib/folio/api/ermUsage.py
 foliolib/folio/api/ermUsageHarvester.py
+foliolib/folio/api/eusageReports.py
 foliolib/folio/api/eventConfig.py
 foliolib/folio/api/feesfines.py
 foliolib/folio/api/finance.py
 foliolib/folio/api/financeStorage.py
 foliolib/folio/api/fincConfig.py
+foliolib/folio/api/folioCustomFields.py
+foliolib/folio/api/folioSpringBase.py
+foliolib/folio/api/folioVertxLib.py
 foliolib/folio/api/gobi.py
+foliolib/folio/api/idmConnect.py
 foliolib/folio/api/innReach.py
 foliolib/folio/api/inventory.py
 foliolib/folio/api/inventoryStorage.py
 foliolib/folio/api/inventoryUpdate.py
 foliolib/folio/api/invoice.py
 foliolib/folio/api/invoiceStorage.py
 foliolib/folio/api/kbEbscoJava.py
```

### Comparing `foliolib-0.3.4a1/setup.cfg` & `foliolib-0.3.5a1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -41,13 +41,12 @@
 	kubernetes>=22.6.0
 setup_requires = 
 	setuptools
 
 [options.entry_points]
 console_scripts = 
 	foliolib = foliolib.cli:cli
-	foliolibapi = foliolib.apiBuilder.cli:cli
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

