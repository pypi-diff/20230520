# Comparing `tmp/Cryptem-0.0.3.tar.gz` & `tmp/Cryptem-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Cryptem-0.0.3.tar", last modified: Wed Oct 19 12:32:01 2022, max compression
+gzip compressed data, was "Cryptem-0.0.4.tar", last modified: Sat May 20 09:29:52 2023, max compression
```

## Comparing `Cryptem-0.0.3.tar` & `Cryptem-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2022-10-19 12:32:01.482639 Cryptem-0.0.3/
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2022-10-19 12:32:01.482639 Cryptem-0.0.3/Cryptem.egg-info/
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     7641 2022-10-19 12:32:01.000000 Cryptem-0.0.3/Cryptem.egg-info/PKG-INFO
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)      198 2022-10-19 12:32:01.000000 Cryptem-0.0.3/Cryptem.egg-info/SOURCES.txt
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)        1 2022-10-19 12:32:01.000000 Cryptem-0.0.3/Cryptem.egg-info/dependency_links.txt
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       31 2022-10-19 12:32:01.000000 Cryptem-0.0.3/Cryptem.egg-info/requires.txt
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)        8 2022-10-19 12:32:01.000000 Cryptem-0.0.3/Cryptem.egg-info/top_level.txt
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     7304 2022-10-19 12:21:15.000000 Cryptem-0.0.3/Cryptem.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     7641 2022-10-19 12:32:01.482639 Cryptem-0.0.3/PKG-INFO
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     6101 2022-08-06 05:09:46.000000 Cryptem-0.0.3/README.md
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)      104 2022-08-06 05:09:46.000000 Cryptem-0.0.3/pyproject.toml
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       38 2022-10-19 12:32:01.482639 Cryptem-0.0.3/setup.cfg
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)      907 2022-10-19 12:22:07.000000 Cryptem-0.0.3/setup.py
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-05-20 09:29:52.148277 Cryptem-0.0.4/
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-05-20 09:29:52.148277 Cryptem-0.0.4/Cryptem.egg-info/
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6566 2023-05-20 09:29:51.000000 Cryptem-0.0.4/Cryptem.egg-info/PKG-INFO
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      198 2023-05-20 09:29:52.000000 Cryptem-0.0.4/Cryptem.egg-info/SOURCES.txt
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)        1 2023-05-20 09:29:51.000000 Cryptem-0.0.4/Cryptem.egg-info/dependency_links.txt
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)       31 2023-05-20 09:29:51.000000 Cryptem-0.0.4/Cryptem.egg-info/requires.txt
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)        8 2023-05-20 09:29:51.000000 Cryptem-0.0.4/Cryptem.egg-info/top_level.txt
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     7689 2023-05-20 09:27:49.000000 Cryptem-0.0.4/Cryptem.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     6566 2023-05-20 09:29:52.148277 Cryptem-0.0.4/PKG-INFO
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6021 2022-10-19 12:50:25.000000 Cryptem-0.0.4/README.md
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      104 2022-08-06 05:09:46.000000 Cryptem-0.0.4/pyproject.toml
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       38 2023-05-20 09:29:52.148277 Cryptem-0.0.4/setup.cfg
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      907 2023-05-20 09:28:59.000000 Cryptem-0.0.4/setup.py
```

### Comparing `Cryptem-0.0.3/Cryptem.egg-info/PKG-INFO` & `Cryptem-0.0.4/Cryptem.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,137 +1,138 @@
 Metadata-Version: 2.1
 Name: Cryptem
-Version: 0.0.3
+Version: 0.0.4
 Summary: Cryptographic applications library based on elliptic curve cryptography
 Home-page: https://ipfs.io/ipns/k2k4r8ld8q6344t8dop0rwuk8f3vhpo42un6zrnrffogaayr7xv59p83
 Author: emendir
 License: UNKNOWN
 Project-URL: Source Code on IPFS, https://ipfs.io/ipns/k2k4r8ld8q6344t8dop0rwuk8f3vhpo42un6zrnrffogaayr7xv59p83
