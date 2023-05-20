# Comparing `tmp/LogicGate-0.2.5.tar.gz` & `tmp/logicgate-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LogicGate-0.2.5.tar", max compression
+gzip compressed data, was "logicgate-0.2.6.tar", max compression
```

## Comparing `LogicGate-0.2.5.tar` & `logicgate-0.2.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1066 2023-04-15 10:25:03.782472 LogicGate-0.2.5/LICENSE
--rw-r--r--   0        0        0    12712 2023-05-02 13:24:30.526632 LogicGate-0.2.5/LogicGate/LogicGate.py
--rw-r--r--   0        0        0     4315 2023-05-02 13:22:24.970750 LogicGate-0.2.5/LogicGate/lgEncrypt.py
--rw-r--r--   0        0        0     5175 2023-04-28 07:51:30.723628 LogicGate-0.2.5/README.rst
--rw-r--r--   0        0        0      773 2023-05-02 13:25:40.426566 LogicGate-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     6066 2023-05-02 13:25:55.297106 LogicGate-0.2.5/setup.py
--rw-r--r--   0        0        0     5902 2023-05-02 13:25:55.300955 LogicGate-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-15 10:25:03.782472 logicgate-0.2.6/LICENSE
+-rw-r--r--   0        0        0    12812 2023-05-17 08:15:09.686291 logicgate-0.2.6/LogicGate/LogicGate.py
+-rw-r--r--   0        0        0     4593 2023-05-17 08:15:15.734285 logicgate-0.2.6/LogicGate/lgEncrypt.py
+-rw-r--r--   0        0        0     5175 2023-04-28 07:51:30.723628 logicgate-0.2.6/README.rst
+-rw-r--r--   0        0        0      827 2023-05-20 00:28:34.207396 logicgate-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     6070 1970-01-01 00:00:00.000000 logicgate-0.2.6/setup.py
+-rw-r--r--   0        0        0     5993 1970-01-01 00:00:00.000000 logicgate-0.2.6/PKG-INFO
```

### Comparing `LogicGate-0.2.5/LICENSE` & `logicgate-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `LogicGate-0.2.5/LogicGate/LogicGate.py` & `logicgate-0.2.6/LogicGate/LogicGate.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 from sys import argv
 import sys, os
 from random import randint
 from math import sqrt
 
 
 def run(
-  filename: str,
-  gate: bool = False,  #show gate in result
-  ascii: bool = True,  #show ascii in result
-  debug: bool = False,  #log during process
-  check: str = '',  #check for error in code, mostly for debug
-  out: bool = True
-):
+    filename: str,
+    gate: bool = False,  #show gate in result
+    ascii: bool = True,  #show ascii in result
+    debug: bool = False,  #log during process
+    check: str = '',  #check for error in code, mostly for debug
+    out: bool = True):
   """To run this filename is the only thing needed, Error will be raised and nothing will return if something went wrong. If ascii is on, it will return the ascii result, otherwise 0.
   
   Arguments, type of input, usecases:
       filename: string, specify which file needed to run
       gate: boolean(True or False), if the result shows gate result or not
       ascii: boolean, if the result converts to ascii and show or not
       debug: boolean, show the unhuman log during the interpute
@@ -35,15 +34,15 @@
     ),  #for error reporting, first is line and second is index, sometimes third for the latest gate called
     aft=None,  #command afterward
     an=None,  #None/True/False -> (1/0/Not)/And/Or
   ) -> tuple:  #(0 or 1, unprocessed commands that may be used by and/or gates in previous commands in list)
     'One line code processor, return one output from a line of input, internal use only'
     if debug: print('called, args:', obj, line, aft, an)
     if len(str(obj)) == 1:  #if the first process string is a single command
-      obj = str(obj)
+      obj = str(obj).upper()
       if obj == "#":
         if aft[:2] == '##':
           return
       AnList = None
       if an != None:
         #if AnList exists, it is an and/or gate, depends on the first index is True(and) or False(or)
         AnList = [an]
@@ -120,83 +119,86 @@
     else:
       #if the first command given is not one command
       sys.stdout = sys.__stdout__
       raise SystemError(
         'Internal error, unexpected arguments received in internal helper function, please do not change the code'
       )
 
-  
   if out:
     sys.stdout = sys.__stdout__
   else:
     sys.stdout = open(os.devnull, 'w')
   if exists(filename):
     with open(filename, 'r') as f:
-      f.seek(0,0)
+      f.seek(0, 0)
       Out = [[]]
       dt = f.readlines()
       if not filename.endswith('.lgeso'):
         sys.tracebacklimit = 0
         sys.stdout = sys.__stdout__
         raise NameError(
-          f'{filename} is not an lgeso file, maybe renaming the file extension to lgeso and try again')
+          f'{filename} is not an lgeso file, maybe renaming the file extension to lgeso and try again'
+        )
       for dtidx, line in enumerate(dt):
         line = line.replace('\n', '')
         if '---' in line:
           Out.append([])
         else:
           try:
             Out[-1].append(
-            str(
-              process(line[0],
-                      line=(dtidx + 1, 1),
-                      aft=(None if len(line) == 1 else line[1:]))[0]))
+              str(
+                process(line[0],
+                        line=(dtidx + 1, 1),
+                        aft=(None if len(line) == 1 else line[1:]))[0]))
           except OverflowError:
             sys.tracebacklimit = 0
             sys.stdout = sys.__stdout__
-            raise OverflowError(f'too many commands in line {dtidx+1}, more than max command on this os ({sys.getrecursionlimit()} commands per line), process overflowed, exited')
+            raise OverflowError(
+              f'too many commands in line {dtidx+1}, more than max command on this os ({sys.getrecursionlimit()} commands per line), process overflowed, exited'
+            )
       hold = ""
       checkOut = ""
       checkhold = []
       if check:
         for char in check:
           checkhold.append(str(bin(ord(char))[2:]))
       if gate:
         print('gates result:')
       for nidx, n in enumerate(Out):
-        checkOut+='-'
+        checkOut += '-'
         Nhold = n.copy()
         if n == []:
           continue
         if gate:
           for chekidx, chek in enumerate(n):
-            if '\033[0;37;41m' in chek and '\033[0;37;40m' in chek:
+            if '\033[0;37;40m' in chek:
               continue
             if chek != '1' and chek != '0' and chek != ' ':
               print(
                 f'error char {repr(chek)} found in index {chekidx}, line {nidx+1}, please report that line of code shown in lgeso file to the dev. '
               )
             if ascii and check:
               if nidx >= len(checkhold):
                 n[chekidx] = f'\033[0;37;41m{chek}\033[0;37;40m'
-                checkOut+=chek
+                checkOut += chek
               else:
                 if len(n) > len(checkhold[nidx]):
-                  for _ in range(len(n)-len(checkhold[nidx])):
+                  for _ in range(len(n) - len(checkhold[nidx])):
                     checkhold[nidx] = '0' + checkhold[nidx]
                 if chek != checkhold[nidx][chekidx]:
                   n[chekidx] = f'\033[0;37;41m{chek}\033[0;37;40m'
-                  checkOut+=chek
+                  checkOut += chek
                 else:
                   n[chekidx] = f'\033[0;37;42m{chek}\033[0;37;40m'
           if nidx < len(checkhold):
             if len(n) < len(checkhold[nidx]):
               for x in checkhold[nidx][len(n):]:
-                n.append(f'\033[0;37;{"46" if int(x) else "45"}m▯\033[0;37;40m')
-                checkOut+='0' if int(x) else '1'
+                n.append(
+                  f'\033[0;37;{"46" if int(x) else "45"}m▯\033[0;37;40m')
+                checkOut += '0' if int(x) else '1'
           n.append(' ')
           print(''.join(n))
         if ascii:
           try:
             hold += chr(int(''.join(Nhold), 2))
           except ValueError:
             print(
@@ -217,31 +219,32 @@
 
 
 def compile(
   filename: str = 'main.lgeso',
   output: str = 'Hello World!',
   randomize: bool = True,
   random_range: list = [1, 5],
-  write:bool = True,
-  override:bool = False,
-  BitLock:int = -1
+  write: bool = True,
+  override: bool = False,
+  BitLock: int = -1
 ) -> None:  #I swear if this thing returns anything somehow somewhere and somewhat, python is dying or my brain is dying
   """compile string to lgeso file, random_range is needed only when randomize is true.
   filename: string, specify which file to write the data into, new file named as filename will be created if it doesn't exist
   output: string, specify what result will be produced
   randomize: boolean, if the data written is pure binary or further encrypted with gates
   random_range: list, the maximum set of gates in the written data will be the square of the second item while the minimum will be the square of the first item.
   write: boolean, if the result is returned or is written to file
   override: boolean, safety checks are off, proceed with caution
   BitLock: integer, if the binary of a character is shorter than this value, 0 will be appended. Defalt is -1, which is off, all negative number will be counted as ignore as well"""
 
   out = ""
   override = not override
   if not output.isascii() and override:
-    raise ValueError(f'message received ({repr(output)}) is not available in ascii')
+    raise ValueError(
+      f'message received ({repr(output)}) is not available in ascii')
   if not output and override:
     output = 'Hello World!'
   if filename and write and override:
     if len(filename) > 6:
       if filename[-6:] != '.lgeso':
         print(f'filename is not an lgeso file, filename changed to {filename}')
         filename += '.lgeso'
@@ -252,37 +255,39 @@
       print(f'filename is not an lgeso file, filename changed to {filename}')
       filename = 'main.lgeso'
   else:
     if override:
       print(f'filename is not an lgeso file, filename changed to {filename}')
       filename = 'main.lgeso'
   with open(filename, 'w') as f:
-    if (len(random_range) != 2 or random_range[0] > random_range[1]) and override:
+    if (len(random_range) != 2
+        or random_range[0] > random_range[1]) and override:
       print('invalid random range received, changed to 1-5')
       random_range = [1, 5]  #when the random_range is not correctly formatted
     for checkidx, check in enumerate(random_range):
       try:
         random_range[checkidx] == int(check)  #if the input is a number or not
       except ValueError:
         if override:
           print('invalid random range received, changed to 1-5')
           random_range = [1, 5]
           break
       else:
-        if (check < 1 or check > (sqrt(sys.getrecursionlimit())//3)) and override:  #avoid overflow error when running
+        if (check < 1 or check > (sqrt(sys.getrecursionlimit()) // 3)
+            ) and override:  #avoid overflow error when running
           print(
             'an item in random range is too large or too small, changed to 1-5'
           )
           random_range = [1, 5]
           break
     for char in output:
       line = str(bin(ord(char))[2:])
       if len(line) < BitLock and BitLock >= 0:
-        for _ in range(BitLock-len(line)):
-          line = '0'+line
+        for _ in range(BitLock - len(line)):
+          line = '0' + line
       for char in line:
         if randomize:
           charGoal = int(char)  #the ideal final output after the randomizing
           for _ in range(
               randint(random_range[0], random_range[1]) *
               randint(random_range[0], random_range[1])):
             gates = randint(0, 3)
```

