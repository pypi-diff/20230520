# Comparing `tmp/file_and_string_encryption-0.0.4.tar.gz` & `tmp/file_and_string_encryption-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file_and_string_encryption-0.0.4.tar", last modified: Sat May 20 15:04:03 2023, max compression
+gzip compressed data, was "file_and_string_encryption-0.0.5.tar", last modified: Sat May 20 17:49:41 2023, max compression
```

## Comparing `file_and_string_encryption-0.0.4.tar` & `file_and_string_encryption-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 15:04:03.608867 file_and_string_encryption-0.0.4/
--rw-rw-rw-   0        0        0     1095 2023-01-07 18:45:09.000000 file_and_string_encryption-0.0.4/LICENSE
--rw-rw-rw-   0        0        0       85 2023-05-14 19:46:17.000000 file_and_string_encryption-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1198 2023-05-20 15:04:03.608867 file_and_string_encryption-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      539 2023-05-14 19:59:38.000000 file_and_string_encryption-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 15:04:03.596346 file_and_string_encryption-0.0.4/file_and_string_encryption/
--rw-rw-rw-   0        0        0      580 2023-05-20 15:01:57.000000 file_and_string_encryption-0.0.4/file_and_string_encryption/__init__.py
--rw-rw-rw-   0        0        0    20395 2023-05-20 15:02:24.000000 file_and_string_encryption-0.0.4/file_and_string_encryption/file_and_string_encryption.py
-drwxrwxrwx   0        0        0        0 2023-05-20 15:04:03.606857 file_and_string_encryption-0.0.4/file_and_string_encryption.egg-info/
--rw-rw-rw-   0        0        0     1198 2023-05-20 15:04:03.000000 file_and_string_encryption-0.0.4/file_and_string_encryption.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-05-20 15:04:03.000000 file_and_string_encryption-0.0.4/file_and_string_encryption.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 15:04:03.000000 file_and_string_encryption-0.0.4/file_and_string_encryption.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-20 15:04:03.000000 file_and_string_encryption-0.0.4/file_and_string_encryption.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-05-20 15:04:03.000000 file_and_string_encryption-0.0.4/file_and_string_encryption.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 15:04:03.608867 file_and_string_encryption-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1739 2023-05-20 15:02:02.000000 file_and_string_encryption-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 17:49:41.546239 file_and_string_encryption-0.0.5/
+-rw-rw-rw-   0        0        0     1095 2023-01-07 18:45:09.000000 file_and_string_encryption-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0       85 2023-05-14 19:46:17.000000 file_and_string_encryption-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1198 2023-05-20 17:49:41.546239 file_and_string_encryption-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      539 2023-05-14 19:59:38.000000 file_and_string_encryption-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 17:49:41.534522 file_and_string_encryption-0.0.5/file_and_string_encryption/
+-rw-rw-rw-   0        0        0      614 2023-05-20 17:47:55.000000 file_and_string_encryption-0.0.5/file_and_string_encryption/__init__.py
+-rw-rw-rw-   0        0        0    20750 2023-05-20 17:47:18.000000 file_and_string_encryption-0.0.5/file_and_string_encryption/file_and_string_encryption.py
+drwxrwxrwx   0        0        0        0 2023-05-20 17:49:41.544235 file_and_string_encryption-0.0.5/file_and_string_encryption.egg-info/
+-rw-rw-rw-   0        0        0     1198 2023-05-20 17:49:41.000000 file_and_string_encryption-0.0.5/file_and_string_encryption.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-05-20 17:49:41.000000 file_and_string_encryption-0.0.5/file_and_string_encryption.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 17:49:41.000000 file_and_string_encryption-0.0.5/file_and_string_encryption.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-20 17:49:41.000000 file_and_string_encryption-0.0.5/file_and_string_encryption.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-05-20 17:49:41.000000 file_and_string_encryption-0.0.5/file_and_string_encryption.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 17:49:41.546239 file_and_string_encryption-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1739 2023-05-20 17:47:54.000000 file_and_string_encryption-0.0.5/setup.py
```

### Comparing `file_and_string_encryption-0.0.4/LICENSE` & `file_and_string_encryption-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `file_and_string_encryption-0.0.4/PKG-INFO` & `file_and_string_encryption-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file_and_string_encryption
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple encryption functions. Do not simply trust this code! Pay attention to how you handle sensitive information!
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `file_and_string_encryption-0.0.4/README.md` & `file_and_string_encryption-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `file_and_string_encryption-0.0.4/file_and_string_encryption/__init__.py` & `file_and_string_encryption-0.0.5/file_and_string_encryption/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,12 +11,13 @@
     encrypt_directory,
     encrypt_file,
     encrypt_file_with_password,
     encrypt_string_with_password,
     generate_password,
     get_random_key,
     hash_password_with_argon2,
+    load_password_encrypted_key,
     save_password_encrypted_key,
     verfiy_hashed_password_with_argon2,
 )
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
```

