# Comparing `tmp/sha256bit-0.0.3.tar.gz` & `tmp/sha256bit-0.0.5.tar.gz`

## Comparing `sha256bit-0.0.3.tar` & `sha256bit-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rwxr-xr-x   0        0        0       44 2020-02-02 00:00:00.000000 sha256bit-0.0.3/publish_to_pypi
--rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 sha256bit-0.0.3/sha256bit/__init__.py
--rwxr-xr-x   0        0        0  3364551 2020-02-02 00:00:00.000000 sha256bit-0.0.3/test/SHA256LongMsg.rsp
--rwxr-xr-x   0        0        0    80540 2020-02-02 00:00:00.000000 sha256bit-0.0.3/test/SHA256ShortMsg.rsp
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 sha256bit-0.0.3/test/__init__.py
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 sha256bit-0.0.3/test/test.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 sha256bit-0.0.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 sha256bit-0.0.3/LICENSE
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 sha256bit-0.0.3/README.md
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 sha256bit-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 sha256bit-0.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0      300 2020-02-02 00:00:00.000000 sha256bit-0.0.5/publish_to_pypi
+-rw-r--r--   0        0        0     5908 2020-02-02 00:00:00.000000 sha256bit-0.0.5/sha256bit/__init__.py
+-rwxr-xr-x   0        0        0  3364551 2020-02-02 00:00:00.000000 sha256bit-0.0.5/test/SHA256LongMsg.rsp
+-rwxr-xr-x   0        0        0    80540 2020-02-02 00:00:00.000000 sha256bit-0.0.5/test/SHA256ShortMsg.rsp
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 sha256bit-0.0.5/test/__init__.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 sha256bit-0.0.5/test/test.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 sha256bit-0.0.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 sha256bit-0.0.5/LICENSE
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 sha256bit-0.0.5/README.md
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 sha256bit-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 sha256bit-0.0.5/PKG-INFO
```

### Comparing `sha256bit-0.0.3/sha256bit/__init__.py` & `sha256bit-0.0.5/sha256bit/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,25 +41,25 @@
         return (x & y) ^ ((~x) & z)
     
     _output_size = 8
     blocksize = 1
     block_size = 64
     digest_size = 32
 
-    def __init__(self, m=None):
+    def __init__(self, m=None, *, bitlen=None):
         """ SHA-256 implementation supporting bit granularity for message input length.
             API is the same as hashlib.
         """
         self._counter = 0
         self._cache = bytearray()
         self._h = copy.deepcopy(sha256bit._h_init)
-        self.hasBitLen = False 
+        self.has_bitlen = False 
         self.finalizing = False
         self._digest = None
-        self.update(m)
+        self.update(m,bitlen=bitlen)
 
     def internal_state(self):
         return {"h":self._h, "cnt":self._counter, "cache":self._cache}
 
     def _compress(self, c):
         w = [0] * 64
         w[0:16] = struct.unpack('!16L', c)
@@ -84,43 +84,43 @@
             c = b
             b = a
             a = (t1 + t2) & sha256bit.F32
 
         for i, (x, y) in enumerate(zip(self._h, [a, b, c, d, e, f, g, h])):
             self._h[i] = (x + y) & sha256bit.F32
 
-    def update(self, m, *, bitLen=None):
+    def update(self, m, *, bitlen=None):
         """ Update the hash object with the bytes in data. Repeated calls
             are equivalent to a single call with the concatenation of all
             the arguments.
         """
         if not m:
             return
 
-        if self.hasBitLen: 
+        if self.has_bitlen: 
             assert self.finalizing, "we support bitLen only for last block"
         
-        if bitLen is not None:
-            if 0 != (bitLen%8):
-                self.hasBitLen = True
+        if bitlen is not None:
+            if 0 != (bitlen%8):
+                self.has_bitlen = True
             else:
-                assert bitLen == len(m)*8, "bitLen=%d, len(m)*8=%d"%(bitLen,len(m)*8)
-            self._counter += bitLen
+                assert bitlen == len(m)*8, "bitLen=%d, len(m)*8=%d"%(bitlen,len(m)*8)
+            self._counter += bitlen
         else:
             self._counter += len(m)*8
         
         self._cache += m
         
         while len(self._cache) > 64:
             self._compress(self._cache[:64])
             self._cache = self._cache[64:]
 
         if len(self._cache) == 64:
             if 0 != (self._counter % 8):
-                assert self.hasBitLen
+                assert self.has_bitlen
                 # at least one bit is issing to form a full block, nothing to do
             else:
                 self._compress(self._cache[:64])
                 self._cache = self._cache[64:]
 
     def _pad(self):
         lastBlockBitLen = self._counter % 512
```

### Comparing `sha256bit-0.0.3/test/SHA256LongMsg.rsp` & `sha256bit-0.0.5/test/SHA256LongMsg.rsp`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.3/test/SHA256ShortMsg.rsp` & `sha256bit-0.0.5/test/SHA256ShortMsg.rsp`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.3/test/test.py` & `sha256bit-0.0.5/test/test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 if __name__ == '__main__':
     import hashlib
     from pysatl import Utils
     import re
     from sha256bit import sha256bit
 
     print("check against hashlib")
+
+    assert hashlib.sha256("abc".encode()).digest() == sha256bit("abc".encode()).digest()
+
     def checkAgainstHashLib(seed,msgBitLen):
         lastBlockBitLen = msgBitLen % 512
         l2block = hashlib.sha256(seed).digest()
         l2block += hashlib.sha256(l2block).digest()
         blockBitLen = len(l2block)*8
         assert blockBitLen == 64*8
         expected = hashlib.sha256()
         dut = sha256bit()
