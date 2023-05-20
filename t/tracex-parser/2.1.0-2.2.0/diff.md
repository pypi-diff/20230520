# Comparing `tmp/tracex_parser-2.1.0.tar.gz` & `tmp/tracex_parser-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracex_parser-2.1.0.tar", max compression
+gzip compressed data, was "tracex_parser-2.2.0.tar", max compression
```

## Comparing `tracex_parser-2.1.0.tar` & `tracex_parser-2.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3266 2023-03-11 03:13:41.437608 tracex_parser-2.1.0/README.md
--rw-r--r--   0        0        0    32000 2023-03-11 03:13:41.437608 tracex_parser-2.1.0/demo_filex.trx
--rw-r--r--   0        0        0    32000 2023-03-11 03:13:41.437608 tracex_parser-2.1.0/demo_netx_tcp.trx
--rw-r--r--   0        0        0    32000 2023-03-11 03:13:41.437608 tracex_parser-2.1.0/demo_netx_udp.trx
--rw-r--r--   0        0        0    32768 2023-03-11 03:13:41.437608 tracex_parser-2.1.0/demo_threadx.trx
--rw-r--r--   0        0        0      889 2023-03-11 03:13:41.437608 tracex_parser-2.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-11 03:13:41.437608 tracex_parser-2.1.0/tracex_parser/__init__.py
--rw-r--r--   0        0        0    11132 2023-03-11 03:13:41.437608 tracex_parser-2.1.0/tracex_parser/events.py
--rwxr-xr-x   0        0        0     9640 2023-03-11 03:13:41.437608 tracex_parser-2.1.0/tracex_parser/file_parser.py
--rw-r--r--   0        0        0     2132 2023-03-11 03:13:41.437608 tracex_parser-2.1.0/tracex_parser/helpers.py
--rw-r--r--   0        0        0     3887 2023-03-11 03:13:57.020071 tracex_parser-2.1.0/setup.py
--rw-r--r--   0        0        0     4114 2023-03-11 03:13:57.020533 tracex_parser-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3266 2023-05-20 16:53:41.535213 tracex_parser-2.2.0/README.md
+-rw-r--r--   0        0        0    32000 2023-05-20 16:53:41.535213 tracex_parser-2.2.0/demo_filex.trx
+-rw-r--r--   0        0        0    32000 2023-05-20 16:53:41.535213 tracex_parser-2.2.0/demo_netx_tcp.trx
+-rw-r--r--   0        0        0    32000 2023-05-20 16:53:41.535213 tracex_parser-2.2.0/demo_netx_udp.trx
+-rw-r--r--   0        0        0    32768 2023-05-20 16:53:41.535213 tracex_parser-2.2.0/demo_threadx.trx
+-rw-r--r--   0        0        0      889 2023-05-20 16:53:41.535213 tracex_parser-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-20 16:53:41.535213 tracex_parser-2.2.0/tracex_parser/__init__.py
+-rw-r--r--   0        0        0    12117 2023-05-20 16:53:41.535213 tracex_parser-2.2.0/tracex_parser/events.py
+-rwxr-xr-x   0        0        0     9640 2023-05-20 16:53:41.535213 tracex_parser-2.2.0/tracex_parser/file_parser.py
+-rw-r--r--   0        0        0     2132 2023-05-20 16:53:41.535213 tracex_parser-2.2.0/tracex_parser/helpers.py
+-rw-r--r--   0        0        0     3887 2023-05-20 16:53:53.340665 tracex_parser-2.2.0/setup.py
+-rw-r--r--   0        0        0     4114 2023-05-20 16:53:53.341123 tracex_parser-2.2.0/PKG-INFO
```

### Comparing `tracex_parser-2.1.0/README.md` & `tracex_parser-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tracex_parser-2.1.0/demo_filex.trx` & `tracex_parser-2.2.0/demo_filex.trx`

 * *Files identical despite different names*

### Comparing `tracex_parser-2.1.0/demo_netx_tcp.trx` & `tracex_parser-2.2.0/demo_netx_tcp.trx`

 * *Files identical despite different names*

### Comparing `tracex_parser-2.1.0/demo_netx_udp.trx` & `tracex_parser-2.2.0/demo_netx_udp.trx`

 * *Files identical despite different names*

### Comparing `tracex_parser-2.1.0/demo_threadx.trx` & `tracex_parser-2.2.0/demo_threadx.trx`

 * *Files identical despite different names*

### Comparing `tracex_parser-2.1.0/pyproject.toml` & `tracex_parser-2.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "tracex_parser"
-version = "2.1.0"
+version = "2.2.0"
 description = "Parser for ThreadX RTOS's trace buffers (aka TraceX)"
 authors = ["Julianne Swinoga <julianneswinoga@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 include = [
     '*.trx',
 ]
