# Comparing `tmp/file_and_string_encryption-0.0.3.tar.gz` & `tmp/file_and_string_encryption-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file_and_string_encryption-0.0.3.tar", last modified: Sat May 20 15:00:17 2023, max compression
+gzip compressed data, was "file_and_string_encryption-0.0.4.tar", last modified: Sat May 20 15:04:03 2023, max compression
```

## Comparing `file_and_string_encryption-0.0.3.tar` & `file_and_string_encryption-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 15:00:17.940234 file_and_string_encryption-0.0.3/
--rw-rw-rw-   0        0        0     1095 2023-01-07 18:45:09.000000 file_and_string_encryption-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       85 2023-05-14 19:46:17.000000 file_and_string_encryption-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1198 2023-05-20 15:00:17.940234 file_and_string_encryption-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      539 2023-05-14 19:59:38.000000 file_and_string_encryption-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 15:00:17.929015 file_and_string_encryption-0.0.3/file_and_string_encryption/
--rw-rw-rw-   0        0        0      580 2023-05-20 14:59:30.000000 file_and_string_encryption-0.0.3/file_and_string_encryption/__init__.py
--rw-rw-rw-   0        0        0    20395 2023-05-20 14:59:01.000000 file_and_string_encryption-0.0.3/file_and_string_encryption/file_and_string_encryption.py
-drwxrwxrwx   0        0        0        0 2023-05-20 15:00:17.938234 file_and_string_encryption-0.0.3/file_and_string_encryption.egg-info/
--rw-rw-rw-   0        0        0     1198 2023-05-20 15:00:17.000000 file_and_string_encryption-0.0.3/file_and_string_encryption.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-05-20 15:00:17.000000 file_and_string_encryption-0.0.3/file_and_string_encryption.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 15:00:17.000000 file_and_string_encryption-0.0.3/file_and_string_encryption.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-20 15:00:17.000000 file_and_string_encryption-0.0.3/file_and_string_encryption.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-05-20 15:00:17.000000 file_and_string_encryption-0.0.3/file_and_string_encryption.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 15:00:17.941234 file_and_string_encryption-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1739 2023-05-20 14:59:36.000000 file_and_string_encryption-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 15:04:03.608867 file_and_string_encryption-0.0.4/
+-rw-rw-rw-   0        0        0     1095 2023-01-07 18:45:09.000000 file_and_string_encryption-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       85 2023-05-14 19:46:17.000000 file_and_string_encryption-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1198 2023-05-20 15:04:03.608867 file_and_string_encryption-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      539 2023-05-14 19:59:38.000000 file_and_string_encryption-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 15:04:03.596346 file_and_string_encryption-0.0.4/file_and_string_encryption/
+-rw-rw-rw-   0        0        0      580 2023-05-20 15:01:57.000000 file_and_string_encryption-0.0.4/file_and_string_encryption/__init__.py
+-rw-rw-rw-   0        0        0    20395 2023-05-20 15:02:24.000000 file_and_string_encryption-0.0.4/file_and_string_encryption/file_and_string_encryption.py
+drwxrwxrwx   0        0        0        0 2023-05-20 15:04:03.606857 file_and_string_encryption-0.0.4/file_and_string_encryption.egg-info/
+-rw-rw-rw-   0        0        0     1198 2023-05-20 15:04:03.000000 file_and_string_encryption-0.0.4/file_and_string_encryption.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-05-20 15:04:03.000000 file_and_string_encryption-0.0.4/file_and_string_encryption.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 15:04:03.000000 file_and_string_encryption-0.0.4/file_and_string_encryption.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-20 15:04:03.000000 file_and_string_encryption-0.0.4/file_and_string_encryption.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-05-20 15:04:03.000000 file_and_string_encryption-0.0.4/file_and_string_encryption.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 15:04:03.608867 file_and_string_encryption-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1739 2023-05-20 15:02:02.000000 file_and_string_encryption-0.0.4/setup.py
```

### Comparing `file_and_string_encryption-0.0.3/LICENSE` & `file_and_string_encryption-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `file_and_string_encryption-0.0.3/PKG-INFO` & `file_and_string_encryption-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file_and_string_encryption
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple encryption functions. Do not simply trust this code! Pay attention to how you handle sensitive information!
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `file_and_string_encryption-0.0.3/README.md` & `file_and_string_encryption-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `file_and_string_encryption-0.0.3/file_and_string_encryption/__init__.py` & `file_and_string_encryption-0.0.4/file_and_string_encryption/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,8 @@
     generate_password,
     get_random_key,
     hash_password_with_argon2,
     save_password_encrypted_key,
     verfiy_hashed_password_with_argon2,
 )
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
```

### Comparing `file_and_string_encryption-0.0.3/file_and_string_encryption/file_and_string_encryption.py` & `file_and_string_encryption-0.0.4/file_and_string_encryption/file_and_string_encryption.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,24 +219,24 @@
     salt, iter, token = decoded[:16], decoded[16:20], b64e(decoded[20:])
     iterations = int.from_bytes(iter, "big")
     key = derive_key_from_password(password.encode(), salt, iterations)
     pw = Fernet(key).decrypt(token).decode()
     return pw
 
 
-def encrypt_data(data: bytes, key: bytes = None) -> tuple(bytes):
+def encrypt_data(data: bytes, key: bytes = None) -> tuple[bytes]:
     """Encypt data using a key. The data must be bytes. You can provide your own key if you want.
      Data can be converted to bytes using pickle. For convenience there is a `data_to_bytes_using_pickle` function which literally is `pickle.dumps(data)`.
 
     Args:
         - data (bytes): Data to encrypt.
         - key (bytes, optional): Specified key to use. Defaults to None.
 
     Returns:
-        tuple(bytes): Tuple containing the encrypted data and the key.
+        tuple[bytes]: Tuple containing the encrypted data and the key.
     """
     if key == None:
         key = Fernet.generate_key()
     fernet = Fernet(key)
     encrypted = fernet.encrypt(data)
     return (encrypted, key)
```

### Comparing `file_and_string_encryption-0.0.3/file_and_string_encryption.egg-info/PKG-INFO` & `file_and_string_encryption-0.0.4/file_and_string_encryption.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file-and-string-encryption
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple encryption functions. Do not simply trust this code! Pay attention to how you handle sensitive information!
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `file_and_string_encryption-0.0.3/setup.py` & `file_and_string_encryption-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 DESCRIPTION = "Simple encryption functions. Do not simply trust this code! Pay attention to how you handle sensitive information!"
 
 # Setting up
 setup(
     name="file_and_string_encryption",
     version=VERSION,
     author="André Herber",
```

