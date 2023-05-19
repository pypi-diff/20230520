# Comparing `tmp/uwu_codec-1.0.tar.gz` & `tmp/uwu_codec-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uwu_codec-1.0.tar", last modified: Tue May 16 22:46:42 2023, max compression
+gzip compressed data, was "uwu_codec-1.1.tar", last modified: Fri May 19 22:36:56 2023, max compression
```

## Comparing `uwu_codec-1.0.tar` & `uwu_codec-1.1.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-05-16 22:46:42.426879 uwu_codec-1.0/
--rw-r--r--   0 goldy     (1001) goldy     (1001)     3637 2023-05-16 22:46:42.426879 uwu_codec-1.0/PKG-INFO
--rw-r--r--   0 goldy     (1001) goldy     (1001)     2719 2023-05-16 22:46:20.000000 uwu_codec-1.0/README.md
--rw-r--r--   0 goldy     (1001) goldy     (1001)     2632 2023-05-16 21:45:11.000000 uwu_codec-1.0/pyproject.toml
--rw-r--r--   0 goldy     (1001) goldy     (1001)       38 2023-05-16 22:46:42.426879 uwu_codec-1.0/setup.cfg
-drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-05-16 22:46:42.425879 uwu_codec-1.0/uwu_codec/
--rw-r--r--   0 goldy     (1001) goldy     (1001)      519 2023-05-16 21:34:26.000000 uwu_codec-1.0/uwu_codec/__init__.py
--rw-r--r--   0 goldy     (1001) goldy     (1001)     1382 2023-05-16 21:47:48.000000 uwu_codec-1.0/uwu_codec/codec.py
-drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-05-16 22:46:42.426879 uwu_codec-1.0/uwu_codec.egg-info/
--rw-r--r--   0 goldy     (1001) goldy     (1001)     3637 2023-05-16 22:46:42.000000 uwu_codec-1.0/uwu_codec.egg-info/PKG-INFO
--rw-r--r--   0 goldy     (1001) goldy     (1001)      229 2023-05-16 22:46:42.000000 uwu_codec-1.0/uwu_codec.egg-info/SOURCES.txt
--rw-r--r--   0 goldy     (1001) goldy     (1001)        1 2023-05-16 22:46:42.000000 uwu_codec-1.0/uwu_codec.egg-info/dependency_links.txt
--rw-r--r--   0 goldy     (1001) goldy     (1001)      106 2023-05-16 22:46:42.000000 uwu_codec-1.0/uwu_codec.egg-info/requires.txt
--rw-r--r--   0 goldy     (1001) goldy     (1001)       10 2023-05-16 22:46:42.000000 uwu_codec-1.0/uwu_codec.egg-info/top_level.txt
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-05-19 22:36:56.191754 uwu_codec-1.1/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)       66 2023-05-16 23:04:32.000000 uwu_codec-1.1/.gitattributes
+-rw-r--r--   0 goldy     (1001) goldy     (1001)       52 2023-05-16 22:47:20.000000 uwu_codec-1.1/.gitignore
+-rwxr-xr-x   0 goldy     (1001) goldy     (1001)       74 2023-05-16 21:46:14.000000 uwu_codec-1.1/Makefile
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     3638 2023-05-19 22:36:56.191754 uwu_codec-1.1/PKG-INFO
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     2719 2023-05-16 22:47:26.000000 uwu_codec-1.1/README.md
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     2633 2023-05-16 23:08:12.000000 uwu_codec-1.1/pyproject.toml
+-rw-r--r--   0 goldy     (1001) goldy     (1001)       38 2023-05-19 22:36:56.191754 uwu_codec-1.1/setup.cfg
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-05-19 22:36:56.190754 uwu_codec-1.1/uwu_codec/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      517 2023-05-19 22:36:45.000000 uwu_codec-1.1/uwu_codec/__init__.py
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     1387 2023-05-19 22:21:52.000000 uwu_codec-1.1/uwu_codec/codec.py
+drwxr-xr-x   0 goldy     (1001) goldy     (1001)        0 2023-05-19 22:36:56.191754 uwu_codec-1.1/uwu_codec.egg-info/
+-rw-r--r--   0 goldy     (1001) goldy     (1001)     3638 2023-05-19 22:36:56.000000 uwu_codec-1.1/uwu_codec.egg-info/PKG-INFO
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      264 2023-05-19 22:36:56.000000 uwu_codec-1.1/uwu_codec.egg-info/SOURCES.txt
+-rw-r--r--   0 goldy     (1001) goldy     (1001)        1 2023-05-19 22:36:56.000000 uwu_codec-1.1/uwu_codec.egg-info/dependency_links.txt
+-rw-r--r--   0 goldy     (1001) goldy     (1001)      106 2023-05-19 22:36:56.000000 uwu_codec-1.1/uwu_codec.egg-info/requires.txt
+-rw-r--r--   0 goldy     (1001) goldy     (1001)       10 2023-05-19 22:36:56.000000 uwu_codec-1.1/uwu_codec.egg-info/top_level.txt
```

### Comparing `uwu_codec-1.0/PKG-INFO` & `uwu_codec-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: uwu_codec
-Version: 1.0
-Summary: Yep, your eyes are not deciving you. An UwU codec. 😳 Currently WIP...
+Version: 1.1
+Summary: Yep, your eyes are not deceiving you. An UwU codec. 😳 Currently WIP...
 Author-email: Goldy <goldy@devgoldy.xyz>
 Project-URL: GitHub, https://github.com/THEGOLDENPRO/uwu-codec
 Project-URL: BugTracker, https://github.com/THEGOLDENPRO/uwu-codec/issues
 Keywords: uwu,UwU,UwU Codec,uwu-codec,uwu encoder,uwu decoder
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `uwu_codec-1.0/README.md` & `uwu_codec-1.1/README.md`

 * *Files identical despite different names*

