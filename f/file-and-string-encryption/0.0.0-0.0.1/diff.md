# Comparing `tmp/file_and_string_encryption-0.0.0.tar.gz` & `tmp/file_and_string_encryption-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file_and_string_encryption-0.0.0.tar", last modified: Sun May 14 20:00:56 2023, max compression
+gzip compressed data, was "file_and_string_encryption-0.0.1.tar", last modified: Sat May 20 14:07:53 2023, max compression
```

## Comparing `file_and_string_encryption-0.0.0.tar` & `file_and_string_encryption-0.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 20:00:55.993866 file_and_string_encryption-0.0.0/
--rw-rw-rw-   0        0        0     1095 2023-01-07 18:45:09.000000 file_and_string_encryption-0.0.0/LICENSE
--rw-rw-rw-   0        0        0       85 2023-05-14 19:46:17.000000 file_and_string_encryption-0.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1198 2023-05-14 20:00:55.992767 file_and_string_encryption-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      539 2023-05-14 19:59:38.000000 file_and_string_encryption-0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 20:00:55.984826 file_and_string_encryption-0.0.0/file_and_string_encryption/
--rw-rw-rw-   0        0        0      338 2023-05-14 19:59:22.000000 file_and_string_encryption-0.0.0/file_and_string_encryption/__init__.py
--rw-rw-rw-   0        0        0    19971 2023-05-14 19:58:36.000000 file_and_string_encryption-0.0.0/file_and_string_encryption/file_and_string_encryption.py
-drwxrwxrwx   0        0        0        0 2023-05-14 20:00:55.991510 file_and_string_encryption-0.0.0/file_and_string_encryption.egg-info/
--rw-rw-rw-   0        0        0     1198 2023-05-14 20:00:55.000000 file_and_string_encryption-0.0.0/file_and_string_encryption.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-05-14 20:00:55.000000 file_and_string_encryption-0.0.0/file_and_string_encryption.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 20:00:55.000000 file_and_string_encryption-0.0.0/file_and_string_encryption.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-14 20:00:55.000000 file_and_string_encryption-0.0.0/file_and_string_encryption.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-05-14 20:00:55.000000 file_and_string_encryption-0.0.0/file_and_string_encryption.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 20:00:55.993866 file_and_string_encryption-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1739 2023-05-14 19:59:24.000000 file_and_string_encryption-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 14:07:53.910111 file_and_string_encryption-0.0.1/
+-rw-rw-rw-   0        0        0     1095 2023-01-07 18:45:09.000000 file_and_string_encryption-0.0.1/LICENSE
+-rw-rw-rw-   0        0        0       85 2023-05-14 19:46:17.000000 file_and_string_encryption-0.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1198 2023-05-20 14:07:53.909091 file_and_string_encryption-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      539 2023-05-14 19:59:38.000000 file_and_string_encryption-0.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 14:07:53.896380 file_and_string_encryption-0.0.1/file_and_string_encryption/
+-rw-rw-rw-   0        0        0      473 2023-05-20 14:05:20.000000 file_and_string_encryption-0.0.1/file_and_string_encryption/__init__.py
+-rw-rw-rw-   0        0        0    21259 2023-05-20 14:05:30.000000 file_and_string_encryption-0.0.1/file_and_string_encryption/file_and_string_encryption.py
+drwxrwxrwx   0        0        0        0 2023-05-20 14:07:53.907074 file_and_string_encryption-0.0.1/file_and_string_encryption.egg-info/
+-rw-rw-rw-   0        0        0     1198 2023-05-20 14:07:53.000000 file_and_string_encryption-0.0.1/file_and_string_encryption.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-05-20 14:07:53.000000 file_and_string_encryption-0.0.1/file_and_string_encryption.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 14:07:53.000000 file_and_string_encryption-0.0.1/file_and_string_encryption.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-20 14:07:53.000000 file_and_string_encryption-0.0.1/file_and_string_encryption.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-05-20 14:07:53.000000 file_and_string_encryption-0.0.1/file_and_string_encryption.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 14:07:53.910111 file_and_string_encryption-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1739 2023-05-20 14:05:25.000000 file_and_string_encryption-0.0.1/setup.py
```

### Comparing `file_and_string_encryption-0.0.0/LICENSE` & `file_and_string_encryption-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `file_and_string_encryption-0.0.0/PKG-INFO` & `file_and_string_encryption-0.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file_and_string_encryption
-Version: 0.0.0
+Version: 0.0.1
 Summary: Simple encryption functions. Do not simply trust this code! Pay attention to how you handle sensitive information!
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `file_and_string_encryption-0.0.0/README.md` & `file_and_string_encryption-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `file_and_string_encryption-0.0.0/file_and_string_encryption/file_and_string_encryption.py` & `file_and_string_encryption-0.0.1/file_and_string_encryption/file_and_string_encryption.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,20 +20,23 @@
 
 from cryptography.fernet import Fernet
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
 from passlib.context import CryptContext
 from easy_tasks import main_and_sub_progress_printer
+import pickle
 
 backend = default_backend()
 iterations = 100_000
 
 
-def _derive_key(password: bytes, salt: bytes, iterations: int = iterations) -> bytes:
+def derive_key_from_password(
+    password: bytes, salt: bytes, iterations: int = iterations
+) -> bytes:
     """Derive a secret key from a given password and salt"""
     kdf = PBKDF2HMAC(
         algorithm=hashes.SHA256(),
         length=32,
         salt=salt,
         iterations=iterations,
         backend=backend,
@@ -41,15 +44,15 @@
     return b64e(kdf.derive(password))
 
 
 def password_encrypt_bytes(
     message: bytes, password: str, iterations: int = iterations
 ) -> bytes:
     salt = secrets_token_bytes(16)
-    key = _derive_key(password.encode(), salt, iterations)
+    key = derive_key_from_password(password.encode(), salt, iterations)
     return b64e(
         b"%b%b%b"
         % (
             salt,
             iterations.to_bytes(4, "big"),
             b64d(Fernet(key).encrypt(message)),
         )
@@ -68,15 +71,15 @@
 
     Returns:
         bytes: Encrypted message.
     """
     if type(message) != bytes:
         message = message.encode()
     salt = secrets_token_bytes(16)
-    key = _derive_key(password.encode(), salt, iterations)
+    key = derive_key_from_password(password.encode(), salt, iterations)
     return b64e(
         b"%b%b%b"
         % (
             salt,
             iterations.to_bytes(4, "big"),
             b64d(Fernet(key).encrypt(message)),
         )
@@ -92,24 +95,65 @@
 
     Returns:
         str: The decrypted message.
     """
     decoded = b64d(token)
     salt, iter, token = decoded[:16], decoded[16:20], b64e(decoded[20:])
     iterations = int.from_bytes(iter, "big")
-    key = _derive_key(password.encode(), salt, iterations)
+    key = derive_key_from_password(password.encode(), salt, iterations)
     pw = Fernet(key).decrypt(token).decode()
     return pw
 
 
+def data_to_bytes_using_pickle(data):
+    return pickle.dumps(data)
+
+
+def bytes_to_data_using_pickle(data):
+    return pickle.loads(data)
+
+
+def encrypt_data(data: bytes, key: bytes = None) -> tuple(bytes, bytes):
+    """Encypt data using a key. The data must be bytes. You can provide your own key if you want.
+     Data can be converted to bytes using pickle. For convenience there is a `data_to_bytes_using_pickle` function which literally is `pickle.dumps(data)`.
+
+    Args:
+        - data (bytes): Data to encrypt.
+        - key (bytes, optional): Specified key to use. Defaults to None.
+
+    Returns:
+        tuple(bytes, bytes): Tuple containing the encrypted data and the key.
+    """
+    if key == None:
+        key = Fernet.generate_key()
+    fernet = Fernet(key)
+    encrypted = fernet.encrypt(data)
+    return (encrypted, key)
+
+
+def decrypt_data(data: bytes, key: bytes) -> bytes:
+    """Decypt data using a key.
+
+    Args:
+        - data (bytes): Encrypted data to decrypt.
+        - key (bytes): Key to use.
+
+    Returns:
+        bytes: Decrypted data.
+    """
+    fernet = Fernet(key)
+    decrypted = fernet.decrypt(data)
+    return decrypted
+
+
 def password_decrypt_non_string(token: bytes, password: str):
     decoded = b64d(token)
     salt, iter, token = decoded[:16], decoded[16:20], b64e(decoded[20:])
     iterations = int.from_bytes(iter, "big")
-    key = _derive_key(password.encode(), salt, iterations)
+    key = derive_key_from_password(password.encode(), salt, iterations)
     pw = Fernet(key).decrypt(token).decode()
     return pw
 
 
 def encrypt_secret(secret, password: str):
     """
     -> encrypted_secret, salt
```

### Comparing `file_and_string_encryption-0.0.0/file_and_string_encryption.egg-info/PKG-INFO` & `file_and_string_encryption-0.0.1/file_and_string_encryption.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file-and-string-encryption
-Version: 0.0.0
+Version: 0.0.1
 Summary: Simple encryption functions. Do not simply trust this code! Pay attention to how you handle sensitive information!
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `file_and_string_encryption-0.0.0/setup.py` & `file_and_string_encryption-0.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.0"
+VERSION = "0.0.1"
 DESCRIPTION = "Simple encryption functions. Do not simply trust this code! Pay attention to how you handle sensitive information!"
 
 # Setting up
 setup(
     name="file_and_string_encryption",
     version=VERSION,
     author="André Herber",
```

