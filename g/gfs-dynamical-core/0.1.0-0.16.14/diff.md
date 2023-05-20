# Comparing `tmp/gfs_dynamical_core-0.1.0.tar.gz` & `tmp/gfs_dynamical_core-0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gfs_dynamical_core-0.1.0.tar", last modified: Sat May 20 06:53:20 2023, max compression
+gzip compressed data, was "gfs_dynamical_core-0.16.14.tar", last modified: Wed Sep 21 13:32:22 2022, max compression
```

## Comparing `gfs_dynamical_core-0.1.0.tar` & `gfs_dynamical_core-0.16.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 requiem   (1000) requiem   (1000)        0 2023-05-20 06:53:20.252424 gfs_dynamical_core-0.1.0/
--rw-rw-r--   0 requiem   (1000) requiem   (1000)       11 2023-05-20 06:48:08.000000 gfs_dynamical_core-0.1.0/LICENSE
--rw-rw-r--   0 requiem   (1000) requiem   (1000)      122 2023-05-20 06:48:08.000000 gfs_dynamical_core-0.1.0/MANIFEST.in
--rw-rw-r--   0 requiem   (1000) requiem   (1000)      798 2023-05-20 06:53:20.252424 gfs_dynamical_core-0.1.0/PKG-INFO
--rw-rw-r--   0 requiem   (1000) requiem   (1000)       19 2023-05-20 06:48:08.000000 gfs_dynamical_core-0.1.0/README.rst
-drwxrwxr-x   0 requiem   (1000) requiem   (1000)        0 2023-05-20 06:53:20.248424 gfs_dynamical_core-0.1.0/gfs_dynamical_core/
--rw-rw-r--   0 requiem   (1000) requiem   (1000)      194 2023-05-20 06:48:08.000000 gfs_dynamical_core-0.1.0/gfs_dynamical_core/__init__.py
-drwxrwxr-x   0 requiem   (1000) requiem   (1000)        0 2023-05-20 06:53:20.248424 gfs_dynamical_core-0.1.0/gfs_dynamical_core/_components/
-drwxrwxr-x   0 requiem   (1000) requiem   (1000)        0 2023-05-20 06:53:20.252424 gfs_dynamical_core-0.1.0/gfs_dynamical_core/_components/gfs/
--rw-rw-r--   0 requiem   (1000) requiem   (1000)    18117 2023-05-20 06:48:08.000000 gfs_dynamical_core-0.1.0/gfs_dynamical_core/_components/gfs/_gfs_dynamics.pyx
-drwxrwxr-x   0 requiem   (1000) requiem   (1000)        0 2023-05-20 06:53:20.252424 gfs_dynamical_core-0.1.0/gfs_dynamical_core.egg-info/
--rw-rw-r--   0 requiem   (1000) requiem   (1000)      798 2023-05-20 06:53:20.000000 gfs_dynamical_core-0.1.0/gfs_dynamical_core.egg-info/PKG-INFO
--rw-rw-r--   0 requiem   (1000) requiem   (1000)      383 2023-05-20 06:53:20.000000 gfs_dynamical_core-0.1.0/gfs_dynamical_core.egg-info/SOURCES.txt
--rw-rw-r--   0 requiem   (1000) requiem   (1000)        1 2023-05-20 06:53:20.000000 gfs_dynamical_core-0.1.0/gfs_dynamical_core.egg-info/dependency_links.txt
--rw-rw-r--   0 requiem   (1000) requiem   (1000)        1 2023-05-20 06:53:20.000000 gfs_dynamical_core-0.1.0/gfs_dynamical_core.egg-info/not-zip-safe
--rw-rw-r--   0 requiem   (1000) requiem   (1000)       95 2023-05-20 06:53:20.000000 gfs_dynamical_core-0.1.0/gfs_dynamical_core.egg-info/requires.txt
--rw-rw-r--   0 requiem   (1000) requiem   (1000)       19 2023-05-20 06:53:20.000000 gfs_dynamical_core-0.1.0/gfs_dynamical_core.egg-info/top_level.txt
--rw-rw-r--   0 requiem   (1000) requiem   (1000)      392 2023-05-20 06:53:20.252424 gfs_dynamical_core-0.1.0/setup.cfg
--rw-rw-r--   0 requiem   (1000) requiem   (1000)     6967 2023-05-20 06:48:08.000000 gfs_dynamical_core-0.1.0/setup.py
+drwxrwxr-x   0 abel      (1000) abel      (1000)        0 2022-09-21 13:32:22.207383 gfs_dynamical_core-0.16.14/
+-rw-rw-r--   0 abel      (1000) abel      (1000)       11 2022-09-21 13:11:52.000000 gfs_dynamical_core-0.16.14/LICENSE
+-rw-rw-r--   0 abel      (1000) abel      (1000)      122 2022-09-21 13:11:52.000000 gfs_dynamical_core-0.16.14/MANIFEST.in
+-rw-rw-r--   0 abel      (1000) abel      (1000)      853 2022-09-21 13:32:22.207383 gfs_dynamical_core-0.16.14/PKG-INFO
+-rw-rw-r--   0 abel      (1000) abel      (1000)       19 2022-09-21 13:31:52.000000 gfs_dynamical_core-0.16.14/README.rst
+drwxrwxr-x   0 abel      (1000) abel      (1000)        0 2022-09-21 13:32:22.199383 gfs_dynamical_core-0.16.14/gfs_dynamical_core/
+-rw-rw-r--   0 abel      (1000) abel      (1000)      642 2022-09-21 13:11:52.000000 gfs_dynamical_core-0.16.14/gfs_dynamical_core/__init__.py
+drwxrwxr-x   0 abel      (1000) abel      (1000)        0 2022-09-21 13:32:22.199383 gfs_dynamical_core-0.16.14/gfs_dynamical_core/_components/
+drwxrwxr-x   0 abel      (1000) abel      (1000)        0 2022-09-21 13:32:22.207383 gfs_dynamical_core-0.16.14/gfs_dynamical_core/_components/gfs/
+-rw-rw-r--   0 abel      (1000) abel      (1000)    18113 2022-09-21 13:25:01.000000 gfs_dynamical_core-0.16.14/gfs_dynamical_core/_components/gfs/_gfs_dynamics.pyx
+drwxrwxr-x   0 abel      (1000) abel      (1000)        0 2022-09-21 13:32:22.207383 gfs_dynamical_core-0.16.14/gfs_dynamical_core.egg-info/
+-rw-rw-r--   0 abel      (1000) abel      (1000)      853 2022-09-21 13:32:20.000000 gfs_dynamical_core-0.16.14/gfs_dynamical_core.egg-info/PKG-INFO
+-rw-rw-r--   0 abel      (1000) abel      (1000)      383 2022-09-21 13:32:22.000000 gfs_dynamical_core-0.16.14/gfs_dynamical_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 abel      (1000) abel      (1000)        1 2022-09-21 13:32:20.000000 gfs_dynamical_core-0.16.14/gfs_dynamical_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 abel      (1000) abel      (1000)        1 2022-09-21 13:13:13.000000 gfs_dynamical_core-0.16.14/gfs_dynamical_core.egg-info/not-zip-safe
+-rw-rw-r--   0 abel      (1000) abel      (1000)       80 2022-09-21 13:32:21.000000 gfs_dynamical_core-0.16.14/gfs_dynamical_core.egg-info/requires.txt
+-rw-rw-r--   0 abel      (1000) abel      (1000)       19 2022-09-21 13:32:21.000000 gfs_dynamical_core-0.16.14/gfs_dynamical_core.egg-info/top_level.txt
+-rw-rw-r--   0 abel      (1000) abel      (1000)      368 2022-09-21 13:32:22.207383 gfs_dynamical_core-0.16.14/setup.cfg
+-rw-rw-r--   0 abel      (1000) abel      (1000)     6947 2022-09-21 13:31:40.000000 gfs_dynamical_core-0.16.14/setup.py
```

### Comparing `gfs_dynamical_core-0.1.0/PKG-INFO` & `gfs_dynamical_core-0.16.14/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 Metadata-Version: 2.1
 Name: gfs_dynamical_core
