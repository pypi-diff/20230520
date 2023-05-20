# Comparing `tmp/paymobpy-1.0.0.tar.gz` & `tmp/paymobpy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paymobpy-1.0.0.tar", last modified: Sat May 20 15:42:14 2023, max compression
+gzip compressed data, was "paymobpy-1.0.1.tar", last modified: Sat May 20 16:29:55 2023, max compression
```

## Comparing `paymobpy-1.0.0.tar` & `paymobpy-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-20 15:42:14.383973 paymobpy-1.0.0/
--rw-r--r--   0 leondaz    (501) staff       (20)      193 2023-05-20 15:42:14.383868 paymobpy-1.0.0/PKG-INFO
--rw-r--r--   0 leondaz    (501) staff       (20)       65 2023-05-20 15:36:20.000000 paymobpy-1.0.0/README.md
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-20 15:42:14.382949 paymobpy-1.0.0/paymobpy/
--rw-r--r--   0 leondaz    (501) staff       (20)     2427 2023-05-20 15:30:04.000000 paymobpy-1.0.0/paymobpy/__init__.py
--rw-r--r--   0 leondaz    (501) staff       (20)      177 2023-05-20 14:43:04.000000 paymobpy-1.0.0/paymobpy/consts.py
--rw-r--r--   0 leondaz    (501) staff       (20)      281 2023-05-20 15:20:58.000000 paymobpy-1.0.0/paymobpy/exceptions.py
--rw-r--r--   0 leondaz    (501) staff       (20)      825 2023-05-20 15:26:08.000000 paymobpy-1.0.0/paymobpy/http_clients.py
--rw-r--r--   0 leondaz    (501) staff       (20)     2517 2023-05-20 15:27:05.000000 paymobpy-1.0.0/paymobpy/schemas.py
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-20 15:42:14.383471 paymobpy-1.0.0/paymobpy.egg-info/
--rw-r--r--   0 leondaz    (501) staff       (20)      193 2023-05-20 15:42:14.000000 paymobpy-1.0.0/paymobpy.egg-info/PKG-INFO
--rw-r--r--   0 leondaz    (501) staff       (20)      277 2023-05-20 15:42:14.000000 paymobpy-1.0.0/paymobpy.egg-info/SOURCES.txt
--rw-r--r--   0 leondaz    (501) staff       (20)        1 2023-05-20 15:42:14.000000 paymobpy-1.0.0/paymobpy.egg-info/dependency_links.txt
--rw-r--r--   0 leondaz    (501) staff       (20)        9 2023-05-20 15:42:14.000000 paymobpy-1.0.0/paymobpy.egg-info/top_level.txt
--rw-r--r--   0 leondaz    (501) staff       (20)       38 2023-05-20 15:42:14.384009 paymobpy-1.0.0/setup.cfg
--rw-r--r--   0 leondaz    (501) staff       (20)      275 2023-05-20 15:34:28.000000 paymobpy-1.0.0/setup.py
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-20 15:42:14.383594 paymobpy-1.0.0/tests/
--rw-r--r--   0 leondaz    (501) staff       (20)     2419 2023-05-20 15:33:32.000000 paymobpy-1.0.0/tests/test_payments.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-20 16:29:55.867656 paymobpy-1.0.1/
+-rw-r--r--   0 leondaz    (501) staff       (20)      193 2023-05-20 16:29:55.867539 paymobpy-1.0.1/PKG-INFO
+-rw-r--r--   0 leondaz    (501) staff       (20)      113 2023-05-20 16:29:46.000000 paymobpy-1.0.1/README.md
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-20 16:29:55.866955 paymobpy-1.0.1/paymobpy/
+-rw-r--r--   0 leondaz    (501) staff       (20)     2441 2023-05-20 15:53:26.000000 paymobpy-1.0.1/paymobpy/__init__.py
+-rw-r--r--   0 leondaz    (501) staff       (20)      177 2023-05-20 14:43:04.000000 paymobpy-1.0.1/paymobpy/consts.py
+-rw-r--r--   0 leondaz    (501) staff       (20)      281 2023-05-20 15:20:58.000000 paymobpy-1.0.1/paymobpy/exceptions.py
+-rw-r--r--   0 leondaz    (501) staff       (20)      825 2023-05-20 15:26:08.000000 paymobpy-1.0.1/paymobpy/http_clients.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     2493 2023-05-20 16:19:48.000000 paymobpy-1.0.1/paymobpy/schemas.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-20 16:29:55.867397 paymobpy-1.0.1/paymobpy.egg-info/
+-rw-r--r--   0 leondaz    (501) staff       (20)      193 2023-05-20 16:29:55.000000 paymobpy-1.0.1/paymobpy.egg-info/PKG-INFO
+-rw-r--r--   0 leondaz    (501) staff       (20)      254 2023-05-20 16:29:55.000000 paymobpy-1.0.1/paymobpy.egg-info/SOURCES.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)        1 2023-05-20 16:29:55.000000 paymobpy-1.0.1/paymobpy.egg-info/dependency_links.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)        9 2023-05-20 16:29:55.000000 paymobpy-1.0.1/paymobpy.egg-info/top_level.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)       38 2023-05-20 16:29:55.867693 paymobpy-1.0.1/setup.cfg
+-rw-r--r--   0 leondaz    (501) staff       (20)      275 2023-05-20 16:29:34.000000 paymobpy-1.0.1/setup.py
```

### Comparing `paymobpy-1.0.0/paymobpy/__init__.py` & `paymobpy-1.0.1/paymobpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 class Paymob:
     def __init__(self, api_key):
         self.api_key = api_key
 
         self._client = PaymobClient(base_url=URLs.BASE_URL)
         self._token = None
 
+    @property
     def auth_token(self):
         if self._token:
             return self._token
 
         raise PaymobError("No token found, did you forget to call .authenticate() ?")
 
     async def authenticate(self) -> str:
```

### Comparing `paymobpy-1.0.0/paymobpy/http_clients.py` & `paymobpy-1.0.1/paymobpy/http_clients.py`

 * *Files identical despite different names*

### Comparing `paymobpy-1.0.0/paymobpy/schemas.py` & `paymobpy-1.0.1/paymobpy/schemas.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,12 +100,11 @@
     is_canceled: bool
     merchant_order_id: str
 
 
 class CreatePaymentKeyRequest(BaseModel):
     expiration: int
     billing_data: Address
-    integration_id: int
 
 
 class CreatePaymentKeyResponse(BaseModel):
     token: str
```

