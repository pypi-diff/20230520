# Comparing `tmp/fuefpyco-0.2.0.tar.gz` & `tmp/fuefpyco-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuefpyco-0.2.0.tar", last modified: Sat May 20 12:54:54 2023, max compression
+gzip compressed data, was "fuefpyco-0.3.0.tar", last modified: Sat May 20 14:22:36 2023, max compression
```

## Comparing `fuefpyco-0.2.0.tar` & `fuefpyco-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:54:54.141960 fuefpyco-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-20 12:54:30.000000 fuefpyco-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-20 12:54:54.141960 fuefpyco-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-20 12:54:30.000000 fuefpyco-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-20 12:54:30.000000 fuefpyco-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-20 12:54:54.141960 fuefpyco-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-20 12:54:30.000000 fuefpyco-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:54:54.137960 fuefpyco-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:54:54.137960 fuefpyco-0.2.0/src/fuefpyco/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-20 12:54:30.000000 fuefpyco-0.2.0/src/fuefpyco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-20 12:54:30.000000 fuefpyco-0.2.0/src/fuefpyco/ds.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-20 12:54:30.000000 fuefpyco-0.2.0/src/fuefpyco/it.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:54:54.137960 fuefpyco-0.2.0/src/fuefpyco/pa/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-20 12:54:30.000000 fuefpyco-0.2.0/src/fuefpyco/pa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-20 12:54:30.000000 fuefpyco-0.2.0/src/fuefpyco/pa/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-05-20 12:54:30.000000 fuefpyco-0.2.0/src/fuefpyco/pa/process_per_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:54:54.137960 fuefpyco-0.2.0/src/fuefpyco/pd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 12:54:30.000000 fuefpyco-0.2.0/src/fuefpyco/pd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-20 12:54:30.000000 fuefpyco-0.2.0/src/fuefpyco/pd/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:54:54.137960 fuefpyco-0.2.0/src/fuefpyco.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-20 12:54:54.000000 fuefpyco-0.2.0/src/fuefpyco.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-20 12:54:54.000000 fuefpyco-0.2.0/src/fuefpyco.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 12:54:54.000000 fuefpyco-0.2.0/src/fuefpyco.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-20 12:54:54.000000 fuefpyco-0.2.0/src/fuefpyco.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-20 12:54:54.000000 fuefpyco-0.2.0/src/fuefpyco.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:54:54.141960 fuefpyco-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-20 12:54:30.000000 fuefpyco-0.2.0/tests/test_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-20 12:54:30.000000 fuefpyco-0.2.0/tests/test_it.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-20 12:54:30.000000 fuefpyco-0.2.0/tests/test_pa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:22:36.043539 fuefpyco-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-20 14:22:10.000000 fuefpyco-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-20 14:22:36.043539 fuefpyco-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-20 14:22:10.000000 fuefpyco-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-20 14:22:10.000000 fuefpyco-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-20 14:22:36.043539 fuefpyco-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-20 14:22:10.000000 fuefpyco-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:22:36.039539 fuefpyco-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:22:36.039539 fuefpyco-0.3.0/src/fuefpyco/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-20 14:22:10.000000 fuefpyco-0.3.0/src/fuefpyco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-20 14:22:10.000000 fuefpyco-0.3.0/src/fuefpyco/ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-20 14:22:10.000000 fuefpyco-0.3.0/src/fuefpyco/it.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:22:36.043539 fuefpyco-0.3.0/src/fuefpyco/pa/
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-20 14:22:10.000000 fuefpyco-0.3.0/src/fuefpyco/pa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-20 14:22:10.000000 fuefpyco-0.3.0/src/fuefpyco/pa/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-05-20 14:22:10.000000 fuefpyco-0.3.0/src/fuefpyco/pa/process_per_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-20 14:22:10.000000 fuefpyco-0.3.0/src/fuefpyco/pa/process_pool_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:22:36.043539 fuefpyco-0.3.0/src/fuefpyco/pd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 14:22:10.000000 fuefpyco-0.3.0/src/fuefpyco/pd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-20 14:22:10.000000 fuefpyco-0.3.0/src/fuefpyco/pd/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:22:36.043539 fuefpyco-0.3.0/src/fuefpyco.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-20 14:22:36.000000 fuefpyco-0.3.0/src/fuefpyco.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-20 14:22:36.000000 fuefpyco-0.3.0/src/fuefpyco.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 14:22:36.000000 fuefpyco-0.3.0/src/fuefpyco.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-20 14:22:36.000000 fuefpyco-0.3.0/src/fuefpyco.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-20 14:22:36.000000 fuefpyco-0.3.0/src/fuefpyco.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:22:36.043539 fuefpyco-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-20 14:22:10.000000 fuefpyco-0.3.0/tests/test_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-20 14:22:10.000000 fuefpyco-0.3.0/tests/test_it.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-20 14:22:10.000000 fuefpyco-0.3.0/tests/test_pa.py
```

### Comparing `fuefpyco-0.2.0/LICENSE` & `fuefpyco-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fuefpyco-0.2.0/PKG-INFO` & `fuefpyco-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuefpyco
-Version: 0.2.0
+Version: 0.3.0
 Summary: Functional Efficient Python Computations
 License: " BSD-3-Clause"
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `fuefpyco-0.2.0/README.md` & `fuefpyco-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `fuefpyco-0.2.0/setup.cfg` & `fuefpyco-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `fuefpyco-0.2.0/src/fuefpyco/ds.py` & `fuefpyco-0.3.0/src/fuefpyco/ds.py`

 * *Files identical despite different names*

