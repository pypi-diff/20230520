# Comparing `tmp/pytket_qir-0.2.0rc1-py3-none-any.whl.zip` & `tmp/pytket_qir-0.2.0rc2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,14 @@
-Zip file size: 9483 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat      867 b- defN 23-May-03 13:56 pytket/extensions/qir/__init__.py
--rw-rw-rw-  2.0 fat       71 b- defN 23-May-03 13:57 pytket/extensions/qir/_metadata.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-May-03 13:56 pytket/extensions/qir/py.typed
--rw-rw-rw-  2.0 fat      718 b- defN 23-May-03 13:56 pytket/extensions/qir/conversion/__init__.py
--rw-rw-rw-  2.0 fat      814 b- defN 23-May-03 13:56 pytket/extensions/qir/conversion/api.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-May-03 13:57 pytket_qir-0.2.0rc1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4296 b- defN 23-May-03 13:57 pytket_qir-0.2.0rc1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-03 13:57 pytket_qir-0.2.0rc1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-May-03 13:57 pytket_qir-0.2.0rc1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      873 b- defN 23-May-03 13:57 pytket_qir-0.2.0rc1.dist-info/RECORD
-10 files, 19296 bytes uncompressed, 7963 bytes compressed:  58.7%
+Zip file size: 17079 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat      882 b- defN 23-May-20 17:24 pytket/qir/__init__.py
+-rw-rw-rw-  2.0 fat       71 b- defN 23-May-20 17:24 pytket/qir/_metadata.py
+-rw-rw-rw-  2.0 fat      733 b- defN 23-May-20 17:24 pytket/qir/conversion/__init__.py
+-rw-rw-rw-  2.0 fat     1946 b- defN 23-May-20 17:24 pytket/qir/conversion/api.py
+-rw-rw-rw-  2.0 fat    26437 b- defN 23-May-20 17:24 pytket/qir/conversion/conversion.py
+-rw-rw-rw-  2.0 fat     4237 b- defN 23-May-20 17:24 pytket/qir/conversion/gatesets.py
+-rw-rw-rw-  2.0 fat     1529 b- defN 23-May-20 17:24 pytket/qir/conversion/module.py
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-May-20 17:24 pytket_qir-0.2.0rc2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4296 b- defN 23-May-20 17:24 pytket_qir-0.2.0rc2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-20 17:24 pytket_qir-0.2.0rc2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-May-20 17:24 pytket_qir-0.2.0rc2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1017 b- defN 23-May-20 17:24 pytket_qir-0.2.0rc2.dist-info/RECORD
+12 files, 52805 bytes uncompressed, 15357 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -1,31 +1,37 @@
-Filename: pytket/extensions/qir/__init__.py
+Filename: pytket/qir/__init__.py
 Comment: 
 
-Filename: pytket/extensions/qir/_metadata.py
+Filename: pytket/qir/_metadata.py
 Comment: 
 
-Filename: pytket/extensions/qir/py.typed
+Filename: pytket/qir/conversion/__init__.py
 Comment: 
 
-Filename: pytket/extensions/qir/conversion/__init__.py
+Filename: pytket/qir/conversion/api.py
 Comment: 
 
-Filename: pytket/extensions/qir/conversion/api.py
+Filename: pytket/qir/conversion/conversion.py
 Comment: 
 
-Filename: pytket_qir-0.2.0rc1.dist-info/LICENSE
+Filename: pytket/qir/conversion/gatesets.py
 Comment: 
 
-Filename: pytket_qir-0.2.0rc1.dist-info/METADATA
+Filename: pytket/qir/conversion/module.py
 Comment: 
 
-Filename: pytket_qir-0.2.0rc1.dist-info/WHEEL
+Filename: pytket_qir-0.2.0rc2.dist-info/LICENSE
 Comment: 
 
-Filename: pytket_qir-0.2.0rc1.dist-info/top_level.txt
+Filename: pytket_qir-0.2.0rc2.dist-info/METADATA
 Comment: 
 
-Filename: pytket_qir-0.2.0rc1.dist-info/RECORD
+Filename: pytket_qir-0.2.0rc2.dist-info/WHEEL
+Comment: 
+
+Filename: pytket_qir-0.2.0rc2.dist-info/top_level.txt
+Comment: 
+
+Filename: pytket_qir-0.2.0rc2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pytket/extensions/qir/__init__.py` & `pytket/qir/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # limitations under the License.
 
 """Backends for processing pytket circuits with Quantinuum devices
 """
 
 # _metadata.py is copied to the folder after installation.
 from ._metadata import __extension_version__, __extension_name__  # type: ignore
-from .conversion import pytket_to_qir
+from .conversion import pytket_to_qir, ReturnTypeQIR
```

## Comparing `pytket/extensions/qir/conversion/__init__.py` & `pytket/qir/conversion/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Backends for processing pytket circuits with Quantinuum devices
 """
 
-from .api import pytket_to_qir
+from .api import pytket_to_qir, ReturnTypeQIR
```

## Comparing `pytket_qir-0.2.0rc1.dist-info/LICENSE` & `pytket_qir-0.2.0rc2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pytket_qir-0.2.0rc1.dist-info/METADATA` & `pytket_qir-0.2.0rc2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-qir
-Version: 0.2.0rc1
+Version: 0.2.0rc2
 Summary: Extension for pytket, providing functions for conversion into to qir
 Author: TKET development team
 Author-email: tket-support@cambridgequantum.com
 License: Apache 2
 Project-URL: Documentation, https://cqcl.github.io/pytket-qir/api/index.html
 Project-URL: Source, https://github.com/CQCL/pytket-qir
 Project-URL: Tracker, https://github.com/CQCL/pytket-qir/issues
```

