# Comparing `tmp/uuyoupinapi-0.1.1.tar.gz` & `tmp/uuyoupinapi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uuyoupinapi-0.1.1.tar", last modified: Sat May 20 12:55:08 2023, max compression
+gzip compressed data, was "uuyoupinapi-0.1.2.tar", last modified: Sat May 20 13:02:39 2023, max compression
```

## Comparing `uuyoupinapi-0.1.1.tar` & `uuyoupinapi-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 12:55:08.975443 uuyoupinapi-0.1.1/
--rw-rw-rw-   0        0        0    35823 2023-04-22 06:02:59.000000 uuyoupinapi-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      432 2023-05-20 12:55:08.974442 uuyoupinapi-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       75 2023-05-13 15:05:54.000000 uuyoupinapi-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-20 12:55:08.975443 uuyoupinapi-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      475 2023-05-20 12:54:38.000000 uuyoupinapi-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-20 12:55:08.968443 uuyoupinapi-0.1.1/uuyoupinapi/
--rw-rw-rw-   0        0        0     5391 2023-05-20 12:54:02.000000 uuyoupinapi-0.1.1/uuyoupinapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 12:55:08.973442 uuyoupinapi-0.1.1/uuyoupinapi.egg-info/
--rw-rw-rw-   0        0        0      432 2023-05-20 12:55:08.000000 uuyoupinapi-0.1.1/uuyoupinapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-05-20 12:55:08.000000 uuyoupinapi-0.1.1/uuyoupinapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 12:55:08.000000 uuyoupinapi-0.1.1/uuyoupinapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-20 12:55:08.000000 uuyoupinapi-0.1.1/uuyoupinapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 13:02:39.296328 uuyoupinapi-0.1.2/
+-rw-rw-rw-   0        0        0    35823 2023-04-22 06:02:59.000000 uuyoupinapi-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      432 2023-05-20 13:02:39.296328 uuyoupinapi-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       75 2023-05-13 15:05:54.000000 uuyoupinapi-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-20 13:02:39.296328 uuyoupinapi-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      475 2023-05-20 13:01:45.000000 uuyoupinapi-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 13:02:39.290332 uuyoupinapi-0.1.2/uuyoupinapi/
+-rw-rw-rw-   0        0        0     5391 2023-05-20 13:01:53.000000 uuyoupinapi-0.1.2/uuyoupinapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 13:02:39.295327 uuyoupinapi-0.1.2/uuyoupinapi.egg-info/
+-rw-rw-rw-   0        0        0      432 2023-05-20 13:02:39.000000 uuyoupinapi-0.1.2/uuyoupinapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-05-20 13:02:39.000000 uuyoupinapi-0.1.2/uuyoupinapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 13:02:39.000000 uuyoupinapi-0.1.2/uuyoupinapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-20 13:02:39.000000 uuyoupinapi-0.1.2/uuyoupinapi.egg-info/top_level.txt
```

### Comparing `uuyoupinapi-0.1.1/LICENSE` & `uuyoupinapi-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `uuyoupinapi-0.1.1/uuyoupinapi/__init__.py` & `uuyoupinapi-0.1.2/uuyoupinapi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,11 +117,11 @@
             "orderStatus": "140",
             "pageIndex": 1,
             "pageSize": 100
         }).json()['data']
         data_to_return = []
         for order in data['orderList']:
             data_to_return.append({
-                'order_id': order['tradeOfferId'],
+                'offer_id': order['tradeOfferId'],
                 'item_name': order['productDetail']['commodityName'],
             })
         return data_to_return
```

