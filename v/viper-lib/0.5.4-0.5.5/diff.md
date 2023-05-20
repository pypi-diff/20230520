# Comparing `tmp/viper_lib-0.5.4.tar.gz` & `tmp/viper_lib-0.5.5.tar.gz`

## Comparing `viper_lib-0.5.4.tar` & `viper_lib-0.5.5.tar`

### file list

```diff
@@ -1,55 +1,56 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper.pth
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/__init__.py
--rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/async_utils.py
--rw-r--r--   0        0        0    10263 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/better_threading.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/cucumber.py
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/cucumber_main.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/exceptions.py
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/format.py
--rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/frozendict.py
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/interactive.py
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/persistent.py
--rw-r--r--   0        0        0    15408 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/pickle_utils.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/test_client.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/test_server.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/warnings.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/abc/__init__.py
--rw-r--r--   0        0        0     7181 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/abc/connection.py
--rw-r--r--   0        0        0     2957 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/abc/flux.py
--rw-r--r--   0        0        0     9410 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/abc/io.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/building/__init__.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/building/cy_clean.py
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/building/cy_compile.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/building/module_tools.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/compress/__init__.py
--rw-r--r--   0        0        0     8976 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/compress/flux.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/crypto/__init__.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/crypto/exceptions.py
--rw-r--r--   0        0        0    27802 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/crypto/flux.py
--rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/crypto/session.py
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/crypto/utils.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/debugging/__init__.py
--rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/debugging/chrono.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/debugging/utils.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/evolve/__init__.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/evolve/primitives.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/evolve/types/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/evolve/types/utils.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/meta/__init__.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/meta/contextual.py
--rw-r--r--   0        0        0     5606 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/meta/decorators.py
--rw-r--r--   0        0        0    16443 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/meta/iterable.py
--rw-r--r--   0        0        0    17549 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/meta/procedural.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/meta/prototype.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/meta/secret.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/meta/specialized.py
--rw-r--r--   0        0        0    15921 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/meta/static.py
--rw-r--r--   0        0        0     6223 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/meta/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/partition/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/partition/memory.py
--rw-r--r--   0        0        0    14044 2020-02-02 00:00:00.000000 viper_lib-0.5.4/Viper/partition/primitives.py
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 viper_lib-0.5.4/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 viper_lib-0.5.4/LICENSE
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 viper_lib-0.5.4/README.md
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 viper_lib-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 viper_lib-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 viper_lib-0.5.5/Viper.pth
+-rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 viper_lib-0.5.5/async_utils.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 viper_lib-0.5.5/cucumber.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 viper_lib-0.5.5/cucumber_main.py
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 viper_lib-0.5.5/persistent.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 viper_lib-0.5.5/test.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 viper_lib-0.5.5/test_client.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 viper_lib-0.5.5/test_server.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 viper_lib-0.5.5/Viper/__init__.py
+-rw-r--r--   0        0        0    10263 2020-02-02 00:00:00.000000 viper_lib-0.5.5/Viper/better_threading.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 viper_lib-0.5.5/Viper/exceptions.py
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 viper_lib-0.5.5/Viper/format.py
+-rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 viper_lib-0.5.5/Viper/frozendict.py
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 viper_lib-0.5.5/Viper/interactive.py
+-rw-r--r--   0        0        0    15408 2020-02-02 00:00:00.000000 viper_lib-0.5.5/Viper/pickle_utils.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 viper_lib-0.5.5/Viper/warnings.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 viper_lib-0.5.5/Viper/abc/__init__.py
+-rw-r--r--   0        0        0     7181 2020-02-02 00:00:00.000000 viper_lib-0.5.5/Viper/abc/connection.py
+-rw-r--r--   0        0        0     2957 2020-02-02 00:00:00.000000 viper_lib-0.5.5/Viper/abc/flux.py
+-rw-r--r--   0        0        0     9410 2020-02-02 00:00:00.000000 viper_lib-0.5.5/Viper/abc/io.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 viper_lib-0.5.5/Viper/building/__init__.py
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 viper_lib-0.5.5/Viper/building/module_tools.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 viper_lib-0.5.5/Viper/compress/__init__.py
+-rw-r--r--   0        0        0     8976 2020-02-02 00:00:00.000000 viper_lib-0.5.5/Viper/compress/flux.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 viper_lib-0.5.5/Viper/debugging/__init__.py
+-rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 viper_lib-0.5.5/Viper/debugging/chrono.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 viper_lib-0.5.5/Viper/debugging/utils.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 viper_lib-0.5.5/Viper/meta/__init__.py
+-rw-r--r--   0        0        0     5606 2020-02-02 00:00:00.000000 viper_lib-0.5.5/Viper/meta/decorators.py
+-rw-r--r--   0        0        0    16443 2020-02-02 00:00:00.000000 viper_lib-0.5.5/Viper/meta/iterable.py
+-rw-r--r--   0        0        0    17549 2020-02-02 00:00:00.000000 viper_lib-0.5.5/Viper/meta/procedural.py
+-rw-r--r--   0        0        0     6223 2020-02-02 00:00:00.000000 viper_lib-0.5.5/Viper/meta/utils.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 viper_lib-0.5.5/building/cy_clean.py
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 viper_lib-0.5.5/building/cy_compile.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 viper_lib-0.5.5/crypto/__init__.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 viper_lib-0.5.5/crypto/exceptions.py
+-rw-r--r--   0        0        0    27802 2020-02-02 00:00:00.000000 viper_lib-0.5.5/crypto/flux.py
+-rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 viper_lib-0.5.5/crypto/session.py
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 viper_lib-0.5.5/crypto/utils.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 viper_lib-0.5.5/evolve/__init__.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 viper_lib-0.5.5/evolve/primitives.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 viper_lib-0.5.5/evolve/types/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 viper_lib-0.5.5/evolve/types/utils.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 viper_lib-0.5.5/meta/contextual.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 viper_lib-0.5.5/meta/prototype.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 viper_lib-0.5.5/meta/secret.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 viper_lib-0.5.5/meta/specialized.py
+-rw-r--r--   0        0        0    15921 2020-02-02 00:00:00.000000 viper_lib-0.5.5/meta/static.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 viper_lib-0.5.5/partition/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 viper_lib-0.5.5/partition/memory.py
+-rw-r--r--   0        0        0    14044 2020-02-02 00:00:00.000000 viper_lib-0.5.5/partition/primitives.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 viper_lib-0.5.5/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 viper_lib-0.5.5/LICENSE
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 viper_lib-0.5.5/README.md
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 viper_lib-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 viper_lib-0.5.5/PKG-INFO
```

