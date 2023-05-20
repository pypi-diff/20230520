# Comparing `tmp/ejelabs-0.1.tar.gz` & `tmp/ejelabs-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ejelabs-0.1.tar", last modified: Wed Apr 19 13:00:49 2023, max compression
+gzip compressed data, was "ejelabs-0.2.tar", last modified: Sat May 20 11:19:26 2023, max compression
```

## Comparing `ejelabs-0.1.tar` & `ejelabs-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 13:00:49.424465 ejelabs-0.1/
--rw-rw-rw-   0        0        0     1064 2023-04-19 12:36:28.000000 ejelabs-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      565 2023-04-19 13:00:49.424465 ejelabs-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-04-19 12:34:47.000000 ejelabs-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 13:00:49.397537 ejelabs-0.1/ejelabs/
--rw-rw-rw-   0        0        0   983908 2023-04-19 12:19:04.000000 ejelabs-0.1/ejelabs/Cracklabs.py
--rw-rw-rw-   0        0        0     3123 2023-04-19 12:23:31.000000 ejelabs-0.1/ejelabs/Main.py
--rw-rw-rw-   0        0        0      108 2023-04-19 12:23:39.000000 ejelabs-0.1/ejelabs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 13:00:49.422491 ejelabs-0.1/ejelabs.egg-info/
--rw-rw-rw-   0        0        0      565 2023-04-19 13:00:49.000000 ejelabs-0.1/ejelabs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-04-19 13:00:49.000000 ejelabs-0.1/ejelabs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 13:00:49.000000 ejelabs-0.1/ejelabs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-04-19 13:00:49.000000 ejelabs-0.1/ejelabs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-19 13:00:49.000000 ejelabs-0.1/ejelabs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-19 13:00:49.426459 ejelabs-0.1/setup.cfg
--rw-rw-rw-   0        0        0      852 2023-04-19 12:49:43.000000 ejelabs-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 11:19:26.014645 ejelabs-0.2/
+-rw-rw-rw-   0        0        0     1064 2023-04-19 12:36:28.000000 ejelabs-0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      565 2023-05-20 11:19:26.014645 ejelabs-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-04-19 12:34:47.000000 ejelabs-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-20 11:19:25.991707 ejelabs-0.2/ejelabs/
+-rw-rw-rw-   0        0        0   983908 2023-04-19 12:19:04.000000 ejelabs-0.2/ejelabs/Cracklabs.py
+-rw-rw-rw-   0        0        0     3385 2023-05-20 11:13:08.000000 ejelabs-0.2/ejelabs/Main.py
+-rw-rw-rw-   0        0        0      108 2023-04-19 12:23:39.000000 ejelabs-0.2/ejelabs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 11:19:26.012678 ejelabs-0.2/ejelabs.egg-info/
+-rw-rw-rw-   0        0        0      565 2023-05-20 11:19:25.000000 ejelabs-0.2/ejelabs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-05-20 11:19:25.000000 ejelabs-0.2/ejelabs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 11:19:25.000000 ejelabs-0.2/ejelabs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-05-20 11:19:25.000000 ejelabs-0.2/ejelabs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-20 11:19:25.000000 ejelabs-0.2/ejelabs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-20 11:19:26.020630 ejelabs-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      852 2023-05-20 11:19:02.000000 ejelabs-0.2/setup.py
```

### Comparing `ejelabs-0.1/LICENSE.txt` & `ejelabs-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ejelabs-0.1/PKG-INFO` & `ejelabs-0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ejelabs
-Version: 0.1
+Version: 0.2
 Summary: ejelabs
 Home-page: https://github.com/looqify/Instalabs
-Download-URL: https://github.com/looqify/Instalabs/archive/refs/tags/0.1.tar.gz
+Download-URL: https://github.com/looqify/Instalabs/archive/refs/tags/0.2.tar.gz
 Author: Looq
 Author-email: looqifi@gmail.com
 License: MIT
 Keywords: looq
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `ejelabs-0.1/ejelabs/Cracklabs.py` & `ejelabs-0.2/ejelabs/Cracklabs.py`

 * *Files identical despite different names*

### Comparing `ejelabs-0.1/ejelabs/Main.py` & `ejelabs-0.2/ejelabs/Main.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,19 +61,25 @@
                            *list(struct.pack('<h', len(encrypted_key))),
                            *list(encrypted_key),
                            *list(cipher_tag),
                            *list(encrypted_password)])
         encrypted = base64.b64encode(encrypted).decode('utf-8')
         return f'#PWD_INSTAGRAM_BROWSER:{version}:{time}:{encrypted}'
 
+    def _encbsc(self,  pw) -> None:
+        time = int(datetime.datetime.now().timestamp())
+        return f'#PWD_INSTAGRAM:0:{time}:{[pw]}'
+
     def _generate(self, seed: Union[str, bytes]) -> None:
         rand = random.Random(seed + str(datetime.date.today()))
         phone_id = str(UUID(int=rand.getrandbits(128), version=4))
         adid = str(UUID(int=rand.getrandbits(128), version=4))
         id = f"android-{''.join(rand.choices(string.hexdigits, k=16))}".lower()
         _uuid = str(UUID(int=rand.getrandbits(128), version=4))
         fdid = str(UUID(int=rand.getrandbits(128), version=4))
         jazoest = self._jazoest(phone_id)
-        return id, phone_id, adid, _uuid, fdid, jazoest
+        _sessid = f'UFS-{UUID(int=rand.getrandbits(128))}-0'
+        _time = str(round(time.time(), 3))
+        return _sessid, _time, id, phone_id, adid, _uuid, fdid, jazoest
 
     def _jazoest(self, phone_id) -> str:
         return f"2{sum(ord(i) for i in phone_id)}"
```

### Comparing `ejelabs-0.1/ejelabs.egg-info/PKG-INFO` & `ejelabs-0.2/ejelabs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ejelabs
-Version: 0.1
+Version: 0.2
 Summary: ejelabs
 Home-page: https://github.com/looqify/Instalabs
-Download-URL: https://github.com/looqify/Instalabs/archive/refs/tags/0.1.tar.gz
+Download-URL: https://github.com/looqify/Instalabs/archive/refs/tags/0.2.tar.gz
 Author: Looq
 Author-email: looqifi@gmail.com
 License: MIT
 Keywords: looq
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `ejelabs-0.1/setup.py` & `ejelabs-0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
     name='ejelabs',
     packages=['ejelabs'],
-    version='0.1',
+    version='0.2',
     license='MIT',
     description='ejelabs',
     author='Looq',
     author_email='looqifi@gmail.com',
     url='https://github.com/looqify/Instalabs',
-    download_url='https://github.com/looqify/Instalabs/archive/refs/tags/0.1.tar.gz',
+    download_url='https://github.com/looqify/Instalabs/archive/refs/tags/0.2.tar.gz',
     keywords=['looq'],
     install_requires=[
         'pycryptodomex',
         'PyNaCl',
         'fake-useragent'
     ],
     classifiers=[
```

