# Comparing `tmp/itkwasm_dicom_emscripten-2.0.2.tar.gz` & `tmp/itkwasm_dicom_emscripten-2.0.3.tar.gz`

## Comparing `itkwasm_dicom_emscripten-2.0.2.tar` & `itkwasm_dicom_emscripten-2.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/itkwasm_dicom_emscripten/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/itkwasm_dicom_emscripten/_version.py
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/itkwasm_dicom_emscripten/apply_presentation_state_to_image_async.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/itkwasm_dicom_emscripten/js_package.py
--rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/itkwasm_dicom_emscripten/read_dicom_encapsulated_pdf_async.py
--rw-r--r--   0        0        0    10552 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/itkwasm_dicom_emscripten/structured_report_to_html_async.py
--rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/itkwasm_dicom_emscripten/structured_report_to_text_async.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/test/__init__.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/test/fixtures.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/test/test_apply_presentation_state_to_image_async.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/test/test_itkwasm_dicom.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/test/test_read_dicom_encapsulated_pdf_async.py
--rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/test/test_structured_report_to_html_async.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/test/test_structured_report_to_text_async.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/.gitignore
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/README.md
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/itkwasm_dicom_emscripten/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/itkwasm_dicom_emscripten/_version.py
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/itkwasm_dicom_emscripten/apply_presentation_state_to_image_async.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/itkwasm_dicom_emscripten/js_package.py
+-rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/itkwasm_dicom_emscripten/read_dicom_encapsulated_pdf_async.py
+-rw-r--r--   0        0        0    10552 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/itkwasm_dicom_emscripten/structured_report_to_html_async.py
+-rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/itkwasm_dicom_emscripten/structured_report_to_text_async.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/test/__init__.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/test/fixtures.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/test/test_apply_presentation_state_to_image_async.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/test/test_itkwasm_dicom.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/test/test_read_dicom_encapsulated_pdf_async.py
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/test/test_structured_report_to_html_async.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/test/test_structured_report_to_text_async.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/.gitignore
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/README.md
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 itkwasm_dicom_emscripten-2.0.3/PKG-INFO
```

### Comparing `itkwasm_dicom_emscripten-2.0.2/itkwasm_dicom_emscripten/apply_presentation_state_to_image_async.py` & `itkwasm_dicom_emscripten-2.0.3/itkwasm_dicom_emscripten/apply_presentation_state_to_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.2/itkwasm_dicom_emscripten/read_dicom_encapsulated_pdf_async.py` & `itkwasm_dicom_emscripten-2.0.3/itkwasm_dicom_emscripten/read_dicom_encapsulated_pdf_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.2/itkwasm_dicom_emscripten/structured_report_to_html_async.py` & `itkwasm_dicom_emscripten-2.0.3/itkwasm_dicom_emscripten/structured_report_to_html_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,43 +89,39 @@
 
     :param processing_details: show currently processed content item
     :type  processing_details: bool
 
     :param unknown_relationship: accept unknown/missing relationship type
     :type  unknown_relationship: bool
 
-    :param invalid_item_value: accept invalid content item value
-(e.g. violation of VR or VM definition)
+    :param invalid_item_value: accept invalid content item value (e.g. violation of VR or VM definition)
     :type  invalid_item_value: bool
 
     :param ignore_constraints: ignore relationship content constraints
     :type  ignore_constraints: bool
 
-    :param ignore_item_errors: do not abort on content item errors, just warn
-(e.g. missing value type specific attributes)
+    :param ignore_item_errors: do not abort on content item errors, just warn (e.g. missing value type specific attributes)
     :type  ignore_item_errors: bool
 
     :param skip_invalid_items: skip invalid content items (incl. sub-tree)
     :type  skip_invalid_items: bool
 
     :param disable_vr_checker: disable check for VR-conformant string values
     :type  disable_vr_checker: bool
 
     :param charset_require: require declaration of ext. charset (default)
     :type  charset_require: bool
 
     :param charset_assume: [c]harset: string, assume charset c if no extended charset declared
     :type  charset_assume: str
 
-    :param charset_check_all: check all data elements with string values
-(default: only PN, LO, LT, SH, ST, UC and UT)
+    :param charset_check_all: check all data elements with string values (default: only PN, LO, LT, SH, ST, UC and UT)
     :type  charset_check_all: bool
 
-    :param convert_to_utf8: convert all element values that are affected
-by Specific Character Set (0008,0005) to UTF-8
+    :param convert_to_utf8: convert all element values that are affected by Specific Character Set (0008,0005) to UTF-8
     :type  convert_to_utf8: bool
 
     :param url_prefix: URL: string. Append specificed URL prefix to hyperlinks of referenced composite objects in the document.
     :type  url_prefix: str
 
     :param html_32: use only HTML version 3.2 compatible features
     :type  html_32: bool
```

### Comparing `itkwasm_dicom_emscripten-2.0.2/itkwasm_dicom_emscripten/structured_report_to_text_async.py` & `itkwasm_dicom_emscripten-2.0.3/itkwasm_dicom_emscripten/structured_report_to_text_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.2/test/fixtures.py` & `itkwasm_dicom_emscripten-2.0.3/test/fixtures.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.2/test/test_apply_presentation_state_to_image_async.py` & `itkwasm_dicom_emscripten-2.0.3/test/test_apply_presentation_state_to_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.2/test/test_itkwasm_dicom.py` & `itkwasm_dicom_emscripten-2.0.3/test/test_itkwasm_dicom.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.2/test/test_read_dicom_encapsulated_pdf_async.py` & `itkwasm_dicom_emscripten-2.0.3/test/test_read_dicom_encapsulated_pdf_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.2/test/test_structured_report_to_html_async.py` & `itkwasm_dicom_emscripten-2.0.3/test/test_structured_report_to_html_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.2/test/test_structured_report_to_text_async.py` & `itkwasm_dicom_emscripten-2.0.3/test/test_structured_report_to_text_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.2/pyproject.toml` & `itkwasm_dicom_emscripten-2.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `itkwasm_dicom_emscripten-2.0.2/PKG-INFO` & `itkwasm_dicom_emscripten-2.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itkwasm-dicom-emscripten
-Version: 2.0.2
+Version: 2.0.3
 Project-URL: Home, https://itk-wasm-dicom-python-docs.on.fleek.co
 Project-URL: Source, https://github.com/InsightSoftwareConsortium/itk-wasm
 Project-URL: Issues, https://github.com/InsightSoftwareConsortium/itk-wasm/issues
 License-Expression: Apache-2.0
 Keywords: emscripten,itkwasm,webassembly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: WebAssembly
```

