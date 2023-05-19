# Comparing `tmp/near-api-0.2.0.tar.gz` & `tmp/near-api-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "near-api-0.2.0.tar", last modified: Fri May 19 20:47:05 2023, max compression
+gzip compressed data, was "near-api-0.2.1.tar", last modified: Fri May 19 23:28:35 2023, max compression
```

## Comparing `near-api-0.2.0.tar` & `near-api-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 frol       (501) staff       (20)        0 2023-05-19 20:47:05.498488 near-api-0.2.0/
--rw-r--r--   0 frol       (501) staff       (20)     1024 2023-05-19 20:36:31.000000 near-api-0.2.0/LICENSE
--rw-r--r--   0 frol       (501) staff       (20)     9722 2023-05-19 20:36:31.000000 near-api-0.2.0/LICENSE-APACHE
--rw-r--r--   0 frol       (501) staff       (20)      180 2023-05-19 20:47:05.498298 near-api-0.2.0/PKG-INFO
--rw-r--r--   0 frol       (501) staff       (20)     1458 2023-05-19 20:36:31.000000 near-api-0.2.0/README.md
-drwxr-xr-x   0 frol       (501) staff       (20)        0 2023-05-19 20:47:05.495990 near-api-0.2.0/near_api/
--rw-r--r--   0 frol       (501) staff       (20)      180 2023-05-19 20:36:31.000000 near-api-0.2.0/near_api/__init__.py
--rw-r--r--   0 frol       (501) staff       (20)     5810 2023-05-19 20:36:31.000000 near-api-0.2.0/near_api/account.py
--rw-r--r--   0 frol       (501) staff       (20)     6514 2023-05-19 20:36:31.000000 near-api-0.2.0/near_api/providers.py
--rw-r--r--   0 frol       (501) staff       (20)     3443 2023-05-19 20:36:31.000000 near-api-0.2.0/near_api/serializer.py
--rw-r--r--   0 frol       (501) staff       (20)     2428 2023-05-19 20:36:31.000000 near-api-0.2.0/near_api/signer.py
--rw-r--r--   0 frol       (501) staff       (20)    12170 2023-05-19 20:36:31.000000 near-api-0.2.0/near_api/transactions.py
-drwxr-xr-x   0 frol       (501) staff       (20)        0 2023-05-19 20:47:05.497260 near-api-0.2.0/near_api.egg-info/
--rw-r--r--   0 frol       (501) staff       (20)      180 2023-05-19 20:47:05.000000 near-api-0.2.0/near_api.egg-info/PKG-INFO
--rw-r--r--   0 frol       (501) staff       (20)      373 2023-05-19 20:47:05.000000 near-api-0.2.0/near_api.egg-info/SOURCES.txt
--rw-r--r--   0 frol       (501) staff       (20)        1 2023-05-19 20:47:05.000000 near-api-0.2.0/near_api.egg-info/dependency_links.txt
--rw-r--r--   0 frol       (501) staff       (20)       24 2023-05-19 20:47:05.000000 near-api-0.2.0/near_api.egg-info/requires.txt
--rw-r--r--   0 frol       (501) staff       (20)        9 2023-05-19 20:47:05.000000 near-api-0.2.0/near_api.egg-info/top_level.txt
--rw-r--r--   0 frol       (501) staff       (20)       38 2023-05-19 20:47:05.498541 near-api-0.2.0/setup.cfg
--rw-r--r--   0 frol       (501) staff       (20)      336 2023-05-19 20:37:19.000000 near-api-0.2.0/setup.py
-drwxr-xr-x   0 frol       (501) staff       (20)        0 2023-05-19 20:47:05.497895 near-api-0.2.0/test/
--rw-r--r--   0 frol       (501) staff       (20)      950 2023-05-19 20:36:31.000000 near-api-0.2.0/test/test_account.py
--rw-r--r--   0 frol       (501) staff       (20)     1724 2023-05-19 20:36:31.000000 near-api-0.2.0/test/test_provider.py
+drwxr-xr-x   0 frol       (501) staff       (20)        0 2023-05-19 23:28:35.045088 near-api-0.2.1/
+-rw-r--r--   0 frol       (501) staff       (20)     1024 2023-05-19 20:36:31.000000 near-api-0.2.1/LICENSE
+-rw-r--r--   0 frol       (501) staff       (20)     9722 2023-05-19 20:36:31.000000 near-api-0.2.1/LICENSE-APACHE
+-rw-r--r--   0 frol       (501) staff       (20)      180 2023-05-19 23:28:35.044829 near-api-0.2.1/PKG-INFO
+-rw-r--r--   0 frol       (501) staff       (20)     1455 2023-05-19 23:10:17.000000 near-api-0.2.1/README.md
+drwxr-xr-x   0 frol       (501) staff       (20)        0 2023-05-19 23:28:35.043098 near-api-0.2.1/near_api/
+-rw-r--r--   0 frol       (501) staff       (20)      180 2023-05-19 20:36:31.000000 near-api-0.2.1/near_api/__init__.py
+-rw-r--r--   0 frol       (501) staff       (20)     5810 2023-05-19 20:36:31.000000 near-api-0.2.1/near_api/account.py
+-rw-r--r--   0 frol       (501) staff       (20)     6514 2023-05-19 20:36:31.000000 near-api-0.2.1/near_api/providers.py
+-rw-r--r--   0 frol       (501) staff       (20)     3443 2023-05-19 20:36:31.000000 near-api-0.2.1/near_api/serializer.py
+-rw-r--r--   0 frol       (501) staff       (20)     2445 2023-05-19 23:05:57.000000 near-api-0.2.1/near_api/signer.py
+-rw-r--r--   0 frol       (501) staff       (20)    12170 2023-05-19 20:36:31.000000 near-api-0.2.1/near_api/transactions.py
+drwxr-xr-x   0 frol       (501) staff       (20)        0 2023-05-19 23:28:35.043955 near-api-0.2.1/near_api.egg-info/
+-rw-r--r--   0 frol       (501) staff       (20)      180 2023-05-19 23:28:35.000000 near-api-0.2.1/near_api.egg-info/PKG-INFO
+-rw-r--r--   0 frol       (501) staff       (20)      373 2023-05-19 23:28:35.000000 near-api-0.2.1/near_api.egg-info/SOURCES.txt
+-rw-r--r--   0 frol       (501) staff       (20)        1 2023-05-19 23:28:35.000000 near-api-0.2.1/near_api.egg-info/dependency_links.txt
+-rw-r--r--   0 frol       (501) staff       (20)       23 2023-05-19 23:28:35.000000 near-api-0.2.1/near_api.egg-info/requires.txt
+-rw-r--r--   0 frol       (501) staff       (20)        9 2023-05-19 23:28:35.000000 near-api-0.2.1/near_api.egg-info/top_level.txt
+-rw-r--r--   0 frol       (501) staff       (20)       38 2023-05-19 23:28:35.045188 near-api-0.2.1/setup.cfg
+-rw-r--r--   0 frol       (501) staff       (20)      335 2023-05-19 23:06:32.000000 near-api-0.2.1/setup.py
+drwxr-xr-x   0 frol       (501) staff       (20)        0 2023-05-19 23:28:35.044543 near-api-0.2.1/test/
+-rw-r--r--   0 frol       (501) staff       (20)      950 2023-05-19 20:36:31.000000 near-api-0.2.1/test/test_account.py
+-rw-r--r--   0 frol       (501) staff       (20)     1724 2023-05-19 20:36:31.000000 near-api-0.2.1/test/test_provider.py
```

### Comparing `near-api-0.2.0/LICENSE` & `near-api-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `near-api-0.2.0/LICENSE-APACHE` & `near-api-0.2.1/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `near-api-0.2.0/README.md` & `near-api-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 *Status: super rough, APIs are subject to change*
 
 A Python library for development of applications that are using NEAR platform.
 
 # Installation
 
 ```bash
-pip install near-api-py
+pip install near-api
 ```
 
 # Usage example
 
 ## Send money
 
 ```python
```

