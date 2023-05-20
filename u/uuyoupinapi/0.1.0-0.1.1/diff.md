# Comparing `tmp/uuyoupinapi-0.1.0.tar.gz` & `tmp/uuyoupinapi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uuyoupinapi-0.1.0.tar", last modified: Sun May 14 08:15:52 2023, max compression
+gzip compressed data, was "uuyoupinapi-0.1.1.tar", last modified: Sat May 20 12:55:08 2023, max compression
```

## Comparing `uuyoupinapi-0.1.0.tar` & `uuyoupinapi-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 08:15:52.774968 uuyoupinapi-0.1.0/
--rw-rw-rw-   0        0        0    35823 2023-04-22 06:02:59.000000 uuyoupinapi-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      432 2023-05-14 08:15:52.774968 uuyoupinapi-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       75 2023-05-13 15:05:54.000000 uuyoupinapi-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-14 08:15:52.774968 uuyoupinapi-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      475 2023-05-14 08:15:35.000000 uuyoupinapi-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-14 08:15:52.768968 uuyoupinapi-0.1.0/uuyoupinapi/
--rw-rw-rw-   0        0        0     5242 2023-05-14 08:15:13.000000 uuyoupinapi-0.1.0/uuyoupinapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 08:15:52.773968 uuyoupinapi-0.1.0/uuyoupinapi.egg-info/
--rw-rw-rw-   0        0        0      432 2023-05-14 08:15:52.000000 uuyoupinapi-0.1.0/uuyoupinapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-05-14 08:15:52.000000 uuyoupinapi-0.1.0/uuyoupinapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 08:15:52.000000 uuyoupinapi-0.1.0/uuyoupinapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-14 08:15:52.000000 uuyoupinapi-0.1.0/uuyoupinapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 12:55:08.975443 uuyoupinapi-0.1.1/
+-rw-rw-rw-   0        0        0    35823 2023-04-22 06:02:59.000000 uuyoupinapi-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      432 2023-05-20 12:55:08.974442 uuyoupinapi-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       75 2023-05-13 15:05:54.000000 uuyoupinapi-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-20 12:55:08.975443 uuyoupinapi-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      475 2023-05-20 12:54:38.000000 uuyoupinapi-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 12:55:08.968443 uuyoupinapi-0.1.1/uuyoupinapi/
+-rw-rw-rw-   0        0        0     5391 2023-05-20 12:54:02.000000 uuyoupinapi-0.1.1/uuyoupinapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 12:55:08.973442 uuyoupinapi-0.1.1/uuyoupinapi.egg-info/
+-rw-rw-rw-   0        0        0      432 2023-05-20 12:55:08.000000 uuyoupinapi-0.1.1/uuyoupinapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-05-20 12:55:08.000000 uuyoupinapi-0.1.1/uuyoupinapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 12:55:08.000000 uuyoupinapi-0.1.1/uuyoupinapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-20 12:55:08.000000 uuyoupinapi-0.1.1/uuyoupinapi.egg-info/top_level.txt
```

### Comparing `uuyoupinapi-0.1.0/LICENSE` & `uuyoupinapi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uuyoupinapi-0.1.0/uuyoupinapi/__init__.py` & `uuyoupinapi-0.1.1/uuyoupinapi/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -85,41 +85,43 @@
         elif method == 'PUT':
             return self.session.put(url, data=data)
         elif method == 'DELETE':
             return self.session.delete(url)
         else:
             raise Exception('Method not supported')
 
-    def get_steam_offer_id_by_order_id(self, order_id):
-        """
-        通过订单号获取steam交易号
-        :param order_id: 订单号
-        :return: steam交易报价号
-        """
-        return self.call_api('GET', '/api/trade/Order/OrderPagedDetail', data={
-            'orderNo': order_id
-        }).json()['Data']['SteamOfferId']
-
     def get_wait_deliver_list(self, game_id=730, return_offer_id=True):
         """
         获取待发货列表（出售）
         :param return_offer_id: 默认为True，是否返回steam交易报价号
         :param game_id: 游戏ID，默认为730(CSGO)
         :return: 待发货列表，格式为[{'order_id': '订单号', 'item_name': '物品名称', 'offer_id': 'steam交易报价号'}... , ...]
         """
-        data = self.call_api('POST', '/api/youpin/bff/trade/sell/page/v1/waitDeliver/waitDeliverList', data={
-            "gameId": game_id,
+        # data = self.call_api('POST', '/api/youpin/bff/trade/sell/page/v1/waitDeliver/waitDeliverList', data={
+        #     "gameId": game_id,
+        #     "pageIndex": 1,
+        #     "pageSize": 1000
+        # })
+        # wait_deliver_list = data.json()['data']['waitDeliverList']
+        # data_to_return = []
+        # if wait_deliver_list is not None:
+        #     for item in wait_deliver_list:
+        #         if item['orderInfoVO']['orderType'] == 1:
+        #             dict_to_append = dict()
+        #             dict_to_append['order_id'] = item['orderInfoVO']['orderNo']
+        #             dict_to_append['item_name'] = item['commodityInfoVO']['commodityName']
+        #             if return_offer_id:
+        #                 dict_to_append['offer_id'] = self.get_steam_offer_id_by_order_id(dict_to_append['order_id'])
+        #             data_to_return.append(dict_to_append)
+        data = self.call_api('POST', '/api/youpin/bff/trade/sale/v1/sell/list', data={
+            "keys": "",
+            "orderStatus": "140",
             "pageIndex": 1,
-            "pageSize": 1000
-        })
-        wait_deliver_list = data.json()['data']['waitDeliverList']
+            "pageSize": 100
+        }).json()['data']
         data_to_return = []
-        if wait_deliver_list is not None:
-            for item in wait_deliver_list:
-                if item['orderInfoVO']['orderType'] == 1:
-                    dict_to_append = dict()
-                    dict_to_append['order_id'] = item['orderInfoVO']['orderNo']
-                    dict_to_append['item_name'] = item['commodityInfoVO']['commodityName']
-                    if return_offer_id:
-                        dict_to_append['offer_id'] = self.get_steam_offer_id_by_order_id(dict_to_append['order_id'])
-                    data_to_return.append(dict_to_append)
+        for order in data['orderList']:
+            data_to_return.append({
+                'order_id': order['tradeOfferId'],
+                'item_name': order['productDetail']['commodityName'],
+            })
         return data_to_return
```

