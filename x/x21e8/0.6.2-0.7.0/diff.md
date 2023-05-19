# Comparing `tmp/x21e8-0.6.2.tar.gz` & `tmp/x21e8-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x21e8-0.6.2.tar", max compression
+gzip compressed data, was "x21e8-0.7.0.tar", max compression
```

## Comparing `x21e8-0.6.2.tar` & `x21e8-0.7.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     5030 2023-05-11 09:08:12.378145 x21e8-0.6.2/README.md
--rw-r--r--   0        0        0      717 2023-05-11 09:08:12.386145 x21e8-0.6.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/application/__init__.py
--rw-r--r--   0        0        0     6082 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/application/liquid.py
--rw-r--r--   0        0        0        1 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/application/notarize.py
--rw-r--r--   0        0        0     2409 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/application/planetmint.py
--rw-r--r--   0        0        0      398 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/application/rddl.py
--rw-r--r--   0        0        0     1743 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/application/token.py
--rw-r--r--   0        0        0      765 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/config.py
--rw-r--r--   0        0        0     1001 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/main.py
--rw-r--r--   0        0        0        0 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/models/__init__.py
--rw-r--r--   0        0        0      182 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/models/issuing_request.py
--rw-r--r--   0        0        0      188 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/models/nft_asset.py
--rw-r--r--   0        0        0      354 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/models/token_related_accounts.py
--rw-r--r--   0        0        0      494 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/models/transfer.py
--rw-r--r--   0        0        0        0 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/network/__init__.py
--rw-r--r--   0        0        0     2220 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/network/liquid/__init__.py
--rwxr-xr-x   0        0        0    97346 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/network/liquid/util.py
--rw-r--r--   0        0        0     1693 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/routers/assets.py
--rw-r--r--   0        0        0      375 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/routers/config.py
--rw-r--r--   0        0        0     1108 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/routers/data.py
--rw-r--r--   0        0        0     3892 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/routers/machine.py
--rw-r--r--   0        0        0      925 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/routers/seed.py
--rw-r--r--   0        0        0      630 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/routers/utils.py
--rw-r--r--   0        0        0      619 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/routers/wallet.py
--rw-r--r--   0        0        0        0 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/utils/__init__.py
--rw-r--r--   0        0        0      256 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/utils/cointype.py
--rw-r--r--   0        0        0     1035 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/utils/encryption.py
--rw-r--r--   0        0        0     2328 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/utils/storage.py
--rw-r--r--   0        0        0        0 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/wallet/__init__.py
--rw-r--r--   0        0        0      628 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/wallet/base_wallet.py
--rw-r--r--   0        0        0        0 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/wallet/planetmint/__init__.py
--rw-r--r--   0        0        0     2771 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/wallet/planetmint/keymanagement.py
--rw-r--r--   0        0        0     3231 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/wallet/planetmint/keystore.py
--rw-r--r--   0        0        0      720 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/wallet/seed.py
--rw-r--r--   0        0        0     4367 2023-05-11 09:08:12.386145 x21e8-0.6.2/x21e8/wallet/sw_wallet.py
--rw-r--r--   0        0        0     6001 1970-01-01 00:00:00.000000 x21e8-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     5030 2023-05-19 22:45:24.773321 x21e8-0.7.0/README.md
+-rw-r--r--   0        0        0      717 2023-05-19 22:45:24.777322 x21e8-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-19 22:45:24.777322 x21e8-0.7.0/x21e8/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 22:45:24.777322 x21e8-0.7.0/x21e8/application/__init__.py
+-rw-r--r--   0        0        0     6082 2023-05-19 22:45:24.777322 x21e8-0.7.0/x21e8/application/liquid.py
+-rw-r--r--   0        0        0        1 2023-05-19 22:45:24.777322 x21e8-0.7.0/x21e8/application/notarize.py
+-rw-r--r--   0        0        0     2409 2023-05-19 22:45:24.777322 x21e8-0.7.0/x21e8/application/planetmint.py
+-rw-r--r--   0        0        0      398 2023-05-19 22:45:24.777322 x21e8-0.7.0/x21e8/application/rddl.py
+-rw-r--r--   0        0        0     1743 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/application/token.py
+-rw-r--r--   0        0        0      765 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/config.py
+-rw-r--r--   0        0        0     1001 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/main.py
+-rw-r--r--   0        0        0        0 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/models/__init__.py
+-rw-r--r--   0        0        0      182 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/models/issuing_request.py
+-rw-r--r--   0        0        0      188 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/models/nft_asset.py
+-rw-r--r--   0        0        0      354 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/models/token_related_accounts.py
+-rw-r--r--   0        0        0      494 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/models/transfer.py
+-rw-r--r--   0        0        0        0 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/network/__init__.py
+-rw-r--r--   0        0        0     2220 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/network/liquid/__init__.py
+-rwxr-xr-x   0        0        0    97346 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/network/liquid/util.py
+-rw-r--r--   0        0        0     1693 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/routers/assets.py
+-rw-r--r--   0        0        0      375 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/routers/config.py
+-rw-r--r--   0        0        0     1096 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/routers/data.py
+-rw-r--r--   0        0        0     3892 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/routers/machine.py
+-rw-r--r--   0        0        0      925 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/routers/seed.py
+-rw-r--r--   0        0        0      630 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/routers/utils.py
+-rw-r--r--   0        0        0      619 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/routers/wallet.py
+-rw-r--r--   0        0        0        0 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/utils/__init__.py
+-rw-r--r--   0        0        0      256 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/utils/cointype.py
+-rw-r--r--   0        0        0     1035 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/utils/encryption.py
+-rw-r--r--   0        0        0     2237 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/utils/storage.py
+-rw-r--r--   0        0        0        0 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/wallet/__init__.py
+-rw-r--r--   0        0        0      628 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/wallet/base_wallet.py
+-rw-r--r--   0        0        0        0 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/wallet/planetmint/__init__.py
+-rw-r--r--   0        0        0     2771 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/wallet/planetmint/keymanagement.py
+-rw-r--r--   0        0        0     3231 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/wallet/planetmint/keystore.py
+-rw-r--r--   0        0        0      720 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/wallet/seed.py
+-rw-r--r--   0        0        0     4367 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/wallet/sw_wallet.py
+-rw-r--r--   0        0        0     6001 1970-01-01 00:00:00.000000 x21e8-0.7.0/PKG-INFO
```

### Comparing `x21e8-0.6.2/README.md` & `x21e8-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.2/pyproject.toml` & `x21e8-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "x21e8"
-version = "0.6.2"
+version = "0.7.0"
 description = "x"
 authors = ["Firat Berk Cakar <firat@riddleandcode.com>", "Jürgen Eckel <juergen@riddleandcode.com"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 TrezorCryptoTestRc = "*"
```

### Comparing `x21e8-0.6.2/x21e8/application/liquid.py` & `x21e8-0.7.0/x21e8/application/liquid.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.2/x21e8/application/planetmint.py` & `x21e8-0.7.0/x21e8/application/planetmint.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.2/x21e8/application/token.py` & `x21e8-0.7.0/x21e8/application/token.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.2/x21e8/config.py` & `x21e8-0.7.0/x21e8/config.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.2/x21e8/main.py` & `x21e8-0.7.0/x21e8/main.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.2/x21e8/network/liquid/__init__.py` & `x21e8-0.7.0/x21e8/network/liquid/__init__.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.2/x21e8/network/liquid/util.py` & `x21e8-0.7.0/x21e8/network/liquid/util.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.2/x21e8/routers/assets.py` & `x21e8-0.7.0/x21e8/routers/assets.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.2/x21e8/routers/data.py` & `x21e8-0.7.0/x21e8/routers/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,17 @@
     prefix="/data",
     tags=["Data"],
     responses={404: {"detail": "Not found"}},
 )
 
 
 @router.post("", tags=["Data"])
