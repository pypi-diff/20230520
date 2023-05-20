# Comparing `tmp/fuefpyco-0.1.0.tar.gz` & `tmp/fuefpyco-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuefpyco-0.1.0.tar", last modified: Sun Feb 19 15:36:11 2023, max compression
+gzip compressed data, was "fuefpyco-0.2.0.tar", last modified: Sat May 20 12:54:54 2023, max compression
```

## Comparing `fuefpyco-0.1.0.tar` & `fuefpyco-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 15:36:11.165240 fuefpyco-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-02-19 15:35:47.000000 fuefpyco-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-02-19 15:36:11.165240 fuefpyco-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-02-19 15:35:47.000000 fuefpyco-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-02-19 15:35:47.000000 fuefpyco-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-02-19 15:36:11.165240 fuefpyco-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-02-19 15:35:47.000000 fuefpyco-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 15:36:11.161240 fuefpyco-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 15:36:11.165240 fuefpyco-0.1.0/src/fuefpyco/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-02-19 15:35:47.000000 fuefpyco-0.1.0/src/fuefpyco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-02-19 15:35:47.000000 fuefpyco-0.1.0/src/fuefpyco/ds.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-02-19 15:35:47.000000 fuefpyco-0.1.0/src/fuefpyco/it.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 15:36:11.165240 fuefpyco-0.1.0/src/fuefpyco/pa/
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-02-19 15:35:47.000000 fuefpyco-0.1.0/src/fuefpyco/pa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 15:36:11.165240 fuefpyco-0.1.0/src/fuefpyco.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-02-19 15:36:11.000000 fuefpyco-0.1.0/src/fuefpyco.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-02-19 15:36:11.000000 fuefpyco-0.1.0/src/fuefpyco.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-19 15:36:11.000000 fuefpyco-0.1.0/src/fuefpyco.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-19 15:36:11.000000 fuefpyco-0.1.0/src/fuefpyco.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-19 15:36:11.000000 fuefpyco-0.1.0/src/fuefpyco.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 15:36:11.165240 fuefpyco-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-02-19 15:35:47.000000 fuefpyco-0.1.0/tests/test_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-02-19 15:35:47.000000 fuefpyco-0.1.0/tests/test_it.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-02-19 15:35:47.000000 fuefpyco-0.1.0/tests/test_pa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:54:54.141960 fuefpyco-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-20 12:54:30.000000 fuefpyco-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-20 12:54:54.141960 fuefpyco-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-20 12:54:30.000000 fuefpyco-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-20 12:54:30.000000 fuefpyco-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-20 12:54:54.141960 fuefpyco-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-20 12:54:30.000000 fuefpyco-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:54:54.137960 fuefpyco-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:54:54.137960 fuefpyco-0.2.0/src/fuefpyco/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-20 12:54:30.000000 fuefpyco-0.2.0/src/fuefpyco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-20 12:54:30.000000 fuefpyco-0.2.0/src/fuefpyco/ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-20 12:54:30.000000 fuefpyco-0.2.0/src/fuefpyco/it.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:54:54.137960 fuefpyco-0.2.0/src/fuefpyco/pa/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-20 12:54:30.000000 fuefpyco-0.2.0/src/fuefpyco/pa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-20 12:54:30.000000 fuefpyco-0.2.0/src/fuefpyco/pa/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-05-20 12:54:30.000000 fuefpyco-0.2.0/src/fuefpyco/pa/process_per_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:54:54.137960 fuefpyco-0.2.0/src/fuefpyco/pd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 12:54:30.000000 fuefpyco-0.2.0/src/fuefpyco/pd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-20 12:54:30.000000 fuefpyco-0.2.0/src/fuefpyco/pd/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:54:54.137960 fuefpyco-0.2.0/src/fuefpyco.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-20 12:54:54.000000 fuefpyco-0.2.0/src/fuefpyco.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-20 12:54:54.000000 fuefpyco-0.2.0/src/fuefpyco.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 12:54:54.000000 fuefpyco-0.2.0/src/fuefpyco.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-20 12:54:54.000000 fuefpyco-0.2.0/src/fuefpyco.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-20 12:54:54.000000 fuefpyco-0.2.0/src/fuefpyco.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:54:54.141960 fuefpyco-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-20 12:54:30.000000 fuefpyco-0.2.0/tests/test_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-20 12:54:30.000000 fuefpyco-0.2.0/tests/test_it.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-20 12:54:30.000000 fuefpyco-0.2.0/tests/test_pa.py
```

### Comparing `fuefpyco-0.1.0/LICENSE` & `fuefpyco-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fuefpyco-0.1.0/PKG-INFO` & `fuefpyco-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuefpyco
-Version: 0.1.0
+Version: 0.2.0
 Summary: Functional Efficient Python Computations
 License: " BSD-3-Clause"
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `fuefpyco-0.1.0/README.md` & `fuefpyco-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `fuefpyco-0.1.0/setup.cfg` & `fuefpyco-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `fuefpyco-0.1.0/src/fuefpyco/ds.py` & `fuefpyco-0.2.0/src/fuefpyco/ds.py`

 * *Files identical despite different names*

