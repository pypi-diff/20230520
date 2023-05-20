# Comparing `tmp/file_and_string_encryption-0.0.2.tar.gz` & `tmp/file_and_string_encryption-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file_and_string_encryption-0.0.2.tar", last modified: Sat May 20 14:53:20 2023, max compression
+gzip compressed data, was "file_and_string_encryption-0.0.3.tar", last modified: Sat May 20 15:00:17 2023, max compression
```

## Comparing `file_and_string_encryption-0.0.2.tar` & `file_and_string_encryption-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 14:53:20.045034 file_and_string_encryption-0.0.2/
--rw-rw-rw-   0        0        0     1095 2023-01-07 18:45:09.000000 file_and_string_encryption-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       85 2023-05-14 19:46:17.000000 file_and_string_encryption-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1198 2023-05-20 14:53:20.043989 file_and_string_encryption-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      539 2023-05-14 19:59:38.000000 file_and_string_encryption-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 14:53:20.032888 file_and_string_encryption-0.0.2/file_and_string_encryption/
--rw-rw-rw-   0        0        0      580 2023-05-20 14:51:56.000000 file_and_string_encryption-0.0.2/file_and_string_encryption/__init__.py
--rw-rw-rw-   0        0        0    20347 2023-05-20 14:51:57.000000 file_and_string_encryption-0.0.2/file_and_string_encryption/file_and_string_encryption.py
-drwxrwxrwx   0        0        0        0 2023-05-20 14:53:20.042890 file_and_string_encryption-0.0.2/file_and_string_encryption.egg-info/
--rw-rw-rw-   0        0        0     1198 2023-05-20 14:53:19.000000 file_and_string_encryption-0.0.2/file_and_string_encryption.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-05-20 14:53:19.000000 file_and_string_encryption-0.0.2/file_and_string_encryption.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 14:53:19.000000 file_and_string_encryption-0.0.2/file_and_string_encryption.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-20 14:53:19.000000 file_and_string_encryption-0.0.2/file_and_string_encryption.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-05-20 14:53:19.000000 file_and_string_encryption-0.0.2/file_and_string_encryption.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 14:53:20.045034 file_and_string_encryption-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1739 2023-05-20 14:51:56.000000 file_and_string_encryption-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 15:00:17.940234 file_and_string_encryption-0.0.3/
+-rw-rw-rw-   0        0        0     1095 2023-01-07 18:45:09.000000 file_and_string_encryption-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       85 2023-05-14 19:46:17.000000 file_and_string_encryption-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1198 2023-05-20 15:00:17.940234 file_and_string_encryption-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      539 2023-05-14 19:59:38.000000 file_and_string_encryption-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 15:00:17.929015 file_and_string_encryption-0.0.3/file_and_string_encryption/
+-rw-rw-rw-   0        0        0      580 2023-05-20 14:59:30.000000 file_and_string_encryption-0.0.3/file_and_string_encryption/__init__.py
+-rw-rw-rw-   0        0        0    20395 2023-05-20 14:59:01.000000 file_and_string_encryption-0.0.3/file_and_string_encryption/file_and_string_encryption.py
+drwxrwxrwx   0        0        0        0 2023-05-20 15:00:17.938234 file_and_string_encryption-0.0.3/file_and_string_encryption.egg-info/
+-rw-rw-rw-   0        0        0     1198 2023-05-20 15:00:17.000000 file_and_string_encryption-0.0.3/file_and_string_encryption.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-05-20 15:00:17.000000 file_and_string_encryption-0.0.3/file_and_string_encryption.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 15:00:17.000000 file_and_string_encryption-0.0.3/file_and_string_encryption.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-20 15:00:17.000000 file_and_string_encryption-0.0.3/file_and_string_encryption.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-05-20 15:00:17.000000 file_and_string_encryption-0.0.3/file_and_string_encryption.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 15:00:17.941234 file_and_string_encryption-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1739 2023-05-20 14:59:36.000000 file_and_string_encryption-0.0.3/setup.py
```

### Comparing `file_and_string_encryption-0.0.2/LICENSE` & `file_and_string_encryption-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `file_and_string_encryption-0.0.2/PKG-INFO` & `file_and_string_encryption-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file_and_string_encryption
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple encryption functions. Do not simply trust this code! Pay attention to how you handle sensitive information!
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `file_and_string_encryption-0.0.2/README.md` & `file_and_string_encryption-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `file_and_string_encryption-0.0.2/file_and_string_encryption/__init__.py` & `file_and_string_encryption-0.0.3/file_and_string_encryption/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,8 @@
     generate_password,
     get_random_key,
     hash_password_with_argon2,
     save_password_encrypted_key,
     verfiy_hashed_password_with_argon2,
 )
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
```