### Comparing `near-api-0.2.0/near_api/account.py` & `near-api-0.2.1/near_api/account.py`

 * *Files identical despite different names*

### Comparing `near-api-0.2.0/near_api/providers.py` & `near-api-0.2.1/near_api/providers.py`

 * *Files identical despite different names*

### Comparing `near-api-0.2.0/near_api/serializer.py` & `near-api-0.2.1/near_api/serializer.py`

 * *Files identical despite different names*

### Comparing `near-api-0.2.0/near_api/signer.py` & `near-api-0.2.1/near_api/signer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 import json
 from typing import Union
 
 import base58
-import ed25519
+from nacl import signing, encoding
 
 
 class KeyPair(object):
 
-    def __init__(self, secret_key: Union[str, bytes] = None):
+    def __init__(self, secret_key: Union[str, bytes, None] = None):
         """
         If no secret_key, a new one is created.
         secret_key must be a base58-encoded string or
         the byte object returned as "secret_key" property of a KeyPair object."""
         if not secret_key:
-            self._secret_key, self._public_key = ed25519.keys.create_keypair()
-            raise Exception("No secret_key")
+            self._secret_key = signing.SigningKey.generate()
         if isinstance(secret_key, bytes):
-            self._secret_key = ed25519.keys.SigningKey(secret_key)
+            self._secret_key = signing.SigningKey(secret_key, encoder=encoding.RawEncoder)
         elif isinstance(secret_key, str):
             secret_key = secret_key.split(':')[-1]