### Comparing `uwu_codec-1.0/pyproject.toml` & `uwu_codec-1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "uwu_codec"
-description = "Yep, your eyes are not deciving you. An UwU codec. 😳 Currently WIP..."
+description = "Yep, your eyes are not deceiving you. An UwU codec. 😳 Currently WIP..."
 authors = [
     {name = "Goldy", email = "goldy@devgoldy.xyz"},
 ]
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 keywords = [
```

### Comparing `uwu_codec-1.0/uwu_codec/__init__.py` & `uwu_codec-1.1/uwu_codec/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,9 +16,8 @@
 
 def enable():
     """🟢 Enable the UwUCodec."""
     codec = UwUCodec()
     codecs.register(lambda _: codecs.CodecInfo(codec.encode, codec.decode, name = "UwU"))
     codecs.register(lambda _: codecs.CodecInfo(codec.encode, codec.decode, name = "uwu"))
 
-__version__: Final[str] = "1.0"
-
+__version__: Final[str] = "1.1"
```

### Comparing `uwu_codec-1.0/uwu_codec/codec.py` & `uwu_codec-1.1/uwu_codec/codec.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,11 +33,11 @@
             string += uwu_byte
 
             if len(string) > 1 and string[-1] in ["U", "O"]:
                 yield decode_table[bytes(string, "ascii")]
                 string = ""
 
     def encode(self, string: str, errors: str = "strict") -> Tuple[bytes, int]:
-        return b"".join(encode_table[x] for x in string), len(string)
+        return b"".join(encode_table[x] for x in str(string)), len(string)
 
     def decode(self, bytes: bytes, errors: str = "strict") -> tuple[str, int]:
         return "".join(x for x in self.__uwu_splitter_gen__(bytes)), len(bytes)
```

### Comparing `uwu_codec-1.0/uwu_codec.egg-info/PKG-INFO` & `uwu_codec-1.1/uwu_codec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: uwu-codec
-Version: 1.0
-Summary: Yep, your eyes are not deciving you. An UwU codec. 😳 Currently WIP...
+Version: 1.1
+Summary: Yep, your eyes are not deceiving you. An UwU codec. 😳 Currently WIP...
 Author-email: Goldy <goldy@devgoldy.xyz>
 Project-URL: GitHub, https://github.com/THEGOLDENPRO/uwu-codec
 Project-URL: BugTracker, https://github.com/THEGOLDENPRO/uwu-codec/issues
 Keywords: uwu,UwU,UwU Codec,uwu-codec,uwu encoder,uwu decoder
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
```

