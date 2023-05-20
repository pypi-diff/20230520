# Comparing `tmp/low_index-1.1.1.tar.gz` & `tmp/low_index-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Apr 25 20:38:33 2022, from Unix
+gzip compressed data, was "low_index-1.2.tar", last modified: Fri May 19 21:29:18 2023, max compression
```

## Comparing `low_index-1.1.1.tar` & `low_index-1.2.tar`

### file list

```diff
@@ -1,23 +1,84 @@
-drwxr-xr-x   0 culler     (501) staff       (20)        0 2022-04-25 20:38:33.000000 low_index-1.1.1/
--rw-r--r--   0 culler     (501) staff       (20)     2418 2022-04-25 20:38:33.000000 low_index-1.1.1/PKG-INFO
-drwxr-xr-x   0 culler     (501) staff       (20)        0 2022-04-25 20:38:33.000000 low_index-1.1.1/cython_src/
-drwxr-xr-x   0 culler     (501) staff       (20)        0 2022-04-25 20:38:33.000000 low_index-1.1.1/python_src/
--rw-r--r--   0 culler     (501) staff       (20)       99 2022-03-11 21:19:19.000000 low_index-1.1.1/pyproject.toml
--rw-r--r--   0 culler     (501) staff       (20)       73 2022-03-20 18:07:55.000000 low_index-1.1.1/MANIFEST.in
--rw-r--r--   0 culler     (501) staff       (20)     1669 2022-04-25 20:38:33.000000 low_index-1.1.1/setup.py
--rw-r--r--   0 culler     (501) staff       (20)      899 2022-04-25 20:38:33.000000 low_index-1.1.1/setup.cfg
--rw-r--r--   0 culler     (501) staff       (20)     1643 2022-03-20 18:07:55.000000 low_index-1.1.1/README.rst
-drwxr-xr-x   0 culler     (501) staff       (20)        0 2022-04-25 20:38:33.000000 low_index-1.1.1/low_index.egg-info/
--rw-r--r--   0 culler     (501) staff       (20)     2418 2022-04-25 20:38:33.000000 low_index-1.1.1/low_index.egg-info/PKG-INFO
--rw-r--r--   0 culler     (501) staff       (20)        1 2022-04-25 20:38:33.000000 low_index-1.1.1/low_index.egg-info/not-zip-safe
--rw-r--r--   0 culler     (501) staff       (20)      399 2022-04-25 20:38:33.000000 low_index-1.1.1/low_index.egg-info/SOURCES.txt
--rw-r--r--   0 culler     (501) staff       (20)       10 2022-04-25 20:38:33.000000 low_index-1.1.1/low_index.egg-info/top_level.txt
--rw-r--r--   0 culler     (501) staff       (20)        1 2022-04-25 20:38:33.000000 low_index-1.1.1/low_index.egg-info/dependency_links.txt
--rw-r--r--   0 culler     (501) staff       (20)     3006 2022-04-25 19:28:36.000000 low_index-1.1.1/python_src/benchmark.py
--rw-r--r--   0 culler     (501) staff       (20)     1270 2022-03-14 16:49:29.000000 low_index-1.1.1/python_src/multi.py
--rw-r--r--   0 culler     (501) staff       (20)     1152 2022-04-25 19:15:38.000000 low_index-1.1.1/python_src/__init__.py
--rw-r--r--   0 culler     (501) staff       (20)     1575 2022-03-14 16:49:29.000000 low_index-1.1.1/python_src/test.py
--rw-r--r--   0 culler     (501) staff       (20)  1255883 2022-04-25 20:38:26.000000 low_index-1.1.1/cython_src/_low_index.c
--rw-r--r--   0 culler     (501) staff       (20)    32641 2022-04-25 18:50:02.000000 low_index-1.1.1/cython_src/covers.pxi
--rw-r--r--   0 culler     (501) staff       (20)     7685 2022-03-09 15:01:05.000000 low_index-1.1.1/cython_src/words.pxi
--rw-r--r--   0 culler     (501) staff       (20)      310 2022-03-17 16:14:49.000000 low_index-1.1.1/cython_src/_low_index.pyx
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-05-19 21:29:18.638376 low_index-1.2/
+-rw-r--r--   0 nmd      (444129884) staff       (20)      107 2023-05-19 21:29:13.000000 low_index-1.2/MANIFEST.in
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2417 2023-05-19 21:29:18.638508 low_index-1.2/PKG-INFO
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1667 2022-10-29 23:41:14.000000 low_index-1.2/README.rst
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-05-19 21:29:18.622019 low_index-1.2/cpp_src/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    12269 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/abstractSimsNode.cpp
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7408 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/abstractSimsNode.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5031 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/coveringSubgraph.cpp
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7022 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/coveringSubgraph.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5977 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/docAbstractSimsNode.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7394 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/docCoveringSubgraph.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4342 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/docLowIndex.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2615 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/docSimsNode.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3928 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/docSimsTree.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1990 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/docSimsTreeBase.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3879 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/docSimsTreeMultiThreaded.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1799 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/docWords.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2407 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/lowIndex.cpp
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4073 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/lowIndex.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-05-19 21:29:18.632803 low_index-1.2/cpp_src/pybind11/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    23883 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/pybind11/attr.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7069 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/pybind11/buffer_info.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)    65654 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/pybind11/cast.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8458 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/pybind11/chrono.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)      120 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/pybind11/common.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2096 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/pybind11/complex.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-05-19 21:29:18.635517 low_index-1.2/cpp_src/pybind11/detail/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    28101 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/pybind11/detail/class.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)    49007 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/pybind11/detail/common.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5491 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/pybind11/detail/descr.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)    17971 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/pybind11/detail/init.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)    24008 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/pybind11/detail/internals.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)    42266 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1513 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/pybind11/detail/typeid.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)    31685 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/pybind11/eigen.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10728 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/pybind11/embed.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4731 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/pybind11/eval.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4695 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/pybind11/functional.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6923 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/pybind11/gil.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8862 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/pybind11/iostream.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)    78946 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/pybind11/numpy.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9051 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/pybind11/operators.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2181 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/pybind11/options.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)   126295 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/pybind11/pybind11.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)    89415 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/pybind11/pytypes.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)    14556 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/pybind11/stl.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)    27013 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/pybind11/stl_bind.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2581 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/simsNode.cpp
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1437 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/simsNode.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2031 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/simsTree.cpp
+-rw-r--r--   0 nmd      (444129884) staff       (20)      781 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/simsTree.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)      895 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/simsTreeBase.cpp
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1403 2023-03-12 16:23:34.000000 low_index-1.2/cpp_src/simsTreeBase.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6666 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/simsTreeMultiThreaded.cpp
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5295 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/simsTreeMultiThreaded.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1740 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/stackedSimsNode.cpp
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2928 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/stackedSimsNode.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)      664 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/types.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4090 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/words.cpp
+-rw-r--r--   0 nmd      (444129884) staff       (20)      613 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/words.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)      931 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/wrapAbstractSimsNode.cpp
+-rw-r--r--   0 nmd      (444129884) staff       (20)      442 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/wrapAll.cpp
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1623 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/wrapCoveringSubgraph.cpp
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1659 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/wrapLowIndex.cpp
+-rw-r--r--   0 nmd      (444129884) staff       (20)      944 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/wrapModule.cpp
+-rw-r--r--   0 nmd      (444129884) staff       (20)      728 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/wrapSimsNode.cpp
+-rw-r--r--   0 nmd      (444129884) staff       (20)      691 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/wrapSimsTree.cpp
+-rw-r--r--   0 nmd      (444129884) staff       (20)      377 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/wrapSimsTreeBase.cpp
+-rw-r--r--   0 nmd      (444129884) staff       (20)      892 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/wrapSimsTreeMultiThreaded.cpp
+-rw-r--r--   0 nmd      (444129884) staff       (20)      482 2022-10-29 23:41:14.000000 low_index-1.2/cpp_src/wrapWords.cpp
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-05-19 21:29:18.637058 low_index-1.2/low_index.egg-info/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2417 2023-05-19 21:29:18.000000 low_index-1.2/low_index.egg-info/PKG-INFO
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1984 2023-05-19 21:29:18.000000 low_index-1.2/low_index.egg-info/SOURCES.txt
+-rw-r--r--   0 nmd      (444129884) staff       (20)        1 2023-05-19 21:29:18.000000 low_index-1.2/low_index.egg-info/dependency_links.txt
+-rw-r--r--   0 nmd      (444129884) staff       (20)        1 2023-05-19 21:23:37.000000 low_index-1.2/low_index.egg-info/not-zip-safe
+-rw-r--r--   0 nmd      (444129884) staff       (20)       10 2023-05-19 21:29:18.000000 low_index-1.2/low_index.egg-info/top_level.txt
+-rw-r--r--   0 nmd      (444129884) staff       (20)       66 2022-10-29 23:41:14.000000 low_index-1.2/pyproject.toml
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-05-19 21:29:18.638162 low_index-1.2/python_src/
+-rw-r--r--   0 nmd      (444129884) staff       (20)      207 2022-10-29 23:41:14.000000 low_index-1.2/python_src/__init__.py
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10093 2023-05-11 19:58:56.000000 low_index-1.2/python_src/benchmark.py
+-rw-r--r--   0 nmd      (444129884) staff       (20)      835 2022-10-29 23:41:14.000000 low_index-1.2/python_src/benchmark_util.py
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6531 2022-10-29 23:41:14.000000 low_index-1.2/python_src/test.py
+-rw-r--r--   0 nmd      (444129884) staff       (20)      898 2023-05-19 21:29:18.639022 low_index-1.2/setup.cfg
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1272 2022-10-29 23:41:14.000000 low_index-1.2/setup.py
```

### Comparing `low_index-1.1.1/PKG-INFO` & `low_index-1.2/low_index.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,63 +1,61 @@
 Metadata-Version: 2.1