-async def set_data(in_data_dict: dict, encrypt: bool = False):
+async def set_data(data: str, encrypt: bool = False):
     try:
-        cid = store_asset(in_data_dict, encrypt_data=encrypt)
+        cid = store_asset(data, encrypt_data=encrypt)
         return {"cid": cid}
     except FileNotFoundError:
         raise HTTPException(
             status_code=421,
             detail="The hardware wallet needs to be provisioned by defining a master seed.",
         )
 
@@ -30,8 +30,8 @@
             data = get_ipfs_file(cid, decrypt)
         except URLError as e:
             raise HTTPException(
                 status_code=421,
                 detail=f"The requested URL could not be resolved: {e.code} : {e.reason}.",
             )
 
-    return {"cid": data}
+    return {"cid-data": data}
```

### Comparing `x21e8-0.6.2/x21e8/routers/machine.py` & `x21e8-0.7.0/x21e8/routers/machine.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.2/x21e8/routers/seed.py` & `x21e8-0.7.0/x21e8/routers/seed.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.2/x21e8/routers/utils.py` & `x21e8-0.7.0/x21e8/routers/utils.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.2/x21e8/routers/wallet.py` & `x21e8-0.7.0/x21e8/routers/wallet.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.2/x21e8/utils/encryption.py` & `x21e8-0.7.0/x21e8/utils/encryption.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.2/x21e8/wallet/base_wallet.py` & `x21e8-0.7.0/x21e8/wallet/base_wallet.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.2/x21e8/wallet/planetmint/keymanagement.py` & `x21e8-0.7.0/x21e8/wallet/planetmint/keymanagement.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.2/x21e8/wallet/planetmint/keystore.py` & `x21e8-0.7.0/x21e8/wallet/planetmint/keystore.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.2/x21e8/wallet/seed.py` & `x21e8-0.7.0/x21e8/wallet/seed.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.2/x21e8/wallet/sw_wallet.py` & `x21e8-0.7.0/x21e8/wallet/sw_wallet.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.6.2/PKG-INFO` & `x21e8-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x21e8
-Version: 0.6.2
+Version: 0.7.0
 Summary: x
 Author: Firat Berk Cakar
 Author-email: firat@riddleandcode.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