-            self._secret_key = ed25519.keys.SigningKey(base58.b58decode(secret_key))
+            self._secret_key = signing.SigningKey(base58.b58decode(secret_key)[:32], encoder=encoding.RawEncoder)
         else:
             raise Exception("Unrecognised")
-        self._public_key = self._secret_key.get_verifying_key()
+        self._public_key = self._secret_key.verify_key
 
     @property
     def public_key(self) -> bytes:
-        return self._public_key.to_bytes()
+        return self._public_key.encode()
 
     def encoded_public_key(self) -> str:
         return base58.b58encode(self.public_key).decode('utf-8')
 
-    def sign(self, message: bytes) -> str:
-        return self._secret_key.sign(message)
+    def sign(self, message: bytes) -> bytes:
+        return self._secret_key.sign(message).signature
 
     @property
     def secret_key(self) -> bytes:
-        return self._secret_key.to_bytes()
+        return self._secret_key.encode()
 
     @property
     def encoded_secret_key(self) -> str:
         return base58.b58encode(self.secret_key).decode('utf-8')
 
     @property
     def corresponding_account_id(self) -> str:
@@ -64,15 +63,15 @@
     def key_pair(self) -> 'KeyPair':
         return self._key_pair
 
     @property
     def public_key(self) -> bytes:
         return self._key_pair.public_key
 
-    def sign(self, message: bytes) -> str:
+    def sign(self, message: bytes) -> bytes:
         return self._key_pair.sign(message)
 
     @classmethod
     def from_json(cls, j: dict):
         return cls(j['account_id'], KeyPair(j['secret_key']))
 
     @classmethod
```

### Comparing `near-api-0.2.0/near_api/transactions.py` & `near-api-0.2.1/near_api/transactions.py`

 * *Files identical despite different names*

### Comparing `near-api-0.2.0/test/test_account.py` & `near-api-0.2.1/test/test_account.py`

 * *Files identical despite different names*

### Comparing `near-api-0.2.0/test/test_provider.py` & `near-api-0.2.1/test/test_provider.py`

 * *Files identical despite different names*

