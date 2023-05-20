# Comparing `tmp/fenjing-0.3.4.tar.gz` & `tmp/fenjing-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.3.4.tar", last modified: Thu May 18 09:11:26 2023, max compression
+gzip compressed data, was "fenjing-0.3.5.tar", last modified: Sat May 20 12:11:01 2023, max compression
```

## Comparing `fenjing-0.3.4.tar` & `fenjing-0.3.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:11:26.248942 fenjing-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-18 09:11:15.000000 fenjing-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-18 09:11:15.000000 fenjing-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-05-18 09:11:26.248942 fenjing-0.3.4/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     6068 2023-05-18 09:11:15.000000 fenjing-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-18 09:11:15.000000 fenjing-0.3.4/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:11:26.248942 fenjing-0.3.4/fenjing/
--rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-05-18 09:11:15.000000 fenjing-0.3.4/fenjing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-18 09:11:15.000000 fenjing-0.3.4/fenjing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-05-18 09:11:15.000000 fenjing-0.3.4/fenjing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-18 09:11:15.000000 fenjing-0.3.4/fenjing/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-18 09:11:15.000000 fenjing-0.3.4/fenjing/config_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-18 09:11:15.000000 fenjing-0.3.4/fenjing/const.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-05-18 09:11:15.000000 fenjing-0.3.4/fenjing/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-18 09:11:15.000000 fenjing-0.3.4/fenjing/form.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-18 09:11:15.000000 fenjing-0.3.4/fenjing/form_cracker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4234 2023-05-18 09:11:15.000000 fenjing-0.3.4/fenjing/full_payload_gen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-05-18 09:11:15.000000 fenjing-0.3.4/fenjing/int_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    27358 2023-05-18 09:11:15.000000 fenjing-0.3.4/fenjing/payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-18 09:11:15.000000 fenjing-0.3.4/fenjing/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-18 09:11:15.000000 fenjing-0.3.4/fenjing/scan_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-18 09:11:15.000000 fenjing-0.3.4/fenjing/shell_payload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:11:26.248942 fenjing-0.3.4/fenjing/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-05-18 09:11:15.000000 fenjing-0.3.4/fenjing/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-18 09:11:15.000000 fenjing-0.3.4/fenjing/waf_func_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-05-18 09:11:15.000000 fenjing-0.3.4/fenjing/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:11:26.248942 fenjing-0.3.4/fenjing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-05-18 09:11:26.000000 fenjing-0.3.4/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-18 09:11:26.000000 fenjing-0.3.4/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 09:11:26.000000 fenjing-0.3.4/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-18 09:11:26.000000 fenjing-0.3.4/fenjing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-18 09:11:26.000000 fenjing-0.3.4/fenjing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-18 09:11:15.000000 fenjing-0.3.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 09:11:26.248942 fenjing-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-18 09:11:15.000000 fenjing-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:11:01.751224 fenjing-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-20 12:10:42.000000 fenjing-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-20 12:10:42.000000 fenjing-0.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-05-20 12:11:01.751224 fenjing-0.3.5/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6068 2023-05-20 12:10:42.000000 fenjing-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-20 12:10:42.000000 fenjing-0.3.5/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:11:01.751224 fenjing-0.3.5/fenjing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/config_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/const.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/form_cracker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4234 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/full_payload_gen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/int_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28571 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/scan_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/shell_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:11:01.751224 fenjing-0.3.5/fenjing/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/waf_func_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-05-20 12:10:42.000000 fenjing-0.3.5/fenjing/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:11:01.751224 fenjing-0.3.5/fenjing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-05-20 12:11:01.000000 fenjing-0.3.5/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-20 12:11:01.000000 fenjing-0.3.5/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 12:11:01.000000 fenjing-0.3.5/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-20 12:11:01.000000 fenjing-0.3.5/fenjing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-20 12:11:01.000000 fenjing-0.3.5/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-20 12:10:42.000000 fenjing-0.3.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 12:11:01.751224 fenjing-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-20 12:10:42.000000 fenjing-0.3.5/setup.py
```

### Comparing `fenjing-0.3.4/LICENSE` & `fenjing-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.4/PKG-INFO` & `fenjing-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.3.4
+Version: 0.3.5
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.3.4/README.md` & `fenjing-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.4/fenjing/cli.py` & `fenjing-0.3.5/fenjing/cli.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.4/fenjing/colorize.py` & `fenjing-0.3.5/fenjing/colorize.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.4/fenjing/config_payload.py` & `fenjing-0.3.5/fenjing/config_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.4/fenjing/const.py` & `fenjing-0.3.5/fenjing/const.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 INTEGER = "integer"
 STRING_STRING_CONCNAT = "string_string_concat"
 STRING_PERCENT = "string_percent"
 STRING_PERCENT_LOWER_C = "string_percent_lower_c"
 STRING_UNDERLINE = "string_underline"
 STRING_LOWERC = "string_lower_c"
 STRING_MANY_PERCENT_LOWER_C = "string_many_percent_lower_c"
+STRING_MANY_FORMAT_C = "string_many_format_c"
 STRING = "string"
 FORMULAR_SUM = "formular_sum"
 ATTRIBUTE = "attribute"
 ITEM = "item"
 CLASS_ATTRIBUTE = "class_attribute"
 CHAINED_ATTRIBUTE_ITEM = "chained_attribute_item"
 EVAL_FUNC = "eval_func"
