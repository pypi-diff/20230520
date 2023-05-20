# Comparing `tmp/paymobpy-1.0.2.tar.gz` & `tmp/paymobpy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paymobpy-1.0.2.tar", last modified: Sat May 20 16:51:06 2023, max compression
+gzip compressed data, was "paymobpy-1.0.3.tar", last modified: Sat May 20 17:11:54 2023, max compression
```

## Comparing `paymobpy-1.0.2.tar` & `paymobpy-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-20 16:51:06.565174 paymobpy-1.0.2/
--rw-r--r--   0 leondaz    (501) staff       (20)      193 2023-05-20 16:51:06.565052 paymobpy-1.0.2/PKG-INFO
--rw-r--r--   0 leondaz    (501) staff       (20)      777 2023-05-20 16:49:04.000000 paymobpy-1.0.2/README.md
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-20 16:51:06.564361 paymobpy-1.0.2/paymobpy/
--rw-r--r--   0 leondaz    (501) staff       (20)     2518 2023-05-20 16:49:46.000000 paymobpy-1.0.2/paymobpy/__init__.py
--rw-r--r--   0 leondaz    (501) staff       (20)      177 2023-05-20 14:43:04.000000 paymobpy-1.0.2/paymobpy/consts.py
--rw-r--r--   0 leondaz    (501) staff       (20)      281 2023-05-20 15:20:58.000000 paymobpy-1.0.2/paymobpy/exceptions.py
--rw-r--r--   0 leondaz    (501) staff       (20)      825 2023-05-20 15:26:08.000000 paymobpy-1.0.2/paymobpy/http_clients.py
--rw-r--r--   0 leondaz    (501) staff       (20)     2493 2023-05-20 16:19:48.000000 paymobpy-1.0.2/paymobpy/schemas.py
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-20 16:51:06.564915 paymobpy-1.0.2/paymobpy.egg-info/
--rw-r--r--   0 leondaz    (501) staff       (20)      193 2023-05-20 16:51:06.000000 paymobpy-1.0.2/paymobpy.egg-info/PKG-INFO
--rw-r--r--   0 leondaz    (501) staff       (20)      254 2023-05-20 16:51:06.000000 paymobpy-1.0.2/paymobpy.egg-info/SOURCES.txt
--rw-r--r--   0 leondaz    (501) staff       (20)        1 2023-05-20 16:51:06.000000 paymobpy-1.0.2/paymobpy.egg-info/dependency_links.txt
--rw-r--r--   0 leondaz    (501) staff       (20)        9 2023-05-20 16:51:06.000000 paymobpy-1.0.2/paymobpy.egg-info/top_level.txt
--rw-r--r--   0 leondaz    (501) staff       (20)       38 2023-05-20 16:51:06.565212 paymobpy-1.0.2/setup.cfg
--rw-r--r--   0 leondaz    (501) staff       (20)      275 2023-05-20 16:50:50.000000 paymobpy-1.0.2/setup.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-20 17:11:54.296650 paymobpy-1.0.3/
+-rw-r--r--   0 leondaz    (501) staff       (20)      193 2023-05-20 17:11:54.296537 paymobpy-1.0.3/PKG-INFO
+-rw-r--r--   0 leondaz    (501) staff       (20)      789 2023-05-20 17:11:18.000000 paymobpy-1.0.3/README.md
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-20 17:11:54.295949 paymobpy-1.0.3/paymobpy/
+-rw-r--r--   0 leondaz    (501) staff       (20)     2530 2023-05-20 17:11:18.000000 paymobpy-1.0.3/paymobpy/__init__.py
+-rw-r--r--   0 leondaz    (501) staff       (20)      177 2023-05-20 14:43:04.000000 paymobpy-1.0.3/paymobpy/consts.py
+-rw-r--r--   0 leondaz    (501) staff       (20)      281 2023-05-20 15:20:58.000000 paymobpy-1.0.3/paymobpy/exceptions.py
+-rw-r--r--   0 leondaz    (501) staff       (20)      825 2023-05-20 15:26:08.000000 paymobpy-1.0.3/paymobpy/http_clients.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     2493 2023-05-20 16:19:48.000000 paymobpy-1.0.3/paymobpy/schemas.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-20 17:11:54.296387 paymobpy-1.0.3/paymobpy.egg-info/
+-rw-r--r--   0 leondaz    (501) staff       (20)      193 2023-05-20 17:11:54.000000 paymobpy-1.0.3/paymobpy.egg-info/PKG-INFO
+-rw-r--r--   0 leondaz    (501) staff       (20)      254 2023-05-20 17:11:54.000000 paymobpy-1.0.3/paymobpy.egg-info/SOURCES.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)        1 2023-05-20 17:11:54.000000 paymobpy-1.0.3/paymobpy.egg-info/dependency_links.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)        9 2023-05-20 17:11:54.000000 paymobpy-1.0.3/paymobpy.egg-info/top_level.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)       38 2023-05-20 17:11:54.296687 paymobpy-1.0.3/setup.cfg
+-rw-r--r--   0 leondaz    (501) staff       (20)      275 2023-05-20 17:11:35.000000 paymobpy-1.0.3/setup.py
```

### Comparing `paymobpy-1.0.2/README.md` & `paymobpy-1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 API_KEY = confik.get("PAYMOB_API_KEY")
 
 
 async def main():
     async with Paymob(api_key=API_KEY) as paymob:
         order = await paymob.create_order(data={})  # put order data here
-        payment = await paymob.pay(500, 'EGP', order.id, 'INTEGRATION_ID', data={})
+        payment = await paymob.request_payment(500, 'EGP', order.id, 'INTEGRATION_ID', data={})
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 order.data is a dict implementing the interface paymobpy.schemas.CreateOrderRequest
```

### Comparing `paymobpy-1.0.2/paymobpy/__init__.py` & `paymobpy-1.0.3/paymobpy/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,15 +51,15 @@
                 "Order with merchant_order_id={id} already exists.".format(
                     id=data.merchant_order_id
                 )
             )
 
         return CreateOrderResponse(**response)
 
-    async def pay(
+    async def request_payment(
         self,
         cents: int,
         currency: str,
         order_id: int,
         integration_id: int,
         data: Mapping,
     ) -> CreatePaymentKeyResponse:
```

### Comparing `paymobpy-1.0.2/paymobpy/http_clients.py` & `paymobpy-1.0.3/paymobpy/http_clients.py`

 * *Files identical despite different names*

### Comparing `paymobpy-1.0.2/paymobpy/schemas.py` & `paymobpy-1.0.3/paymobpy/schemas.py`

 * *Files identical despite different names*

