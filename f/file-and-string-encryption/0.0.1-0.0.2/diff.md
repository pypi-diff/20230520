# Comparing `tmp/file_and_string_encryption-0.0.1.tar.gz` & `tmp/file_and_string_encryption-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file_and_string_encryption-0.0.1.tar", last modified: Sat May 20 14:07:53 2023, max compression
+gzip compressed data, was "file_and_string_encryption-0.0.2.tar", last modified: Sat May 20 14:53:20 2023, max compression
```

## Comparing `file_and_string_encryption-0.0.1.tar` & `file_and_string_encryption-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 14:07:53.910111 file_and_string_encryption-0.0.1/
--rw-rw-rw-   0        0        0     1095 2023-01-07 18:45:09.000000 file_and_string_encryption-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       85 2023-05-14 19:46:17.000000 file_and_string_encryption-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1198 2023-05-20 14:07:53.909091 file_and_string_encryption-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      539 2023-05-14 19:59:38.000000 file_and_string_encryption-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 14:07:53.896380 file_and_string_encryption-0.0.1/file_and_string_encryption/
--rw-rw-rw-   0        0        0      473 2023-05-20 14:05:20.000000 file_and_string_encryption-0.0.1/file_and_string_encryption/__init__.py
--rw-rw-rw-   0        0        0    21259 2023-05-20 14:05:30.000000 file_and_string_encryption-0.0.1/file_and_string_encryption/file_and_string_encryption.py
-drwxrwxrwx   0        0        0        0 2023-05-20 14:07:53.907074 file_and_string_encryption-0.0.1/file_and_string_encryption.egg-info/
--rw-rw-rw-   0        0        0     1198 2023-05-20 14:07:53.000000 file_and_string_encryption-0.0.1/file_and_string_encryption.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-05-20 14:07:53.000000 file_and_string_encryption-0.0.1/file_and_string_encryption.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 14:07:53.000000 file_and_string_encryption-0.0.1/file_and_string_encryption.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-20 14:07:53.000000 file_and_string_encryption-0.0.1/file_and_string_encryption.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-05-20 14:07:53.000000 file_and_string_encryption-0.0.1/file_and_string_encryption.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 14:07:53.910111 file_and_string_encryption-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1739 2023-05-20 14:05:25.000000 file_and_string_encryption-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 14:53:20.045034 file_and_string_encryption-0.0.2/
+-rw-rw-rw-   0        0        0     1095 2023-01-07 18:45:09.000000 file_and_string_encryption-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       85 2023-05-14 19:46:17.000000 file_and_string_encryption-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1198 2023-05-20 14:53:20.043989 file_and_string_encryption-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      539 2023-05-14 19:59:38.000000 file_and_string_encryption-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 14:53:20.032888 file_and_string_encryption-0.0.2/file_and_string_encryption/
+-rw-rw-rw-   0        0        0      580 2023-05-20 14:51:56.000000 file_and_string_encryption-0.0.2/file_and_string_encryption/__init__.py
+-rw-rw-rw-   0        0        0    20347 2023-05-20 14:51:57.000000 file_and_string_encryption-0.0.2/file_and_string_encryption/file_and_string_encryption.py
+drwxrwxrwx   0        0        0        0 2023-05-20 14:53:20.042890 file_and_string_encryption-0.0.2/file_and_string_encryption.egg-info/
+-rw-rw-rw-   0        0        0     1198 2023-05-20 14:53:19.000000 file_and_string_encryption-0.0.2/file_and_string_encryption.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-05-20 14:53:19.000000 file_and_string_encryption-0.0.2/file_and_string_encryption.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 14:53:19.000000 file_and_string_encryption-0.0.2/file_and_string_encryption.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-20 14:53:19.000000 file_and_string_encryption-0.0.2/file_and_string_encryption.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-05-20 14:53:19.000000 file_and_string_encryption-0.0.2/file_and_string_encryption.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 14:53:20.045034 file_and_string_encryption-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1739 2023-05-20 14:51:56.000000 file_and_string_encryption-0.0.2/setup.py
```

### Comparing `file_and_string_encryption-0.0.1/LICENSE` & `file_and_string_encryption-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `file_and_string_encryption-0.0.1/PKG-INFO` & `file_and_string_encryption-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file_and_string_encryption
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple encryption functions. Do not simply trust this code! Pay attention to how you handle sensitive information!
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `file_and_string_encryption-0.0.1/README.md` & `file_and_string_encryption-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `file_and_string_encryption-0.0.1/file_and_string_encryption/file_and_string_encryption.py` & `file_and_string_encryption-0.0.2/file_and_string_encryption/file_and_string_encryption.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,115 +23,45 @@
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
 from passlib.context import CryptContext
 from easy_tasks import main_and_sub_progress_printer
 import pickle
 
 backend = default_backend()
-iterations = 100_000
 
 
-def derive_key_from_password(
-    password: bytes, salt: bytes, iterations: int = iterations
-) -> bytes:
-    """Derive a secret key from a given password and salt"""
-    kdf = PBKDF2HMAC(
-        algorithm=hashes.SHA256(),
-        length=32,
-        salt=salt,
-        iterations=iterations,
-        backend=backend,
-    )
-    return b64e(kdf.derive(password))
-
-
-def password_encrypt_bytes(
-    message: bytes, password: str, iterations: int = iterations
-) -> bytes:
-    salt = secrets_token_bytes(16)
-    key = derive_key_from_password(password.encode(), salt, iterations)
-    return b64e(
-        b"%b%b%b"
-        % (
-            salt,
-            iterations.to_bytes(4, "big"),
-            b64d(Fernet(key).encrypt(message)),
-        )
-    )
-
-
-def encrypt_string_with_password(
-    message: str, password: str, iterations: int = 100000
-) -> bytes:
-    """Encrypt a message using a password. Iterations have an influence on the safety, the higher the stonger the longer the computation time.
-
-    Args:
-        message (str): Message to encyrypt.
-        password (str): Password to use.
-        iterations (int, optional): Iterations have an influence on the safety, the higher the stonger the longer the computation time. Defaults to 100000.
-
-    Returns:
-        bytes: Encrypted message.
-    """
-    if type(message) != bytes:
-        message = message.encode()
-    salt = secrets_token_bytes(16)
-    key = derive_key_from_password(password.encode(), salt, iterations)
-    return b64e(
-        b"%b%b%b"
-        % (
-            salt,
-            iterations.to_bytes(4, "big"),
-            b64d(Fernet(key).encrypt(message)),
-        )
-    )
-
-
-def decrypt_string_with_password(token: bytes, password: str) -> str:
-    """Decrypt a message aka token using a password.
-
-    Args:
-        token (bytes): Your massage aka token.
-        password (str): The password.
-
-    Returns:
-        str: The decrypted message.
-    """
-    decoded = b64d(token)
-    salt, iter, token = decoded[:16], decoded[16:20], b64e(decoded[20:])
-    iterations = int.from_bytes(iter, "big")
-    key = derive_key_from_password(password.encode(), salt, iterations)
-    pw = Fernet(key).decrypt(token).decode()
-    return pw
+def bytes_to_data_using_pickle(data):
+    return pickle.loads(data)
 
 
 def data_to_bytes_using_pickle(data):
     return pickle.dumps(data)
 
 
-def bytes_to_data_using_pickle(data):
-    return pickle.loads(data)
-
-
-def encrypt_data(data: bytes, key: bytes = None) -> tuple(bytes, bytes):
-    """Encypt data using a key. The data must be bytes. You can provide your own key if you want.
-     Data can be converted to bytes using pickle. For convenience there is a `data_to_bytes_using_pickle` function which literally is `pickle.dumps(data)`.
+def derive_key_from_password(
+    password: bytes, salt: bytes, iterations: int = 100_000
+) -> bytes:
+    """Derives a key from a password using the `hashes.SHA256()` algorithm and `PBKDF2HMAC` from `cryptography.hazmat.primitives.kdf.pbkdf2`.
 
     Args:
-        - data (bytes): Data to encrypt.
-        - key (bytes, optional): Specified key to use. Defaults to None.
+        password (bytes): Password to use in the form of bytes.
+        salt (bytes): The salt to give to PBKDF2HMAC. Could be generated by `secrets_token_bytes()` of the secrets module.
+        iterations (int, optional): The iterations to give to PBKDF2HMAC. Higher is better but takes longer. Defaults to 100_000.
 
     Returns:
-        tuple(bytes, bytes): Tuple containing the encrypted data and the key.
+        bytes: key
     """
-    if key == None:
-        key = Fernet.generate_key()
-    fernet = Fernet(key)
-    encrypted = fernet.encrypt(data)
-    return (encrypted, key)
+    kdf = PBKDF2HMAC(
+        algorithm=hashes.SHA256(),
+        length=32,
+        salt=salt,
+        iterations=iterations,
+        backend=backend,
+    )
+    return b64e(kdf.derive(password))
 
 
 def decrypt_data(data: bytes, key: bytes) -> bytes:
     """Decypt data using a key.
 
     Args:
         - data (bytes): Encrypted data to decrypt.
@@ -141,43 +71,124 @@
         bytes: Decrypted data.
     """
     fernet = Fernet(key)
     decrypted = fernet.decrypt(data)
     return decrypted
 
 
-def password_decrypt_non_string(token: bytes, password: str):
-    decoded = b64d(token)
-    salt, iter, token = decoded[:16], decoded[16:20], b64e(decoded[20:])
-    iterations = int.from_bytes(iter, "big")
-    key = derive_key_from_password(password.encode(), salt, iterations)
-    pw = Fernet(key).decrypt(token).decode()
-    return pw
-
+def decrypt_directory(
+    target_dir_path: str,
+    enc_dir_path: str,
+    keypath: str | None | bytes,
+    error_if_target_is_file: bool = True,
+):
+    """Decrypts all files in a directory. Keeps the original directory structure.
 
-def encrypt_secret(secret, password: str):
-    """
-    -> encrypted_secret, salt
+    Args:
+        target_dir_path (str): Path for the decrypted directory.
+        enc_dir_path (str): Path to the encrypted directory.
+        keypath (str | None | bytes): Path to the key or alternativley the key itself.
+        error_if_target_is_file (bool, optional): Raise an exception if target_filepath is already a file. Defaults to True.
     """
-    salt = os.urandom(16)
+    enc_dir_path = os.path.normpath(enc_dir_path)
 
-    kdf = PBKDF2HMAC(
-        algorithm=hashes.SHA256(),
-        length=32,
-        salt=salt,
-        iterations=400000,
+    l1 = len(list(os.walk(enc_dir_path)))
+
+    main_and_sub_progress_printer(
+        0,
+        l1,
+        0,
+        0,
+        mainpre_string="Progress on dirpaths: ",
+        subpre_string="Progress on files in current dir: ",
     )
+    for main_index, (root, dirs, files) in enumerate(os.walk(enc_dir_path)):
+        sub_path = root.replace(enc_dir_path, "")
+        sub_path = sub_path.lstrip("\\")
+        l2 = len(files)
+        for sub_index, f in enumerate(files):
+            fp = os.path.join(root, f)
+            nfp = os.path.join(target_dir_path, sub_path, f)
+            decrypt_file(nfp, fp, keypath, error_if_target_is_file)
+            main_and_sub_progress_printer(
+                main_index + 1,
+                l1,
+                sub_index + 1,
+                l2,
+                mainpre_string="Progress on dirpaths: ",
+                subpre_string="Progress on files in current dir: ",
+            )
 
-    key = b64e(kdf.derive(password.encode()))
 
-    f = Fernet(key)
+def decrypt_file(
+    to_be_filepath: str,
+    enc_filepath: str,
+    keypath: str | bytes,
+    error_if_target_is_file: bool = True,
+):
+    """Decrypt a file using the generated key. The file was decrypted with encrypt_file.
 
-    encrypted_secret = f.encrypt(secret.encode())
+    Args:
+        - to_be_filepath (str): The path at which the file shall be generated, including the filename.
+        - enc_filepath (str): The path to the encrypted file.
+        - keypath (str | bytes): The path to the key or alternativley the key itself.
+    """
+    if error_if_target_is_file and os.path.isfile(to_be_filepath):
+        raise FileExistsError(
+            f"There is already a file in the to_be_filepath location.\n\tto_be_filepath: {to_be_filepath}"
+        )
+    if isinstance(keypath, str):
+        with open(keypath, "rb") as f:
+            key = f.read()
+    else:
+        key = keypath
+    fernet = Fernet(key)
+    with open(enc_filepath, "rb") as encrypted_file:
+        encrypted = encrypted_file.read()
+    decrypted = fernet.decrypt(encrypted)
+    filename, fileext = os.path.splitext(os.path.basename(to_be_filepath))
+    basepath = os.path.dirname(to_be_filepath)
+    if not os.path.isdir(basepath):
+        os.makedirs(basepath)
+    pre_filepath = os.path.join(basepath, filename)
+    with open(pre_filepath, "wb") as decrypted_file:
+        decrypted_file.write(decrypted)
+    if os.path.isdir(to_be_filepath):
+        os.removedirs(to_be_filepath)
+    os.rename(pre_filepath, to_be_filepath)
 
-    return encrypted_secret, salt
+
+def decrypt_file_with_password(
+    to_be_filepath: str, enc_filepath: str, keypath: str, password: str
+):
+    """Decrypt a file using a password. The file was decrypted using encrypt_file_with_password.
+
+    Args:
+        - to_be_filepath (str): The path at which the file shall be generated, including the filename.
+        - enc_filepath (str): The path to the encrypted file.
+        - keypath (str): The path to the encrypted key.
+        - password (str): The password to decrypt the actual key.
+    """
+    with open(keypath, "rb") as f:
+        enc_key = f.read()
+    key = decrypt_string_with_password(enc_key, password)
+    fernet = Fernet(key)
+    with open(enc_filepath, "rb") as encrypted_file:
+        encrypted = encrypted_file.read()
+    decrypted = fernet.decrypt(encrypted)
+    filename, fileext = os.path.splitext(os.path.basename(to_be_filepath))
+    basepath = os.path.dirname(to_be_filepath)
+    if not os.path.isdir(basepath):
+        os.makedirs(basepath)
+    pre_filepath = os.path.join(basepath, filename)
+    with open(pre_filepath, "wb") as decrypted_file:
+        decrypted_file.write(decrypted)
+    if os.path.isdir(to_be_filepath):
+        os.removedirs(to_be_filepath)
+    os.rename(pre_filepath, to_be_filepath)
 
 
 def decrypt_secret(encrypted_secret, password: str, salt):
     kdf = PBKDF2HMAC(
         algorithm=hashes.SHA256(),
         length=32,
         salt=salt,
@@ -190,166 +201,151 @@
 
     secret_msg = f.decrypt(encrypted_secret)
     secret_msg = secret_msg.decode()
 
     return secret_msg
 
 
-def generate_password(length=16):
-    chars = ascii_letters + punctuation + digits
-    password = str()
-    while True:
-        password = "".join(secrets_choice(chars) for i in range(length))
-        if (
-            any(c.islower() for c in password)
-            and any(c.isupper() for c in password)
-            # and sum(c.isdigit() for c in password) >= 3
-            and any(c.isdigit() for c in password)
-            and any(punctuation)
-        ):
-            break
-
-    return password
-
-
-def encrypt_image_alt(img_path: str, target_dir: str, password: str):
-    BildName = os.path.basename(img_path)
-    key = Fernet.generate_key()
-    s_key = encrypt_string_with_password(key, password)
-    pfad = os.path.join(target_dir, f"{BildName}_key.txt")
-    with open(pfad, mode="wb") as keyValue:  # target_dir + f"/{BildName}_key.txt"
-        keyValue.write(s_key)
-
-    # Encrypt image
-    with open(img_path, "rb") as f:
-        content = f.read()
-    hexValue = binascii.hexlify(content)
-
-    f = Fernet(key)
-    encHexVal = f.encrypt(hexValue)
-
-    pfad = os.path.join(target_dir, f"{BildName}_encryptedHex.txt")
-    with open(
-        pfad, mode="wb"
-    ) as hexValueFile:  # target_dir + f"/{BildName}_encryptedHex.txt"
-        hexValueFile.write(encHexVal)
-
-    # Verification checks
-    a = f.decrypt(encHexVal)
-
-    # hexed bytes is same encoding as 'ascii'
-    pfad = os.path.join(target_dir, f"{BildName}_realValue.txt")
-    with open(pfad, mode="wb") as writeHex:  # target_dir + f"/{BildName}_realValue.txt"
-        originalHex = writeHex.write(hexValue)
-
-    with open(
-        pfad, mode="r", encoding="ascii"
-    ) as reading:  # target_dir + f"/{BildName}_realValue.txt"
-        realValue = reading.read()
-
-
-def decrypt_image_alt(
-    img_name: str, source_dir: str, password: str, ZielOrdner: str = ""
-):
-    if ZielOrdner == "":
-        ZielOrdner = source_dir
-
-    pfad = os.path.join(source_dir, f"{img_name}_key.txt")
-    with open(pfad, mode="rb") as keyValue:
-        s_key = keyValue.read()
-        key = decrypt_string_with_password(s_key, password)
-        f = Fernet(key)
-
-    pfad = os.path.join(source_dir, f"{img_name}_encryptedHex.txt")
-    with open(pfad, mode="rb") as imageHexValue:
-        encHexValue = imageHexValue.read()
-    hexValue = f.decrypt(encHexValue)
-    binValue = binascii.unhexlify(hexValue)
-
-    pfad = os.path.join(source_dir, f"{img_name}_realValue.txt")
-    with open(pfad, mode="rb") as compare:
-        realContents = compare.read()
-
-    pfad = os.path.join(ZielOrdner, img_name)
-    with open(pfad, "wb") as file:
-        file.write(binValue)
+def decrypt_string_with_password(token: bytes, password: str) -> str:
+    """Decrypt a message aka token using a password.
 
+    Args:
+        token (bytes): Your massage aka token.
+        password (str): The password.
 
-def encrypt_image_with_password(img_path: str, target_dir: str, password: str):
-    BildName = os.path.basename(img_path)
+    Returns:
+        str: The decrypted message.
+    """
+    decoded = b64d(token)
+    salt, iter, token = decoded[:16], decoded[16:20], b64e(decoded[20:])
+    iterations = int.from_bytes(iter, "big")
+    key = derive_key_from_password(password.encode(), salt, iterations)
+    pw = Fernet(key).decrypt(token).decode()
+    return pw
 
-    # key
-    key = Fernet.generate_key()
-    s_key = encrypt_string_with_password(key, password)
-    pfad = os.path.join(target_dir, f"{BildName}_key.txt")
-    with open(pfad, mode="wb") as keyValue:
-        keyValue.write(s_key)
-
-    # Encrypt image
-    with open(img_path, "rb") as f:
-        content = f.read()
-    hexValue = binascii.hexlify(content)
 
-    f = Fernet(key)
-    encHexVal = f.encrypt(hexValue)
+def encrypt_data(data: bytes, key: bytes = None) -> tuple(bytes, bytes):
+    """Encypt data using a key. The data must be bytes. You can provide your own key if you want.
+     Data can be converted to bytes using pickle. For convenience there is a `data_to_bytes_using_pickle` function which literally is `pickle.dumps(data)`.
 
-    pfad = os.path.join(target_dir, f"{BildName}_encryptedHex.txt")
-    with open(pfad, mode="wb") as hexValueFile:
-        hexValueFile.write(encHexVal)
+    Args:
+        - data (bytes): Data to encrypt.
+        - key (bytes, optional): Specified key to use. Defaults to None.
 
-    # Verification checks
-    a = f.decrypt(encHexVal)
+    Returns:
+        tuple(bytes, bytes): Tuple containing the encrypted data and the key.
+    """
+    if key == None:
+        key = Fernet.generate_key()
+    fernet = Fernet(key)
+    encrypted = fernet.encrypt(data)
+    return (encrypted, key)
 
 
-def decrypt_image_with_password(
-    to_be_img_path: str, encrypted_path: str, key_path: str, password: str
+def encrypt_directory(
+    dir_path: str,
+    enc_dir_path: str,
+    keypath: str | None = None,
+    key: bytes = None,
+    error_if_enc_is_file: bool = True,
+    error_if_key_is_file: bool = True,
 ):
-    with open(key_path, mode="rb") as keyValue:
-        s_key = keyValue.read()
-        key = decrypt_string_with_password(s_key, password)
-        f = Fernet(key)
+    """Uses `encrypt_file` for all files in a directory. Keeps the original directory structure.
 
-    with open(encrypted_path, mode="rb") as imageHexValue:
-        encHexValue = imageHexValue.read()
-    hexValue = f.decrypt(encHexValue)
-    binValue = binascii.unhexlify(hexValue)
+    Args:
+        dir_path (str): Path to the directory to encrypt.
+        enc_dir_path (str): Path for the encrypted directory.
+        keypath (str | None, optional): Path for the key to be saved at, including the filename. Defaults to None, meaning it won't be saved.
+        key (bytes, optional): You can provide a specific key here. Defaults to None.
+        error_if_enc_is_file (bool, optional): Raise an exception if enc_filepath is already a file. Defaults to True.
+        error_if_key_is_file (bool, optional): Raise an exception if keypath is already a file. Defaults to True.
 
-    with open(to_be_img_path, "wb") as file:
-        file.write(binValue)
+    Returns:
+        bytes: The used key.
+    """
+    dir_path = os.path.normpath(dir_path)
+    if key == None:
+        key = get_random_key()
 
+    l1 = len(list(os.walk(dir_path)))
 
-def hash_password_argon2(password: str, argon2_default_rounds=55):
-    context = CryptContext(
-        schemes=["argon2"],
-        default="argon2",
-        argon2__default_rounds=argon2_default_rounds,
+    main_and_sub_progress_printer(
+        0,
+        l1,
+        0,
+        0,
+        mainpre_string="Progress on dirpaths: ",
+        subpre_string="Progress on files in current dir: ",
     )
-    hashed_password = context.hash(password)
-    return hashed_password
+    for main_index, (root, dirs, files) in enumerate(os.walk(dir_path)):
+        sub_path = root.replace(dir_path, "")
+        sub_path = sub_path.lstrip("\\")
+        l2 = len(files)
+        for sub_index, f in enumerate(files):
+            fp = os.path.join(root, f)
+            nfp = os.path.join(enc_dir_path, sub_path, f)
+            encrypt_file(
+                fp, nfp, keypath, key, error_if_enc_is_file, error_if_key_is_file
+            )
+            main_and_sub_progress_printer(
+                main_index + 1,
+                l1,
+                sub_index + 1,
+                l2,
+                mainpre_string="Progress on dirpaths: ",
+                subpre_string="Progress on files in current dir: ",
+            )
+    return key
 
 
-def verfiy_hashed_password_argon2(
-    password: str, hashed_password, argon2_default_rounds=55
+def encrypt_file(
+    filepath: str,
+    enc_filepath: str,
+    keypath: str | None = None,
+    key: bytes = None,
+    error_if_enc_is_file: bool = True,
+    error_if_key_is_file: bool = True,
 ):
-    _cryptcontext = CryptContext(
-        schemes=["argon2"],
-        default="argon2",
-        argon2__default_rounds=argon2_default_rounds,
-    )
-    crypt_check = _cryptcontext.verify(password, hashed_password)
-    return crypt_check
-
+    """Encrypt a file and save the unprotected key as a file under the specified location.
 
-def get_random_key():
-    """Generate a random key.
+    Args:
+        - filepath (str): The path to the file.
+        - enc_filepath (str): The path for the encrypted file, including the filename.
+        - keypath (str | None): The path for the unprotected key, including the filename. Defaults to None, meaning it won't be saved.
+        - key (bytes, optional): You can reuse the key of earlier encryptions or generate a key using the function get_random_key. Defaults to None.
+        - error_if_enc_is_file (bool, optional): Raise an exception if enc_filepath is already a file. Defaults to True.
+        - error_if_key_is_file (bool, optional): Raise an exception if keypath is already a file. Defaults to True.
 
     Returns:
         bytes: The key generated by Fernet.generate_key()
     """
-    return Fernet.generate_key()
+    if error_if_key_is_file and os.path.isfile(enc_filepath):
+        raise FileExistsError(
+            f"There is already a file in the enc_filepath location.\n\tenc_filepath: {enc_filepath}"
+        )
+    if key == None:
+        key = Fernet.generate_key()
+    if not os.path.isdir(os.path.dirname(enc_filepath)):
+        os.makedirs(os.path.dirname(enc_filepath))
+    if keypath != None:
+        if not os.path.isdir(os.path.dirname(keypath)):
+            os.makedirs(os.path.dirname(keypath))
+        if error_if_enc_is_file and os.path.isfile(keypath):
+            raise FileExistsError(
+                f"There is already a file in the keypath location.\n\tkeypath: {keypath}"
+            )
+        with open(keypath, "wb") as f:
+            f.write(key)
+    fernet = Fernet(key)
+    with open(filepath, "rb") as original_file:
+        original = original_file.read()
+    encrypted = fernet.encrypt(original)
+    with open(enc_filepath, "wb") as encrypted_file:
+        encrypted_file.write(encrypted)
+    return key
 
 
 def encrypt_file_with_password(
     filepath: str,
     enc_filepath: str,
     password: str,
     keypath: str | None = None,
@@ -384,209 +380,133 @@
     with open(filepath, "rb") as original_file:
         original = original_file.read()
     encrypted = fernet.encrypt(original)
     with open(enc_filepath, "wb") as encrypted_file:
         encrypted_file.write(encrypted)
 
 
-def encrypt_file(
-    filepath: str,
-    enc_filepath: str,
-    keypath: str | None = None,
-    key: bytes = None,
-    error_if_enc_is_file: bool = True,
-    error_if_key_is_file: bool = True,
-):
-    """Encrypt a file and save the unprotected key as a file under the specified location.
+def encrypt_secret(secret, password: str):
+    """
+    -> encrypted_secret, salt
+    """
+    salt = os.urandom(16)
+
+    kdf = PBKDF2HMAC(
+        algorithm=hashes.SHA256(),
+        length=32,
+        salt=salt,
+        iterations=400000,
+    )
+
+    key = b64e(kdf.derive(password.encode()))
+
+    f = Fernet(key)
+
+    encrypted_secret = f.encrypt(secret.encode())
+
+    return encrypted_secret, salt
+
+
+def encrypt_string_with_password(
+    message: str, password: str, iterations: int = 100000
+) -> bytes:
+    """Encrypt a message using a password. Iterations have an influence on the safety, the higher the stonger the longer the computation time.
 
     Args:
-        filepath (str): The path to the file.
-        enc_filepath (str): The path for the encrypted file, including the filename.
-        keypath (str | None): The path for the unprotected key, including the filename. Defaults to None, meaning it won't be saved.
-        key (bytes, optional): You can reuse the key of earlier encryptions or generate a key using the function get_random_key. Defaults to None.
-        error_if_enc_is_file (bool): Raise an exception if enc_filepath is already a file.
-        error_if_key_is_file (bool): Raise an exception if keypath is already a file.
+        message (str): Message to encyrypt.
+        password (str): Password to use.
+        iterations (int, optional): Iterations have an influence on the safety, the higher the stonger the longer the computation time. Defaults to 100000.
 
     Returns:
-        bytes: The key generated by Fernet.generate_key()
+        bytes: Encrypted message.
     """
-    if error_if_key_is_file and os.path.isfile(enc_filepath):
-        raise FileExistsError(
-            f"There is already a file in the enc_filepath location.\n\tenc_filepath: {enc_filepath}"
+    if type(message) != bytes:
+        message = message.encode()
+    salt = secrets_token_bytes(16)
+    key = derive_key_from_password(password.encode(), salt, iterations)
+    return b64e(
+        b"%b%b%b"
+        % (
+            salt,
+            iterations.to_bytes(4, "big"),
+            b64d(Fernet(key).encrypt(message)),
         )
-    if key == None:
-        key = Fernet.generate_key()
-    if not os.path.isdir(os.path.dirname(enc_filepath)):
-        os.makedirs(os.path.dirname(enc_filepath))
-    if keypath != None:
-        if not os.path.isdir(os.path.dirname(keypath)):
-            os.makedirs(os.path.dirname(keypath))
-        if error_if_enc_is_file and os.path.isfile(keypath):
-            raise FileExistsError(
-                f"There is already a file in the keypath location.\n\tkeypath: {keypath}"
-            )
-        with open(keypath, "wb") as f:
-            f.write(key)
-    fernet = Fernet(key)
-    with open(filepath, "rb") as original_file:
-        original = original_file.read()
-    encrypted = fernet.encrypt(original)
-    with open(enc_filepath, "wb") as encrypted_file:
-        encrypted_file.write(encrypted)
-    return key
+    )
 
 
-def decrypt_file_with_password(
-    to_be_filepath: str, enc_filepath: str, keypath: str, password: str
-):
-    """Decrypt a file using a password. The file was decrypted using encrypt_file_with_password.
+def generate_password(length=16):
+    chars = ascii_letters + punctuation + digits
+    password = str()
+    while True:
+        password = "".join(secrets_choice(chars) for i in range(length))
+        if (
+            any(c.islower() for c in password)
+            and any(c.isupper() for c in password)
+            # and sum(c.isdigit() for c in password) >= 3
+            and any(c.isdigit() for c in password)
+            and any(punctuation)
+        ):
+            break
 
-    Args:
-        to_be_filepath (str): The path at which the file shall be generated, including the filename.
-        enc_filepath (str): The path to the encrypted file.
-        keypath (str): The path to the encrypted key.
-        password (str): The password to decrypt the actual key.
-    """
-    with open(keypath, "rb") as f:
-        enc_key = f.read()
-    key = decrypt_string_with_password(enc_key, password)
-    fernet = Fernet(key)
-    with open(enc_filepath, "rb") as encrypted_file:
-        encrypted = encrypted_file.read()
-    decrypted = fernet.decrypt(encrypted)
-    filename, fileext = os.path.splitext(os.path.basename(to_be_filepath))
-    basepath = os.path.dirname(to_be_filepath)
-    if not os.path.isdir(basepath):
-        os.makedirs(basepath)
-    pre_filepath = os.path.join(basepath, filename)
-    with open(pre_filepath, "wb") as decrypted_file:
-        decrypted_file.write(decrypted)
-    if os.path.isdir(to_be_filepath):
-        os.removedirs(to_be_filepath)
-    os.rename(pre_filepath, to_be_filepath)
+    return password
 
 
-def decrypt_file(
-    to_be_filepath: str,
-    enc_filepath: str,
-    keypath: str | bytes,
-    error_if_target_is_file: bool = True,
-):
-    """Decrypt a file using the generated key. The file was decrypted with encrypt_file.
+def get_random_key():
+    """Generate a random key.
 
-    Args:
-        to_be_filepath (str): The path at which the file shall be generated, including the filename.
-        enc_filepath (str): The path to the encrypted file.
-        keypath (str | bytes): The path to the key or alternativley the key itself.
+    Returns:
+        bytes: The key generated by Fernet.generate_key()
     """
-    if error_if_target_is_file and os.path.isfile(to_be_filepath):
-        raise FileExistsError(
-            f"There is already a file in the to_be_filepath location.\n\tto_be_filepath: {to_be_filepath}"
-        )
-    if isinstance(keypath, str):
-        with open(keypath, "rb") as f:
-            key = f.read()
-    else:
-        key = keypath
-    fernet = Fernet(key)
-    with open(enc_filepath, "rb") as encrypted_file:
-        encrypted = encrypted_file.read()
-    decrypted = fernet.decrypt(encrypted)
-    filename, fileext = os.path.splitext(os.path.basename(to_be_filepath))
-    basepath = os.path.dirname(to_be_filepath)
-    if not os.path.isdir(basepath):
-        os.makedirs(basepath)
-    pre_filepath = os.path.join(basepath, filename)
-    with open(pre_filepath, "wb") as decrypted_file:
-        decrypted_file.write(decrypted)
-    if os.path.isdir(to_be_filepath):
-        os.removedirs(to_be_filepath)
-    os.rename(pre_filepath, to_be_filepath)
+    return Fernet.generate_key()
 
 
-def encrypt_directory(
-    dir_path: str,
-    enc_dir_path: str,
-    keypath: str | None = None,
-    key: bytes = None,
-    error_if_enc_is_file: bool = True,
-    error_if_key_is_file: bool = True,
-):
-    dir_path = os.path.normpath(dir_path)
-    if key == None:
-        key = get_random_key()
+def hash_password_with_argon2(password: str, argon2_default_rounds=55):
+    """Hash a password using argon2. Hashed passwords can be used to ckeck wheather you know the real password with the help of the function `verfiy_hashed_password_with_argon2`.
 
-    l1 = len(list(os.walk(dir_path)))
+    Args:
+        password (str): Password to hash.
+        argon2_default_rounds (int, optional): Rounds of the default argon2 hash function. Defaults to 55.
 
-    main_and_sub_progress_printer(
-        0,
-        l1,
-        0,
-        0,
-        mainpre_string="Progress on dirpaths: ",
-        subpre_string="Progress on files in current dir: ",
+    Returns:
+        str: Hashed password.
+    """
+    context = CryptContext(
+        schemes=["argon2"],
+        default="argon2",
+        argon2__default_rounds=argon2_default_rounds,
     )
-    for main_index, (root, dirs, files) in enumerate(os.walk(dir_path)):
-        sub_path = root.replace(dir_path, "")
-        sub_path = sub_path.lstrip("\\")
-        l2 = len(files)
-        for sub_index, f in enumerate(files):
-            fp = os.path.join(root, f)
-            nfp = os.path.join(enc_dir_path, sub_path, f)
-            encrypt_file(
-                fp, nfp, keypath, key, error_if_enc_is_file, error_if_key_is_file
-            )
-            main_and_sub_progress_printer(
-                main_index + 1,
-                l1,
-                sub_index + 1,
-                l2,
-                mainpre_string="Progress on dirpaths: ",
-                subpre_string="Progress on files in current dir: ",
-            )
-    return key
+    hashed_password = context.hash(password)
+    return hashed_password
 
 
-def decrypt_directory(
-    target_dir_path: str,
-    enc_dir_path: str,
-    keypath: str | None | bytes = None,
-    error_if_target_is_file: bool = True,
-):
-    enc_dir_path = os.path.normpath(enc_dir_path)
+def password_decrypt_non_string(token: bytes, password: str):
+    decoded = b64d(token)
+    salt, iter, token = decoded[:16], decoded[16:20], b64e(decoded[20:])
+    iterations = int.from_bytes(iter, "big")
+    key = derive_key_from_password(password.encode(), salt, iterations)
+    pw = Fernet(key).decrypt(token).decode()
+    return pw
 
-    l1 = len(list(os.walk(enc_dir_path)))
 
-    main_and_sub_progress_printer(
-        0,
-        l1,
-        0,
-        0,
-        mainpre_string="Progress on dirpaths: ",
-        subpre_string="Progress on files in current dir: ",
+def password_encrypt_bytes(
+    message: bytes, password: str, iterations: int = 100_000
+) -> bytes:
+    salt = secrets_token_bytes(16)
+    key = derive_key_from_password(password.encode(), salt, iterations)
+    return b64e(
+        b"%b%b%b"
+        % (
+            salt,
+            iterations.to_bytes(4, "big"),
+            b64d(Fernet(key).encrypt(message)),
+        )
     )
-    for main_index, (root, dirs, files) in enumerate(os.walk(enc_dir_path)):
-        sub_path = root.replace(enc_dir_path, "")
-        sub_path = sub_path.lstrip("\\")
-        l2 = len(files)
-        for sub_index, f in enumerate(files):
-            fp = os.path.join(root, f)
-            nfp = os.path.join(target_dir_path, sub_path, f)
-            decrypt_file(nfp, fp, keypath, error_if_target_is_file)
-            main_and_sub_progress_printer(
-                main_index + 1,
-                l1,
-                sub_index + 1,
-                l2,
-                mainpre_string="Progress on dirpaths: ",
-                subpre_string="Progress on files in current dir: ",
-            )
 
 
-def save_key(
+def save_password_encrypted_key(
     key: bytes,
     keypath: str,
     password: str | None = None,
     error_if_key_is_file: bool = True,
 ):
     """Save the key returned by an encryption function. Additionally you can encrypt the key by setting the password.
 
@@ -610,14 +530,36 @@
     keypath_parent = os.path.dirname(keypath)
     if not os.path.isdir(keypath_parent):
         os.makedirs(keypath_parent)
     with open(keypath, "wb") as f:
         f.write(encryptet_key)
 
 
+def verfiy_hashed_password_with_argon2(
+    password: str, hashed_password, argon2_default_rounds=55
+):
+    """Verify a password using argon2. Input the hashed password and the password to be verified to check wheather you know the real password.
+
+    Args:
+        password (str): Password to be verified.
+        hashed_password (bool): Hashed password.
+        argon2_default_rounds (int, optional): Rounds of the default argon2 hash function. Defaults to 55.
+
+    Returns:
+        bool: True if the password is correct, False otherwise.
+    """
+    _cryptcontext = CryptContext(
+        schemes=["argon2"],
+        default="argon2",
+        argon2__default_rounds=argon2_default_rounds,
+    )
+    crypt_check = _cryptcontext.verify(password, hashed_password)
+    return crypt_check
+
+
 if __name__ == "__main__":
     # encrypt_directory(
     #     r"Code Sammlung\Passwort",
     #     r"C:\Users\Creed\OneDrive\Schul-Dokumente\Programmieren\Python\Code Sammlung\mehr\test",
     #     r"C:\Users\Creed\OneDrive\Schul-Dokumente\Programmieren\Python\Code Sammlung\mehr\KEY",
     # )
     decrypt_directory(
```

### Comparing `file_and_string_encryption-0.0.1/file_and_string_encryption.egg-info/PKG-INFO` & `file_and_string_encryption-0.0.2/file_and_string_encryption.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file-and-string-encryption
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple encryption functions. Do not simply trust this code! Pay attention to how you handle sensitive information!
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `file_and_string_encryption-0.0.1/setup.py` & `file_and_string_encryption-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 DESCRIPTION = "Simple encryption functions. Do not simply trust this code! Pay attention to how you handle sensitive information!"
 
 # Setting up
 setup(
     name="file_and_string_encryption",
     version=VERSION,
     author="André Herber",
```

