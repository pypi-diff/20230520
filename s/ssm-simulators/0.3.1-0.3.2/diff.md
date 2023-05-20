# Comparing `tmp/ssm-simulators-0.3.1.tar.gz` & `tmp/ssm-simulators-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssm-simulators-0.3.1.tar", last modified: Sat May 20 15:52:42 2023, max compression
+gzip compressed data, was "ssm-simulators-0.3.2.tar", last modified: Sat May 20 16:04:07 2023, max compression
```

## Comparing `ssm-simulators-0.3.1.tar` & `ssm-simulators-0.3.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 afengler (2138194415) 1085805755        0 2023-05-20 15:52:42.918268 ssm-simulators-0.3.1/
--rw-r--r--   0 afengler (2138194415) 1085805755     1074 2023-04-02 00:47:26.000000 ssm-simulators-0.3.1/LICENSE
--rw-r--r--   0 afengler (2138194415) 1085805755      208 2023-04-02 00:47:26.000000 ssm-simulators-0.3.1/MANIFEST.in
--rw-r--r--   0 afengler (2138194415) 1085805755      589 2023-05-20 15:52:42.917624 ssm-simulators-0.3.1/PKG-INFO
--rw-r--r--   0 afengler (2138194415) 1085805755     7076 2023-04-02 00:47:26.000000 ssm-simulators-0.3.1/README.md
-drwxr-xr-x   0 afengler (2138194415) 1085805755        0 2023-05-20 15:52:42.868865 ssm-simulators-0.3.1/notebooks/
--rw-r--r--   0 afengler (2138194415) 1085805755    63124 2023-04-16 00:15:21.000000 ssm-simulators-0.3.1/notebooks/basic_tutorial copy.ipynb
--rw-r--r--   0 afengler (2138194415) 1085805755    11456 2023-04-02 00:47:26.000000 ssm-simulators-0.3.1/notebooks/basic_tutorial.ipynb
--rw-r--r--   0 afengler (2138194415) 1085805755   197778 2023-04-02 00:47:26.000000 ssm-simulators-0.3.1/notebooks/basic_tutorial_tmp.ipynb
--rw-r--r--   0 afengler (2138194415) 1085805755       85 2023-04-02 00:47:26.000000 ssm-simulators-0.3.1/pyproject.toml
--rw-r--r--   0 afengler (2138194415) 1085805755       38 2023-05-20 15:52:42.918446 ssm-simulators-0.3.1/setup.cfg
--rw-r--r--   0 afengler (2138194415) 1085805755     1649 2023-05-20 15:28:33.000000 ssm-simulators-0.3.1/setup.py
-drwxr-xr-x   0 afengler (2138194415) 1085805755        0 2023-05-20 15:52:42.880157 ssm-simulators-0.3.1/src/
--rw-r--r--   0 afengler (2138194415) 1085805755  2466308 2023-05-20 15:52:21.000000 ssm-simulators-0.3.1/src/cssm.cpp
--rw-r--r--   0 afengler (2138194415) 1085805755   115338 2023-05-20 15:18:43.000000 ssm-simulators-0.3.1/src/cssm.pyx
-drwxr-xr-x   0 afengler (2138194415) 1085805755        0 2023-05-20 15:52:42.887757 ssm-simulators-0.3.1/ssm_simulators.egg-info/
--rw-r--r--   0 afengler (2138194415) 1085805755      589 2023-05-20 15:52:42.000000 ssm-simulators-0.3.1/ssm_simulators.egg-info/PKG-INFO
--rw-r--r--   0 afengler (2138194415) 1085805755      753 2023-05-20 15:52:42.000000 ssm-simulators-0.3.1/ssm_simulators.egg-info/SOURCES.txt
--rw-r--r--   0 afengler (2138194415) 1085805755        1 2023-05-20 15:52:42.000000 ssm-simulators-0.3.1/ssm_simulators.egg-info/dependency_links.txt
--rw-r--r--   0 afengler (2138194415) 1085805755       92 2023-05-20 15:52:42.000000 ssm-simulators-0.3.1/ssm_simulators.egg-info/requires.txt
--rw-r--r--   0 afengler (2138194415) 1085805755       10 2023-05-20 15:52:42.000000 ssm-simulators-0.3.1/ssm_simulators.egg-info/top_level.txt
-drwxr-xr-x   0 afengler (2138194415) 1085805755        0 2023-05-20 15:52:42.889580 ssm-simulators-0.3.1/ssms/
--rw-r--r--   0 afengler (2138194415) 1085805755      136 2023-04-02 00:47:26.000000 ssm-simulators-0.3.1/ssms/__init__.py
-drwxr-xr-x   0 afengler (2138194415) 1085805755        0 2023-05-20 15:52:42.900632 ssm-simulators-0.3.1/ssms/basic_simulators/
--rw-r--r--   0 afengler (2138194415) 1085805755       90 2023-04-02 00:47:26.000000 ssm-simulators-0.3.1/ssms/basic_simulators/__init__.py
--rw-r--r--   0 afengler (2138194415) 1085805755     2625 2023-04-02 00:47:26.000000 ssm-simulators-0.3.1/ssms/basic_simulators/boundary_functions.py
--rw-r--r--   0 afengler (2138194415) 1085805755     3738 2023-04-02 00:47:26.000000 ssm-simulators-0.3.1/ssms/basic_simulators/drift_functions.py
--rw-r--r--   0 afengler (2138194415) 1085805755    41275 2023-04-15 01:35:19.000000 ssm-simulators-0.3.1/ssms/basic_simulators/simulator.py
-drwxr-xr-x   0 afengler (2138194415) 1085805755        0 2023-05-20 15:52:42.904336 ssm-simulators-0.3.1/ssms/config/
--rw-r--r--   0 afengler (2138194415) 1085805755       22 2023-04-02 00:47:26.000000 ssm-simulators-0.3.1/ssms/config/__init__.py
--rw-r--r--   0 afengler (2138194415) 1085805755    29679 2023-05-11 00:51:46.000000 ssm-simulators-0.3.1/ssms/config/config.py
-drwxr-xr-x   0 afengler (2138194415) 1085805755        0 2023-05-20 15:52:42.908887 ssm-simulators-0.3.1/ssms/dataset_generators/
--rw-r--r--   0 afengler (2138194415) 1085805755       43 2023-04-02 00:47:26.000000 ssm-simulators-0.3.1/ssms/dataset_generators/__init__.py
--rw-r--r--   0 afengler (2138194415) 1085805755    26096 2023-04-16 01:44:17.000000 ssm-simulators-0.3.1/ssms/dataset_generators/lan_mlp.py
--rw-r--r--   0 afengler (2138194415) 1085805755    29000 2023-04-02 00:47:26.000000 ssm-simulators-0.3.1/ssms/dataset_generators/snpe.py
-drwxr-xr-x   0 afengler (2138194415) 1085805755        0 2023-05-20 15:52:42.915258 ssm-simulators-0.3.1/ssms/support_utils/
--rw-r--r--   0 afengler (2138194415) 1085805755       46 2023-05-20 15:30:39.000000 ssm-simulators-0.3.1/ssms/support_utils/__init__.py
--rw-r--r--   0 afengler (2138194415) 1085805755     7149 2023-04-02 00:47:26.000000 ssm-simulators-0.3.1/ssms/support_utils/kde_class.py
+drwxr-xr-x   0 afengler (2138194415) 1085805755        0 2023-05-20 16:04:07.746640 ssm-simulators-0.3.2/
+-rw-r--r--   0 afengler (2138194415) 1085805755     1074 2023-04-02 00:47:26.000000 ssm-simulators-0.3.2/LICENSE
+-rw-r--r--   0 afengler (2138194415) 1085805755      208 2023-04-02 00:47:26.000000 ssm-simulators-0.3.2/MANIFEST.in
+-rw-r--r--   0 afengler (2138194415) 1085805755      589 2023-05-20 16:04:07.746013 ssm-simulators-0.3.2/PKG-INFO
+-rw-r--r--   0 afengler (2138194415) 1085805755     7076 2023-04-02 00:47:26.000000 ssm-simulators-0.3.2/README.md
+drwxr-xr-x   0 afengler (2138194415) 1085805755        0 2023-05-20 16:04:07.715448 ssm-simulators-0.3.2/notebooks/
+-rw-r--r--   0 afengler (2138194415) 1085805755    63124 2023-04-16 00:15:21.000000 ssm-simulators-0.3.2/notebooks/basic_tutorial copy.ipynb
+-rw-r--r--   0 afengler (2138194415) 1085805755    11456 2023-04-02 00:47:26.000000 ssm-simulators-0.3.2/notebooks/basic_tutorial.ipynb
+-rw-r--r--   0 afengler (2138194415) 1085805755   197778 2023-04-02 00:47:26.000000 ssm-simulators-0.3.2/notebooks/basic_tutorial_tmp.ipynb
+-rw-r--r--   0 afengler (2138194415) 1085805755       85 2023-04-02 00:47:26.000000 ssm-simulators-0.3.2/pyproject.toml
+-rw-r--r--   0 afengler (2138194415) 1085805755       38 2023-05-20 16:04:07.746790 ssm-simulators-0.3.2/setup.cfg
+-rw-r--r--   0 afengler (2138194415) 1085805755     1649 2023-05-20 16:03:31.000000 ssm-simulators-0.3.2/setup.py
+drwxr-xr-x   0 afengler (2138194415) 1085805755        0 2023-05-20 16:04:07.727495 ssm-simulators-0.3.2/src/
+-rw-r--r--   0 afengler (2138194415) 1085805755  2469726 2023-05-20 16:03:59.000000 ssm-simulators-0.3.2/src/cssm.cpp
+-rw-r--r--   0 afengler (2138194415) 1085805755   115338 2023-05-20 15:18:43.000000 ssm-simulators-0.3.2/src/cssm.pyx
+drwxr-xr-x   0 afengler (2138194415) 1085805755        0 2023-05-20 16:04:07.732477 ssm-simulators-0.3.2/ssm_simulators.egg-info/
+-rw-r--r--   0 afengler (2138194415) 1085805755      589 2023-05-20 16:04:07.000000 ssm-simulators-0.3.2/ssm_simulators.egg-info/PKG-INFO
+-rw-r--r--   0 afengler (2138194415) 1085805755      753 2023-05-20 16:04:07.000000 ssm-simulators-0.3.2/ssm_simulators.egg-info/SOURCES.txt
+-rw-r--r--   0 afengler (2138194415) 1085805755        1 2023-05-20 16:04:07.000000 ssm-simulators-0.3.2/ssm_simulators.egg-info/dependency_links.txt
+-rw-r--r--   0 afengler (2138194415) 1085805755       92 2023-05-20 16:04:07.000000 ssm-simulators-0.3.2/ssm_simulators.egg-info/requires.txt
+-rw-r--r--   0 afengler (2138194415) 1085805755       10 2023-05-20 16:04:07.000000 ssm-simulators-0.3.2/ssm_simulators.egg-info/top_level.txt
+drwxr-xr-x   0 afengler (2138194415) 1085805755        0 2023-05-20 16:04:07.733579 ssm-simulators-0.3.2/ssms/
+-rw-r--r--   0 afengler (2138194415) 1085805755      136 2023-05-20 16:03:36.000000 ssm-simulators-0.3.2/ssms/__init__.py
+drwxr-xr-x   0 afengler (2138194415) 1085805755        0 2023-05-20 16:04:07.737411 ssm-simulators-0.3.2/ssms/basic_simulators/
+-rw-r--r--   0 afengler (2138194415) 1085805755       90 2023-04-02 00:47:26.000000 ssm-simulators-0.3.2/ssms/basic_simulators/__init__.py
+-rw-r--r--   0 afengler (2138194415) 1085805755     2625 2023-04-02 00:47:26.000000 ssm-simulators-0.3.2/ssms/basic_simulators/boundary_functions.py
+-rw-r--r--   0 afengler (2138194415) 1085805755     3738 2023-04-02 00:47:26.000000 ssm-simulators-0.3.2/ssms/basic_simulators/drift_functions.py
+-rw-r--r--   0 afengler (2138194415) 1085805755    41275 2023-04-15 01:35:19.000000 ssm-simulators-0.3.2/ssms/basic_simulators/simulator.py
+drwxr-xr-x   0 afengler (2138194415) 1085805755        0 2023-05-20 16:04:07.738783 ssm-simulators-0.3.2/ssms/config/
+-rw-r--r--   0 afengler (2138194415) 1085805755       22 2023-04-02 00:47:26.000000 ssm-simulators-0.3.2/ssms/config/__init__.py
+-rw-r--r--   0 afengler (2138194415) 1085805755    29679 2023-05-11 00:51:46.000000 ssm-simulators-0.3.2/ssms/config/config.py
+drwxr-xr-x   0 afengler (2138194415) 1085805755        0 2023-05-20 16:04:07.741140 ssm-simulators-0.3.2/ssms/dataset_generators/
+-rw-r--r--   0 afengler (2138194415) 1085805755       43 2023-04-02 00:47:26.000000 ssm-simulators-0.3.2/ssms/dataset_generators/__init__.py
+-rw-r--r--   0 afengler (2138194415) 1085805755    26096 2023-04-16 01:44:17.000000 ssm-simulators-0.3.2/ssms/dataset_generators/lan_mlp.py
+-rw-r--r--   0 afengler (2138194415) 1085805755    29000 2023-04-02 00:47:26.000000 ssm-simulators-0.3.2/ssms/dataset_generators/snpe.py
+drwxr-xr-x   0 afengler (2138194415) 1085805755        0 2023-05-20 16:04:07.745167 ssm-simulators-0.3.2/ssms/support_utils/
+-rw-r--r--   0 afengler (2138194415) 1085805755       46 2023-05-20 16:03:42.000000 ssm-simulators-0.3.2/ssms/support_utils/__init__.py
+-rw-r--r--   0 afengler (2138194415) 1085805755     7149 2023-04-02 00:47:26.000000 ssm-simulators-0.3.2/ssms/support_utils/kde_class.py
```

### Comparing `ssm-simulators-0.3.1/LICENSE` & `ssm-simulators-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ssm-simulators-0.3.1/PKG-INFO` & `ssm-simulators-0.3.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-simulators
-Version: 0.3.1
+Version: 0.3.2
 Summary: SSMS is a package collecting simulators and training data generators for a bunch of generative models of interest in the cognitive science / neuroscience and approximate bayesian computation communities
 Home-page: https://github.com/AlexanderFengler/ssms
 Author: Alexander Fenger
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ssm-simulators-0.3.1/README.md` & `ssm-simulators-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ssm-simulators-0.3.1/notebooks/basic_tutorial copy.ipynb` & `ssm-simulators-0.3.2/notebooks/basic_tutorial copy.ipynb`

 * *Files identical despite different names*

### Comparing `ssm-simulators-0.3.1/notebooks/basic_tutorial.ipynb` & `ssm-simulators-0.3.2/notebooks/basic_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ssm-simulators-0.3.1/notebooks/basic_tutorial_tmp.ipynb` & `ssm-simulators-0.3.2/notebooks/basic_tutorial_tmp.ipynb`

 * *Files identical despite different names*

### Comparing `ssm-simulators-0.3.1/setup.py` & `ssm-simulators-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
                                 compiler_directives = {"language_level": "3"})
 except ImportError:
     ext_modules = [Extension('cssm', ['src/cssm.pyx'], language = 'c++')]
 
 
 setup(  
         name = 'ssm-simulators',
-        version='0.3.1',
+        version='0.3.2',
         author = 'Alexander Fenger',
         url = 'https://github.com/AlexanderFengler/ssms',
         packages= ['ssms', 'ssms.basic_simulators', 'ssms.config', 'ssms.dataset_generators', 'ssms.support_utils'],
         description='SSMS is a package collecting simulators and training data generators for a bunch of generative models of interest in the cognitive science / neuroscience and approximate bayesian computation communities',
         install_requires= ['numpy >= 1.17.0', 'scipy >= 1.6.3', 'cython >= 0.29.23', 'pandas >= 1.0.0', 'scikit-learn >= 0.24.0', 'psutil >= 5.0.0'],
         setup_requires= ['numpy >= 1.17.0', 'scipy >= 1.6.3', 'cython >= 0.29.23', 'pandas >= 1.0.0', 'scikit-learn >= 0.24.0', 'psutil >= 5.0.0'],
         include_dirs = [numpy.get_include()] ,
```

### Comparing `ssm-simulators-0.3.1/src/cssm.cpp` & `ssm-simulators-0.3.2/src/cssm.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "language": "c++",
         "name": "cssm",
@@ -19,16 +19,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -213,15 +213,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -252,15 +252,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -1122,195 +1122,195 @@
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
 #define __Pyx_FastGilFuncInit()
 
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":689
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":696
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":703
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":713
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":717
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":721
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":724
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1341,42 +1341,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":728
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":732
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2088,20 +2088,28 @@
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -35656,15 +35664,15 @@
   __Pyx_XDECREF(__pyx_v_boundary_params_tmp);
   __Pyx_XDECREF(__pyx_9genexpr14__pyx_v_key);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":734
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -35673,29 +35681,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":734
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -35706,15 +35714,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":737
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -35723,29 +35731,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":737
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -35756,15 +35764,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":740
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -35773,29 +35781,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":740
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -35806,15 +35814,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":743
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -35823,29 +35831,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":743
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -35856,15 +35864,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":746
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -35873,29 +35881,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":746
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -35906,212 +35914,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":749
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":750
+    /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":753
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":749
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":928
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":928
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":932
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":934
+    /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":936
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":932
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":940
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -36127,15 +36135,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -36143,53 +36151,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":941
+      /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":943
+    /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":944
+      /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
@@ -36197,30 +36205,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":941
+    /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":940
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -36235,15 +36243,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":946
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -36259,15 +36267,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -36275,53 +36283,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":947
+      /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":949
+    /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":950
+      /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
@@ -36329,30 +36337,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":947
+    /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":946
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -36367,15 +36375,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":952
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -36391,15 +36399,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -36407,53 +36415,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":953
+      /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":955
+    /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":956
+      /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
@@ -36461,30 +36469,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":953
+    /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":952
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -36499,176 +36507,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":966
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":978
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":966
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":981
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":993
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":981
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":996
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":1003
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":996
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":1010
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":1006
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+/* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":1017
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":1013
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -50802,26 +50810,26 @@
   __pyx_slice_ = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice_)) __PYX_ERR(0, 220, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice_);
   __Pyx_GIVEREF(__pyx_slice_);
   __pyx_tuple__2 = PyTuple_Pack(2, __pyx_slice_, __pyx_slice_); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 220, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":944
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__19);
   __Pyx_GIVEREF(__pyx_tuple__19);
 
-  /* "../../../.local/lib/python3.10/site-packages/numpy/__init__.pxd":950
+  /* "../../../miniconda3/envs/ssms_dev/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(1, 950, __pyx_L1_error)
@@ -51437,52 +51445,67 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -54668,28 +54691,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -55343,44 +55366,62 @@
     return ret;
 }
 
 /* TypeImport */
   #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
```

### Comparing `ssm-simulators-0.3.1/src/cssm.pyx` & `ssm-simulators-0.3.2/src/cssm.pyx`

 * *Files identical despite different names*

### Comparing `ssm-simulators-0.3.1/ssm_simulators.egg-info/PKG-INFO` & `ssm-simulators-0.3.2/ssm_simulators.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssm-simulators
-Version: 0.3.1
+Version: 0.3.2
 Summary: SSMS is a package collecting simulators and training data generators for a bunch of generative models of interest in the cognitive science / neuroscience and approximate bayesian computation communities
 Home-page: https://github.com/AlexanderFengler/ssms
 Author: Alexander Fenger
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ssm-simulators-0.3.1/ssm_simulators.egg-info/SOURCES.txt` & `ssm-simulators-0.3.2/ssm_simulators.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ssm-simulators-0.3.1/ssms/basic_simulators/boundary_functions.py` & `ssm-simulators-0.3.2/ssms/basic_simulators/boundary_functions.py`

 * *Files identical despite different names*

### Comparing `ssm-simulators-0.3.1/ssms/basic_simulators/drift_functions.py` & `ssm-simulators-0.3.2/ssms/basic_simulators/drift_functions.py`

 * *Files identical despite different names*

### Comparing `ssm-simulators-0.3.1/ssms/basic_simulators/simulator.py` & `ssm-simulators-0.3.2/ssms/basic_simulators/simulator.py`

 * *Files identical despite different names*

### Comparing `ssm-simulators-0.3.1/ssms/config/config.py` & `ssm-simulators-0.3.2/ssms/config/config.py`

 * *Files identical despite different names*

### Comparing `ssm-simulators-0.3.1/ssms/dataset_generators/lan_mlp.py` & `ssm-simulators-0.3.2/ssms/dataset_generators/lan_mlp.py`

 * *Files identical despite different names*

### Comparing `ssm-simulators-0.3.1/ssms/dataset_generators/snpe.py` & `ssm-simulators-0.3.2/ssms/dataset_generators/snpe.py`

 * *Files identical despite different names*

### Comparing `ssm-simulators-0.3.1/ssms/support_utils/kde_class.py` & `ssm-simulators-0.3.2/ssms/support_utils/kde_class.py`

 * *Files identical despite different names*