-        bitLen=0
-        while(bitLen+blockBitLen<msgBitLen):
+        bitlen=0
+        while(bitlen+blockBitLen<msgBitLen):
             expected.update(l2block)
             dut.update(l2block)
-            bitLen += blockBitLen
+            bitlen += blockBitLen
             l2block = hashlib.sha256(l2block).digest()
             l2block += hashlib.sha256(l2block).digest()
         # last block
         l2block = l2block[0:lastBlockBitLen//8]
         assert len(l2block) == lastBlockBitLen //8
         expected.update(l2block)
         dut.update(l2block)
@@ -29,59 +32,62 @@
 
     for seedByte in range(0, 5):
         for msgBitLen in range(0,1024*4, 8):
             seed = bytearray([seedByte])
             checkAgainstHashLib(seed,msgBitLen)
 
     print("check few minimal hardcoded test vectors")
-    def check(msg, bitLen, sig):
+    def check(msg, bitlen, sig):
         m = sha256bit()
         if isinstance(msg,str):
             msg=msg.encode('ascii')
         descr = "msg      = "+Utils.hexstr(msg)+"\n"
-        descr+= "bitLen   = %d\n"%bitLen
+        descr+= "bitlen   = %d\n"%bitlen
         descr+= "expected = "+sig+"\n"
         try:
             
-            m.update(msg, bitLen=bitLen)
+            m.update(msg, bitlen=bitlen)
             digest = m.hexdigest()
         except Exception as e:
             print(descr)
             raise e
         errMsg ='\n'
         errMsg+= descr
         errMsg+= "digest   = "+digest+"\n"
         assert digest == sig, errMsg
 
     tests = [
-        {"msg":"","bitLen":0,"digest":'e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855'},
-        {"msg":"a","bitLen":8,"digest":'ca978112ca1bbdcafac231b39a23dc4da786eff8147c4e72b9807785afee48bb'},
-        {"msg":Utils.ba("00"),"bitLen":1,"digest":'bd4f9e98beb68c6ead3243b1b4c7fed75fa4feaab1f84795cbd8a98676a2a375'},
-        {"msg":Utils.ba("80"),"bitLen":2,"digest":'18f331f626210ff9bad6995d8cff6e891adba50eb2fdbddcaa921221cdc333ae'},
+        {"msg":"","bitlen":0,"digest":'e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855'},
+        {"msg":"a","bitlen":8,"digest":'ca978112ca1bbdcafac231b39a23dc4da786eff8147c4e72b9807785afee48bb'},
+        {"msg":Utils.ba("00"),"bitlen":1,"digest":'bd4f9e98beb68c6ead3243b1b4c7fed75fa4feaab1f84795cbd8a98676a2a375'},
+        {"msg":Utils.ba("80"),"bitlen":2,"digest":'18f331f626210ff9bad6995d8cff6e891adba50eb2fdbddcaa921221cdc333ae'},
     ]
 
     for test in tests:
-        check(test["msg"],test["bitLen"],test["digest"])
+        check(test["msg"],test["bitlen"],test["digest"])
+
+    assert sha256bit(b'\x00',bitlen=1).hexdigest() == 'bd4f9e98beb68c6ead3243b1b4c7fed75fa4feaab1f84795cbd8a98676a2a375'
+
 
     print("check against 'short' and 'long' bit oriented test vectors from NIST CAVP")
     # (https://csrc.nist.gov/CSRC/media/Projects/Cryptographic-Algorithm-Validation-Program/documents/shs/shabittestvectors.zip)
 
     from pathlib import Path
     resource_path = Path(__file__).parent 
     for tvFile in ["SHA256ShortMsg.rsp","SHA256LongMsg.rsp"]:
         tvPath = resource_path.joinpath(tvFile)
         with open(tvPath) as f:
             for l in f:
                 if l.startswith("Len"):
-                    bitLen = int(re.search(r"Len = (.+)",l).group(1))
+                    bitlen = int(re.search(r"Len = (.+)",l).group(1))
                 if l.startswith("Msg"):
                     msg = Utils.ba(re.search(r"Msg = (.+)",l).group(1))
-                    if bitLen==0:
+                    if bitlen==0:
                         msg=bytes(0)
                 if l.startswith("MD"):
                     MD = re.search(r"MD = (.+)",l).group(1)
-                    check(msg,bitLen,MD)
+                    check(msg,bitlen,MD)
 
     print("All test PASS")
```

### Comparing `sha256bit-0.0.3/.gitignore` & `sha256bit-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.3/LICENSE` & `sha256bit-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.3/pyproject.toml` & `sha256bit-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sha256bit-0.0.3/PKG-INFO` & `sha256bit-0.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: sha256bit
-Version: 0.0.3
+Version: 0.0.5
 Summary: SHA256 with bit granularity for message input length
 Project-URL: Homepage, https://github.com/sebastien-riou/sha256bit
 Project-URL: Bug Tracker, https://github.com/sebastien-riou/sha256bit/issues
 Author: Sebastien Riou
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # sha256bit
 SHA256 with bit granularity for message input length.
 
+## Usage
 
+    >>> from sha256bit import sha256bit
+    >>> sha256bit(inbits,bitlen=len(inbits)).hexdigest()
+    'bd4f9e98beb68c6ead3243b1b4c7fed75fa4feaab1f84795cbd8a98676a2a375'
+    
 ## Build the package
 ````
 python3 -m build
 ````
 
 ## Test
 Tests can run without creating/installing the package:
```

