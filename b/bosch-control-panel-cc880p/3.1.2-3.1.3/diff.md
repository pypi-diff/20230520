# Comparing `tmp/bosch-control-panel-cc880p-3.1.2.tar.gz` & `tmp/bosch-control-panel-cc880p-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bosch-control-panel-cc880p-3.1.2.tar", last modified: Sat May 20 15:46:23 2023, max compression
+gzip compressed data, was "bosch-control-panel-cc880p-3.1.3.tar", last modified: Sat May 20 17:17:14 2023, max compression
```

## Comparing `bosch-control-panel-cc880p-3.1.2.tar` & `bosch-control-panel-cc880p-3.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:46:23.563196 bosch-control-panel-cc880p-3.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-05-20 15:46:23.563196 bosch-control-panel-cc880p-3.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20428 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-20 15:46:23.563196 bosch-control-panel-cc880p-3.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:46:23.559196 bosch-control-panel-cc880p-3.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:46:23.555196 bosch-control-panel-cc880p-3.1.2/src/bosch/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:46:23.555196 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:46:23.559196 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:46:23.559196 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/cli/cmds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    18830 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/cp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:46:23.559196 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/models/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/models/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/models/cp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/models/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/models/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-20 15:46:11.000000 bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 15:46:23.563196 bosch-control-panel-cc880p-3.1.2/src/bosch_control_panel_cc880p.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-05-20 15:46:23.000000 bosch-control-panel-cc880p-3.1.2/src/bosch_control_panel_cc880p.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-20 15:46:23.000000 bosch-control-panel-cc880p-3.1.2/src/bosch_control_panel_cc880p.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 15:46:23.000000 bosch-control-panel-cc880p-3.1.2/src/bosch_control_panel_cc880p.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-20 15:46:23.000000 bosch-control-panel-cc880p-3.1.2/src/bosch_control_panel_cc880p.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-20 15:46:23.000000 bosch-control-panel-cc880p-3.1.2/src/bosch_control_panel_cc880p.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-20 15:46:23.000000 bosch-control-panel-cc880p-3.1.2/src/bosch_control_panel_cc880p.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:17:14.319379 bosch-control-panel-cc880p-3.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-05-20 17:17:14.319379 bosch-control-panel-cc880p-3.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20428 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-20 17:17:14.319379 bosch-control-panel-cc880p-3.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:17:14.311379 bosch-control-panel-cc880p-3.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:17:14.307378 bosch-control-panel-cc880p-3.1.3/src/bosch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:17:14.307378 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:17:14.311379 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:17:14.315379 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/cli/cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18937 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/cp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:17:14.315379 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/models/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/models/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/models/cp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/models/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/models/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:17:14.319379 bosch-control-panel-cc880p-3.1.3/src/bosch_control_panel_cc880p.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-05-20 17:17:14.000000 bosch-control-panel-cc880p-3.1.3/src/bosch_control_panel_cc880p.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-20 17:17:14.000000 bosch-control-panel-cc880p-3.1.3/src/bosch_control_panel_cc880p.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 17:17:14.000000 bosch-control-panel-cc880p-3.1.3/src/bosch_control_panel_cc880p.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-20 17:17:14.000000 bosch-control-panel-cc880p-3.1.3/src/bosch_control_panel_cc880p.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-20 17:17:14.000000 bosch-control-panel-cc880p-3.1.3/src/bosch_control_panel_cc880p.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-20 17:17:14.000000 bosch-control-panel-cc880p-3.1.3/src/bosch_control_panel_cc880p.egg-info/top_level.txt
```

### Comparing `bosch-control-panel-cc880p-3.1.2/LICENSE` & `bosch-control-panel-cc880p-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.2/PKG-INFO` & `bosch-control-panel-cc880p-3.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bosch-control-panel-cc880p
-Version: 3.1.2
+Version: 3.1.3
 Summary: Library to interface with the old CC880p Bosch COntrol Panels
 Home-page: https://github.com/hgomes88/bosch-control-panel-cc880p
 Author: Hugo Gomes
 Author-email: hgomes88@gmail.com
 Project-URL: Tracker, https://github.com/hgomes88/bosch-control-panel-cc880p/issues
 Project-URL: Download, https://pypi.org/project/bosch-control-panel-cc880p/
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bosch-control-panel-cc880p Version: 3.1.2 Summary:
+Metadata-Version: 2.1 Name: bosch-control-panel-cc880p Version: 3.1.3 Summary:
 Library to interface with the old CC880p Bosch COntrol Panels Home-page: https:
 //github.com/hgomes88/bosch-control-panel-cc880p Author: Hugo Gomes Author-
 email: hgomes88@gmail.com Project-URL: Tracker, https://github.com/hgomes88/
 bosch-control-panel-cc880p/issues Project-URL: Download, https://pypi.org/
 project/bosch-control-panel-cc880p/ Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