-Name: low_index
-Version: 1.1.1
+Name: low-index
+Version: 1.2
 Summary: Enumerates low index subgroups of a finitely presented group
 Home-page: https://github.com/3-manifolds/low_index
 Author: Marc Culler, Nathan M. Dunfield and Matthias Goerner
 Author-email: culler@marc-culler.info, nathan@dunfield.info, enischte@gmail.com
 License: GPLv2+
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Cython
+Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Description-Content-Type: text/x-rst
 
 Low Index Subgroups
 ===================
 
 The low_index project provides a Python module which implements a variant
 of Charles Sims' Low Index Subgroups algorithm for enumerating all of
 the conjugacy classes of subgroups of a finitely presented group with
 finite index less than a given bound.
 
 The package is available on pypi, so the simplest way to install it for
-Python versions 3.6 - 3.10 is to use pip:
+Python versions 3.6 - 3.11 is to use pip:
 
 .. code-block:: bash
 
     pip3 install low-index
 
 Here is a sample computation:
 
 .. code-block:: python
 
     >>> from low_index import *
     >>>  # Conjugacy classes of subgroups of F_3 with index at most 4: 
-    >>> sgps = SimsTree(rank=3, max_degree=4).list()
-    >>> len(sgps)
+    >>> reps = permutation_reps(rank = 3, short_relators = [], long_relators = [], max_degree = 4)
+    >>> len(reps)
     653
     >>> from snappy import *
     >>> G = Manifold('K11n34').fundamental_group(); G
     Generators:
        a,b,c
     Relators:
        aaBcbbcAc
        aacAbCBBaCAAbbcBc
     >>> # Degree at most 7 covers of the exterior of the Conway knot:
-    >>> t = SimsTree(G.num_generators(), 7, G.relators(), num_long_relators=1)
-    >>> sgrps = t.list()
-    >>> len(sgps)
+    >>> reps = permutation_reps(G.num_generators(), G.relators()[:1], G.relators()[1:], 7)
+    >>> len(reps)
     52
-    >>> sgps[25].permutation_rep()
-    [[1, 0, 3, 5, 2, 4], [0, 2, 4, 1, 5, 3], [2, 3, 4, 0, 1, 5]]
+    >>> reps[25]
+    [[1, 0, 3, 2, 5, 6, 4], [1, 4, 0, 6, 2, 5, 3], [3, 0, 2, 6, 4, 1, 5]]
 
 
 Credits
 =======
 
 Primarily developed by `Marc Culler <https://marc-culler.info>`_,
 `Nathan Dunfield <http://dunfield.info>`_, and `Matthias Goerner
@@ -69,9 +67,7 @@
 Copyright 2022 by Marc Culler, Nathan Dunfield, Matthias Goerner
 and others.
 
 This code is released under the `GNU General Public License, version 2
 <http://www.gnu.org/licenses/gpl-2.0.txt>`_ or (at your option) any
 later version as published by the Free Software Foundation.
 
-
-
```

### Comparing `low_index-1.1.1/setup.cfg` & `low_index-1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 author_email = culler@marc-culler.info, nathan@dunfield.info, enischte@gmail.com
 license = GPLv2+
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 	Operating System :: OS Independent
-	Programming Language :: Cython
+	Programming Language :: C++
 	Programming Language :: Python
 	Topic :: Scientific/Engineering :: Mathematics
 
 [options]
-python_requires > = 3
+python_requires > = 3.6
 packages = low_index
 package_dir = 
 	low_index = python_src
 zip_safe = False
 
 [egg_info]
 tag_build =
```

### Comparing `low_index-1.1.1/README.rst` & `low_index-1.2/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -3,43 +3,42 @@
 
 The low_index project provides a Python module which implements a variant
 of Charles Sims' Low Index Subgroups algorithm for enumerating all of
 the conjugacy classes of subgroups of a finitely presented group with
 finite index less than a given bound.
 
 The package is available on pypi, so the simplest way to install it for
-Python versions 3.6 - 3.10 is to use pip:
+Python versions 3.6 - 3.11 is to use pip:
 
 .. code-block:: bash
 
     pip3 install low-index
 
 Here is a sample computation:
 
 .. code-block:: python
 
     >>> from low_index import *
     >>>  # Conjugacy classes of subgroups of F_3 with index at most 4: 