### Comparing `viper_lib-0.5.4/Viper/async_utils.py` & `viper_lib-0.5.5/async_utils.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/better_threading.py` & `viper_lib-0.5.5/Viper/better_threading.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/cucumber_main.py` & `viper_lib-0.5.5/cucumber_main.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/format.py` & `viper_lib-0.5.5/Viper/format.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/frozendict.py` & `viper_lib-0.5.5/Viper/frozendict.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,16 +80,14 @@
     def __ror__(self, __value: Mapping[K, V]) -> "frozendict[K, V]":
         return frozendict(super().__ror__(__value))
     
     @staticmethod
     def fromkeys(iterable : Iterable[K], value : V | None = None) -> "frozendict[K, V | None]":
         return frozendict(super().fromkeys(iterable, value))
 
-
 clean_annotations(frozendict)
-replace_module("Viper.frozendict", frozendict)
 
 
 
 
 
 del clean_annotations, replace_module, Any, Iterable, Mapping, TypeVar, K, V
```

### Comparing `viper_lib-0.5.4/Viper/interactive.py` & `viper_lib-0.5.5/Viper/interactive.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/persistent.py` & `viper_lib-0.5.5/persistent.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/pickle_utils.py` & `viper_lib-0.5.5/Viper/pickle_utils.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/test_client.py` & `viper_lib-0.5.5/test_client.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/test_server.py` & `viper_lib-0.5.5/test_server.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/warnings.py` & `viper_lib-0.5.5/Viper/warnings.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/abc/connection.py` & `viper_lib-0.5.5/Viper/abc/connection.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/abc/flux.py` & `viper_lib-0.5.5/Viper/abc/flux.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/abc/io.py` & `viper_lib-0.5.5/Viper/abc/io.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/building/cy_clean.py` & `viper_lib-0.5.5/building/cy_clean.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/building/cy_compile.py` & `viper_lib-0.5.5/building/cy_compile.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/building/module_tools.py` & `viper_lib-0.5.5/Viper/building/module_tools.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/compress/flux.py` & `viper_lib-0.5.5/Viper/compress/flux.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/crypto/exceptions.py` & `viper_lib-0.5.5/crypto/exceptions.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/crypto/flux.py` & `viper_lib-0.5.5/crypto/flux.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/crypto/session.py` & `viper_lib-0.5.5/crypto/session.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/crypto/utils.py` & `viper_lib-0.5.5/crypto/utils.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/debugging/chrono.py` & `viper_lib-0.5.5/Viper/debugging/chrono.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/debugging/utils.py` & `viper_lib-0.5.5/Viper/debugging/utils.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/evolve/primitives.py` & `viper_lib-0.5.5/evolve/primitives.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/meta/contextual.py` & `viper_lib-0.5.5/meta/contextual.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/meta/decorators.py` & `viper_lib-0.5.5/Viper/meta/decorators.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/meta/iterable.py` & `viper_lib-0.5.5/Viper/meta/iterable.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/meta/procedural.py` & `viper_lib-0.5.5/Viper/meta/procedural.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/meta/secret.py` & `viper_lib-0.5.5/meta/secret.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/meta/specialized.py` & `viper_lib-0.5.5/meta/specialized.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/meta/static.py` & `viper_lib-0.5.5/meta/static.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/meta/utils.py` & `viper_lib-0.5.5/Viper/meta/utils.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/Viper/partition/primitives.py` & `viper_lib-0.5.5/partition/primitives.py`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/.gitignore` & `viper_lib-0.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/LICENSE` & `viper_lib-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/README.md` & `viper_lib-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `viper_lib-0.5.4/pyproject.toml` & `viper_lib-0.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "viper_lib"
-version = "0.5.4"
+version = "0.5.5"
 authors = [
   { name="Vincent Raulin", email="vincent.raulin.n7@gmail.com" },
 ]
 description = "A Python library full of useful Python tools."
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
```

### Comparing `viper_lib-0.5.4/PKG-INFO` & `viper_lib-0.5.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viper_lib
-Version: 0.5.4
+Version: 0.5.5
 Summary: A Python library full of useful Python tools.
 Project-URL: Repository, https://github.com/MrVoustache/Viper
 Project-URL: Bug Tracker, https://github.com/MrVoustache/Viper/issues
 Author-email: Vincent Raulin <vincent.raulin.n7@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Vincent Raulin
```