```

### Comparing `fenjing-0.3.4/fenjing/form.py` & `fenjing-0.3.5/fenjing/form.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.4/fenjing/form_cracker.py` & `fenjing-0.3.5/fenjing/form_cracker.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.4/fenjing/full_payload_gen.py` & `fenjing-0.3.5/fenjing/full_payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.4/fenjing/int_vars.py` & `fenjing-0.3.5/fenjing/int_vars.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.4/fenjing/payload_gen.py` & `fenjing-0.3.5/fenjing/payload_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,14 +247,24 @@
         return [
             (UNSATISFIED, )
         ]
     return [
         (LITERAL, str(value))
     ]
 
+@req_gen
+def gen_positive_integer_hex(context: dict, value: int):
+    if value < 0:
+        return [
+            (UNSATISFIED, )
+        ]
+    return [
+        (LITERAL, hex(value))
+    ]
+
 
 @req_gen
 def gen_positive_integer_sum(context: dict, value: int):
     if value < 0:
         return [
             (UNSATISFIED, )
         ]
@@ -459,14 +469,29 @@
         (LITERAL, ")|list|first|last)*"),
         (INTEGER, 2),
         (LITERAL, "][dict(chr=x)|join]("),
         (INTEGER, 37),
         (LITERAL, "))"),
     ]
 
+@req_gen
+def gen_string_percent_urlencodelong(context):
+    return [
+        (LITERAL, "((lipsum,)|map(((lipsum|string|list|batch(3)|first|last)" + 
+            "~(lipsum|string|list|batch(15)|first|last)" + 
+            "~(lipsum|string|list|batch(20)|first|last)" + 
+            "~(x|pprint|list|batch(4)|first|last)" + 
+            "~(x|pprint|list|batch(2)|first|last)" + 
+            "~(lipsum|string|list|batch(5)|first|last)" + 
+            "~(lipsum|string|list|batch(8)|first|last)" + 
+            "~(x|pprint|list|batch(3)|first|last)" + 
+            "~(x|pprint|list|batch(4)|first|last)))|list|first|first)")
+    ]
+
+
 # ---
 
 
 @req_gen
 def gen_string_lower_c_literal1(context):
     return [
         (LITERAL, "'c'")
@@ -613,14 +638,26 @@
 def gen_string_underline_tupleselect(context):
     return [
         (LITERAL, "(()|select|string|batch("),
         (INTEGER, 25),
         (LITERAL, ")|first|last)")
     ]
 
+@req_gen
+def gen_string_many_format_c_complex(context, num):
+    parts = "(({c})*{l})".format(
+        c="{1:2}|string|replace({1:2}|string|batch(4)|first|last,{}|join)|replace(1|string,{}|join)|replace(2|string,LOWERC)",
+        l=num
+    ).partition("LOWERC")
+    return [
+        (LITERAL, parts[0]),
+        (STRING_LOWERC, ),
+        (LITERAL, parts[2])
+    ]
+
 
 # ---
 # 以下的gen_string会互相依赖，但是产生互相依赖时传入的字符串长度会减少所以不会发生无限调用
 
 @req_gen
 def gen_string_1(context: dict, value: str):
     chars = [c if c != "\'" else "\\\'" for c in value]
@@ -887,19 +924,19 @@
     # (FORMAT(97,98,99))
     # FORMAT = (CS.format)
     # CS = (C*L)
     if re.match("^[a-z]+$", value): # avoid infinite recursion
         return [
             (UNSATISFIED, )
         ]
-    cs = "(({c})*{l})".format(
-        c="{1:2}|string|replace({1:2}|string|batch(4)|first|last,{}|join)|replace(1|string,{}|join)|replace(2|string,dict(c=1)|join)",
-        l=len(value)
-    )
-    format_func = (ATTRIBUTE, (LITERAL, cs), "format")
+    # cs = "(({c})*{l})".format(
+    #     c="{1:2}|string|replace({1:2}|string|batch(4)|first|last,{}|join)|replace(1|string,{}|join)|replace(2|string,dict(c=x)|join)",
+    #     l=len(value)
+    # )
+    format_func = (ATTRIBUTE, (STRING_MANY_FORMAT_C, len(value)), "format")
     req = [
         (LITERAL, "("),
         format_func,
         (LITERAL, "("),
         (LITERAL, ",".join(str(ord(c)) for c in value)),
         (LITERAL, "))")
     ]
```

### Comparing `fenjing-0.3.4/fenjing/requester.py` & `fenjing-0.3.5/fenjing/requester.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.4/fenjing/scan_url.py` & `fenjing-0.3.5/fenjing/scan_url.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.4/fenjing/shell_payload.py` & `fenjing-0.3.5/fenjing/shell_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.4/fenjing/templates/index.html` & `fenjing-0.3.5/fenjing/templates/index.html`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.4/fenjing/waf_func_gen.py` & `fenjing-0.3.5/fenjing/waf_func_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.4/fenjing/webui.py` & `fenjing-0.3.5/fenjing/webui.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.4/fenjing.egg-info/PKG-INFO` & `fenjing-0.3.5/fenjing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.3.4
+Version: 0.3.5
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.3.4/fenjing.egg-info/SOURCES.txt` & `fenjing-0.3.5/fenjing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.4/setup.py` & `fenjing-0.3.5/setup.py`

 * *Files identical despite different names*