```

### Comparing `tracex_parser-2.1.0/tracex_parser/events.py` & `tracex_parser-2.2.0/tracex_parser/events.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 class CommonArg:
     """
     Holds string mappings for common arguments so that we can
     reference this mapping in TraceXEvent, instead of a raw string.
     """
     stack_ptr = 'stack_ptr'
     queue_ptr = 'queue_ptr'
+    pool_ptr = 'pool_ptr'
     timeout = 'timeout'
     # The following will attempted to be looked up in the object registry and mapped to strings
     obj_id = 'obj_id'
     thread_ptr = 'thread_ptr'
     next_thread = 'next_thread'
 
 
@@ -139,19 +140,31 @@
     4: tracex_event_factory('ISRExitEvent', 'isrExit',
                             [CommonArg.stack_ptr, 'isr_num', 'sys_state', 'preempt_dis']),
     5: tracex_event_factory('TimeSliceEvent', 'timeSlice',
                             ['nxt_thread', 'sys_state', 'preempt_disable', CommonArg.stack_ptr]),
     6: tracex_event_factory('RunningEvent', 'running',
                             ['_1', '_2', '_3', '_4']),  # No args that we care about
     10: tracex_event_factory('BlockAllocateEvent', 'blockAlloc',
-                             ['pool_ptr', 'mem_ptr', CommonArg.timeout, 'rem_blocks']),
+                             [CommonArg.pool_ptr, 'mem_ptr', CommonArg.timeout, 'rem_blocks']),
+    11: tracex_event_factory('BlockPoolCreate', 'blockPoolCreate',
+                             [CommonArg.pool_ptr, 'pool_start', 'total_blocks', 'block_size']),
+    12: tracex_event_factory('BlockPoolDelete', 'blockPoolDel',
+                             [CommonArg.pool_ptr, CommonArg.stack_ptr, '_3', '_4']),
+    13: tracex_event_factory('BlockPoolInfo', 'blockPoolInfo',
+                             [CommonArg.pool_ptr, '_2', '_3', '_4']),
+    14: tracex_event_factory('BlockPoolPerformanceInfo', 'blockPoolPerfInfo',
+                             [CommonArg.pool_ptr, '_2', '_3', '_4']),
+    15: tracex_event_factory('BlockPoolPerformanceSystemInfo', 'blockPoolPerfSysInfo',
+                             ['_1', '_2', '_3', '_4']),  # No args that we care about
+    16: tracex_event_factory('BlockPoolPrioritize', 'blockPoolPrioritize',
+                             [CommonArg.pool_ptr, 'suspend_cnt', CommonArg.stack_ptr, '_4']),
     17: tracex_event_factory('BlockReleaseEvent', 'blockRelease',
-                             ['pool_ptr', 'mem_ptr', 'suspended', CommonArg.stack_ptr]),
+                             [CommonArg.pool_ptr, 'mem_ptr', 'suspended', CommonArg.stack_ptr]),
     27: tracex_event_factory('ByteReleaseEvent', 'byteRelease',
-                             ['pool_ptr', 'mem_ptr', 'suspended', 'avail_bytes']),
+                             [CommonArg.pool_ptr, 'mem_ptr', 'suspended', 'avail_bytes']),
     32: tracex_event_factory('FlagsGetEvent', 'flagsGet',
                              ['group_ptr', 'req_flags', 'cur_flags', 'get_opt']),
     36: tracex_event_factory('FlagsSetEvent', 'flagsSet',
                              ['group_ptr', 'flags', 'set_opt', 'suspend_cnt']),
     50: tracex_event_factory('MtxCreateEvent', 'mtxCreate',
                              [CommonArg.obj_id, 'inheritance', CommonArg.stack_ptr, '_4']),
     51: tracex_event_factory('MtxDeleteEvent', 'mtxDel',
```

### Comparing `tracex_parser-2.1.0/tracex_parser/file_parser.py` & `tracex_parser-2.2.0/tracex_parser/file_parser.py`

 * *Files identical despite different names*

### Comparing `tracex_parser-2.1.0/tracex_parser/helpers.py` & `tracex_parser-2.2.0/tracex_parser/helpers.py`

 * *Files identical despite different names*

### Comparing `tracex_parser-2.1.0/setup.py` & `tracex_parser-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['tracex_parser']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'tracex-parser',
-    'version': '2.1.0',
+    'version': '2.2.0',
     'description': "Parser for ThreadX RTOS's trace buffers (aka TraceX)",
     'long_description': "# TraceX Parser\n[![Documentation Status](https://readthedocs.org/projects/tracex_parser/badge/?version=latest)](https://tracex_parser.readthedocs.io/en/latest/?badge=latest)\n[![CircleCI](https://circleci.com/gh/julianneswinoga/tracex_parser.svg?style=shield)](https://circleci.com/gh/julianneswinoga/tracex_parser)\n[![Coverage Status](https://coveralls.io/repos/github/julianneswinoga/tracex_parser/badge.svg?branch=master)](https://coveralls.io/github/julianneswinoga/tracex_parser?branch=master)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tracex_parser)](https://pypi.org/project/tracex_parser/)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/tracex_parser)\n\nThis python package parses ThreadX trace buffers into both human and machine-readable formats.\nDon't know where to begin? Check out the [quick-start](https://tracex-parser.readthedocs.io/en/latest/quickstart.html) documentation.\nMore documentation about ThreadX trace buffers can be found [here](https://docs.microsoft.com/en-us/azure/rtos/tracex/chapter5).\n\n## Install\n`pip3 install tracex-parser`\n\n## Example trace buffers\nIn the repository source there are a couple example TraceX traces which can be used to verify that things are working correctly.\n### As a python module\n[documentation](https://tracex-parser.readthedocs.io/en/latest/py-interface.html)\n```pycon\n>>> from tracex_parser.file_parser import parse_tracex_buffer\n>>> events, obj_map = parse_tracex_buffer('./demo_threadx.trx')\n>>> events\n[4265846278:thread 7 threadResume(thread_ptr=thread 6,prev_state=0xd,stack_ptr=0x12980,next_thread=), 4265846441:thread 7 mtxPut(obj_id=mutex 0,owning_thread=0x6adc,own_cnt=0x1,stack_ptr=0x129a0), 4265846566:thread 7 mtxPut(obj_id=mutex 0,owning_thread=0x6adc,own_cnt=0x2,stack_ptr=0x129a0)]\n>>> obj_map[0xeea4]\n{'obj_reg_entry_obj_available **': '0x0', 'obj_reg_entry_obj_type **': '0x1', 'thread_reg_entry_obj_ptr': '0xeea4', 'obj_reg_entry_obj_parameter_1': '0xef4c', 'obj_reg_entry_obj_parameter_2': '0x3fc', 'thread_reg_entry_obj_name': b'System Timer Thread'}\n```\n\n### As a command line utility\n[documentation](https://tracex-parser.readthedocs.io/en/latest/cli-interface.html)\nThe `file_parser` module can also be run as a script, which will provide simple statistics on the trace as well as dumping all the events in the trace:\n```console\n$ python3 -m tracex_parser.file_parser -vvv ./demo_threadx.trx\nParsing ./demo_threadx.trx\ntotal events: 974\nobject registry size: 16\ndelta ticks: 156206\nEvent Histogram:\nqueueSend           493\nqueueReceive        428\nthreadResume        19\nthreadSuspend       16\nmtxPut              4\nisrExit             3\nisrEnter            3\nsemGet              2\nsemPut              2\nthreadSleep         2\nmtxGet              2\nAll events:\n4265846278:thread 7 threadResume(thread_ptr=thread 6,prev_state=0xd,stack_ptr=0x12980,next_thread=)\n4265846441:thread 7 mtxPut(obj_id=mutex 0,owning_thread=0x6adc,own_cnt=0x1,stack_ptr=0x129a0)\n4265846566:thread 7 mtxPut(obj_id=mutex 0,owning_thread=0x6adc,own_cnt=0x2,stack_ptr=0x129a0)\n4265846825:thread 4 threadSuspend(thread_ptr=thread 4,new_state=0x6,stack_ptr=0x11d70,next_thread=thread 7)\n4265846953:thread 4 semGet(obj_id=semaphore 0,timeout=WaitForever,cur_cnt=0x0,stack_ptr=0x11d98)\n...\n",
     'author': 'Julianne Swinoga',
     'author_email': 'julianneswinoga@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `tracex_parser-2.1.0/PKG-INFO` & `tracex_parser-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracex-parser
-Version: 2.1.0
+Version: 2.2.0
 Summary: Parser for ThreadX RTOS's trace buffers (aka TraceX)
 License: MIT
 Author: Julianne Swinoga
 Author-email: julianneswinoga@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