### Comparing `file_and_string_encryption-0.0.2/file_and_string_encryption/file_and_string_encryption.py` & `file_and_string_encryption-0.0.3/file_and_string_encryption/file_and_string_encryption.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,17 +39,17 @@
 
 def derive_key_from_password(
     password: bytes, salt: bytes, iterations: int = 100_000
 ) -> bytes:
     """Derives a key from a password using the `hashes.SHA256()` algorithm and `PBKDF2HMAC` from `cryptography.hazmat.primitives.kdf.pbkdf2`.
 
     Args:
-        password (bytes): Password to use in the form of bytes.
-        salt (bytes): The salt to give to PBKDF2HMAC. Could be generated by `secrets_token_bytes()` of the secrets module.
-        iterations (int, optional): The iterations to give to PBKDF2HMAC. Higher is better but takes longer. Defaults to 100_000.
+        - password (bytes): Password to use in the form of bytes.
+        - salt (bytes): The salt to give to PBKDF2HMAC. Could be generated by `secrets_token_bytes()` of the secrets module.
+        - iterations (int, optional): The iterations to give to PBKDF2HMAC. Higher is better but takes longer. Defaults to 100_000.
 
     Returns:
         bytes: key
     """
     kdf = PBKDF2HMAC(
         algorithm=hashes.SHA256(),
         length=32,
@@ -80,18 +80,18 @@
     enc_dir_path: str,
     keypath: str | None | bytes,
     error_if_target_is_file: bool = True,
 ):
     """Decrypts all files in a directory. Keeps the original directory structure.
 
     Args:
-        target_dir_path (str): Path for the decrypted directory.
-        enc_dir_path (str): Path to the encrypted directory.
-        keypath (str | None | bytes): Path to the key or alternativley the key itself.
-        error_if_target_is_file (bool, optional): Raise an exception if target_filepath is already a file. Defaults to True.
+        - target_dir_path (str): Path for the decrypted directory.
+        - enc_dir_path (str): Path to the encrypted directory.
+        - keypath (str | None | bytes): Path to the key or alternativley the key itself.
+        - error_if_target_is_file (bool, optional): Raise an exception if target_filepath is already a file. Defaults to True.
     """
     enc_dir_path = os.path.normpath(enc_dir_path)
 
     l1 = len(list(os.walk(enc_dir_path)))
 
     main_and_sub_progress_printer(
         0,
@@ -205,38 +205,38 @@
     return secret_msg
 
 
 def decrypt_string_with_password(token: bytes, password: str) -> str:
     """Decrypt a message aka token using a password.
 
     Args:
-        token (bytes): Your massage aka token.
-        password (str): The password.
+        - token (bytes): Your massage aka token.
+        - password (str): The password.
 
     Returns:
         str: The decrypted message.
     """
     decoded = b64d(token)
     salt, iter, token = decoded[:16], decoded[16:20], b64e(decoded[20:])
     iterations = int.from_bytes(iter, "big")
     key = derive_key_from_password(password.encode(), salt, iterations)
     pw = Fernet(key).decrypt(token).decode()
     return pw
 
 
-def encrypt_data(data: bytes, key: bytes = None) -> tuple(bytes, bytes):
+def encrypt_data(data: bytes, key: bytes = None) -> tuple(bytes):
     """Encypt data using a key. The data must be bytes. You can provide your own key if you want.
      Data can be converted to bytes using pickle. For convenience there is a `data_to_bytes_using_pickle` function which literally is `pickle.dumps(data)`.
 
     Args:
         - data (bytes): Data to encrypt.
         - key (bytes, optional): Specified key to use. Defaults to None.
 
     Returns:
-        tuple(bytes, bytes): Tuple containing the encrypted data and the key.
+        tuple(bytes): Tuple containing the encrypted data and the key.
     """
     if key == None:
         key = Fernet.generate_key()
     fernet = Fernet(key)
     encrypted = fernet.encrypt(data)
     return (encrypted, key)
 
@@ -248,20 +248,20 @@
     key: bytes = None,
     error_if_enc_is_file: bool = True,
     error_if_key_is_file: bool = True,
 ):
     """Uses `encrypt_file` for all files in a directory. Keeps the original directory structure.
 
     Args:
-        dir_path (str): Path to the directory to encrypt.
-        enc_dir_path (str): Path for the encrypted directory.
-        keypath (str | None, optional): Path for the key to be saved at, including the filename. Defaults to None, meaning it won't be saved.
-        key (bytes, optional): You can provide a specific key here. Defaults to None.
-        error_if_enc_is_file (bool, optional): Raise an exception if enc_filepath is already a file. Defaults to True.
-        error_if_key_is_file (bool, optional): Raise an exception if keypath is already a file. Defaults to True.
+        - dir_path (str): Path to the directory to encrypt.
+        - enc_dir_path (str): Path for the encrypted directory.
+        - keypath (str | None, optional): Path for the key to be saved at, including the filename. Defaults to None, meaning it won't be saved.
+        - key (bytes, optional): You can provide a specific key here. Defaults to None.
+        - error_if_enc_is_file (bool, optional): Raise an exception if enc_filepath is already a file. Defaults to True.
+        - error_if_key_is_file (bool, optional): Raise an exception if keypath is already a file. Defaults to True.
 
     Returns:
         bytes: The used key.
     """
     dir_path = os.path.normpath(dir_path)
     if key == None:
         key = get_random_key()