```

### Comparing `bosch-control-panel-cc880p-3.1.2/README.md` & `bosch-control-panel-cc880p-3.1.3/README.md`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.2/setup.cfg` & `bosch-control-panel-cc880p-3.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/cli/cli.py` & `bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/cli/cli.py`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/cli/cmds.py` & `bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/cli/cmds.py`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/cli/parser.py` & `bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/cli/parser.py`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/cp.py` & `bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/cp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Control Panel."""
 import asyncio
 import dataclasses
 import datetime
 import logging
 from asyncio import AbstractEventLoop
 from asyncio import Task
+from asyncio.exceptions import CancelledError
 from enum import Enum
 from typing import List
 from typing import Optional
 from typing import Type
 from typing import Union
 
 from bosch.control_panel.cc880p.models.callbacks import ControlPanelListener
@@ -207,22 +208,22 @@
         """Send a new request."""
         n_resp_bytes = resp_type.size if resp_type else 1
         resp = await self.send_command(
             message=request.encode(),
             n_resp_bytes=n_resp_bytes,
             timeout=3
         )
-        if resp:
-            if resp_type:
-                if len(resp) != resp_type.size:
-                    raise ValueError(
-                        f'The size of the frame should be {resp_type.size}'
-                        f' but is {len(resp)}'
-                    )
-            self._handle_data(resp)
+        if resp_type:
+            size_resp = len(resp) if resp else 0
+            if size_resp != resp_type.size:
+                raise ValueError(
+                    f'The size of the frame should be {resp_type.size}'
+                    f' but is {size_resp}'
+                )
+        self._handle_data(resp)
 
     async def send_command(
         self,
         message: bytes,
         n_resp_bytes=0,
         timeout=3
     ) -> Optional[bytes]:
@@ -529,11 +530,13 @@
 
     async def _connection_task(self):
         while True:
             try:
                 if not self.connected:
                     _LOGGER.info('Connecting')
                     await self._connect()
+            except CancelledError:
+                break
             except BaseException:
                 _LOGGER.error('Connection failed')
             finally:
                 await asyncio.sleep(3)
```

### Comparing `bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/models/cp.py` & `bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/models/cp.py`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/models/requests.py` & `bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/models/requests.py`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/models/responses.py` & `bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/models/responses.py`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.2/src/bosch/control_panel/cc880p/utils.py` & `bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/utils.py`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.2/src/bosch_control_panel_cc880p.egg-info/PKG-INFO` & `bosch-control-panel-cc880p-3.1.3/src/bosch_control_panel_cc880p.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bosch-control-panel-cc880p
-Version: 3.1.2
+Version: 3.1.3
 Summary: Library to interface with the old CC880p Bosch COntrol Panels
 Home-page: https://github.com/hgomes88/bosch-control-panel-cc880p
 Author: Hugo Gomes
 Author-email: hgomes88@gmail.com
 Project-URL: Tracker, https://github.com/hgomes88/bosch-control-panel-cc880p/issues
 Project-URL: Download, https://pypi.org/project/bosch-control-panel-cc880p/
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bosch-control-panel-cc880p Version: 3.1.2 Summary:
+Metadata-Version: 2.1 Name: bosch-control-panel-cc880p Version: 3.1.3 Summary:
 Library to interface with the old CC880p Bosch COntrol Panels Home-page: https:
 //github.com/hgomes88/bosch-control-panel-cc880p Author: Hugo Gomes Author-
 email: hgomes88@gmail.com Project-URL: Tracker, https://github.com/hgomes88/
 bosch-control-panel-cc880p/issues Project-URL: Download, https://pypi.org/
 project/bosch-control-panel-cc880p/ Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
```

### Comparing `bosch-control-panel-cc880p-3.1.2/src/bosch_control_panel_cc880p.egg-info/SOURCES.txt` & `bosch-control-panel-cc880p-3.1.3/src/bosch_control_panel_cc880p.egg-info/SOURCES.txt`

 * *Files identical despite different names*