### Comparing `LogicGate-0.2.5/LogicGate/lgEncrypt.py` & `logicgate-0.2.6/LogicGate/lgEncrypt.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,109 +1,125 @@
 from os.path import exists
 from os import remove
 from sys import getrecursionlimit as maxcur
 from math import sqrt
 from random import randint
 try:
-  exec(f'import {"LogicGate" if (__name__=="__main__") else "".join(str(__name__).rsplit("".join((__file__.split("/")[-1]).rsplit(".py", 1)), 1))+"LogicGate"} as lg')
+  exec(
+    f'import {"LogicGate" if (__name__=="__main__") else "".join(str(__name__).rsplit("".join((__file__.split("/")[-1]).rsplit(".py", 1)), 1))+"LogicGate"} as lg'
+  )
 except ModuleNotFoundError:
   raise ImportError('module require LogicGate, LogicGate not found')
 except ImportError:
   raise ImportError('module require LogicGate, LogicGate not found')
 
 
-  
-def encrypt(filename:str = "main.lgeso", key_file:str = "key.lgeso", msg:str = "Hello World!"):
+def encrypt(filename: str = "main.lgeso",
+            key_file: str = "key.lgeso",
+            msg: str = "Hello World!"):
   """
   an encryption module with the help of LogicGate main module, LogicGate.py is needed.
   Note: this encryption method is not safe, anyone with the data of the 2 files will be able to see the information. 
   filename: string, file to write the encrypted code to
   key_file: string, file to keep the key string into
   msg: string, word to encrypt
   """
 
   if not msg.isascii():