@@ -351,18 +351,18 @@
     keypath: str | None = None,
     error_if_enc_is_file: bool = True,
     error_if_key_is_file: bool = True,
 ):
     """Encrypt a file and save the encrypted key as a file. The key will be encrypted using a password and the function encrypt_string_with_password.
 
     Args:
-        filepath (str): The path to the file.
-        enc_filepath (str): The path for the encrypted file, including the filename.
-        keypath (str | None): The path for the unprotected key, including the filename. Defaults to None, meaning it won't be saved.
-        password (str): Your password.
+        - filepath (str): The path to the file.
+        - enc_filepath (str): The path for the encrypted file, including the filename.
+        - keypath (str | None): The path for the unprotected key, including the filename. Defaults to None, meaning it won't be saved.
+        - password (str): Your password.
     """
     if error_if_enc_is_file and os.path.isfile(enc_filepath):
         raise FileExistsError(
             f"There is already a file in the enc_filepath location.\n\tenc_filepath: {enc_filepath}"
         )
     if error_if_key_is_file and os.path.isfile(keypath):
         raise FileExistsError(
@@ -408,17 +408,17 @@
 
 def encrypt_string_with_password(
     message: str, password: str, iterations: int = 100000
 ) -> bytes:
     """Encrypt a message using a password. Iterations have an influence on the safety, the higher the stonger the longer the computation time.
 
     Args:
-        message (str): Message to encyrypt.
-        password (str): Password to use.
-        iterations (int, optional): Iterations have an influence on the safety, the higher the stonger the longer the computation time. Defaults to 100000.
+        - message (str): Message to encyrypt.
+        - password (str): Password to use.
+        - iterations (int, optional): Iterations have an influence on the safety, the higher the stonger the longer the computation time. Defaults to 100000.
 
     Returns:
         bytes: Encrypted message.
     """
     if type(message) != bytes:
         message = message.encode()
     salt = secrets_token_bytes(16)
@@ -459,16 +459,16 @@
     return Fernet.generate_key()
 
 
 def hash_password_with_argon2(password: str, argon2_default_rounds=55):
     """Hash a password using argon2. Hashed passwords can be used to ckeck wheather you know the real password with the help of the function `verfiy_hashed_password_with_argon2`.
 
     Args:
-        password (str): Password to hash.
-        argon2_default_rounds (int, optional): Rounds of the default argon2 hash function. Defaults to 55.
+        - password (str): Password to hash.
+        - argon2_default_rounds (int, optional): Rounds of the default argon2 hash function. Defaults to 55.
 
     Returns:
         str: Hashed password.
     """
     context = CryptContext(
         schemes=["argon2"],
         default="argon2",
@@ -507,18 +507,18 @@
     keypath: str,
     password: str | None = None,
     error_if_key_is_file: bool = True,
 ):
     """Save the key returned by an encryption function. Additionally you can encrypt the key by setting the password.
 
     Args:
-        key (bytes): Key returned by an encryption function.
-        keypath (str): The path for the key to be written to.
-        password (str | None, optional): A password to encrypt the key. Defaults to None.
-        error_if_key_is_file (bool, optional): Throw an exception if there already is a file. Defaults to True.
+        - key (bytes): Key returned by an encryption function.
+        - keypath (str): The path for the key to be written to.
+        - password (str | None, optional): A password to encrypt the key. Defaults to None.
+        - error_if_key_is_file (bool, optional): Throw an exception if there already is a file. Defaults to True.
 
     Raises:
         FileExistsError: If keypath is occupied.
     """
     if error_if_key_is_file and os.path.isfile(keypath):
         raise FileExistsError(
             f"There is already a file in the keypath location.\n\tkeypath: {keypath}"
@@ -536,17 +536,17 @@
 
 def verfiy_hashed_password_with_argon2(
     password: str, hashed_password, argon2_default_rounds=55
 ):
     """Verify a password using argon2. Input the hashed password and the password to be verified to check wheather you know the real password.
 
     Args:
-        password (str): Password to be verified.
-        hashed_password (bool): Hashed password.
-        argon2_default_rounds (int, optional): Rounds of the default argon2 hash function. Defaults to 55.
+        - password (str): Password to be verified.
+        - hashed_password (bool): Hashed password.
+        - argon2_default_rounds (int, optional): Rounds of the default argon2 hash function. Defaults to 55.
 
     Returns:
         bool: True if the password is correct, False otherwise.
     """
     _cryptcontext = CryptContext(
         schemes=["argon2"],
         default="argon2",
```

### Comparing `file_and_string_encryption-0.0.2/file_and_string_encryption.egg-info/PKG-INFO` & `file_and_string_encryption-0.0.3/file_and_string_encryption.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file-and-string-encryption
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple encryption functions. Do not simply trust this code! Pay attention to how you handle sensitive information!
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `file_and_string_encryption-0.0.2/setup.py` & `file_and_string_encryption-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 DESCRIPTION = "Simple encryption functions. Do not simply trust this code! Pay attention to how you handle sensitive information!"
 
 # Setting up
 setup(
     name="file_and_string_encryption",
     version=VERSION,
     author="André Herber",
```