### Comparing `fuefpyco-0.2.0/src/fuefpyco/it.py` & `fuefpyco-0.3.0/src/fuefpyco/it.py`

 * *Files identical despite different names*

### Comparing `fuefpyco-0.2.0/src/fuefpyco/pa/__init__.py` & `fuefpyco-0.3.0/src/fuefpyco/pa/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,16 +5,21 @@
  - argument check by mypy. We enforce the function to be executed takes a single argument, typically a dataclass
    of the actual parameters. This restriction is due to **kwargs being quite hard to check.
  - MaybeResult-based exception propagation and process-level retries -- we don't want a single crash to bring the whole
    computation down. Note that if the function itself already returns MaybeResult, those get nested.
 
 There are multiple implementations, each with its own vices and virtues. In particular:
  - ProcessPerTask -- launches a new process for every task. Gives the most timeout-retry control, slowest, memory-safe.
+ - ProcessPoolExecutor -- submits tasks to a process pool executor. Less control on timeouts, but faster.
 
 To use, instantiate the respective class, and feed it to the `mapreduce` function along with your `f` (the "map") and
 inputs (an iterable). The "reduce" part is given via the return value being a Monoid, with the summing happening
 usually in the main process.
+
+Additionally, both input and output class in the mapreduce must be serializable, as well as the `f` itself.
 """
 
 from fuefpyco.pa.core import mapreduce  # noqa: F401
 from fuefpyco.pa.process_per_task import Config as PPTConfig  # noqa: F401
 from fuefpyco.pa.process_per_task import ProcessPerTask  # noqa: F401
+from fuefpyco.pa.process_pool_executor import Config as PPEConfig  # noqa: F401
+from fuefpyco.pa.process_pool_executor import ProcessPoolExecutor  # noqa: F401
```

### Comparing `fuefpyco-0.2.0/src/fuefpyco/pa/core.py` & `fuefpyco-0.3.0/src/fuefpyco/pa/core.py`

 * *Files identical despite different names*

### Comparing `fuefpyco-0.2.0/src/fuefpyco/pa/process_per_task.py` & `fuefpyco-0.3.0/src/fuefpyco/pa/process_per_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
  - mp.Queue is used to retrieve the results from local workers. In case of huge data volumes, this may bring some
    troubles -- you may want to write disks instead, with the ipc being the file names only.
 
 To use, instantiate the dataclass ProcessPerTask, with the config field containing all the tweakable behaviour, and
 pass to the core.mapreduce method.
 """
 
-# TODO instead of full timeout, wait just on the queue
-# TODO retries
+# TODO https://github.com/tmi/fuefpyco/issues/3 instead of full timeout, wait just on the queue
+# TODO https://github.com/tmi/fuefpyco/issues/2 retries
 
 import logging
 import time
 from dataclasses import dataclass
 from multiprocessing import Process, Queue, get_context
 from queue import Empty as EmptyQueueException
 from typing import Callable, Generic, Iterable, Iterator, Optional, TypeVar
@@ -66,15 +66,15 @@
     try:
         result = MaybeResult(f(arg), [])
     except Exception as e:
         result = MaybeResult(None, [Failure(f"failure with args {arg}", e)])
     q.put(_IntermediateResult(result=result, p_id=p_id))
 
 
-def process_per_task_mapreduce(f: Callable[[T], TMonoid], s: Iterable[T], c: Config) -> MaybeResult[TMonoid]:
+def _mapreduce(f: Callable[[T], TMonoid], s: Iterable[T], c: Config) -> MaybeResult[TMonoid]:
     if c.task_retries > 0:
         raise NotImplementedError("non-zero retries are not implemented yet")
     result: MaybeResult[TMonoid] = MaybeResult.empty()
     ctx = get_context(c.mp_context)
     queue = ctx.Queue()
 
     running: dict[int, _ProgressTracker] = {}
@@ -144,8 +144,8 @@
 
 
 @dataclass
 class ProcessPerTask:
     config: Config
 
     def mapreduce(self, f: Callable[[T], TMonoid], s: Iterable[T]) -> MaybeResult[TMonoid]:
-        return process_per_task_mapreduce(f, s, self.config)
+        return _mapreduce(f, s, self.config)
```

### Comparing `fuefpyco-0.2.0/src/fuefpyco/pd/generators.py` & `fuefpyco-0.3.0/src/fuefpyco/pd/generators.py`

 * *Files identical despite different names*

### Comparing `fuefpyco-0.2.0/src/fuefpyco.egg-info/PKG-INFO` & `fuefpyco-0.3.0/src/fuefpyco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuefpyco
-Version: 0.2.0
+Version: 0.3.0
 Summary: Functional Efficient Python Computations
 License: " BSD-3-Clause"
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `fuefpyco-0.2.0/tests/test_ds.py` & `fuefpyco-0.3.0/tests/test_ds.py`

 * *Files identical despite different names*

### Comparing `fuefpyco-0.2.0/tests/test_it.py` & `fuefpyco-0.3.0/tests/test_it.py`

 * *Files identical despite different names*

