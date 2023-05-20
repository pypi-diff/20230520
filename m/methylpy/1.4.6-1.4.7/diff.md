# Comparing `tmp/methylpy-1.4.6.tar.gz` & `tmp/methylpy-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/methylpy-1.4.6.tar", last modified: Sat Sep 26 17:21:44 2020, max compression
+gzip compressed data, was "dist/methylpy-1.4.7.tar", last modified: Sat May 20 00:52:35 2023, max compression
```

## Comparing `methylpy-1.4.6.tar` & `methylpy-1.4.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 yupeng    (9301) yupeng    (9302)        0 2020-09-26 17:21:44.000000 methylpy-1.4.6/
-drwxrwxr-x   0 yupeng    (9301) yupeng    (9302)        0 2020-09-26 17:21:43.000000 methylpy-1.4.6/bin/
--rwxrwxr-x   0 yupeng    (9301) yupeng    (9302)      106 2017-10-09 18:38:36.000000 methylpy-1.4.6/bin/methylpy
-drwxrwxr-x   0 yupeng    (9301) yupeng    (9302)        0 2020-09-26 17:21:43.000000 methylpy-1.4.6/docs/
--rw-rw-r--   0 yupeng    (9301) yupeng    (9302)    19646 2020-09-26 17:21:42.000000 methylpy-1.4.6/docs/README.rst
-drwxrwxr-x   0 yupeng    (9301) yupeng    (9302)        0 2020-09-26 17:21:43.000000 methylpy-1.4.6/methylpy/
--rw-rw-r--   0 yupeng    (9301) yupeng    (9302)    59331 2020-07-30 05:25:22.000000 methylpy-1.4.6/methylpy/DMRfind.py
--rwxrwxr-x   0 yupeng    (9301) yupeng    (9302)       22 2020-09-26 17:21:28.000000 methylpy-1.4.6/methylpy/__init__.py
--rw-rw-r--   0 yupeng    (9301) yupeng    (9302)    64757 2019-09-06 03:48:05.000000 methylpy-1.4.6/methylpy/call_mc_pe.py
--rw-rw-r--   0 yupeng    (9301) yupeng    (9302)   105768 2020-09-26 17:20:06.000000 methylpy-1.4.6/methylpy/call_mc_se.py
--rw-rw-r--   0 yupeng    (9301) yupeng    (9302)    97419 2020-01-16 03:42:07.000000 methylpy-1.4.6/methylpy/parser.py
--rw-rw-r--   0 yupeng    (9301) yupeng    (9302)    12795 2017-10-23 17:41:43.000000 methylpy-1.4.6/methylpy/rms.cpp
--rwxrwxr-x   0 yupeng    (9301) yupeng    (9302)    53352 2017-10-23 17:41:43.000000 methylpy-1.4.6/methylpy/run_rms_tests.out
--rw-rw-r--   0 yupeng    (9301) yupeng    (9302)    45523 2019-04-02 00:59:49.000000 methylpy-1.4.6/methylpy/utilities.py
-drwxrwxr-x   0 yupeng    (9301) yupeng    (9302)        0 2020-09-26 17:21:44.000000 methylpy-1.4.6/methylpy.egg-info/
--rw-rw-r--   0 yupeng    (9301) yupeng    (9302)    24452 2020-09-26 17:21:43.000000 methylpy-1.4.6/methylpy.egg-info/PKG-INFO
--rw-rw-r--   0 yupeng    (9301) yupeng    (9302)      425 2020-09-26 17:21:43.000000 methylpy-1.4.6/methylpy.egg-info/SOURCES.txt
--rw-rw-r--   0 yupeng    (9301) yupeng    (9302)        1 2020-09-26 17:21:43.000000 methylpy-1.4.6/methylpy.egg-info/dependency_links.txt
--rw-rw-r--   0 yupeng    (9301) yupeng    (9302)       40 2020-09-26 17:21:43.000000 methylpy-1.4.6/methylpy.egg-info/requires.txt
--rw-rw-r--   0 yupeng    (9301) yupeng    (9302)        9 2020-09-26 17:21:43.000000 methylpy-1.4.6/methylpy.egg-info/top_level.txt
-drwxrwxr-x   0 yupeng    (9301) yupeng    (9302)        0 2020-09-26 17:21:44.000000 methylpy-1.4.6/test/
--rw-rw-r--   0 yupeng    (9301) yupeng    (9302)     2124 2017-11-09 21:57:48.000000 methylpy-1.4.6/test/test.py
--rw-rw-r--   0 yupeng    (9301) yupeng    (9302)    11366 2017-11-01 18:18:45.000000 methylpy-1.4.6/LICENSE.txt
--rw-rw-r--   0 yupeng    (9301) yupeng    (9302)       50 2017-11-16 07:17:39.000000 methylpy-1.4.6/MANIFEST.in
--rw-rw-r--   0 yupeng    (9301) yupeng    (9302)    15875 2020-01-16 03:42:07.000000 methylpy-1.4.6/README.md
--rw-rw-r--   0 yupeng    (9301) yupeng    (9302)       79 2020-09-26 17:21:44.000000 methylpy-1.4.6/setup.cfg
--rw-rw-r--   0 yupeng    (9301) yupeng    (9302)     1078 2020-09-26 17:21:36.000000 methylpy-1.4.6/setup.py
--rw-rw-r--   0 yupeng    (9301) yupeng    (9302)    24452 2020-09-26 17:21:44.000000 methylpy-1.4.6/PKG-INFO
+drwxrwxr-x   0 yupeng    (9301) yupeng    (9302)        0 2023-05-20 00:52:35.000000 methylpy-1.4.7/
+drwxrwxr-x   0 yupeng    (9301) yupeng    (9302)        0 2023-05-20 00:52:34.000000 methylpy-1.4.7/bin/
+-rwxrwxr-x   0 yupeng    (9301) yupeng    (9302)      106 2017-10-09 18:38:36.000000 methylpy-1.4.7/bin/methylpy
+drwxrwxr-x   0 yupeng    (9301) yupeng    (9302)        0 2023-05-20 00:52:34.000000 methylpy-1.4.7/docs/
+-rw-rw-r--   0 yupeng    (9301) yupeng    (9302)    19950 2023-05-20 00:52:22.000000 methylpy-1.4.7/docs/README.rst
+drwxrwxr-x   0 yupeng    (9301) yupeng    (9302)        0 2023-05-20 00:52:35.000000 methylpy-1.4.7/methylpy/
+-rw-rw-r--   0 yupeng    (9301) yupeng    (9302)    59331 2023-05-20 00:49:58.000000 methylpy-1.4.7/methylpy/DMRfind.py
+-rwxrwxr-x   0 yupeng    (9301) yupeng    (9302)       22 2023-05-20 00:51:32.000000 methylpy-1.4.7/methylpy/__init__.py
+-rw-rw-r--   0 yupeng    (9301) yupeng    (9302)    64757 2019-09-06 03:48:05.000000 methylpy-1.4.7/methylpy/call_mc_pe.py
+-rw-rw-r--   0 yupeng    (9301) yupeng    (9302)   105768 2020-09-26 17:20:06.000000 methylpy-1.4.7/methylpy/call_mc_se.py
+-rw-rw-r--   0 yupeng    (9301) yupeng    (9302)    97423 2023-05-20 00:51:22.000000 methylpy-1.4.7/methylpy/parser.py
+-rw-rw-r--   0 yupeng    (9301) yupeng    (9302)    12795 2017-10-23 17:41:43.000000 methylpy-1.4.7/methylpy/rms.cpp
+-rwxrwxr-x   0 yupeng    (9301) yupeng    (9302)    53352 2017-10-23 17:41:43.000000 methylpy-1.4.7/methylpy/run_rms_tests.out
+-rw-rw-r--   0 yupeng    (9301) yupeng    (9302)    45523 2019-04-02 00:59:49.000000 methylpy-1.4.7/methylpy/utilities.py
+drwxrwxr-x   0 yupeng    (9301) yupeng    (9302)        0 2023-05-20 00:52:35.000000 methylpy-1.4.7/methylpy.egg-info/
+-rw-rw-r--   0 yupeng    (9301) yupeng    (9302)    24844 2023-05-20 00:52:33.000000 methylpy-1.4.7/methylpy.egg-info/PKG-INFO
+-rw-rw-r--   0 yupeng    (9301) yupeng    (9302)      425 2023-05-20 00:52:33.000000 methylpy-1.4.7/methylpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 yupeng    (9301) yupeng    (9302)        1 2023-05-20 00:52:33.000000 methylpy-1.4.7/methylpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 yupeng    (9301) yupeng    (9302)       40 2023-05-20 00:52:33.000000 methylpy-1.4.7/methylpy.egg-info/requires.txt
+-rw-rw-r--   0 yupeng    (9301) yupeng    (9302)        9 2023-05-20 00:52:33.000000 methylpy-1.4.7/methylpy.egg-info/top_level.txt
+drwxrwxr-x   0 yupeng    (9301) yupeng    (9302)        0 2023-05-20 00:52:35.000000 methylpy-1.4.7/test/
+-rw-rw-r--   0 yupeng    (9301) yupeng    (9302)     2124 2017-11-09 21:57:48.000000 methylpy-1.4.7/test/test.py
+-rw-rw-r--   0 yupeng    (9301) yupeng    (9302)    11366 2017-11-01 18:18:45.000000 methylpy-1.4.7/LICENSE.txt
+-rw-rw-r--   0 yupeng    (9301) yupeng    (9302)       50 2017-11-16 07:17:39.000000 methylpy-1.4.7/MANIFEST.in
+-rw-rw-r--   0 yupeng    (9301) yupeng    (9302)    16169 2023-05-20 00:48:27.000000 methylpy-1.4.7/README.md
+-rw-rw-r--   0 yupeng    (9301) yupeng    (9302)       79 2023-05-20 00:52:35.000000 methylpy-1.4.7/setup.cfg
+-rw-rw-r--   0 yupeng    (9301) yupeng    (9302)     1078 2023-05-20 00:51:43.000000 methylpy-1.4.7/setup.py
+-rw-rw-r--   0 yupeng    (9301) yupeng    (9302)    24844 2023-05-20 00:52:35.000000 methylpy-1.4.7/PKG-INFO
```

### Comparing `methylpy-1.4.6/docs/README.rst` & `methylpy-1.4.7/docs/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -101,17 +101,28 @@
 ================
 
 Step 1 - Download methylpy
 ^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 The easiest way of installing methylpy will be through PyPI by running
 ``pip install methylpy``. The command ``pip install --upgrade methylpy``