-    raise ValueError(f'message received ({repr(msg)}) is not available in ascii')
-  k, f, kOut, fOut = ['']*4
+    raise ValueError(
+      f'message received ({repr(msg)}) is not available in ascii')
+  k, f, kOut, fOut = [''] * 4
   data = []
   chekK = []
   chekF = []
   for char in msg:
     data.append(str(bin(ord(char))[2:]))
   for i in data:
     k = ''
     f = ''
     if len(i) < 7:
-      i = '0'*(7-len(i)) + i
+      i = '0' * (7 - len(i)) + i
     for idx, char in enumerate(i):
-      while randint(0, 1)==randint(0, 1):
+      while randint(0, 1) == randint(0, 1):
         rand = randint(0, 1)
         k += str(rand)
         f += str(rand)
       k += '0' if int(char) else '1'
       f += str(char)
-    while char:=randint(0, 1)==randint(0, 1):
+    while char := randint(0, 1) == randint(0, 1):
       k += str(int(char))
       f += str(int(char))
-    if len(k)%7 != 0 or len(f)%7 != 0:
-      k = '0'*(7-(len(k)%7)) + k
-      f = '0'*(7-(len(f)%7)) + f
+    if len(k) % 7 != 0 or len(f) % 7 != 0:
+      k = '0' * (7 - (len(k) % 7)) + k
+      f = '0' * (7 - (len(f) % 7)) + f
     tempK = []
     tempF = []
     for kIdx in range(0, len(k), 7):