-    >>> sgps = SimsTree(rank=3, max_degree=4).list()
-    >>> len(sgps)
+    >>> reps = permutation_reps(rank = 3, short_relators = [], long_relators = [], max_degree = 4)
+    >>> len(reps)
     653
     >>> from snappy import *
     >>> G = Manifold('K11n34').fundamental_group(); G
     Generators:
        a,b,c
     Relators:
        aaBcbbcAc
        aacAbCBBaCAAbbcBc
     >>> # Degree at most 7 covers of the exterior of the Conway knot:
-    >>> t = SimsTree(G.num_generators(), 7, G.relators(), num_long_relators=1)
-    >>> sgrps = t.list()
-    >>> len(sgps)
+    >>> reps = permutation_reps(G.num_generators(), G.relators()[:1], G.relators()[1:], 7)
+    >>> len(reps)
     52
-    >>> sgps[25].permutation_rep()
-    [[1, 0, 3, 5, 2, 4], [0, 2, 4, 1, 5, 3], [2, 3, 4, 0, 1, 5]]
+    >>> reps[25]
+    [[1, 0, 3, 2, 5, 6, 4], [1, 4, 0, 6, 2, 5, 3], [3, 0, 2, 6, 4, 1, 5]]
 
 
 Credits
 =======
 
 Primarily developed by `Marc Culler <https://marc-culler.info>`_,
 `Nathan Dunfield <http://dunfield.info>`_, and `Matthias Goerner
```

### Comparing `low_index-1.1.1/low_index.egg-info/PKG-INFO` & `low_index-1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,61 @@
 Metadata-Version: 2.1
-Name: low-index
-Version: 1.1.1
+Name: low_index
+Version: 1.2
 Summary: Enumerates low index subgroups of a finitely presented group
 Home-page: https://github.com/3-manifolds/low_index
 Author: Marc Culler, Nathan M. Dunfield and Matthias Goerner
 Author-email: culler@marc-culler.info, nathan@dunfield.info, enischte@gmail.com
 License: GPLv2+
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Cython
+Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Description-Content-Type: text/x-rst
 
 Low Index Subgroups
 ===================
 
 The low_index project provides a Python module which implements a variant
 of Charles Sims' Low Index Subgroups algorithm for enumerating all of
 the conjugacy classes of subgroups of a finitely presented group with
 finite index less than a given bound.
 
 The package is available on pypi, so the simplest way to install it for
-Python versions 3.6 - 3.10 is to use pip:
+Python versions 3.6 - 3.11 is to use pip:
 
 .. code-block:: bash
 
     pip3 install low-index
 
 Here is a sample computation:
 
 .. code-block:: python
 
     >>> from low_index import *
     >>>  # Conjugacy classes of subgroups of F_3 with index at most 4: 
-    >>> sgps = SimsTree(rank=3, max_degree=4).list()
-    >>> len(sgps)
+    >>> reps = permutation_reps(rank = 3, short_relators = [], long_relators = [], max_degree = 4)
+    >>> len(reps)
     653
     >>> from snappy import *
     >>> G = Manifold('K11n34').fundamental_group(); G
     Generators:
        a,b,c
     Relators:
        aaBcbbcAc
        aacAbCBBaCAAbbcBc
     >>> # Degree at most 7 covers of the exterior of the Conway knot:
-    >>> t = SimsTree(G.num_generators(), 7, G.relators(), num_long_relators=1)
-    >>> sgrps = t.list()
-    >>> len(sgps)
+    >>> reps = permutation_reps(G.num_generators(), G.relators()[:1], G.relators()[1:], 7)
+    >>> len(reps)
     52
-    >>> sgps[25].permutation_rep()
-    [[1, 0, 3, 5, 2, 4], [0, 2, 4, 1, 5, 3], [2, 3, 4, 0, 1, 5]]
+    >>> reps[25]
+    [[1, 0, 3, 2, 5, 6, 4], [1, 4, 0, 6, 2, 5, 3], [3, 0, 2, 6, 4, 1, 5]]
 
 
 Credits
 =======
 
 Primarily developed by `Marc Culler <https://marc-culler.info>`_,
 `Nathan Dunfield <http://dunfield.info>`_, and `Matthias Goerner
@@ -69,9 +67,7 @@
 Copyright 2022 by Marc Culler, Nathan Dunfield, Matthias Goerner
 and others.
 
 This code is released under the `GNU General Public License, version 2
 <http://www.gnu.org/licenses/gpl-2.0.txt>`_ or (at your option) any
 later version as published by the Free Software Foundation.
 
-
-
```

