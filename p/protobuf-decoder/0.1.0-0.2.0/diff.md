# Comparing `tmp/protobuf_decoder-0.1.0.tar.gz` & `tmp/protobuf_decoder-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protobuf_decoder-0.1.0.tar", last modified: Sun Oct  9 15:10:18 2022, max compression
+gzip compressed data, was "protobuf_decoder-0.2.0.tar", last modified: Sat May 20 11:03:40 2023, max compression
```

## Comparing `protobuf_decoder-0.1.0.tar` & `protobuf_decoder-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dannyhan   (501) staff       (20)        0 2022-10-09 15:10:18.783888 protobuf_decoder-0.1.0/
--rw-r--r--   0 dannyhan   (501) staff       (20)     1066 2022-10-09 06:36:46.000000 protobuf_decoder-0.1.0/LICENSE
--rw-r--r--   0 dannyhan   (501) staff       (20)     1955 2022-10-09 15:10:18.783773 protobuf_decoder-0.1.0/PKG-INFO
--rw-r--r--   0 dannyhan   (501) staff       (20)     1472 2022-10-09 06:36:46.000000 protobuf_decoder-0.1.0/README.md
-drwxr-xr-x   0 dannyhan   (501) staff       (20)        0 2022-10-09 15:10:18.783111 protobuf_decoder-0.1.0/protobuf_decoder/
--rw-r--r--   0 dannyhan   (501) staff       (20)        0 2022-10-09 06:36:46.000000 protobuf_decoder-0.1.0/protobuf_decoder/__init__.py
--rw-r--r--   0 dannyhan   (501) staff       (20)     8555 2022-10-09 14:49:09.000000 protobuf_decoder-0.1.0/protobuf_decoder/protobuf_decoder.py
-drwxr-xr-x   0 dannyhan   (501) staff       (20)        0 2022-10-09 15:10:18.783619 protobuf_decoder-0.1.0/protobuf_decoder.egg-info/
--rw-r--r--   0 dannyhan   (501) staff       (20)     1955 2022-10-09 15:10:18.000000 protobuf_decoder-0.1.0/protobuf_decoder.egg-info/PKG-INFO
--rw-r--r--   0 dannyhan   (501) staff       (20)      252 2022-10-09 15:10:18.000000 protobuf_decoder-0.1.0/protobuf_decoder.egg-info/SOURCES.txt
--rw-r--r--   0 dannyhan   (501) staff       (20)        1 2022-10-09 15:10:18.000000 protobuf_decoder-0.1.0/protobuf_decoder.egg-info/dependency_links.txt
--rw-r--r--   0 dannyhan   (501) staff       (20)       17 2022-10-09 15:10:18.000000 protobuf_decoder-0.1.0/protobuf_decoder.egg-info/top_level.txt
--rw-r--r--   0 dannyhan   (501) staff       (20)       38 2022-10-09 15:10:18.783926 protobuf_decoder-0.1.0/setup.cfg
--rw-r--r--   0 dannyhan   (501) staff       (20)      662 2022-10-09 15:01:06.000000 protobuf_decoder-0.1.0/setup.py
+drwxr-xr-x   0 dannyhan   (501) staff       (20)        0 2023-05-20 11:03:40.705109 protobuf_decoder-0.2.0/
+-rw-r--r--   0 dannyhan   (501) staff       (20)     1066 2022-10-09 06:36:46.000000 protobuf_decoder-0.2.0/LICENSE
+-rw-r--r--   0 dannyhan   (501) staff       (20)     2116 2023-05-20 11:03:40.704996 protobuf_decoder-0.2.0/PKG-INFO
+-rw-r--r--   0 dannyhan   (501) staff       (20)     1633 2022-11-21 13:17:41.000000 protobuf_decoder-0.2.0/README.md
+drwxr-xr-x   0 dannyhan   (501) staff       (20)        0 2023-05-20 11:03:40.704390 protobuf_decoder-0.2.0/protobuf_decoder/
+-rw-r--r--   0 dannyhan   (501) staff       (20)        0 2022-11-21 13:17:41.000000 protobuf_decoder-0.2.0/protobuf_decoder/__init__.py
+-rw-r--r--   0 dannyhan   (501) staff       (20)    12490 2023-05-20 11:02:52.000000 protobuf_decoder-0.2.0/protobuf_decoder/protobuf_decoder.py
+drwxr-xr-x   0 dannyhan   (501) staff       (20)        0 2023-05-20 11:03:40.704827 protobuf_decoder-0.2.0/protobuf_decoder.egg-info/
+-rw-r--r--   0 dannyhan   (501) staff       (20)     2116 2023-05-20 11:03:40.000000 protobuf_decoder-0.2.0/protobuf_decoder.egg-info/PKG-INFO
+-rw-r--r--   0 dannyhan   (501) staff       (20)      252 2023-05-20 11:03:40.000000 protobuf_decoder-0.2.0/protobuf_decoder.egg-info/SOURCES.txt
+-rw-r--r--   0 dannyhan   (501) staff       (20)        1 2023-05-20 11:03:40.000000 protobuf_decoder-0.2.0/protobuf_decoder.egg-info/dependency_links.txt
+-rw-r--r--   0 dannyhan   (501) staff       (20)       17 2023-05-20 11:03:40.000000 protobuf_decoder-0.2.0/protobuf_decoder.egg-info/top_level.txt
+-rw-r--r--   0 dannyhan   (501) staff       (20)       38 2023-05-20 11:03:40.705144 protobuf_decoder-0.2.0/setup.cfg
+-rw-r--r--   0 dannyhan   (501) staff       (20)      662 2023-05-20 11:03:39.000000 protobuf_decoder-0.2.0/setup.py
```

### Comparing `protobuf_decoder-0.1.0/LICENSE` & `protobuf_decoder-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `protobuf_decoder-0.1.0/PKG-INFO` & `protobuf_decoder-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protobuf_decoder
-Version: 0.1.0
+Version: 0.2.0
 Summary: Decode protobuf without proto file
 Home-page: https://github.com/dannyhann/protobuf_decoder
 Author: danny han
 Author-email: rhrnak0501@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -40,14 +40,15 @@
     {
       "a": "테스트"
     }
 
     # binary
     0A 09 ED 85 8C EC 8A A4 ED 8A B8
 """
+from protobuf_decoder.protobuf_decoder import Parser
 
 test_target = "0A 09 ED 85 8C EC 8A A4 ED 8A B8"
 parsed_data = Parser().parse(test_target)
 >> parsed_data
 >> [ParsedResult(field=1, wire_type="string", data='테스트')]
 ```
 