-      tempK.append(k[kIdx:kIdx+7])
+      tempK.append(k[kIdx:kIdx + 7])
     for fIdx in range(0, len(f), 7):
-      tempF.append(f[fIdx:fIdx+7])
+      tempF.append(f[fIdx:fIdx + 7])
     if len(tempF) != len(tempK):
-      raise SystemError("length of passes doesn't match, internal error raised")
+      raise SystemError(
+        "length of passes doesn't match, internal error raised")
     chekF.append(''.join(tempF))
     chekK.append(''.join(tempK))
     for ko in tempK:
       kOut += chr(int(str(''.join(ko)), 2))
     for fo in tempF:
       fOut += chr(int(str(''.join(fo)), 2))
   checkBuf = []
   check = []
   for fChek, kChek in zip(chekF, chekK):
     for objF, objK in zip(fChek, kChek):
-      if objK!=objF:
+      if objK != objF:
         checkBuf.append(objF)
   for chek in range(0, len(checkBuf), 7):
-    check.append(checkBuf[chek:chek+7])
-  for n in range(0, len(data)-1):
+    check.append(checkBuf[chek:chek + 7])
+  for n in range(0, len(data) - 1):
     if str(data[n]) != ''.join(check[n]):
-      
-      print('BitWarning: bit unaligned\ndata bit : compile bit\n'+str(data[n])+
-          ' : '+''.join(check[n])+'\n')
-  lg.compile(filename, fOut, random_range=(10, sqrt(maxcur())//3), override=True, BitLock=7)
-  lg.compile(key_file, kOut, random_range=(10, sqrt(maxcur())//3), override=True, BitLock=7)
-        
 
+      print('BitWarning: bit unaligned\ndata bit : compile bit\n' +
+            str(data[n]) + ' : ' + ''.join(check[n]) + '\n')
+  lg.compile(filename,
+             fOut,
+             random_range=(10, sqrt(maxcur()) // 3),
+             override=True,
+             BitLock=7)
+  lg.compile(key_file,
+             kOut,
+             random_range=(10, sqrt(maxcur()) // 3),
+             override=True,
+             BitLock=7)
 
-def decrypt(filename:str, key_file:str, sause:bool=False):
+
+def decrypt(filename: str, key_file: str, sause: bool = False):
   """basic decryption, filename and keyfile is required.
   If sause is True, no printing will happen but result given, normally used for another module's extra encryption
   NOTE: 2 files, __decrypt__.lgeso and __decrypt2__.lgeso, will be used for temperary data store and bypasser for LogicGate.run lgeso file locker.
   THE TWO FILES WILL BE CLEARED, WRITTEN AND DELETED AFTER USING THIS FUNCTON"""
   if exists(filename) and exists(key_file):
     with open(filename, 'r') as f, open(key_file, 'r') as k:
-      df=open('__decrypt__.lgeso', 'w')
-      dk=open('__decrypt2__.lgeso', 'w')
+      df = open('__decrypt__.lgeso', 'w')
+      dk = open('__decrypt2__.lgeso', 'w')
       Fdt = f.read()
       Kdt = k.read()
       df.write(Fdt)
       dk.write(Kdt)
       df.close()
       dk.close()
-      out = lg.run('__decrypt__.lgeso', ascii=True, gate=True, check=lg.run('__decrypt2__.lgeso', ascii=True, out=False), out=False).split('-')
-      do=open('__decrypt__.lgeso', 'w')
+      out = lg.run('__decrypt__.lgeso',
+                   ascii=True,
+                   gate=True,
+                   check=lg.run('__decrypt2__.lgeso', ascii=True, out=False),
+                   out=False).split('-')
+      do = open('__decrypt__.lgeso', 'w')
       out = ''.join(out)
       outP = []
       for O in range(0, len(out), 7):
-        outP.append(out[O:O+7])
+        outP.append(out[O:O + 7])
       for n in outP:
         do.write("\n".join(n))
         do.write("\n---\n")
       print('\n\n\n')
       do.close()
       uh = lg.run('__decrypt__.lgeso', gate=True, out=not sause)
       remove('__decrypt__.lgeso')
@@ -113,8 +129,8 @@
     print("filename or key_file doesn't exist, exiting")
 
 
 if __name__ == '__main__':
   f = 'encFile'
   k = 'encKey'
   encrypt(f, k, 'Hello World!')
-  decrypt(f, k)
+  decrypt(f, k)
```

### Comparing `LogicGate-0.2.5/README.rst` & `logicgate-0.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `LogicGate-0.2.5/pyproject.toml` & `logicgate-0.2.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "LogicGate"
-version = "0.2.5"
+version = "0.2.6"
 description = "an esolang designed for manual encryption with logic gates"
 license = "MIT"
 authors = ["Taokyle <taokyle415@gmail.com>"]
 readme = "README.rst"
 repository = "https://replit.com/@s3D27ZHOU/LogicGate"
+keywords = ["logic", "gate", "encrypt", "encryption"]
 packages = [
     { include = "LogicGate.py", from = "LogicGate" },
     { include = "lgEncrypt.py", from = "LogicGate"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `LogicGate-0.2.5/setup.py` & `logicgate-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 package_dir = \
 {'': 'LogicGate'}
 
 modules = \
 ['LogicGate', 'lgEncrypt']
 setup_kwargs = {
     'name': 'logicgate',
-    'version': '0.2.5',
+    'version': '0.2.6',
     'description': 'an esolang designed for manual encryption with logic gates',
     'long_description': 'LogicGate\n=========\n\nThis language is inspired by logic gates, by using simple alphabet you\ncould make a program.\n\nIt is designed as a way for manual encryption, which kinda failed\n\nAll you can do in this language is to make a program with logic gates,\nsounds difficult and indeed it is.\n\nStartup\n-------\n\nFirst, make a logic gate file. The file extension should be lgeso\n\nRunner\n------\n\nTo use it, import the python file **LogicGate.py** in your python\nscript, or just run the LogicGate.py.\nRemember for the run function, only\nthe filename argument is needed. The run function will return an exit\ncode if you use the run function, and outputs of the file will be\nprinted(binary to ascii, and logical binary if enabled). The compile\nfunction does the otherwise, it doesn’t return anything but it can write\ncode into lgeso file.\n\nSpecial encrypt module\n----------------------\na special encrypt module is included in this package, which is lgEncrypt.py. \nit contain two functions, encrypt() and decrypt().\nencrypt() generates a key file and a data file, they are pure random string when transfered to ascii, but shows message when both being processed by decrypt()\nencrypth) have 3 arguments, data file name, key file name, message\nThey are very self explainatory\n\ndecrypt() have 3 arguments, data file, key file, sause\nthe first 2 is very self explainatory, for sause parameter it determinates if the output text is shown or returned for further decryption, assuming the message through encrypt() is encrypted beforehand\n\nsyntax\n------\n\nFor syntax it is very straight forward. It process each character in\neach line as each command For gates with multiple inputs (such as or,\nand) type like other syntax, the quota for the gate will automatically\nbe processed. No linking between words, unless the syntax at the middle\nis invalid\n\nBasic gates(gates that doesn’t require includes):\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\nA (and gate): the next **2** results will be accepted as inputs. If both\ninputs are 1, output is 1, else 0\n\nO (or gate): the next **2** results will be accepted as inputs. If one\nof the inputs are 1, output is 1, else 0\n\nN (not gate): the next **1** result will be accepted as inputs. If the\ninput is 1, output is 0, else 0\n\n1 and 0 (True and False): **NO** result will be accepted as inputs. They\nare the results, self explanatory\n\nspecial syntax\n~~~~~~~~~~~~~~\n\nThere are 2 special syntax\n\n—-- (three hyphens): new word, used for the ascii output separating the\nbinary for ascii translation\n\n### (three hashes): comment everything after the syntax\n\nFor any of the special syntax, they are not being interpreted as special\nsyntax unless the entire syntax appears. They can be anywhere in a line,\nand that line will act like what the syntax shows (if the special syntax\nappears in the same line, they will be scanned and processed according\nto here)\n\nexamples\n========\n\nThis is a hello world in LogicGate\n\n``1\\n 0\\n 0\\n 1\\n 0\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 0\\n 1\\n 0\\n 1\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 1\\n 1\\n ---\\n 1\\n 0\\n 0\\n 0\\n 0\\n 0\\n ---\\n 1\\n 0\\n 1\\n 0\\n 1\\n 1\\n 1\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 1\\n 1\\n ---\\n 1\\n 1\\n 1\\n 0\\n 0\\n 1\\n 0\\n ---\\n 1\\n 1\\n 0\\n 1\\n 1\\n 0\\n 0\\n ---\\n 1\\n 1\\n 0\\n 0\\n 1\\n 0\\n 0\\n ---\\n 1\\n 0\\n 0\\n 0\\n 0\\n 1\\n``\n\nanother version generated by LogicGate.compile():\n``O1NNAANNNNA1AA1AO0AA1AO1NNANNAA1A1111111111\\n NNANNAAAO0O000001\\n OO0NNN10\\n O1O1NNA1O01\\n NNOONNA0O0000\\n 0\\n AA0NNANNOONNNNAO0A1O0000001\\n ---\\n OO1O1OAO1NNAO111111\\n NNNNO0NNAA1O0N01\\n OANNOA0O00000\\n ANNNNA001\\n NNA11\\n NNANNA1ANNO0001\\n NNAANNAOOA1NNAO10110111\\n ---\\n OA111\\n A1OA1OO0A1O1NNA1O0ONNNNNNN0000\\n A1O0A00\\n A1O0NNAO0O0A111\\n NNAO1NNONNNNA1O1111\\n O0A1OANNA0NNOO0ON10000\\n 0\\n ---\\n O0NNN0\\n A1ANNNNNNNNNNO101\\n O00\\n NNA1OO1ONNAO10110\\n OAA1110\\n OO0AAO0AAONNO0O0NNO00001100\\n NNO0A0ONNN10\\n ---\\n O0O1O0A1NNO1ANNO0AA1O1AA1A1A11111\\n NNANNO1ONNNNNNNNNNO0AO11101\\n O0OONNNNAAO0N11000\\n A1O0N0\\n OONNNNOA1ONNOO0AA11100100\\n NNO0ON00\\n O0OA1NNA1O100\\n ---\\n O0OO1OO1A1O1000\\n NNOO0AONNONNO0A0NNA0NNA010010\\n NNAA0OOOA0O000001\\n A0NNNNN1\\n AO0NNNNA1OO0001\\n O0OA1O0O0OO0OA1O00000\\n ---\\n 1\\n A0NNAO0A0OA0NNA1A0000\\n NNO0NNA1NNOO011\\n NNO0NNA0A0A0NNOO000\\n ANNA1AA1NNNNNNNNAA1NNAA1A111111\\n NNA1ANNA1OAO1O11111\\n A1A1NNA1O1NNANNA1AA1111\\n ---\\n ONNNNAOO11110\\n OANNOONNA1AA1110111\\n AA0NNNNNNO0O0A0O0N10\\n NNNNNNOA110\\n O1OONNA1101\\n A1NNNNA11\\n ANNOONNAAO1A1ANNA11111011\\n ---\\n O0NNO0AO0A111\\n NNNNNNA1O0ONNA1NNNNO0NNANNOOA1ANNNNAA11110111\\n NNO11\\n AO0AN101\\n OAA1000\\n 1\\n O0A0NNO0O0NNA0A0NNA1ON10\\n ---\\n O0N0\\n NNNNNNO0ONNA1N00\\n O00\\n O0AN01\\n NNONNNNNNNNA111\\n NNNNONNOO0000\\n AONNO0ANNO00101\\n ---\\n O1ONNANNNNA1111\\n NNNNOOOO0NNAA1NNONNO1011111\\n NNA0A0A01\\n AA1N10\\n O1OANNNNNNA1ONNNNOO1AOOO1AAN0110111110\\n 0\\n OOAO0NNO0A0OAANNA0AONNO0001100000\\n ---\\n A1A1NNO0NNA11\\n OA100\\n NNANNOA1001\\n 0\\n NNO0OA0O000\\n ANNO0OONNA1O11001\\n ---``\n\nSources\n-------\n\n`gitbub\n<https://github.com/TaokyleYT/LogicGate/>`__\\\n\nEsolang wiki:\n`LogicGate <https://esolangs.org/wiki/LogicGate>`__\\\n\nReplit up-to-date version:\n`replit <https://replit.com/@s3D27ZHOU/LogicGate>`__\n',
     'author': 'Taokyle',
     'author_email': 'taokyle415@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://replit.com/@s3D27ZHOU/LogicGate',
     'package_dir': package_dir,
     'py_modules': modules,
     'python_requires': '>=3.10,<4.0',
 }
```

### Comparing `LogicGate-0.2.5/PKG-INFO` & `logicgate-0.2.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: logicgate
-Version: 0.2.5
+Version: 0.2.6
 Summary: an esolang designed for manual encryption with logic gates
 Home-page: https://replit.com/@s3D27ZHOU/LogicGate
 License: MIT
+Keywords: logic,gate,encrypt,encryption
 Author: Taokyle
 Author-email: taokyle415@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://replit.com/@s3D27ZHOU/LogicGate
 Project-URL: esolang wiki, https://esolangs.org/wiki/LogicGate
 Project-URL: github, https://github.com/TaokyleYT/LogicGate
 Project-URL: up-to-date source code(replit), https://replit.com/@s3D27ZHOU/LogicGate
 Description-Content-Type: text/x-rst
 
 LogicGate
```