-updates methylpy to latest version. Alternatively, methylpy can be
-installed through github: enter the directory where you would like to
-install methylpy and run
+updates methylpy to latest version.
+
+Methylpy can also be installed through
+`anaconda <https://www.anaconda.com/download/>`__ or [miniconda]
+(https://docs.conda.io/en/latest/miniconda.html).
+
+::
+
+    conda env create --name methylpy_env
+    conda activate methylpy_env
+    conda install -y -c bioconda -c conda-forge methylpy              
+
+Alternatively, methylpy can be installed through github: enter the
+directory where you would like to install methylpy and run
 
 ::
 
     git clone https://github.com/yupenghe/methylpy.git
     cd methylpy/
     python setup.py install
 
@@ -178,15 +189,15 @@
     g++ -O3 -l gsl -l gslcblas -o run_rms_tests.out rms.cpp
 
 In Ubuntu (>=16.04), please try the below commands first.
 
 ::
 
     cd methylpy/methylpy/
-    g++ -o run_rms_tests.out rms.cpp `gsl-config --cflags —libs`
+    g++ -o run_rms_tests.out rms.cpp `gsl-config --cflags --libs`
 
 Lastly, the compiled file ``run_rms_tests.out`` needs to be copied to
 the directory where methylpy is installed. You can get the directory by
 running the blow commands in python console (``python`` to open a python
 console):
 
 ::
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `methylpy-1.4.6/methylpy/DMRfind.py` & `methylpy-1.4.7/methylpy/DMRfind.py`

 * *Files identical despite different names*

### Comparing `methylpy-1.4.6/methylpy/call_mc_pe.py` & `methylpy-1.4.7/methylpy/call_mc_pe.py`

 * *Files identical despite different names*

### Comparing `methylpy-1.4.6/methylpy/call_mc_se.py` & `methylpy-1.4.7/methylpy/call_mc_se.py`

 * *Files identical despite different names*

### Comparing `methylpy-1.4.6/methylpy/parser.py` & `methylpy-1.4.7/methylpy/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -430,15 +430,15 @@
                                      help="Integer indicating the maximum distance two sites can be "
                                      + "from one another for their methylation counts to be combined. "
                                      + "This option helps with low coverage experiments where you may "
                                      + "want to leverage the correlation of methylation between sites "
                                      + "to get more statistical power.")
      
      parser_dmrfind_opt.add_argument("--resid-cutoff",
-                                     type=int,
+                                     type=float,
                                      default=0.01,
                                      help="Results will have to show deviations in the contingency "
                                      + "table in the same direction as the rest of the window")
      
      parser_dmrfind_opt.add_argument("--keep-temp-files",
                                      type=str2bool,
                                      default=False,
@@ -518,15 +518,15 @@
                                       type=int,
                                       default=0,
                                       help="The minimum number of differentially methylated sites "
                                       + "that a differentially methylated region needs to contain to be "
                                       + "reported")
 
      parser_mergedms_opt.add_argument("--resid-cutoff",
-                                      type=int,
+                                      type=float,
                                       default=0.01,
                                       help="Results will have to show deviations in the contingency "
                                       + "table in the same direction as the rest of the window")
 
      parser_mergedms_opt.add_argument("--num-sims",
                                       type=int,
                                       default=3000,
```

### Comparing `methylpy-1.4.6/methylpy/rms.cpp` & `methylpy-1.4.7/methylpy/rms.cpp`

 * *Files identical despite different names*

### Comparing `methylpy-1.4.6/methylpy/run_rms_tests.out` & `methylpy-1.4.7/methylpy/run_rms_tests.out`

 * *Files identical despite different names*

### Comparing `methylpy-1.4.6/methylpy/utilities.py` & `methylpy-1.4.7/methylpy/utilities.py`

 * *Files identical despite different names*

### Comparing `methylpy-1.4.6/methylpy.egg-info/PKG-INFO` & `methylpy-1.4.7/methylpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: methylpy
-Version: 1.4.6
+Version: 1.4.7
 Summary: Bisulfite sequencing data processing and differential methylation analysis
 Home-page: UNKNOWN
 Author: Yupeng He
 Author-email: yupeng.he.bioinfo@gmail.com
 License: LICENSE.txt
 Description-Content-Type: UNKNOWN
 Description: methylpy
@@ -110,17 +110,28 @@
         ================
         
         Step 1 - Download methylpy
         ^^^^^^^^^^^^^^^^^^^^^^^^^^
         
         The easiest way of installing methylpy will be through PyPI by running
         ``pip install methylpy``. The command ``pip install --upgrade methylpy``
-        updates methylpy to latest version. Alternatively, methylpy can be
-        installed through github: enter the directory where you would like to
-        install methylpy and run
+        updates methylpy to latest version.
+        
+        Methylpy can also be installed through
+        `anaconda <https://www.anaconda.com/download/>`__ or [miniconda]
+        (https://docs.conda.io/en/latest/miniconda.html).
+        
+        ::
+        
+            conda env create --name methylpy_env
+            conda activate methylpy_env
+            conda install -y -c bioconda -c conda-forge methylpy              
+        
+        Alternatively, methylpy can be installed through github: enter the
+        directory where you would like to install methylpy and run
         
         ::
         
             git clone https://github.com/yupenghe/methylpy.git
             cd methylpy/
             python setup.py install
         
@@ -187,15 +198,15 @@
             g++ -O3 -l gsl -l gslcblas -o run_rms_tests.out rms.cpp
         
         In Ubuntu (>=16.04), please try the below commands first.
         
         ::
         
             cd methylpy/methylpy/
-            g++ -o run_rms_tests.out rms.cpp `gsl-config --cflags —libs`
+            g++ -o run_rms_tests.out rms.cpp `gsl-config --cflags --libs`
         
         Lastly, the compiled file ``run_rms_tests.out`` needs to be copied to
         the directory where methylpy is installed. You can get the directory by
         running the blow commands in python console (``python`` to open a python
         console):
         
         ::
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `methylpy-1.4.6/test/test.py` & `methylpy-1.4.7/test/test.py`

 * *Files identical despite different names*

### Comparing `methylpy-1.4.6/LICENSE.txt` & `methylpy-1.4.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `methylpy-1.4.6/README.md` & `methylpy-1.4.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,23 @@
 See [here](https://docs.docker.com/storage/volumes/) for details.
 
 
 # Install methylpy
 #### Step 1 - Download methylpy
 The easiest way of installing methylpy will be through PyPI by running `pip install methylpy`. The
 command `pip install --upgrade methylpy` updates methylpy to latest version.
+
+Methylpy can also be installed through [anaconda](https://www.anaconda.com/download/) or 
+[miniconda] (https://docs.conda.io/en/latest/miniconda.html). 
+```
+conda env create --name methylpy_env
+conda activate methylpy_env
+conda install -y -c bioconda -c conda-forge methylpy              
+```
+
 Alternatively, methylpy can be installed through github: enter the directory where you would
 like to install methylpy and run
 ```
 git clone https://github.com/yupenghe/methylpy.git
 cd methylpy/
 python setup.py install
 ```
@@ -114,15 +123,15 @@
 ```
 cd methylpy/methylpy/
 g++ -O3 -l gsl -l gslcblas -o run_rms_tests.out rms.cpp
 ```
 In Ubuntu (>=16.04), please try the below commands first.
 ```
 cd methylpy/methylpy/
-g++ -o run_rms_tests.out rms.cpp `gsl-config --cflags —libs`
+g++ -o run_rms_tests.out rms.cpp `gsl-config --cflags --libs`
 ```
 
 Lastly, the compiled file `run_rms_tests.out` needs to be copied to the
 directory where methylpy is installed. You can get the directory by running
 the blow commands in python console (`python` to open a python console):
 ```
 import methylpy
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `methylpy-1.4.6/setup.py` & `methylpy-1.4.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-methylpy_version = '1.4.6'
+methylpy_version = '1.4.7'
 
 setup(
     name='methylpy',
     version=methylpy_version,
     author='Yupeng He',
     author_email='yupeng.he.bioinfo@gmail.com',
     packages=['methylpy'],
```

### Comparing `methylpy-1.4.6/PKG-INFO` & `methylpy-1.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: methylpy
-Version: 1.4.6
+Version: 1.4.7
 Summary: Bisulfite sequencing data processing and differential methylation analysis
 Home-page: UNKNOWN
 Author: Yupeng He
 Author-email: yupeng.he.bioinfo@gmail.com
 License: LICENSE.txt
 Description-Content-Type: UNKNOWN
 Description: methylpy
@@ -110,17 +110,28 @@
         ================
         
         Step 1 - Download methylpy
         ^^^^^^^^^^^^^^^^^^^^^^^^^^
         
         The easiest way of installing methylpy will be through PyPI by running
         ``pip install methylpy``. The command ``pip install --upgrade methylpy``
-        updates methylpy to latest version. Alternatively, methylpy can be
-        installed through github: enter the directory where you would like to
-        install methylpy and run
+        updates methylpy to latest version.
+        
+        Methylpy can also be installed through
+        `anaconda <https://www.anaconda.com/download/>`__ or [miniconda]
+        (https://docs.conda.io/en/latest/miniconda.html).
+        
+        ::
+        
+            conda env create --name methylpy_env
+            conda activate methylpy_env
+            conda install -y -c bioconda -c conda-forge methylpy              
+        
+        Alternatively, methylpy can be installed through github: enter the
+        directory where you would like to install methylpy and run
         
         ::
         
             git clone https://github.com/yupenghe/methylpy.git
             cd methylpy/
             python setup.py install
         
@@ -187,15 +198,15 @@
             g++ -O3 -l gsl -l gslcblas -o run_rms_tests.out rms.cpp
         
         In Ubuntu (>=16.04), please try the below commands first.
         
         ::
         
             cd methylpy/methylpy/
-            g++ -o run_rms_tests.out rms.cpp `gsl-config --cflags —libs`
+            g++ -o run_rms_tests.out rms.cpp `gsl-config --cflags --libs`
         
         Lastly, the compiled file ``run_rms_tests.out`` needs to be copied to
         the directory where methylpy is installed. You can get the directory by
         running the blow commands in python console (``python`` to open a python
         console):
         
         ::
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