@@ -69,14 +70,16 @@
             "b": 150
             }
     }
 
     # binary
     1a 03 08 96 01
 """
+from protobuf_decoder.protobuf_decoder import Parser
+
 test_target = "1a 03 08 96 01"
 parsed_data = Parser().parse(test_target)
 
 >> parsed_data
 >> [ParsedResult(field=3, wire_type="length_delimited", data=[ParsedResult(field=1, wire_type="varint", data=150)])]
 ```
 
@@ -92,14 +95,16 @@
       "a": "✊"
     }
 
     # binary
     0A 03 E2 9C 8A
 
     """
+from protobuf_decoder.protobuf_decoder import Parser
+
 test_target = "0A 03 E2 9C 8A"
 parsed_data = Parser().parse(test_target)
 >> parsed_data
 >> [ParsedResult(field=1, wire_type="string", data='✊')]
 ```
 
 # Reference
```

### Comparing `protobuf_decoder-0.1.0/README.md` & `protobuf_decoder-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     {
       "a": "테스트"
     }
 
     # binary
     0A 09 ED 85 8C EC 8A A4 ED 8A B8
 """
+from protobuf_decoder.protobuf_decoder import Parser
 
 test_target = "0A 09 ED 85 8C EC 8A A4 ED 8A B8"
 parsed_data = Parser().parse(test_target)
 >> parsed_data
 >> [ParsedResult(field=1, wire_type="string", data='테스트')]
 ```
 
@@ -53,14 +54,16 @@
             "b": 150
             }
     }
 
     # binary
     1a 03 08 96 01
 """
+from protobuf_decoder.protobuf_decoder import Parser
+
 test_target = "1a 03 08 96 01"
 parsed_data = Parser().parse(test_target)
 
 >> parsed_data
 >> [ParsedResult(field=3, wire_type="length_delimited", data=[ParsedResult(field=1, wire_type="varint", data=150)])]
 ```
 
@@ -76,14 +79,16 @@
       "a": "✊"
     }
 
     # binary
     0A 03 E2 9C 8A
 
     """
+from protobuf_decoder.protobuf_decoder import Parser
+
 test_target = "0A 03 E2 9C 8A"
 parsed_data = Parser().parse(test_target)
 >> parsed_data
 >> [ParsedResult(field=1, wire_type="string", data='✊')]
 ```
 
 # Reference
```

### Comparing `protobuf_decoder-0.1.0/protobuf_decoder.egg-info/PKG-INFO` & `protobuf_decoder-0.2.0/protobuf_decoder.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protobuf-decoder
-Version: 0.1.0
+Version: 0.2.0
 Summary: Decode protobuf without proto file
 Home-page: https://github.com/dannyhann/protobuf_decoder
 Author: danny han
 Author-email: rhrnak0501@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -40,14 +40,15 @@
     {
       "a": "테스트"
     }
 
     # binary
     0A 09 ED 85 8C EC 8A A4 ED 8A B8
 """
+from protobuf_decoder.protobuf_decoder import Parser
 
 test_target = "0A 09 ED 85 8C EC 8A A4 ED 8A B8"
 parsed_data = Parser().parse(test_target)
 >> parsed_data
 >> [ParsedResult(field=1, wire_type="string", data='테스트')]
 ```
 
@@ -69,14 +70,16 @@
             "b": 150
             }
     }
 
     # binary
     1a 03 08 96 01
 """
+from protobuf_decoder.protobuf_decoder import Parser
+
 test_target = "1a 03 08 96 01"
 parsed_data = Parser().parse(test_target)
 
 >> parsed_data
 >> [ParsedResult(field=3, wire_type="length_delimited", data=[ParsedResult(field=1, wire_type="varint", data=150)])]
 ```
 
@@ -92,14 +95,16 @@
       "a": "✊"
     }
 
     # binary
     0A 03 E2 9C 8A
 
     """
+from protobuf_decoder.protobuf_decoder import Parser
+
 test_target = "0A 03 E2 9C 8A"
 parsed_data = Parser().parse(test_target)
 >> parsed_data
 >> [ParsedResult(field=1, wire_type="string", data='✊')]
 ```
 
 # Reference
```

### Comparing `protobuf_decoder-0.1.0/setup.py` & `protobuf_decoder-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="protobuf_decoder",
-    version="0.1.0",
+    version="0.2.0",
     author="danny han",
     author_email="rhrnak0501@gmail.com",
     description="Decode protobuf without proto file",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dannyhann/protobuf_decoder",
     packages=setuptools.find_packages(),
```