-Version: 0.1.0
+Version: 0.16.14
 Summary: Only the dynamical core of the climt repository
 Home-page: https://github.com/Ai33L/gfs_dynamical_core.git
 Author: Rodrigo Caballero
 Author-email: rodrigo.caballero@misu.su.se
 License: BSD license
 Keywords: gfs_dynamical_core
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE
+
+GFS dynamical core
+
+
+To be added
+
```

### Comparing `gfs_dynamical_core-0.1.0/gfs_dynamical_core/_components/gfs/_gfs_dynamics.pyx` & `gfs_dynamical_core-0.16.14/gfs_dynamical_core/_components/gfs/_gfs_dynamics.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -291,16 +291,16 @@
 
     nlm = int((ntrunc+1)*(ntrunc+2)/2)
 
     pyLap = np.zeros(nlm, dtype=np.double)
     pyInvLap = np.zeros(nlm, dtype=np.double)
     pyGaussWeights = np.zeros(nlats, dtype=np.double)
 
-    pyDegree = np.zeros(nlm, dtype=np.int64)
-    pyOrder = np.zeros(nlm, dtype=np.int64)
+    pyDegree = np.zeros(nlm, dtype=np.int)
+    pyOrder = np.zeros(nlm, dtype=np.int)
 
     pyLats = np.zeros((nlats, nlons), dtype=np.double)
     pyLons = np.zeros((nlats, nlons), dtype=np.double)
     pyAreaWeights = np.zeros((nlats, nlons), dtype=np.double)
 
     pyDmhyb = np.zeros((3, ntrunc+1, nlevs, nlevs),
                        dtype=np.double)
