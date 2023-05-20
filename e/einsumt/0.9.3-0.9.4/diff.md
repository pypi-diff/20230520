# Comparing `tmp/einsumt-0.9.3.tar.gz` & `tmp/einsumt-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "einsumt-0.9.3.tar", last modified: Tue Nov 15 22:49:25 2022, max compression
+gzip compressed data, was "einsumt-0.9.4.tar", last modified: Sat May 20 12:29:08 2023, max compression
```

## Comparing `einsumt-0.9.3.tar` & `einsumt-0.9.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-11-15 22:49:25.956009 einsumt-0.9.3/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1076 2022-11-15 22:49:05.000000 einsumt-0.9.3/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     2710 2022-11-15 22:49:25.956009 einsumt-0.9.3/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2179 2022-11-15 22:49:05.000000 einsumt-0.9.3/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-11-15 22:49:25.956009 einsumt-0.9.3/einsumt.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2710 2022-11-15 22:49:25.000000 einsumt-0.9.3/einsumt.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      161 2022-11-15 22:49:25.000000 einsumt-0.9.3/einsumt.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-11-15 22:49:25.000000 einsumt-0.9.3/einsumt.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2022-11-15 22:49:25.000000 einsumt-0.9.3/einsumt.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     8858 2022-11-15 22:49:05.000000 einsumt-0.9.3/einsumt.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2022-11-15 22:49:25.956009 einsumt-0.9.3/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      793 2022-11-15 22:49:05.000000 einsumt-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:29:08.602362 einsumt-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-20 12:29:01.000000 einsumt-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-20 12:29:08.602362 einsumt-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-20 12:29:01.000000 einsumt-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:29:08.602362 einsumt-0.9.4/einsumt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-20 12:29:08.000000 einsumt-0.9.4/einsumt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-20 12:29:08.000000 einsumt-0.9.4/einsumt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 12:29:08.000000 einsumt-0.9.4/einsumt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-20 12:29:08.000000 einsumt-0.9.4/einsumt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-05-20 12:29:01.000000 einsumt-0.9.4/einsumt.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 12:29:08.602362 einsumt-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-20 12:29:01.000000 einsumt-0.9.4/setup.py
```

### Comparing `einsumt-0.9.3/LICENSE` & `einsumt-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `einsumt-0.9.3/PKG-INFO` & `einsumt-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: einsumt
-Version: 0.9.3
+Version: 0.9.4
 Summary: Multithreaded version of numpy.einsum function
 Home-page: https://github.com/mrkwjc/einsumt
 Author: Marek Wojciechowski
 Author-email: mrkwjc@gmail.com
 License: MIT
 Keywords: numpy,einsum,hpc
 Classifier: Programming Language :: Python :: 2
```

### Comparing `einsumt-0.9.3/README.md` & `einsumt-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `einsumt-0.9.3/einsumt.egg-info/PKG-INFO` & `einsumt-0.9.4/einsumt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: einsumt
-Version: 0.9.3
+Version: 0.9.4
 Summary: Multithreaded version of numpy.einsum function
 Home-page: https://github.com/mrkwjc/einsumt
 Author: Marek Wojciechowski
 Author-email: mrkwjc@gmail.com
 License: MIT
 Keywords: numpy,einsum,hpc
 Classifier: Programming Language :: Python :: 2
```

### Comparing `einsumt-0.9.3/einsumt.py` & `einsumt-0.9.4/einsumt.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,17 +30,22 @@
                fresh pool is created. Otherwise, the 'pool' attribute is
                assumed to be a multiprocessing.pool.ThreadPool instance.
 
         idx  - specifies the subscript along which operands are divided
                into chunks
 
                Argument 'idx' have to be a single subscript letter, and should
-               be contained in the given subscripts, otherwise ValueError is
-               risen. If 'idx' is None or it is not given, then the longest
-               dimension in operands is searched.
+               be contained in the given input subscripts, otherwise ValueError
+               is rised. If 'idx' is None or it is not given, then the longest
+               dimension in operands is searched. NOTE: index which repeats
+               in any of the input subscripts cannot be used for chunking
+               operands. If such an index is explicitly given by 'idx'
+               then ValueError is raised. If no correct index is found when
+               automaitic searching is used then einsumt falls back to
+               np.einsum (this is rather exceptional case though).
 
     WARNING: Current implementation allows for string subscripts
              specification only
     """
     pool = kwargs.pop('pool', None)
     idx = kwargs.pop('idx', None)
     # If single processor fall back to np.einsum
@@ -80,14 +85,18 @@
     osub = osub.strip() # be sure osub is stripped
     # Get index along which we will chunk operands
     # If not given we try to search for longest dimension
     if idx is not None:  # and idx in indices...
         if idx not in iosubs[0]:
             raise ValueError("Index '%s' is not present in input subscripts"
                              % idx)
+        if sum([i.count(idx)>1 for i in isubs]):
+            raise ValueError("Index '%s' cannot be used. It repeats at least "
+                             "in one of the input operands"
+                             % idx)
         cidx = idx  # given index for chunks
         cdims = []
         for si, oi in zip(isubs, ops):
             k = si.find(cidx)
             cdims.append(oi.shape[k] if k >= 0 else 0)
         if len(set(cdims)) > 2:  # set elements can be 0 and one number
             raise ValueError("Different operand lengths along index '%s'"
@@ -95,16 +104,20 @@
         cdim = max(cdims)  # dimension along cidx
     else:
         maxdim = []
         maxidx = []
         for si, oi in zip(isubs, ops):
             mdim = max(oi.shape)
             midx = si[oi.shape.index(mdim)]
-            maxdim.append(mdim)
-            maxidx.append(midx)
+            if not sum([i.count(midx)>1 for i in isubs]):  # if not repeated
+                maxdim.append(mdim)
+                maxidx.append(midx)
+        if len(maxidx) == 0:
+            # No proper index is found -> fall back to np.einsum
+            return np.einsum(*operands, **kwargs)
         cdim = max(maxdim)                    # max dimension of input arrays
         cidx = maxidx[maxdim.index(cdim)]     # index chosen for chunks
     # Position of established index in subscripts
     cpos = [si.find(cidx) for si in isubs]  # positions of cidx in inputs
     opos = osub.find(cidx)                  # position of cidx in output
     ##
     # Determining chunk ranges
```

### Comparing `einsumt-0.9.3/setup.py` & `einsumt-0.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="einsumt",
-    version="0.9.3",
+    version="0.9.4",
     author="Marek Wojciechowski",
     author_email="mrkwjc@gmail.com",
     description="Multithreaded version of numpy.einsum function",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mrkwjc/einsumt",
     packages=setuptools.find_packages(),
```