### Comparing `file_and_string_encryption-0.0.4/file_and_string_encryption/file_and_string_encryption.py` & `file_and_string_encryption-0.0.5/file_and_string_encryption/file_and_string_encryption.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,25 +243,23 @@
 
 def encrypt_directory(
     dir_path: str,
     enc_dir_path: str,
     keypath: str | None = None,
     key: bytes = None,
     error_if_enc_is_file: bool = True,
-    error_if_key_is_file: bool = True,
 ):
     """Uses `encrypt_file` for all files in a directory. Keeps the original directory structure.
 
     Args:
         - dir_path (str): Path to the directory to encrypt.
         - enc_dir_path (str): Path for the encrypted directory.
         - keypath (str | None, optional): Path for the key to be saved at, including the filename. Defaults to None, meaning it won't be saved.
         - key (bytes, optional): You can provide a specific key here. Defaults to None.
         - error_if_enc_is_file (bool, optional): Raise an exception if enc_filepath is already a file. Defaults to True.
-        - error_if_key_is_file (bool, optional): Raise an exception if keypath is already a file. Defaults to True.
 
     Returns:
         bytes: The used key.
     """
     dir_path = os.path.normpath(dir_path)
     if key == None:
         key = get_random_key()
@@ -279,17 +277,15 @@
     for main_index, (root, dirs, files) in enumerate(os.walk(dir_path)):
         sub_path = root.replace(dir_path, "")
         sub_path = sub_path.lstrip("\\")
         l2 = len(files)
         for sub_index, f in enumerate(files):
             fp = os.path.join(root, f)
             nfp = os.path.join(enc_dir_path, sub_path, f)
-            encrypt_file(
-                fp, nfp, keypath, key, error_if_enc_is_file, error_if_key_is_file
-            )
+            encrypt_file(fp, nfp, keypath, key, error_if_enc_is_file, False)
             main_and_sub_progress_printer(
                 main_index + 1,
                 l1,
                 sub_index + 1,
                 l2,
                 mainpre_string="Progress on dirpaths: ",
                 subpre_string="Progress on files in current dir: ",
@@ -314,26 +310,26 @@
         - key (bytes, optional): You can reuse the key of earlier encryptions or generate a key using the function get_random_key. Defaults to None.
         - error_if_enc_is_file (bool, optional): Raise an exception if enc_filepath is already a file. Defaults to True.
         - error_if_key_is_file (bool, optional): Raise an exception if keypath is already a file. Defaults to True.
 
     Returns:
         bytes: The key generated by Fernet.generate_key()
     """
-    if error_if_key_is_file and os.path.isfile(enc_filepath):
+    if error_if_enc_is_file and os.path.isfile(enc_filepath):
         raise FileExistsError(
             f"There is already a file in the enc_filepath location.\n\tenc_filepath: {enc_filepath}"
         )
     if key == None:
         key = Fernet.generate_key()
     if not os.path.isdir(os.path.dirname(enc_filepath)):
         os.makedirs(os.path.dirname(enc_filepath))
     if keypath != None:
         if not os.path.isdir(os.path.dirname(keypath)):
             os.makedirs(os.path.dirname(keypath))
-        if error_if_enc_is_file and os.path.isfile(keypath):
+        if error_if_key_is_file and os.path.isfile(keypath):
             raise FileExistsError(
                 f"There is already a file in the keypath location.\n\tkeypath: {keypath}"
             )
         with open(keypath, "wb") as f:
             f.write(key)
     fernet = Fernet(key)
     with open(filepath, "rb") as original_file:
@@ -474,14 +470,32 @@
         default="argon2",
         argon2__default_rounds=argon2_default_rounds,
     )
     hashed_password = context.hash(password)
     return hashed_password
 
 
+def load_password_encrypted_key(
+    keypath: str,
+    password: str | None = None,
+):
+    """Load the password encrypted key from a file.
+
+    Args:
+        keypath (str): Path to the file containing the password encrypted key.
+        password (str | None, optional): If the key is password encrypted, you obviously need the password. Defaults to None.
+
+    Returns:
+        str: The decrypted key.
+    """
+    with open(keypath, "rb") as f:
+        encrypted_key = f.read()
+    return decrypt_string_with_password(encrypted_key, password)
+
+
 def password_decrypt_non_string(token: bytes, password: str):
     decoded = b64d(token)
     salt, iter, token = decoded[:16], decoded[16:20], b64e(decoded[20:])
     iterations = int.from_bytes(iter, "big")
     key = derive_key_from_password(password.encode(), salt, iterations)
     pw = Fernet(key).decrypt(token).decode()
     return pw
@@ -504,15 +518,15 @@
 
 def save_password_encrypted_key(
     key: bytes,
     keypath: str,
     password: str | None = None,
     error_if_key_is_file: bool = True,
 ):
-    """Save the key returned by an encryption function. Additionally you can encrypt the key by setting the password.
+    """Save the key returned by an encryption function. You can but don't have to encrypt the key with a password.
 
     Args:
         - key (bytes): Key returned by an encryption function.
         - keypath (str): The path for the key to be written to.
         - password (str | None, optional): A password to encrypt the key. Defaults to None.
         - error_if_key_is_file (bool, optional): Throw an exception if there already is a file. Defaults to True.
```

### Comparing `file_and_string_encryption-0.0.4/file_and_string_encryption.egg-info/PKG-INFO` & `file_and_string_encryption-0.0.5/file_and_string_encryption.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file-and-string-encryption
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple encryption functions. Do not simply trust this code! Pay attention to how you handle sensitive information!
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `file_and_string_encryption-0.0.4/setup.py` & `file_and_string_encryption-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.4"
+VERSION = "0.0.5"
 DESCRIPTION = "Simple encryption functions. Do not simply trust this code! Pay attention to how you handle sensitive information!"
 
 # Setting up
 setup(
     name="file_and_string_encryption",
     version=VERSION,
     author="André Herber",
```