```

### Comparing `gfs_dynamical_core-0.1.0/gfs_dynamical_core.egg-info/PKG-INFO` & `gfs_dynamical_core-0.16.14/gfs_dynamical_core.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 Metadata-Version: 2.1
 Name: gfs-dynamical-core
-Version: 0.1.0
+Version: 0.16.14
 Summary: Only the dynamical core of the climt repository
 Home-page: https://github.com/Ai33L/gfs_dynamical_core.git
 Author: Rodrigo Caballero
 Author-email: rodrigo.caballero@misu.su.se
 License: BSD license
 Keywords: gfs_dynamical_core
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE
+
+GFS dynamical core
+
+
+To be added
+
```

### Comparing `gfs_dynamical_core-0.1.0/setup.py` & `gfs_dynamical_core-0.16.14/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,28 +26,27 @@
     print('Suitable numpy unavailable, installing...')
     pip_main(['install', 'numpy'])
     import numpy as np
 
 
 include_dirs = [np.get_include()]
 
-# with open('README.rst') as readme_file:
-#     readme = readme_file.read()
+with open('README.rst') as readme_file:
+    readme = readme_file.read()
 
-# with open('HISTORY.rst') as history_file:
-#     history = history_file.read()
+with open('HISTORY.rst') as history_file:
+    history = history_file.read()
 
 requirements = [
     'numpy>=1.16.0',
     'pint>=0.7.0',
     'xarray>=0.8.0',
-    'sympl==0.4.1',
+    'sympl==0.4.0',
     'cython>=0.25',
     'scipy>=0.18.1',
-    'climt>=0.16.25',
 ]
 
 test_requirements = [
     'pytest>=2.9.2',
     'mock>=2.0.0',
 ]
 
@@ -99,24 +98,24 @@
 
 
 # Compile libraries
 
 if 'FC' not in os.environ:
     if operating_system == 'Darwin':
         # guess_compiler_name('FC')
-        os.environ['FC'] = 'gfortran-10'
-        os.environ['F77'] = 'gfortran-10'
+        os.environ['FC'] = 'gfortran-6'
+        os.environ['F77'] = 'gfortran-6'
     else:
         os.environ['FC'] = 'gfortran'
         os.environ['F77'] = 'gfortran'
 
 if 'CC' not in os.environ:
     if operating_system == 'Darwin':
         # guess_compiler_name('CC')
-        os.environ['CC'] = 'gcc-10'
+        os.environ['CC'] = 'gcc-6'
     else:
         os.environ['CC'] = 'gcc'
 
 if 'GFS_OPT_FLAGS' not in os.environ:
     os.environ['GFS_OPT_FLAGS'] = '-O3'
 
 if operating_system == 'Windows' :
@@ -128,20 +127,20 @@
     default_link_args = ['-l:libgfortran.a', '-l:libquadmath.a', '-l:libm.a']
     default_compile_args = ['-DMS_WIN64']
 
 os.environ['FFLAGS'] = '-fPIC -fno-range-check ' + os.environ['GFS_OPT_FLAGS']
 os.environ['CFLAGS'] = '-fPIC ' + os.environ['GFS_OPT_FLAGS']
 
 if operating_system == 'Darwin':
-#     gcc_dir = find_homebrew_gcc()
-#     for root, dirs, files in os.walk(gcc_dir):
-#         for line in files:
-#             if re.match('libgfortran.a', line):
-#                 if not ('i386' in root):
-#                     lib_path_list.append(root)
+    gcc_dir = find_homebrew_gcc()
+    for root, dirs, files in os.walk(gcc_dir):
+        for line in files:
+            if re.match('libgfortran.a', line):
+                if not ('i386' in root):
+                    lib_path_list.append(root)
 
     os.environ['FFLAGS'] += ' -mmacosx-version-min=10.7'
     os.environ['CFLAGS'] += ' -mmacosx-version-min=10.7'
     default_link_args = []
     os.environ['LDSHARED'] = os.environ['CC']+' -bundle -undefined dynamic_lookup -arch x86_64'
 
 print('Compilers: ', os.environ['CC'], os.environ['FC'])
@@ -197,17 +196,17 @@
 
         # lib_path+'/libshtns_omp.a', openblas_path, os.environ['COMPILER_PATH']+'../lib/libfftw3.a'] + default_link_args),
 
     ]
 
 setup(
     name='gfs_dynamical_core',
-    version='0.1.0',
+    version='0.16.14',
     description='Only the dynamical core of the climt repository',
-    long_description='',
+    long_description=readme + '\n\n' + history,
     author="Rodrigo Caballero",
     author_email='rodrigo.caballero@misu.su.se',
     url='https://github.com/Ai33L/gfs_dynamical_core.git',
     packages=[
         'gfs_dynamical_core',
     ],
     package_dir={'gfs_dynamical_core':
```