### Comparing `fuefpyco-0.1.0/src/fuefpyco/it.py` & `fuefpyco-0.2.0/src/fuefpyco/it.py`

 * *Files identical despite different names*

### Comparing `fuefpyco-0.1.0/src/fuefpyco/pa/__init__.py` & `fuefpyco-0.2.0/src/fuefpyco/pa/process_per_task.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,53 @@
 """
-This module provides parallel execution to map-reduce computations: single function to be applied on a sequence
-of arguments, and the result being a monoid sum. The primary advantages over existing python high level interfaces are:
- - timeouts on the process level -- even when the GIL is held by the computation, you can still time it out
- - argument check by mypy. We enforce the function to be executed takes a single argument, typically a dataclass
-   of the actual parameters. This restriction is due to **kwargs being quite hard to check.
- - MaybeResult-based exception propagation and process-level retries -- we don't want a single crash to bring the whole
-   computation down. Note that if the function itself already returns MaybeResult, those get nested.
-
-Notes:
-  - Retry applies in the case of timeout or any exception thrown by the function. A case of non-zero exit of
-    the process with _any_ result returned is considered a success, and the non-zero exit code is provided
-    in a message in the `failure.origin` field.
-  - In case of a retry, the failure reason(s) are returned as well, with the attempt counter prepended to
-    the `failure.origin` field.
-  - We use mp.Queue to retrieve the results from local workers. In case of huge data volumes, this may bring some
-    troubles -- you may want to write disks instead, with the ipc being the file names only.
+Implements MapReduce via vanilla processes. Every task is processed by exactly one process.
+Parallelism is by starting `n` processes at the start and giving each its own task, waiting for any to finish and
+starting new ones to keep the number of running `n`.
+
+Features:
+ - timeout of a task (by killing the respective processes),
+ - retry of a task (by re-submitting a new process),
+   - applies in the case of timeout or any exception thrown by the function. A case of non-zero exit of
+     the process with _any_ result returned is considered a success, and the non-zero exit code is provided
+     in a message in the `failure.origin` field,
+   - in case of a retry, the failure reason(s) are returned as well, with the attempt counter prepended to
+     the `failure.origin` field.
+ - low memory consumption (no risk of memory leak across multiple tasks),
+ - slower throughput (has to start multiple processes),
+ - mp.Queue is used to retrieve the results from local workers. In case of huge data volumes, this may bring some
+   troubles -- you may want to write disks instead, with the ipc being the file names only.
+
+To use, instantiate the dataclass ProcessPerTask, with the config field containing all the tweakable behaviour, and
+pass to the core.mapreduce method.
 """
 
+# TODO instead of full timeout, wait just on the queue
+# TODO retries
+
 import logging
 import time
 from dataclasses import dataclass
 from multiprocessing import Process, Queue, get_context
 from queue import Empty as EmptyQueueException
-from typing import Callable, Generic, Iterable, Iterator, Literal, Optional, TypeVar
+from typing import Callable, Generic, Iterable, Iterator, Optional, TypeVar
 
 from fuefpyco.ds import Failure, MaybeResult, TMonoid
 
 logger = logging.getLogger(__name__)
 
 _process_join_grace = 3  # number of seconds we wait to join processes that returned. 0 should suffice
 
 
 @dataclass
-class ComputationConfig:
+class Config:
     parallelism: int
-    single_task_timeout_s: int
-    retry: int = 0
-    implementation: Literal["process"] = "process"  # TODO add processes with reusal
+    task_timeout_s: int
+    task_retries: int = 0
+
+    mp_context: str = "forkserver"
 
 
 T = TypeVar("T")
 
 
 @dataclass
 class _IntermediateResult(Generic[TMonoid]):