-Description: An easy-to-use object-oriented API for working with cryptography: encrypting/decrypting data and files as well as signing data and verifying signatures.  
-        Can be used for asymmetric and symmetric cryptography, signature verification, and supports password-like private keys.
-        Uses elliptic curve cryptography for the data encryption and data signing, the file encryption however uses AES.  
-        Built on the eciespy, cryptography, coincurve and hashlib modules.
-        
-        ## Classes `Crypt` and `Encryptor`:
-        The `Crypt` class is a cryptographic tool used by the holder of a private key for encrypting and signing data. It's counterpart is the `Encryptor` class, which using a specific public key can ecrypt data and verify signatures.  
-        These classes also include functionality for more efficient file encryption using AES secret keys, where the secret key is automatically asymmetrically encrypted and embedded in the symmetrically encrypted file. This means that the usage of this file encryption system is asymmetric (private & public key), although the encryption of the file itself is not.   
-        Can be used for single-session asymmetric (public-key/private-key) cryptography
-        as well as for (optionally password secured) multi-session (i.e. reused keys) asymmetric (public-key/private-key) or symetric (private-key-only) cryptography.  
-        __Single-session__ means the keys are used only as long as the Crypt instance exists, so when the program is restarted different keys are used.  
-        __Multi-session__ means that the same keys can be reused after restarting the program, a simplified form of the private key must be memorised by the user as a password (although you can of course use a longer key-like string instead of a typical password).
-        
-        # Encryption
-        ## Usage:
-        `from Cryptem import Crypt`
-        ### - __Single-Session Asymetric Encryption__ (public-key and private-key):
-        Communication Receiver:
-          
-            crypt = Crypt() # create Crypt object with new random public and private keys
-            public_key = crypt.public_key # read public key
-        
-          Give `public_key` (the public key) to Sender (the code in the program below).
-        
-        Communication Sender/Encryptor:
-          
-            # Object-Oriented Approach:
-            from Cryptem import Encryptor
-            encryptor = Encryptor(public_key)  # crete Encryptor object with Receiver's public key
-            cipher = encryptor.Encrypt("Hello there!".encode('utf-8')) # encrypt a message
-            
-            # Functional Approach:
-            cipher = Encrypt("Hello there!".encode('utf-8'), public_key)
-        
-          Transmit `cipher` to Receiver.
-        
-        Communication Receiver:
-          
-            # continued from above
-            plaintext = crypt.Decrypt(cipher).decode('utf-8') # decrypt message
-        
-        ### - __Multi-Session Asymetric Encryption__ (public-key and private-key):  
-        Communication Receiver:
-            
-            crypt = Crypt("mypassword")   # create Crypt object with a password, from which private and ublic keys are generated
-            public_key = crypt.public_key # read public key
-              
-        Give `public_key` to Sender.
-        
-        Communication Sender/Encryptor:
-            
-            encryptor = Encryptor(public_key)  # crete Encryptor object with Receiver's public key
-            cipher = encryptor.Encrypt("Hello there!".encode('utf-8')) # encrypt a message
-        
-        Transmit `cipher` to Receiver.
-        
-        Communication Receiver/Decryptor:
-        
-            # continued from above
-            plaintext = crypt.Decrypt(cipher).decode('utf-8') # decrypt message
-        
-        
-        ###  - __Multi-Session Symmetric Enryption__ (private-key only):  
-          Sender/Encryptor:
-          
-              crypt = Crypt("our_password")
-              cipher = crypt.Encrypt("Hello there!".encode('utf-8'))
-          
-          SECURELY & PRIVATELY transmit the password to the Receiver (this is the downside and weakness of symmetric encryption).
-          
-          Transmit `cipher` to other Receiver.
-          
-          Receiver:
-          
-              # continued from aboveplaintext
-              crypt = Crypt("our_password")
-              plaintext = crypt.Decrypt(cipher).decode('utf-8')
-        ## File Encryption:
-        Because the encryption technologies used above are rather inefficient when applied to larger quantities of data, the Crypt and Encryptor classes have fcuntions that implement symmetric AES encryption. The secret AES key is encrypted with asymmetric elliptic curve cryptography (exactly as the encryption methods above) and embedded into the file, so that the API user (programmer) need not worry about it, and can use the file encryption functionality in exactly the same way as the bytearray-encryption function above.
-        
-        Sender/Encryptor:
-        
-            crypt = Crypt() # create Crypt object with new random public and private keys
-            public_key = crypt.public_key # read public key
-        
-          Give `public_key` (the public key) to Sender (the code in the program below).
-        
-          Communication Sender/Encryptor:
-        
-            # Object-Oriented Approach:
-            encryptor = Encryptor(public_key)  # crete Encryptor object with Receiver's public key
-            encryptor.EncryptFile("/path/to/file", "/where/to/save/encrypted/file") # encrypt a file
-        
-            # Functional Approach:
-            EncryptFile("/path/to/file", "/where/to/save/encrypted/file", public_key)
-        
-          Transmit the encrypted file to Receiver.
-        
-          Communication Receiver:
-        
-            # continued from above
-            plaintext = crypt.DecryptFile("/path/to/encrypted/file", "/path/to/decrypted/file") # decrypt file
-        
-        # Signing
-        CURRENTLY SEEMS TO BE BROKEN, ERROR SOURCE IN THE UNDERLYING COINCURVE MODULE  
-        Digital cryptographic signing data means creating a signature from and for a piece of data using a certain private key (in this case a password). Anybody can verify that the signature was indeed created using the private key by using the corresponding public key.
-        
-          Sender/Signer:
-          
-            data = "hello there!".encode("utf-8")
-            
-            crypt = Crypt("my_password")  # create a Crypt object using a password
-            public_key = crypt.public_key # this is the public key you should share with others
-            signature = crypt.Sign(data)  # creating a signature for data
-            
-          Transmit `data`, `public_key` and `signature` to Receiver/Verifier.
-          
-          Receiver/Verifier:
-          
-            encryptor = Encryptor(public_key)
-            assert(encryptor.VerifySignature(data, signature)) # checking the validity of data's signature using the signer's public key
-            
-            
-            
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+
+An easy-to-use object-oriented API for working with cryptography: encrypting/decrypting data and files as well as signing data and verifying signatures.  
+Can be used for asymmetric and symmetric cryptography, signature verification, and supports password-like private keys.
+Uses elliptic curve cryptography for the data encryption and data signing, the file encryption however uses AES.  
+Built on the eciespy, cryptography, coincurve and hashlib modules.
+
+## Classes `Crypt` and `Encryptor`:
+The `Crypt` class is a cryptographic tool used by the holder of a private key for encrypting and signing data. It's counterpart is the `Encryptor` class, which using a specific public key can ecrypt data and verify signatures.  
+These classes also include functionality for more efficient file encryption using AES secret keys, where the secret key is automatically asymmetrically encrypted and embedded in the symmetrically encrypted file. This means that the usage of this file encryption system is asymmetric (private & public key), although the encryption of the file itself is not.   
+Can be used for single-session asymmetric (public-key/private-key) cryptography
+as well as for (optionally password secured) multi-session (i.e. reused keys) asymmetric (public-key/private-key) or symetric (private-key-only) cryptography.  
+__Single-session__ means the keys are used only as long as the Crypt instance exists, so when the program is restarted different keys are used.  
+__Multi-session__ means that the same keys can be reused after restarting the program, a simplified form of the private key must be memorised by the user as a password (although you can of course use a longer key-like string instead of a typical password).
+
+# Encryption
+## Usage:
+`from Cryptem import Crypt`
+### - __Single-Session Asymetric Encryption__ (public-key and private-key):
+Communication Receiver:
+  
+    crypt = Crypt() # create Crypt object with new random public and private keys
+    public_key = crypt.public_key # read public key
+
+  Give `public_key` (the public key) to Sender (the code in the program below).
+
+Communication Sender/Encryptor:
+  
+    # Object-Oriented Approach:
+    from Cryptem import Encryptor
+    encryptor = Encryptor(public_key)  # crete Encryptor object with Receiver's public key
+    cipher = encryptor.Encrypt("Hello there!".encode('utf-8')) # encrypt a message
+    
+    # Functional Approach:
+    cipher = Encrypt("Hello there!".encode('utf-8'), public_key)
+
+  Transmit `cipher` to Receiver.
+
+Communication Receiver:
+  
+    # continued from above
+    plaintext = crypt.Decrypt(cipher).decode('utf-8') # decrypt message
+
+### - __Multi-Session Asymetric Encryption__ (public-key and private-key):  
+Communication Receiver:
+    
+    crypt = Crypt("mypassword")   # create Crypt object with a password, from which private and ublic keys are generated
+    public_key = crypt.public_key # read public key
+      
+Give `public_key` to Sender.
+
+Communication Sender/Encryptor:
+    
+    encryptor = Encryptor(public_key)  # crete Encryptor object with Receiver's public key
+    cipher = encryptor.Encrypt("Hello there!".encode('utf-8')) # encrypt a message
+
+Transmit `cipher` to Receiver.
+
+Communication Receiver/Decryptor:
+
+    # continued from above
+    plaintext = crypt.Decrypt(cipher).decode('utf-8') # decrypt message
+
+
+###  - __Multi-Session Symmetric Enryption__ (private-key only):  
+  Sender/Encryptor:
+  
+      crypt = Crypt("our_password")
+      cipher = crypt.Encrypt("Hello there!".encode('utf-8'))
+  
+  SECURELY & PRIVATELY transmit the password to the Receiver (this is the downside and weakness of symmetric encryption).
+  
+  Transmit `cipher` to other Receiver.
+  
+  Receiver:
+  
+      # continued from aboveplaintext
+      crypt = Crypt("our_password")
+      plaintext = crypt.Decrypt(cipher).decode('utf-8')
+## File Encryption:
+Because the encryption technologies used above are rather inefficient when applied to larger quantities of data, the Crypt and Encryptor classes have fcuntions that implement symmetric AES encryption. The secret AES key is encrypted with asymmetric elliptic curve cryptography (exactly as the encryption methods above) and embedded into the file, so that the API user (programmer) need not worry about it, and can use the file encryption functionality in exactly the same way as the bytearray-encryption function above.
+
+Sender/Encryptor:
+
+    crypt = Crypt() # create Crypt object with new random public and private keys
+    public_key = crypt.public_key # read public key
+
+  Give `public_key` (the public key) to Sender (the code in the program below).
+
+  Communication Sender/Encryptor:
+
+    # Object-Oriented Approach:
+    encryptor = Encryptor(public_key)  # crete Encryptor object with Receiver's public key
+    encryptor.EncryptFile("/path/to/file", "/where/to/save/encrypted/file") # encrypt a file
+
+    # Functional Approach:
+    EncryptFile("/path/to/file", "/where/to/save/encrypted/file", public_key)
+
+  Transmit the encrypted file to Receiver.
+
+  Communication Receiver:
+
+    # continued from above
+    plaintext = crypt.DecryptFile("/path/to/encrypted/file", "/path/to/decrypted/file") # decrypt file
+
+# Signing
+Digital cryptographic signing data means creating a signature from and for a piece of data using a certain private key (in this case a password). Anybody can verify that the signature was indeed created using the private key by using the corresponding public key.
+
+  Sender/Signer:
+  
+    data = "hello there!".encode("utf-8")
+    
+    crypt = Crypt("my_password")  # create a Crypt object using a password
+    public_key = crypt.public_key # this is the public key you should share with others
+    signature = crypt.Sign(data)  # creating a signature for data
+    
+  Transmit `data`, `public_key` and `signature` to Receiver/Verifier.
+  
+  Receiver/Verifier:
+  
+    encryptor = Encryptor(public_key)
+    assert(encryptor.VerifySignature(data, signature)) # checking the validity of data's signature using the signer's public key
+    
+    
+    
+
```

### Comparing `Cryptem-0.0.3/Cryptem.py` & `Cryptem-0.0.4/Cryptem.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,16 +62,16 @@
 
             ## transmit cipher to other person
 
             codec2 = Crypt("my_password")
             plaintext = codec2.Decrypt(cipher).decode('utf-8')
     """
 
-    public_key = ""
-    __private_key = ""
+    public_key = ""  # string
+    __private_key = ""  # coincurve.keys.PrivateKey
 
     def __init__(self, password=None):
         if password == None:
             key = generate_key()    # generate new random key
         else:
             # creating a cryptographic hash from the password, to create a larger encryption key from it
             hashGen = hashlib.sha256()
@@ -125,14 +125,17 @@
         return self.__private_key.sign(data)
 
     def SignSmall(self, data: bytearray):
         hashGen = hashlib.sha256()
         hashGen.update(self.Sign(data))
         return hashGen.hexdigest()
 
+    def VerifySignature(self, data: bytes, signature: bytes):
+        return VerifySignature(data, self.public_key, signature)
+
 
 class Encryptor:
     def __init__(self, public_key):
         self.public_key = public_key
 
     def Encrypt(self, data):
         return Encrypt(data, self.public_key)
@@ -202,8 +205,14 @@
     with open(encrypted_file, 'wb') as file:
         file.write(encrypted_data)
 
 
 def VerifySignature(data: bytes, public_key: bytes, signature: bytes):
     if isinstance(public_key, str):
         public_key = bytes(bytearray.fromhex(public_key))
+    elif isinstance(data, bytearray):
+        public_key = bytes(public_key)
+    if isinstance(data, bytearray):
+        data = bytes(data)
+    if isinstance(signature, bytearray):
+        signature = bytes(signature)
     return verify_signature(signature, data, public_key)
```

### Comparing `Cryptem-0.0.3/PKG-INFO` & `Cryptem-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,137 +1,138 @@
 Metadata-Version: 2.1
 Name: Cryptem
-Version: 0.0.3
+Version: 0.0.4
 Summary: Cryptographic applications library based on elliptic curve cryptography
 Home-page: https://ipfs.io/ipns/k2k4r8ld8q6344t8dop0rwuk8f3vhpo42un6zrnrffogaayr7xv59p83
 Author: emendir
 License: UNKNOWN
 Project-URL: Source Code on IPFS, https://ipfs.io/ipns/k2k4r8ld8q6344t8dop0rwuk8f3vhpo42un6zrnrffogaayr7xv59p83
-Description: An easy-to-use object-oriented API for working with cryptography: encrypting/decrypting data and files as well as signing data and verifying signatures.  
-        Can be used for asymmetric and symmetric cryptography, signature verification, and supports password-like private keys.
-        Uses elliptic curve cryptography for the data encryption and data signing, the file encryption however uses AES.  
-        Built on the eciespy, cryptography, coincurve and hashlib modules.
-        
-        ## Classes `Crypt` and `Encryptor`:
-        The `Crypt` class is a cryptographic tool used by the holder of a private key for encrypting and signing data. It's counterpart is the `Encryptor` class, which using a specific public key can ecrypt data and verify signatures.  
-        These classes also include functionality for more efficient file encryption using AES secret keys, where the secret key is automatically asymmetrically encrypted and embedded in the symmetrically encrypted file. This means that the usage of this file encryption system is asymmetric (private & public key), although the encryption of the file itself is not.   
-        Can be used for single-session asymmetric (public-key/private-key) cryptography
-        as well as for (optionally password secured) multi-session (i.e. reused keys) asymmetric (public-key/private-key) or symetric (private-key-only) cryptography.  
-        __Single-session__ means the keys are used only as long as the Crypt instance exists, so when the program is restarted different keys are used.  
-        __Multi-session__ means that the same keys can be reused after restarting the program, a simplified form of the private key must be memorised by the user as a password (although you can of course use a longer key-like string instead of a typical password).
-        
-        # Encryption
-        ## Usage:
-        `from Cryptem import Crypt`
-        ### - __Single-Session Asymetric Encryption__ (public-key and private-key):
-        Communication Receiver:
-          
-            crypt = Crypt() # create Crypt object with new random public and private keys
-            public_key = crypt.public_key # read public key
-        
-          Give `public_key` (the public key) to Sender (the code in the program below).
-        
-        Communication Sender/Encryptor:
-          
-            # Object-Oriented Approach:
-            from Cryptem import Encryptor
-            encryptor = Encryptor(public_key)  # crete Encryptor object with Receiver's public key
-            cipher = encryptor.Encrypt("Hello there!".encode('utf-8')) # encrypt a message
-            
-            # Functional Approach:
-            cipher = Encrypt("Hello there!".encode('utf-8'), public_key)
-        
-          Transmit `cipher` to Receiver.
-        
-        Communication Receiver:
-          
-            # continued from above
-            plaintext = crypt.Decrypt(cipher).decode('utf-8') # decrypt message
-        
-        ### - __Multi-Session Asymetric Encryption__ (public-key and private-key):  
-        Communication Receiver:
-            
-            crypt = Crypt("mypassword")   # create Crypt object with a password, from which private and ublic keys are generated
-            public_key = crypt.public_key # read public key
-              
-        Give `public_key` to Sender.
-        
-        Communication Sender/Encryptor:
-            
-            encryptor = Encryptor(public_key)  # crete Encryptor object with Receiver's public key
-            cipher = encryptor.Encrypt("Hello there!".encode('utf-8')) # encrypt a message
-        
-        Transmit `cipher` to Receiver.
-        
-        Communication Receiver/Decryptor:
-        
-            # continued from above
-            plaintext = crypt.Decrypt(cipher).decode('utf-8') # decrypt message
-        
-        
-        ###  - __Multi-Session Symmetric Enryption__ (private-key only):  
-          Sender/Encryptor:
-          
-              crypt = Crypt("our_password")
-              cipher = crypt.Encrypt("Hello there!".encode('utf-8'))
-          
-          SECURELY & PRIVATELY transmit the password to the Receiver (this is the downside and weakness of symmetric encryption).
-          
-          Transmit `cipher` to other Receiver.
-          
-          Receiver:
-          
-              # continued from aboveplaintext
-              crypt = Crypt("our_password")
-              plaintext = crypt.Decrypt(cipher).decode('utf-8')
-        ## File Encryption:
-        Because the encryption technologies used above are rather inefficient when applied to larger quantities of data, the Crypt and Encryptor classes have fcuntions that implement symmetric AES encryption. The secret AES key is encrypted with asymmetric elliptic curve cryptography (exactly as the encryption methods above) and embedded into the file, so that the API user (programmer) need not worry about it, and can use the file encryption functionality in exactly the same way as the bytearray-encryption function above.
-        
-        Sender/Encryptor:
-        
-            crypt = Crypt() # create Crypt object with new random public and private keys
-            public_key = crypt.public_key # read public key
-        
-          Give `public_key` (the public key) to Sender (the code in the program below).
-        
-          Communication Sender/Encryptor:
-        
-            # Object-Oriented Approach:
-            encryptor = Encryptor(public_key)  # crete Encryptor object with Receiver's public key
-            encryptor.EncryptFile("/path/to/file", "/where/to/save/encrypted/file") # encrypt a file
-        
-            # Functional Approach:
-            EncryptFile("/path/to/file", "/where/to/save/encrypted/file", public_key)
-        
-          Transmit the encrypted file to Receiver.
-        
-          Communication Receiver:
-        
-            # continued from above
-            plaintext = crypt.DecryptFile("/path/to/encrypted/file", "/path/to/decrypted/file") # decrypt file
-        
-        # Signing
-        CURRENTLY SEEMS TO BE BROKEN, ERROR SOURCE IN THE UNDERLYING COINCURVE MODULE  
-        Digital cryptographic signing data means creating a signature from and for a piece of data using a certain private key (in this case a password). Anybody can verify that the signature was indeed created using the private key by using the corresponding public key.
-        
-          Sender/Signer:
-          
-            data = "hello there!".encode("utf-8")
-            
-            crypt = Crypt("my_password")  # create a Crypt object using a password
-            public_key = crypt.public_key # this is the public key you should share with others
-            signature = crypt.Sign(data)  # creating a signature for data
-            
-          Transmit `data`, `public_key` and `signature` to Receiver/Verifier.
-          
-          Receiver/Verifier:
-          
-            encryptor = Encryptor(public_key)
-            assert(encryptor.VerifySignature(data, signature)) # checking the validity of data's signature using the signer's public key
-            
-            
-            
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+
+An easy-to-use object-oriented API for working with cryptography: encrypting/decrypting data and files as well as signing data and verifying signatures.  
+Can be used for asymmetric and symmetric cryptography, signature verification, and supports password-like private keys.
+Uses elliptic curve cryptography for the data encryption and data signing, the file encryption however uses AES.  
+Built on the eciespy, cryptography, coincurve and hashlib modules.
+
+## Classes `Crypt` and `Encryptor`:
+The `Crypt` class is a cryptographic tool used by the holder of a private key for encrypting and signing data. It's counterpart is the `Encryptor` class, which using a specific public key can ecrypt data and verify signatures.  
+These classes also include functionality for more efficient file encryption using AES secret keys, where the secret key is automatically asymmetrically encrypted and embedded in the symmetrically encrypted file. This means that the usage of this file encryption system is asymmetric (private & public key), although the encryption of the file itself is not.   
+Can be used for single-session asymmetric (public-key/private-key) cryptography
+as well as for (optionally password secured) multi-session (i.e. reused keys) asymmetric (public-key/private-key) or symetric (private-key-only) cryptography.  
+__Single-session__ means the keys are used only as long as the Crypt instance exists, so when the program is restarted different keys are used.  
+__Multi-session__ means that the same keys can be reused after restarting the program, a simplified form of the private key must be memorised by the user as a password (although you can of course use a longer key-like string instead of a typical password).
+
+# Encryption
+## Usage:
+`from Cryptem import Crypt`
+### - __Single-Session Asymetric Encryption__ (public-key and private-key):
+Communication Receiver:
+  
+    crypt = Crypt() # create Crypt object with new random public and private keys
+    public_key = crypt.public_key # read public key
+
+  Give `public_key` (the public key) to Sender (the code in the program below).
+
+Communication Sender/Encryptor:
+  
+    # Object-Oriented Approach:
+    from Cryptem import Encryptor
+    encryptor = Encryptor(public_key)  # crete Encryptor object with Receiver's public key
+    cipher = encryptor.Encrypt("Hello there!".encode('utf-8')) # encrypt a message
+    
+    # Functional Approach:
+    cipher = Encrypt("Hello there!".encode('utf-8'), public_key)
+
+  Transmit `cipher` to Receiver.
+
+Communication Receiver:
+  
+    # continued from above
+    plaintext = crypt.Decrypt(cipher).decode('utf-8') # decrypt message
+
+### - __Multi-Session Asymetric Encryption__ (public-key and private-key):  
+Communication Receiver:
+    
+    crypt = Crypt("mypassword")   # create Crypt object with a password, from which private and ublic keys are generated
+    public_key = crypt.public_key # read public key
+      
+Give `public_key` to Sender.
+
+Communication Sender/Encryptor:
+    
+    encryptor = Encryptor(public_key)  # crete Encryptor object with Receiver's public key
+    cipher = encryptor.Encrypt("Hello there!".encode('utf-8')) # encrypt a message
+
+Transmit `cipher` to Receiver.
+
+Communication Receiver/Decryptor:
+
+    # continued from above
+    plaintext = crypt.Decrypt(cipher).decode('utf-8') # decrypt message
+
+
+###  - __Multi-Session Symmetric Enryption__ (private-key only):  
+  Sender/Encryptor:
+  
+      crypt = Crypt("our_password")
+      cipher = crypt.Encrypt("Hello there!".encode('utf-8'))
+  
+  SECURELY & PRIVATELY transmit the password to the Receiver (this is the downside and weakness of symmetric encryption).
+  
+  Transmit `cipher` to other Receiver.
+  
+  Receiver:
+  
+      # continued from aboveplaintext
+      crypt = Crypt("our_password")
+      plaintext = crypt.Decrypt(cipher).decode('utf-8')
+## File Encryption:
+Because the encryption technologies used above are rather inefficient when applied to larger quantities of data, the Crypt and Encryptor classes have fcuntions that implement symmetric AES encryption. The secret AES key is encrypted with asymmetric elliptic curve cryptography (exactly as the encryption methods above) and embedded into the file, so that the API user (programmer) need not worry about it, and can use the file encryption functionality in exactly the same way as the bytearray-encryption function above.
+
+Sender/Encryptor:
+
+    crypt = Crypt() # create Crypt object with new random public and private keys
+    public_key = crypt.public_key # read public key
+
+  Give `public_key` (the public key) to Sender (the code in the program below).
+
+  Communication Sender/Encryptor:
+
+    # Object-Oriented Approach:
+    encryptor = Encryptor(public_key)  # crete Encryptor object with Receiver's public key
+    encryptor.EncryptFile("/path/to/file", "/where/to/save/encrypted/file") # encrypt a file
+
+    # Functional Approach:
+    EncryptFile("/path/to/file", "/where/to/save/encrypted/file", public_key)
+
+  Transmit the encrypted file to Receiver.
+
+  Communication Receiver:
+
+    # continued from above
+    plaintext = crypt.DecryptFile("/path/to/encrypted/file", "/path/to/decrypted/file") # decrypt file
+
+# Signing
+Digital cryptographic signing data means creating a signature from and for a piece of data using a certain private key (in this case a password). Anybody can verify that the signature was indeed created using the private key by using the corresponding public key.
+
+  Sender/Signer:
+  
+    data = "hello there!".encode("utf-8")
+    
+    crypt = Crypt("my_password")  # create a Crypt object using a password
+    public_key = crypt.public_key # this is the public key you should share with others
+    signature = crypt.Sign(data)  # creating a signature for data
+    
+  Transmit `data`, `public_key` and `signature` to Receiver/Verifier.
+  
+  Receiver/Verifier:
+  
+    encryptor = Encryptor(public_key)
+    assert(encryptor.VerifySignature(data, signature)) # checking the validity of data's signature using the signer's public key
+    
+    
+    
+
```

### Comparing `Cryptem-0.0.3/README.md` & `Cryptem-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,14 @@
 
   Communication Receiver:
 
     # continued from above
     plaintext = crypt.DecryptFile("/path/to/encrypted/file", "/path/to/decrypted/file") # decrypt file
 
 # Signing
-CURRENTLY SEEMS TO BE BROKEN, ERROR SOURCE IN THE UNDERLYING COINCURVE MODULE  
 Digital cryptographic signing data means creating a signature from and for a piece of data using a certain private key (in this case a password). Anybody can verify that the signature was indeed created using the private key by using the corresponding public key.
 
   Sender/Signer:
   
     data = "hello there!".encode("utf-8")
     
     crypt = Crypt("my_password")  # create a Crypt object using a password
```

### Comparing `Cryptem-0.0.3/setup.py` & `Cryptem-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Cryptem",
-    version="0.0.3",
+    version="0.0.4",
     author="emendir",
     description="Cryptographic applications library based on elliptic curve cryptography",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://ipfs.io/ipns/k2k4r8ld8q6344t8dop0rwuk8f3vhpo42un6zrnrffogaayr7xv59p83",
 
     project_urls={
```