@@ -59,19 +66,19 @@
     try:
         result = MaybeResult(f(arg), [])
     except Exception as e:
         result = MaybeResult(None, [Failure(f"failure with args {arg}", e)])
     q.put(_IntermediateResult(result=result, p_id=p_id))
 
 
-def mapreduce(f: Callable[[T], TMonoid], s: Iterable[T], c: ComputationConfig) -> MaybeResult[TMonoid]:
-    if c.retry > 0:
+def process_per_task_mapreduce(f: Callable[[T], TMonoid], s: Iterable[T], c: Config) -> MaybeResult[TMonoid]:
+    if c.task_retries > 0:
         raise NotImplementedError("non-zero retries are not implemented yet")
     result: MaybeResult[TMonoid] = MaybeResult.empty()
-    ctx = get_context("forkserver")
+    ctx = get_context(c.mp_context)
     queue = ctx.Queue()
 
     running: dict[int, _ProgressTracker] = {}
     capacity: Callable[[], int] = lambda: c.parallelism - len(running)
     it: Optional[Iterator[T]] = iter(s)
     p_id = 0
 
@@ -94,15 +101,15 @@
         if capacity() == c.parallelism:
             if running:
                 raise ValueError(f"internal error: expected no processes running, but {len(running)} entries remain")
             logger.debug("all processes completed, breaking main loop")
             break
         # wait for next result
         oldest_submit = min(e.submit_time_s for e in running.values())
-        next_timeout = oldest_submit + c.single_task_timeout_s
+        next_timeout = oldest_submit + c.task_timeout_s
         current_time = time.monotonic_ns() // 1e9
         if next_timeout > current_time:
             try:
                 wait_time = next_timeout - current_time
                 logger.debug(f"about to wait for {wait_time} seconds for a result")
                 intermediate = queue.get(timeout=wait_time)
                 tracker = running.pop(intermediate.p_id)
@@ -130,7 +137,15 @@
                     None, [Failure(f"timed out with arg {convict.arg}", Exception())]
                 )
                 result = result + sentence
                 logger.debug(f"killing process #{p_id} with pid {convict.p.pid}")
                 convict.p.kill()
                 break
     return result
+
+
+@dataclass
+class ProcessPerTask:
+    config: Config
+
+    def mapreduce(self, f: Callable[[T], TMonoid], s: Iterable[T]) -> MaybeResult[TMonoid]:
+        return process_per_task_mapreduce(f, s, self.config)
```

### Comparing `fuefpyco-0.1.0/src/fuefpyco.egg-info/PKG-INFO` & `fuefpyco-0.2.0/src/fuefpyco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuefpyco
-Version: 0.1.0
+Version: 0.2.0
 Summary: Functional Efficient Python Computations
 License: " BSD-3-Clause"
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `fuefpyco-0.1.0/tests/test_ds.py` & `fuefpyco-0.2.0/tests/test_ds.py`

 * *Files identical despite different names*

### Comparing `fuefpyco-0.1.0/tests/test_it.py` & `fuefpyco-0.2.0/tests/test_it.py`

 * *Files identical despite different names*

### Comparing `fuefpyco-0.1.0/tests/test_pa.py` & `fuefpyco-0.2.0/tests/test_pa.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from dataclasses import dataclass, replace
 
 from typing_extensions import Self
 
 from fuefpyco.ds import Failure, msum
-from fuefpyco.pa import ComputationConfig, mapreduce
+from fuefpyco.pa import PPTConfig, ProcessPerTask, mapreduce
 
 
 @dataclass
 class AMonoid:
     a: int
 
     def __add__(self, other: Self) -> Self:
@@ -26,15 +26,15 @@
     if a > 9:
         raise _error
     return AMonoid(a=a * 2)
 
 
 def test_mapreduce_happy():
     logging.basicConfig(level="DEBUG", force=True)
-    config = ComputationConfig(parallelism=4, single_task_timeout_s=1)
+    config = ProcessPerTask(PPTConfig(parallelism=4, task_timeout_s=1))
     input_seq = [1, 2, 3]
     result = mapreduce(simple_f, input_seq, config)
     assert result.result == msum((simple_f(e) for e in input_seq), AMonoid)
     assert result.failure == []
 
     seq_with_error = [1, 2, 10]
     result = mapreduce(simple_f, seq_with_error, config)
```

