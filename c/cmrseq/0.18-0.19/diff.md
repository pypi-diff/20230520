# Comparing `tmp/cmrseq-0.18.tar.gz` & `tmp/cmrseq-0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmrseq-0.18.tar", last modified: Fri Mar 24 17:47:46 2023, max compression
+gzip compressed data, was "cmrseq-0.19.tar", last modified: Sat May 20 15:03:23 2023, max compression
```

## Comparing `cmrseq-0.18.tar` & `cmrseq-0.19.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 17:47:46.772192 cmrseq-0.18/
--rw-rw-rw-   0 root         (0) root         (0)    35076 2023-03-24 12:13:18.000000 cmrseq-0.18/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3033 2023-03-24 17:47:46.772192 cmrseq-0.18/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2541 2023-03-22 12:30:34.000000 cmrseq-0.18/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 17:47:46.764233 cmrseq-0.18/cmrseq/
--rw-rw-rw-   0 root         (0) root         (0)      454 2023-03-24 17:47:46.000000 cmrseq-0.18/cmrseq/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 17:47:46.764233 cmrseq-0.18/cmrseq/contrib/
--rw-rw-rw-   0 root         (0) root         (0)      115 2023-03-22 12:30:34.000000 cmrseq-0.18/cmrseq/contrib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10174 2023-03-22 12:30:34.000000 cmrseq-0.18/cmrseq/contrib/sequences.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 17:47:46.764233 cmrseq-0.18/cmrseq/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-24 17:47:35.000000 cmrseq-0.18/cmrseq/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    26566 2023-03-24 16:07:12.000000 cmrseq-0.18/cmrseq/core/_sequence.py
--rw-rw-rw-   0 root         (0) root         (0)     6080 2023-03-22 12:30:34.000000 cmrseq-0.18/cmrseq/core/_system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 17:47:46.768213 cmrseq-0.18/cmrseq/core/bausteine/
--rw-rw-rw-   0 root         (0) root         (0)      651 2023-03-22 12:30:34.000000 cmrseq-0.18/cmrseq/core/bausteine/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6728 2023-03-22 12:30:34.000000 cmrseq-0.18/cmrseq/core/bausteine/_adc.py
--rw-rw-rw-   0 root         (0) root         (0)    10380 2023-03-24 12:13:18.000000 cmrseq-0.18/cmrseq/core/bausteine/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1063 2023-03-22 12:30:34.000000 cmrseq-0.18/cmrseq/core/bausteine/_delay.py
--rw-rw-rw-   0 root         (0) root         (0)    19687 2023-03-24 12:07:22.000000 cmrseq-0.18/cmrseq/core/bausteine/_gradients.py
--rw-rw-rw-   0 root         (0) root         (0)     8276 2023-03-22 12:30:34.000000 cmrseq-0.18/cmrseq/core/bausteine/_rf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 17:47:46.768213 cmrseq-0.18/cmrseq/io/
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-03-22 12:30:34.000000 cmrseq-0.18/cmrseq/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6074 2023-03-22 12:30:34.000000 cmrseq-0.18/cmrseq/io/_json.py
--rw-rw-rw-   0 root         (0) root         (0)    25157 2023-03-24 12:07:22.000000 cmrseq-0.18/cmrseq/io/_phillips_load.py
--rw-rw-rw-   0 root         (0) root         (0)    53567 2023-03-22 12:30:34.000000 cmrseq-0.18/cmrseq/io/_pulseq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 17:47:46.768213 cmrseq-0.18/cmrseq/parametric_definitions/
--rw-rw-rw-   0 root         (0) root         (0)      466 2023-03-22 12:30:34.000000 cmrseq-0.18/cmrseq/parametric_definitions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13588 2023-03-24 16:07:12.000000 cmrseq-0.18/cmrseq/parametric_definitions/diffusion.py
--rw-rw-rw-   0 root         (0) root         (0)     7685 2023-03-22 12:30:34.000000 cmrseq-0.18/cmrseq/parametric_definitions/excitation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 17:47:46.772192 cmrseq-0.18/cmrseq/parametric_definitions/readout/
--rw-rw-rw-   0 root         (0) root         (0)      648 2023-03-22 12:30:34.000000 cmrseq-0.18/cmrseq/parametric_definitions/readout/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16753 2023-03-22 12:30:34.000000 cmrseq-0.18/cmrseq/parametric_definitions/readout/_cartesian_single_lines.py
--rw-rw-rw-   0 root         (0) root         (0)    11880 2023-03-22 12:30:34.000000 cmrseq-0.18/cmrseq/parametric_definitions/readout/_epi.py
--rw-rw-rw-   0 root         (0) root         (0)     3511 2023-03-24 12:13:18.000000 cmrseq-0.18/cmrseq/parametric_definitions/readout/_radial.py
--rw-rw-rw-   0 root         (0) root         (0)    10626 2023-03-22 12:30:34.000000 cmrseq-0.18/cmrseq/parametric_definitions/readout/_spiral.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 17:47:46.772192 cmrseq-0.18/cmrseq/parametric_definitions/sequences/
--rw-rw-rw-   0 root         (0) root         (0)      485 2023-03-22 12:30:34.000000 cmrseq-0.18/cmrseq/parametric_definitions/sequences/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13141 2023-03-24 12:13:18.000000 cmrseq-0.18/cmrseq/parametric_definitions/sequences/_gradient_echo.py
--rw-rw-rw-   0 root         (0) root         (0)     7787 2023-03-22 12:30:34.000000 cmrseq-0.18/cmrseq/parametric_definitions/sequences/_spin_echo.py
--rw-rw-rw-   0 root         (0) root         (0)    18401 2023-03-24 12:13:18.000000 cmrseq-0.18/cmrseq/parametric_definitions/sequences/_ssfp.py
--rw-rw-rw-   0 root         (0) root         (0)    27016 2023-03-24 16:07:12.000000 cmrseq-0.18/cmrseq/parametric_definitions/velocity.py
--rw-rw-rw-   0 root         (0) root         (0)    15930 2023-03-22 12:30:34.000000 cmrseq-0.18/cmrseq/plotting.py
--rw-rw-rw-   0 root         (0) root         (0)    11966 2023-03-22 12:30:34.000000 cmrseq-0.18/cmrseq/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 17:47:46.764233 cmrseq-0.18/cmrseq.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3033 2023-03-24 17:47:46.000000 cmrseq-0.18/cmrseq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1282 2023-03-24 17:47:46.000000 cmrseq-0.18/cmrseq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-24 17:47:46.000000 cmrseq-0.18/cmrseq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-03-24 17:47:46.000000 cmrseq-0.18/cmrseq.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-03-24 17:47:46.000000 cmrseq-0.18/cmrseq.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-24 17:47:46.772192 cmrseq-0.18/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1635 2023-03-22 12:30:35.000000 cmrseq-0.18/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 15:03:23.528070 cmrseq-0.19/
+-rw-rw-rw-   0 root         (0) root         (0)    35076 2023-04-12 07:05:08.000000 cmrseq-0.19/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3033 2023-05-20 15:03:23.528070 cmrseq-0.19/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2541 2023-04-12 07:05:08.000000 cmrseq-0.19/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 15:03:23.508062 cmrseq-0.19/cmrseq/
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-05-20 15:03:23.000000 cmrseq-0.19/cmrseq/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 15:03:23.512063 cmrseq-0.19/cmrseq/contrib/
+-rw-rw-rw-   0 root         (0) root         (0)      115 2023-04-12 07:05:08.000000 cmrseq-0.19/cmrseq/contrib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10174 2023-04-12 07:05:08.000000 cmrseq-0.19/cmrseq/contrib/sequences.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 15:03:23.512063 cmrseq-0.19/cmrseq/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-20 15:03:04.000000 cmrseq-0.19/cmrseq/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    31132 2023-05-20 14:01:47.000000 cmrseq-0.19/cmrseq/core/_sequence.py
+-rw-rw-rw-   0 root         (0) root         (0)     6328 2023-04-12 16:23:47.000000 cmrseq-0.19/cmrseq/core/_system.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 15:03:23.516065 cmrseq-0.19/cmrseq/core/bausteine/
+-rw-rw-rw-   0 root         (0) root         (0)      678 2023-04-12 11:43:49.000000 cmrseq-0.19/cmrseq/core/bausteine/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6728 2023-04-12 07:05:08.000000 cmrseq-0.19/cmrseq/core/bausteine/_adc.py
+-rw-rw-rw-   0 root         (0) root         (0)    10380 2023-04-12 07:05:08.000000 cmrseq-0.19/cmrseq/core/bausteine/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2023-04-12 07:05:08.000000 cmrseq-0.19/cmrseq/core/bausteine/_delay.py
+-rw-rw-rw-   0 root         (0) root         (0)    19958 2023-05-20 14:45:45.000000 cmrseq-0.19/cmrseq/core/bausteine/_gradients.py
+-rw-rw-rw-   0 root         (0) root         (0)    14389 2023-04-13 09:15:52.000000 cmrseq-0.19/cmrseq/core/bausteine/_rf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 15:03:23.520066 cmrseq-0.19/cmrseq/io/
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-12 07:05:08.000000 cmrseq-0.19/cmrseq/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6074 2023-04-12 07:05:08.000000 cmrseq-0.19/cmrseq/io/_json.py
+-rw-rw-rw-   0 root         (0) root         (0)    25750 2023-05-20 14:45:45.000000 cmrseq-0.19/cmrseq/io/_phillips_load.py
+-rw-rw-rw-   0 root         (0) root         (0)    53656 2023-05-20 14:39:53.000000 cmrseq-0.19/cmrseq/io/_pulseq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 15:03:23.520066 cmrseq-0.19/cmrseq/parametric_definitions/
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-04-12 07:05:08.000000 cmrseq-0.19/cmrseq/parametric_definitions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13840 2023-04-15 09:54:10.000000 cmrseq-0.19/cmrseq/parametric_definitions/diffusion.py
+-rw-rw-rw-   0 root         (0) root         (0)    14607 2023-05-20 14:45:45.000000 cmrseq-0.19/cmrseq/parametric_definitions/excitation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 15:03:23.524068 cmrseq-0.19/cmrseq/parametric_definitions/readout/
+-rw-rw-rw-   0 root         (0) root         (0)      648 2023-04-12 07:05:08.000000 cmrseq-0.19/cmrseq/parametric_definitions/readout/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16753 2023-04-12 07:05:08.000000 cmrseq-0.19/cmrseq/parametric_definitions/readout/_cartesian_single_lines.py
+-rw-rw-rw-   0 root         (0) root         (0)    23860 2023-05-20 14:45:45.000000 cmrseq-0.19/cmrseq/parametric_definitions/readout/_epi.py
+-rw-rw-rw-   0 root         (0) root         (0)     8143 2023-04-12 07:06:42.000000 cmrseq-0.19/cmrseq/parametric_definitions/readout/_radial.py
+-rw-rw-rw-   0 root         (0) root         (0)    10626 2023-04-12 07:05:08.000000 cmrseq-0.19/cmrseq/parametric_definitions/readout/_spiral.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 15:03:23.524068 cmrseq-0.19/cmrseq/parametric_definitions/sequences/
+-rw-rw-rw-   0 root         (0) root         (0)      485 2023-04-12 07:05:08.000000 cmrseq-0.19/cmrseq/parametric_definitions/sequences/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13141 2023-04-12 07:05:08.000000 cmrseq-0.19/cmrseq/parametric_definitions/sequences/_gradient_echo.py
+-rw-rw-rw-   0 root         (0) root         (0)     8209 2023-05-20 14:45:45.000000 cmrseq-0.19/cmrseq/parametric_definitions/sequences/_spin_echo.py
+-rw-rw-rw-   0 root         (0) root         (0)    18605 2023-04-13 15:56:56.000000 cmrseq-0.19/cmrseq/parametric_definitions/sequences/_ssfp.py
+-rw-rw-rw-   0 root         (0) root         (0)    27016 2023-04-12 07:05:08.000000 cmrseq-0.19/cmrseq/parametric_definitions/velocity.py
+-rw-rw-rw-   0 root         (0) root         (0)    16067 2023-04-12 16:23:47.000000 cmrseq-0.19/cmrseq/plotting.py
+-rw-rw-rw-   0 root         (0) root         (0)    11966 2023-04-12 07:05:08.000000 cmrseq-0.19/cmrseq/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 15:03:23.512063 cmrseq-0.19/cmrseq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3033 2023-05-20 15:03:23.000000 cmrseq-0.19/cmrseq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-05-20 15:03:23.000000 cmrseq-0.19/cmrseq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-20 15:03:23.000000 cmrseq-0.19/cmrseq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-05-20 15:03:23.000000 cmrseq-0.19/cmrseq.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-20 15:03:23.000000 cmrseq-0.19/cmrseq.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-20 15:03:23.528070 cmrseq-0.19/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1635 2023-04-12 07:05:08.000000 cmrseq-0.19/setup.py
```

### Comparing `cmrseq-0.18/LICENSE` & `cmrseq-0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `cmrseq-0.18/PKG-INFO` & `cmrseq-0.19/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmrseq
-Version: 0.18
+Version: 0.19
 Summary: UNKNOWN
 Home-page: https://gitlab.ethz.ch/jweine/cmrseq
 Author: Jonathan Weine, Charles McGrath
 Author-email: weine@biomed.ee.ethz.ch, mcgrath@biomed.ee.ethz.ch
 License: UNKNOWN
 Project-URL: Documentation, https://people.ee.ethz.ch/~jweine/cmrseq/latest/index.html
 Project-URL: Source, https://gitlab.ethz.ch/jweine/cmrseq
```

### Comparing `cmrseq-0.18/README.rst` & `cmrseq-0.19/README.rst`

 * *Files identical despite different names*

### Comparing `cmrseq-0.18/cmrseq/contrib/sequences.py` & `cmrseq-0.19/cmrseq/contrib/sequences.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.18/cmrseq/core/_sequence.py` & `cmrseq-0.19/cmrseq/core/_sequence.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """ This Module contains the implementation of the core functionality Sequence"""
 __all__ = ["Sequence"]
 
 from copy import deepcopy
 from typing import List, Union, Iterable, Tuple
 from warnings import warn
+import re
 
 import numpy as np
 from pint import Quantity
 from tqdm import tqdm
 
 from cmrseq.core.bausteine._base import SequenceBaseBlock
 from cmrseq.core.bausteine._adc import ADC
@@ -48,21 +49,64 @@
         """ """
         self._check_sys_compatibility(other._system_specs)
         for b in other._blocks:
             self._add_unique_block_name(b)
             self._blocks.append(b)
         return self
 
+    def __getitem__(self, item: Union[str, int, slice, tuple]):
+        """ Possible ways to index/query blocks in a sequence:
+
+        .. code::
+
+            seq[0], seq[0:4], seq[(0, 4, 1)] -> returns block by index assuming ordering
+                        according to start time
+
+            seq["trapezoidal_0"] -> returns block by name
+
+
+
+        :param item:
+        :return:
+        """
+        if isinstance(item, str):
+            return self._block_lookup[item]
+        elif isinstance(item, int):
+            names_and_times = self._create_sorted_block_list(reversed=False)
+            return self._block_lookup[names_and_times[item][0]]
+        elif isinstance(item, slice):
+            names_and_times = self._create_sorted_block_list(reversed=False)
+            return [self._block_lookup[k] for k, _ in names_and_times[item]]
+        elif isinstance(item, tuple):
+            if not all([isinstance(i, int) for i in item]):
+                raise NotImplementedError("When indexing with a tuple, all tuple entries must"
+                                          f" be of type int. But got {item}!")
+            names_and_times = self._create_sorted_block_list(reversed=False)
+            return [self._block_lookup[names_and_times[i][0]] for i in item]
+        else:
+            raise NotImplementedError(f"{type(item)} is not in the list of possible block"
+                                      f" queries [str, int, slice, Tuple[int]]")
+
+    def __iter__(self):
+        """Returns an iterator yielding blocks sorted by theirs start time"""
+        start_times = self._create_sorted_block_list(reversed=False)
+        return (self._block_lookup[k] for (k, _) in start_times)
+
     def _check_sys_compatibility(self, system_specs: SystemSpec):
         equalities = [self._system_specs.__dict__[k] == system_specs.__dict__[k]
                       for k in self._system_specs.__dict__.keys()]
         if not all(equalities):
             raise ValueError("System specifications of added sequence do not match. Addition "
                              "for different system specifications is not implemented")
 
+    def _create_sorted_block_list(self, reversed: bool = False):
+        start_times = [(k, b.tmin) for k, b in self._block_lookup.items()]
+        start_times.sort(key=lambda x: float(x[1].m_as("ms")), reverse=reversed)
+        return start_times
+
     def add_block(self, block: SequenceBaseBlock, copy: bool = True) -> None:
         """ Add the instance of block to the internal List of sequence blocks.
 
         **Note**: The internal definiton of blocks is mutuable, therefore if the new block is not
         copied, subsequent alterations can have unwanted side-effects inside the sequence.
 
         :raises ValueError: If block.validate() fails to validate using the system specs of self
@@ -81,32 +125,77 @@
             raise ValueError("New block does not validate against sequence system specifications."
                              f"Resulting in following ValueError: {err}") from err
         if copy:
             block = deepcopy(block)
         self._blocks.append(block)
         self._add_unique_block_name(block)
 
+    def rename_blocks(self, old_names: List[str], new_names: List[str]):
+        """ Renames blocks and updates block lookup map"""
+        for old, new in zip(old_names, new_names):
+            bl = self._block_lookup[old]
+            bl.name = new
+        self._block_lookup = {}
+        for block in self._blocks:
+            self._add_unique_block_name(block)
+
     def remove_block(self, block_name: str):
         """ Removes block from internal lookup """
         block = self.get_block(block_name)
         if block is None:
             raise ValueError(f"Tried to remove non-existing block; \n "
                              f"'{block_name}' not in {self.blocks}")
         block_index = [block is b for b in self._blocks].index(True)
         del self._blocks[block_index]
         del self._block_lookup[block_name]
 
-    def get_block(self, block_name: str) -> Union[SequenceBaseBlock]:
+    def get_block(self, block_name: Union[str, Iterable[str]] = None,
+                  partial_string_match: Union[str, Iterable[str]] = None,
+                  regular_expression: Union[str, Iterable[str]] = None) \
+                  -> Union[SequenceBaseBlock, List[SequenceBaseBlock]]:
         """ Returns reference to the block whose member `name` matches the specified argument.
         If no block with given name is present in the sequence, it returns None
 
-        :param block_name: Name of the block
-        :return: SequenceBaseBlock or None
+        .. note::
+
+            Checks which keyword argument to use from left to right as specified in the signature.
+            If multiple are specified uses only the first one.
+
+        :raises: ValueError if no keyword-argument is specified
+
+        :param block_name: String or iterable of strings exactly matching a set of blocks contained
+                            in the sequence
+        :param partial_string_match: str or iterable of strings that specify partial string matches.
+                            All blocks partially matching at least one are returned.
+        :param regular_expression: str or iterable of strings containing regular expressions that
+                            are matched against the block-names. All blocks, matching at least one
+                            of the given expressions are returned.
+        :return: SequenceBaseBlock or List of SequenceBaseBlocks depending on the specified argument
         """
-        return self._block_lookup.get(block_name, None)
+        if block_name is not None:
+            if isinstance(block_name, str):
+                return self._block_lookup.get(block_name, None)
+            else:
+                return [self._block_lookup[bn] for bn in block_name]
+        elif partial_string_match is not None:
+            if isinstance(partial_string_match, str):
+                partial_string_match = [partial_string_match, ]
+            partial_string_match = "|".join([f"(?:.*{p}.*)" for p in partial_string_match])
+            matched_block_names = [block for name, block in self._block_lookup.items()
+                                   if re.match(partial_string_match, name)]
+            return matched_block_names
+        elif regular_expression is not None:
+            if isinstance(regular_expression, str):
+                regular_expression = [regular_expression,]
+            regular_expression = "|".join([f"(?:{p})" for p in regular_expression])
+            matched_block_names = [block for name, block in self._block_lookup.items()
+                                   if re.match(regular_expression, name)]
+            return matched_block_names
+        else:
+            raise ValueError("At least one on the keyword arguments must be specified")
 
     def append(self, other: Union['Sequence', SequenceBaseBlock],
                copy: bool = True, end_time: Quantity = None) -> None:
         """If both system specifications match, copies all blocks from `other` shifts them by own
         tmax and adds the blocks to own collection
 
         :raises ValueError: If other fails to validate using the system specs of self
```

### Comparing `cmrseq-0.18/cmrseq/core/_system.py` & `cmrseq-0.19/cmrseq/core/_system.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,19 +11,21 @@
 # pylint: disable=R0902, R0913, C0103
 class SystemSpec():
     """ Specifications of MR-System limits. """
     #: Quantity[mT/m]: Maximum gradient amplitude
     max_grad: Quantity
     #: Quantity[mT/m/ms]: Maximum gradient slew rate
     max_slew: Quantity
-    #: Quantity[ms]: delta t of radio-frequency grid
+    #: Quantity[uT]: Peak power for B1 fields (in micro tesla)
+    rf_peak_power: Quantity
+    #: Quantity[ms]: Not in use yet...
     rf_dead_time: Quantity
-    #: ...
+    #: Quantity[ms]: Not in use yet...
     rf_ringdown_time: Quantity
-    #: ...
+    #: Quantity[ms]: Not in use yet...
     adc_dead_time: Quantity
     #: Quantity[ms]: delta t of radio-frequency grid, defaults to 10us
     rf_raster_time: Quantity
     #: Quantity[ms]: delta t of gradient grid, defaults to 10us
     grad_raster_time: Quantity
     #: Quantity[ms]: delta t of adc grid, defaults to 10us
     adc_raster_time: Quantity
@@ -35,27 +37,29 @@
     # if False
 
     def __init__(self,
                  gamma: Quantity = Quantity(42.576, "MHz/T"),
                  grad_raster_time: Quantity = Quantity(1e-2, "ms"),
                  max_grad: Quantity = Quantity(40, "mT/m"),
                  max_slew: Quantity = Quantity(120, "mT/m/ms"),
+                 rf_peak_power: Quantity = Quantity(20, "uT"),
                  rf_raster_time: Quantity = Quantity(1e-2, "ms"),
                  rf_dead_time: Quantity = Quantity(0., "ms"),
                  rf_ringdown_time: Quantity = Quantity(1e-3, "ms"),
                  adc_raster_time: Quantity = Quantity(1e-2, "ms"),
                  adc_dead_time: Quantity = Quantity(0., "ms"),
                  b0: Quantity = Quantity(1.5, "T")):
 
         if max_grad.to_base_units().units == Quantity(1., "1/m/s").units:
             max_grad = (max_grad * gamma).to("mT/m")
 
         if max_slew.to_base_units().units == Quantity(1., "1/m/s**2").units:
             max_slew = (max_slew * gamma).to("mT/m/ms")
 
+        self.rf_peak_power = rf_peak_power.to("uT")
         self.rf_dead_time = rf_dead_time.to("ms")
         self.rf_ringdown_time = rf_ringdown_time.to("ms")
         self.adc_dead_time = adc_dead_time.to("ms")
         self.rf_raster_time = rf_raster_time.to("ms")
         self.grad_raster_time = grad_raster_time.to("ms")
         self.adc_raster_time = adc_raster_time.to("ms")
         self.gamma = gamma.to("MHz/T")
```

### Comparing `cmrseq-0.18/cmrseq/core/bausteine/__init__.py` & `cmrseq-0.19/cmrseq/core/bausteine/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ Module containing all atoms/building blocks of the definable MRI sequences"""
 __all__ = ["TrapezoidalGradient", "ArbitraryGradient", "Gradient",
-           "SincRFPulse", "ArbitraryRFPulse", "RFPulse",
+           "SincRFPulse", "HardRFPulse", "ArbitraryRFPulse", "RFPulse",
            "SymmetricADC", "GridSamplingADC", "ADC",
            "Delay", "SequenceBaseBlock"]
 
 from cmrseq.core.bausteine._gradients import Gradient, TrapezoidalGradient, ArbitraryGradient
-from cmrseq.core.bausteine._rf import RFPulse, SincRFPulse, ArbitraryRFPulse
+from cmrseq.core.bausteine._rf import RFPulse, SincRFPulse,HardRFPulse, ArbitraryRFPulse
 from cmrseq.core.bausteine._adc import ADC, SymmetricADC, GridSamplingADC
 from cmrseq.core.bausteine._delay import Delay
 from cmrseq.core.bausteine._base import SequenceBaseBlock
```

### Comparing `cmrseq-0.18/cmrseq/core/bausteine/_adc.py` & `cmrseq-0.19/cmrseq/core/bausteine/_adc.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.18/cmrseq/core/bausteine/_base.py` & `cmrseq-0.19/cmrseq/core/bausteine/_base.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.18/cmrseq/core/bausteine/_delay.py` & `cmrseq-0.19/cmrseq/core/bausteine/_delay.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.18/cmrseq/core/bausteine/_gradients.py` & `cmrseq-0.19/cmrseq/core/bausteine/_gradients.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,19 +238,21 @@
         duration_raster = system_specs.time_to_raster(duration)
         if not np.isclose(duration.m_as("ms") - duration_raster.m_as("ms"), 0., rtol=1e-6):
             raise ValueError(f"Specified duration not on raster: {duration.m_as('ms'):1.6f}/"
                              f"{system_specs.grad_raster_time.m_as('ms'):1.6f} is not an integer")
 
         p_half = duration_raster / 2.
         q = area / (system_specs.max_grad / system_specs.minmax_risetime)  # pylint: disable=C0103
-        rise_time = np.abs(p_half - np.sqrt(p_half ** 2 - q))
+        radicant = (p_half ** 2 - q).to("ms**2")
+        if np.isclose(radicant.m, 0., atol=1e-5):
+            radicant = Quantity(0, "ms**2")
+        rise_time = np.abs(p_half - np.sqrt(radicant))
         rise_time = system_specs.time_to_raster(rise_time, raster="grad")
         flat_duration = duration - 2 * rise_time
         amplitude = area / (duration - rise_time)
-
         return TrapezoidalGradient(system_specs=system_specs, orientation=orientation,
                                    amplitude=amplitude.to("mT/m"),
                                    flat_duration=flat_duration.to("ms"),
                                    rise_time=rise_time.to("ms"), delay=delay, name=name)
 
     @classmethod
     # pylint: disable=W1401
@@ -281,15 +283,18 @@
         duration_raster = system_specs.time_to_raster(flat_duration, raster="grad")
         if not np.isclose(flat_duration.m_as("ms") - duration_raster.m_as("ms"), 0., rtol=1e-6):
             raise ValueError(f"Specified duration not on raster: {flat_duration.m_as('ms'):1.6f}/"
                              f"{system_specs.grad_raster_time.m_as('ms'):1.6f} is not an integer")
 
         p_half = flat_duration / 2.
         q = - area / (system_specs.max_grad / system_specs.minmax_risetime)  # pylint: disable=C0103
-        rise_time = - p_half + np.sqrt(p_half ** 2 - q)
+        radicant = (p_half ** 2 - q).to("ms**2")
+        if np.isclose(radicant.m, 0., atol=1e-5):
+            radicant = Quantity(0, "ms**2")
+        rise_time = - p_half + np.sqrt(radicant)
         rise_time = system_specs.time_to_raster(rise_time, raster="grad")
         amplitude = area / (flat_duration + rise_time)
         return TrapezoidalGradient(system_specs=system_specs, orientation=orientation,
                                    amplitude=amplitude.to("mT/m"),
                                    flat_duration=flat_duration.to("ms"),
                                    rise_time=rise_time.to("ms"), delay=delay, name=name)
```

### Comparing `cmrseq-0.18/cmrseq/io/_json.py` & `cmrseq-0.19/cmrseq/io/_json.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.18/cmrseq/io/_phillips_load.py` & `cmrseq-0.19/cmrseq/io/_phillips_load.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,45 +30,43 @@
     _sq_object_sizes: List[dict]
 
     def __init__(self, filename: str):
         assert os.path.exists(filename)
 
         # self.rf_amps, self.rf_fm, self.sequence_objects, self.grad_waveforms = [], [], [], []
         self.filename = filename
-        _file_handle = open(self.filename, "rb")
+        with open(self.filename, "rb") as _file_handle:
+            id_version = np.fromfile(_file_handle, np.int32, 1)
 
-        id_version = np.fromfile(_file_handle, np.int32, 1)
+            # Read raw waveform samples
+            n_gradient_blocks = int(np.fromfile(_file_handle, np.int32, 1))
+            self.grad_waveforms = [self.read_waveform(_file_handle) for _ in range(n_gradient_blocks)]
+
+            n_rf_blocks = int(np.fromfile(_file_handle, np.int32, 1))
+            self.rf_amps = [self.read_waveform(_file_handle) for _ in range(n_rf_blocks)]
+
+            n_rf_blocks = int(np.fromfile(_file_handle, np.int32, 1))
+            self.rf_fm = [self.read_waveform(_file_handle) for _ in range(n_rf_blocks)]
+
+            # Read sequence objects
+            n_sequence_objects = int(np.fromfile(_file_handle, np.int32, 1))
+            self.sequence_objects = [self.parse_sequence_objects(_file_handle) for _ in
+                                    tqdm(range(n_sequence_objects),
+                                        desc="Reading sequence objects ...")]
 
-        # Read raw waveform samples
-        n_gradient_blocks = int(np.fromfile(_file_handle, np.int32, 1))
-        self.grad_waveforms = [self.read_waveform(_file_handle) for _ in range(n_gradient_blocks)]
-
-        n_rf_blocks = int(np.fromfile(_file_handle, np.int32, 1))
-        self.rf_amps = [self.read_waveform(_file_handle) for _ in range(n_rf_blocks)]
-
-        n_rf_blocks = int(np.fromfile(_file_handle, np.int32, 1))
-        self.rf_fm = [self.read_waveform(_file_handle) for _ in range(n_rf_blocks)]
-
-        # Read sequence objects
-        n_sequence_objects = int(np.fromfile(_file_handle, np.int32, 1))
-        self.sequence_objects = [self.parse_sequence_objects(_file_handle) for _ in
-                                 tqdm(range(n_sequence_objects),
-                                      desc="Reading sequence objects ...")]
-
-        for sq_id in range(n_sequence_objects):
-            self.sequence_objects[sq_id]["id"] = sq_id
-
-        try:
-            self._read_gveex(file=_file_handle)
-        except Exception as e:
-            import traceback
-            warn(f"Encountered error in parsing information after actual waveforms. This could mean "
-                 f"the GVE file is corrupted. Raised Exception:")
-            traceback.print_exc()
-        _file_handle.close()
+            for sq_id in range(n_sequence_objects):
+                self.sequence_objects[sq_id]["id"] = sq_id
+
+            try:
+                self._read_gveex(file=_file_handle)
+            except Exception as e:
+                import traceback
+                warn(f"Encountered error in parsing information after actual waveforms. This could mean "
+                    f"the GVE file is corrupted. Raised Exception:")
+                traceback.print_exc()
 
     @staticmethod
     def read_waveform(file):
         """ Extracts the id, size and number of samples from the given file assuming the
         byte pointer is at the location of the waveform"""
         waveform = {}
         waveform["id"] = int(np.fromfile(file, np.int32, 1))
@@ -179,24 +177,30 @@
         if s["fm_id"] != -1:
             s["fm_waveform"] = self.find_waveform(self.rf_fm, s["fm_waveform"])
         return s
 
     @staticmethod
     def read_aq(file):
         name = "".join([chr(c) for c in np.fromfile(file, np.int8, 32)])
-        mem_block_names = ["name", "start", "dur", "ref", "rep", "interval", "samples", "nucleus"]
+        mem_block_names = ["start", "dur", "ref", "rep", "interval", "samples", "nucleus"]
         mem_block_dtypes = ["f4", "f4","f4", "i4", "f4", "i4", "i4"]
         mem_dt = [(n, d) for n, d in zip(mem_block_names, mem_block_dtypes)]
         temp = np.fromfile(file, mem_dt, 1)[0]
         s = {n:v for n, v in zip(mem_block_names, temp)}
-        s["name"] = name
+        s["name"] = name.strip()
         return s
 
     def _read_gveex(self, file):
-        version = int(np.fromfile(file, np.int32, 1))
+        version = np.fromfile(file, np.int32, 1)
+        
+        # If file is exhausted no extensions were appended
+        if version.size == 0:
+            return 
+        version = int(version)
+
         self.version = 'legacy'
         if not (1 <= version < self._VERSION_ALL):
             warn("GVE Extension not found. Skipping. \n")
             return
 
         for n in range(len(self._VERSION_HR)):
             # Version is stored as binary mask for the 5  version_hr entries
@@ -395,14 +399,15 @@
         g_list = self._make_gradients(seq_obj, rotate_to_xyz)
 
         # Process RF events
         rf_list = [self._make_rf_block(rf_dict=rf) for rf in seq_obj["rf"]]
 
         # Process AQ events
         aq_list = [self._make_aq_block(aq_dict=aq) for aq in seq_obj["aq"] if aq.get("samples", 0) > 0]
+        aq_list = [b for l in aq_list for b in l]
 
         # TODO: Translate seq_obj ref time to delay.
         return g_list + rf_list + aq_list
 
     def _make_gradients(self, sequence_obj, rotate_to_xyz: bool):
         sequence_blocks = []
         for direction, gradients in zip(np.eye(3, 3), sequence_obj["gradients"]):
@@ -523,14 +528,20 @@
         rf_block = cmrseq.bausteine.ArbitraryRFPulse(system_specs=self.system_specs,
                                                      time_points=t,
                                                      waveform=wf,
                                                      name=rf_dict["name"].strip(),
                                                      snap_to_raster=False)
         return rf_block
 
-    def _make_aq_block(self, aq_dict: dict):
-        delay = self.system_specs.time_to_raster(Quantity(aq_dict["start"] - aq_dict["ref"], "ms"))
-        adc = cmrseq.bausteine.SymmetricADC(system_specs=self.system_specs,
-                                            duration=Quantity(aq_dict["dur"], "ms"),
-                                            delay=delay,
-                                            num_samples=aq_dict["samples"])
-        return adc
+    def _make_aq_block(self, aq_dict: dict) -> List[cmrseq.bausteine.SymmetricADC]:
+        number_of_composite_aqs = aq_dict["rep"]
+        delay_first = self.system_specs.time_to_raster(Quantity(aq_dict["start"] - aq_dict["ref"], "ms"))
+        delay_add = Quantity(aq_dict["dur"], "ms") + Quantity(aq_dict["interval"], "ms")
+
+        adc_blocks = []
+        for n in range(number_of_composite_aqs):
+            adc = cmrseq.bausteine.SymmetricADC(system_specs=self.system_specs,
+                                                duration=Quantity(aq_dict["dur"], "ms"),
+                                                delay=delay_first + delay_add * n,
+                                                num_samples=aq_dict["samples"])
+            adc_blocks.append(adc)
+        return adc_blocks
```

### Comparing `cmrseq-0.18/cmrseq/io/_pulseq.py` & `cmrseq-0.19/cmrseq/io/_pulseq.py`

 * *Files 2% similar despite different names*

```diff
@@ -828,17 +828,19 @@
             delay = Quantity(np.around((rfb.tmin - rf_reference_times[block_idx]).m_as("us")), "us")
             freq = rfb.frequency_offset.to("Hz")
             phase_off = rfb.phase_offset.to("rad")
             shape_ids = [shape_id, phase_id, time_id]
             # Check if block definition already exists
             defidx = 0
             for defidx, bdef in block_definitions.items():
-                if all([np.allclose(bdef[k], q, atol=1e-6) for k, q in zip(
-                            ["amplitude", "delay", "frequency_offset", "phase_offset", "shape_ids"],
-                            [peak_amp, delay, freq, phase_off, shape_ids])]):
+                temp = [(bdef[k], q) for k, q in zip(
+                    ["amplitude", "delay", "frequency_offset", "phase_offset"],
+                    [peak_amp, delay, freq, phase_off])]
+                temp.append((np.array(bdef["shape_ids"]), np.array(shape_ids)))
+                if all([np.allclose(a, b, rtol=1e-6) for a, b in temp]):
                     block_associations[block_idx] = defidx
                     break
 
             if defidx == len(block_definitions.keys()) and block_associations[block_idx] == 0:
                 block_definitions[len(block_definitions.keys()) + 1] = dict(
                     phase_offset=phase_off, shape_ids=shape_ids,
                     frequency_offset=freq, delay=delay, amplitude=peak_amp)
@@ -887,15 +889,15 @@
             timings = adcb.adc_timing
             dwell = Quantity(np.around((timings[1] - timings[0]).m_as("ns"), decimals=8), "ns")
             num_samples = timings.shape[0]
 
             # Check if that block is already defined
             defidx = 0
             for defidx, bdef in block_definitions.items():
-                if all([np.allclose(bdef[k], q, atol=1e-6) for k, q in zip(
+                if all([np.allclose(bdef[k], q, rtol=1e-6) for k, q in zip(
                          ["num_samples", "dwell", "delay", "phase_offset", "frequency_offset"],
                          [num_samples, dwell, delay, adcb.phase_offset, adcb.frequency_offset])]):
                     block_associations[block_idx] = defidx
                     break
 
             if defidx == len(block_definitions.keys()) and block_associations[block_idx] == 0:
                 block_definitions[len(block_definitions.keys()) + 1] = dict(
@@ -1043,15 +1045,15 @@
                         n_unique_wfs = len(unique_arbitrary_wf.keys())
                         wf_id = n_unique_wfs + id_offset + 1
                         unique_arbitrary_wf[wf_id] = normed_amp
 
                     # Check if that block is already defined
                     defidx = 0
                     for defidx, bdef in block_definitions.items():
-                        if all([np.allclose(bdef[k], q, atol=1e-6) for k, q in zip(
+                        if all([np.allclose(bdef[k], q, rtol=1e-6) for k, q in zip(
                                                     ["delay", "shape_ids", "amplitude"],
                                                     [delay, [wf_id, time_id], peak_amp])]):
                             block_associations[-1] = defidx
                             break
 
                     if defidx == len(block_definitions.keys()) and block_associations[-1] == 0:
                         block_definitions[len(block_definitions.keys()) + 1] = dict(
```

### Comparing `cmrseq-0.18/cmrseq/parametric_definitions/diffusion.py` & `cmrseq-0.19/cmrseq/parametric_definitions/diffusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from typing import Union, List
 
 import numpy as np
 from pint import Quantity
 import scipy.optimize
 
+import cmrseq
 from cmrseq import bausteine, Sequence, SystemSpec
 
 
 # pylint: disable=W1401, R0913, C0103
 def bipolar(system_specs: SystemSpec,
             dt: Quantity,
             Dt: Quantity,
@@ -178,16 +179,19 @@
         return seqlist
 
 
 # pylint: disable=R0914
 def shortest_m012(system_specs: SystemSpec,
                   direction: np.ndarray, bvalues: Quantity,
                   start_time: Quantity = Quantity(0., "ms"),
-                  flip_decoding: bool = False):
-    """
+                  flip_decoding: bool = False) -> cmrseq.Sequence:
+    """ Finds the shortest possible second order motion compensated diffusion weighting
+    gradient waveform according to Stoeck et al. (DOI: 10.1002/mrm.25784).
+
+    Compare cmrseq.seqdefs.diffusion.m012 for more information
 
     :param system_specs:
     :param direction:
     :param bvalues:
     :param start_time:
     :param flip_decoding:
     :return:
```

### Comparing `cmrseq-0.18/cmrseq/parametric_definitions/readout/__init__.py` & `cmrseq-0.19/cmrseq/parametric_definitions/readout/__init__.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.18/cmrseq/parametric_definitions/readout/_cartesian_single_lines.py` & `cmrseq-0.19/cmrseq/parametric_definitions/readout/_cartesian_single_lines.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.18/cmrseq/parametric_definitions/readout/_spiral.py` & `cmrseq-0.19/cmrseq/parametric_definitions/readout/_spiral.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.18/cmrseq/parametric_definitions/sequences/_gradient_echo.py` & `cmrseq-0.19/cmrseq/parametric_definitions/sequences/_gradient_echo.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.18/cmrseq/parametric_definitions/sequences/_spin_echo.py` & `cmrseq-0.19/cmrseq/parametric_definitions/sequences/_spin_echo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ This module contains parametric definitions of complete multi-TR SE-based sequences"""
 __all__ = ["single_line_cartesian2d", "se_ssepi"]
 
-from typing import List
+from typing import List, Union
 from warnings import warn
 from types import SimpleNamespace
 
 import numpy as np
 from pint import Quantity
 
 import cmrseq
@@ -70,16 +70,18 @@
 def se_ssepi(system_specs: cmrseq.SystemSpec,
              field_of_view: Quantity,
              matrix_size: np.ndarray,
              echo_time: Quantity,
              slice_thickness: Quantity,
              slice_orientation: np.ndarray,
              pulse_duration: Quantity,
-             tbw_product: float,
-             adc_duration: Quantity,
+             epi_slope_sampling: bool = False,
+             tbw_product: float = 4,
+             max_epi_duration: Quantity = None,
+             epi_water_fat_shift: Union[str, float, int] = "minimum",
              partial_fourier_lines: int = 0,
              blip_direction: str = "up"):
     """Defines a single shot EPI sequence. If the specified echo time is too short, the shortest
     possible echo-time is used.
 
     .. note::
 
@@ -91,29 +93,32 @@
     :param system_specs:  SystemSpecification
     :param field_of_view: spatial extend in readout and phase encoding direction; shape = (2, )
     :param matrix_size: number of pixels in readout and phase encoding direction; shape = (2, )
     :param echo_time: Time at which the central k-space line is placed
     :param slice_thickness: Thickness of slice-selective excitation definitions
     :param slice_orientation: Slice normal of excitation slice
     :param pulse_duration: Duration of the excitation & refocusing pulses
+    :param epi_slope_sampling: If yes the epi readout uses slope sampling
     :param tbw_product: Time-bandwidth product of the inc-Pulses used for excitation and refocus
-    :param adc_duration: Duration of each adc block (corresponding one k-space line)
+    :param adc_duration: Duration of each adc block (corresponding one k-space line) optional
     :param partial_fourier_lines: number of lines to skip before k-space center, allowing shorter
                                     echo times
     :param blip_direction: from ["up", "down"] defining the direction of phase-encoding kspace
                                 travers
     :return: sequence object
     """
     # Define EPI-readout
-    readout = cmrseq.seqdefs.readout.epi_cartesian(system_specs=system_specs,
-                                                   field_of_view=field_of_view,
-                                                   matrix_size=matrix_size,
-                                                   blip_direction=blip_direction,
-                                                   partial_fourier_lines=partial_fourier_lines,
-                                                   adc_duration=adc_duration)
+    readout = cmrseq.seqdefs.readout.single_shot_epi(system_specs=system_specs,
+                                                     field_of_view=field_of_view,
+                                                     matrix_size=matrix_size,
+                                                     blip_direction=blip_direction,
+                                                     partial_fourier_lines=partial_fourier_lines,
+                                                     slope_sampling=epi_slope_sampling,
+                                                     water_fat_shift=epi_water_fat_shift,
+                                                     max_total_duration=max_epi_duration)
     k_center_idx = int(np.floor(matrix_size[1] / 2) - partial_fourier_lines)
 
     # Construct the excitation blocks
     excitation = cmrseq.seqdefs.excitation.slice_selective_se_pulses(
                                                 system_specs=system_specs,
                                                 echo_time=echo_time,
                                                 slice_thickness=slice_thickness,
```

### Comparing `cmrseq-0.18/cmrseq/parametric_definitions/sequences/_ssfp.py` & `cmrseq-0.19/cmrseq/parametric_definitions/sequences/_ssfp.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,17 @@
         .            ADC   \/  \/      |||||||||||||||||||||                       .
         .                  ______                                                  .
         .            SS:  /      \    _______________________                      .
         .                         \__/                       \__/                  .
         .                              _____________________                       .
         .            RO:  ________    /                     \                      .
         .                         \__/                       \__/                  .
-        .            PE:  ________    ______________________                       .
-        .                         \__/                      \__/                   .
+        .                                                    __                    .
+        .            PE:  ________    ______________________/  \                   .
+        .                         \__/                                             .
 
 
     :param system_specs: SystemSpecification
     :param matrix_size: array of shape (2, )
     :param inplane_resolution: Quantity[Length] of shape (2, )
     :param repetition_time: Quantity[Time] containing the required repetition_time
     :param slice_thickness: Quantity[Length] containing the required slice-thickness
@@ -80,15 +81,15 @@
         prephaser_duration = cmrseq.bausteine.TrapezoidalGradient.from_area(
                                 system_specs, np.array([1., 0., 0]), combined_gradient_area).duration
         rf_seq.remove_block("slice_select_rewind_0")
 
         rf_seq.append(cmrseq.bausteine.TrapezoidalGradient.from_dur_area(system_specs,
                                                                          np.array([0., 0., -1.]),
                                                                          prephaser_duration,
-                                                                         ss_refocus.area[-1] / 2,
+                                                                         ss_refocus.area[-1],
                                                                          name="slice_select_rewind"))
         ss_refocus = rf_seq.get_block("slice_select_rewind_0")
     else:
         prephaser_duration = None
 
     # Construct the readout and phase encoding gradients
     ro_blocks = cmrseq.seqdefs.readout.multi_line_cartesian(
@@ -97,15 +98,15 @@
                                     matrix_size=matrix_size,
                                     inplane_resolution=inplane_resolution,
                                     adc_duration=adc_duration,
                                     prephaser_duration=prephaser_duration,
                                     dummy_shots=dummy_shots)
 
     if prephaser_duration is None:
-        prephaser_duration = ro_blocks[dummy_shots].get_block("radial_prephaser_0").duration
+        prephaser_duration = ro_blocks[-1].get_block("ro_prephaser_0").duration
 
     # Create the slice selection compensation
     ss_compensate = deepcopy(ss_refocus)
     ss_compensate.name = "slice_select_prewind"
 
     # Adjust alternating phase offset for adc-events
     for ro_idx, ro_b in enumerate(ro_blocks):
@@ -143,20 +144,21 @@
                                                     system_specs=system_specs,
                                                     slice_thickness=slice_thickness,
                                                     flip_angle=flip_angle_phase,
                                                     pulse_duration=pulse_duration,
                                                     slice_position_offset=slice_position_offset,
                                                     time_bandwidth_product=time_bandwidth_product,
                                                     slice_normal=np.array([0., 0., 1.]))
-        rf_seq.remove_block("slice_select_rewind_0")
-        rf_seq.append(cmrseq.bausteine.TrapezoidalGradient.from_dur_area(system_specs,
-                                                                         np.array([0., 0., -1.]),
-                                                                         prephaser_duration,
-                                                                         ss_refocus.area[-1],
-                                                                         name="slice_select_rewind"))
+        if fuse_slice_rewind_and_prephaser:
+            rf_seq.remove_block("slice_select_rewind_0")
+            rf_seq.append(cmrseq.bausteine.TrapezoidalGradient.from_dur_area(system_specs,
+                                                                             np.array([0., 0., -1.]),
+                                                                             prephaser_duration,
+                                                                             ss_refocus.area[-1],
+                                                                             name="slice_select_rewind"))
         if fuse_slice_rewind_and_prephaser:
             ro_b.shift_in_time(
                 rf_seq.duration - min(ss_refocus.duration, prephaser_duration)+tr_delay_half)
         else:
             ro_b.shift_in_time(
                 rf_seq.duration + tr_delay_half)
 
@@ -309,20 +311,21 @@
             system_specs=system_specs,
             slice_thickness=slice_thickness,
             flip_angle=flip_angle_phase,
             pulse_duration=pulse_duration,
             slice_position_offset=slice_position_offset,
             time_bandwidth_product=time_bandwidth_product,
             slice_normal=np.array([0., 0., 1.]))
-        rf_seq.remove_block("slice_select_rewind_0")
-        rf_seq.append(cmrseq.bausteine.TrapezoidalGradient.from_dur_area(system_specs,
-                                                                         np.array([0., 0., -1.]),
-                                                                         prephaser_duration,
-                                                                         ss_refocus.area[-1],
-                                                                         name="slice_select_rewind"))
+        if fuse_slice_rewind_and_prephaser:
+            rf_seq.remove_block("slice_select_rewind_0")
+            rf_seq.append(cmrseq.bausteine.TrapezoidalGradient.from_dur_area(system_specs,
+                                                                             np.array([0., 0., -1.]),
+                                                                             prephaser_duration,
+                                                                             ss_refocus.area[-1],
+                                                                             name="slice_select_rewind"))
 
         cur_ro = deepcopy(ro_ref)
         sa = np.sin(angle)
         ca = np.cos(angle)
         R = np.array([[ca, -sa, 0], [sa, ca, 0], [0, 0, 1]])
 
         cur_ro.rotate_gradients(R)
```

### Comparing `cmrseq-0.18/cmrseq/parametric_definitions/velocity.py` & `cmrseq-0.19/cmrseq/parametric_definitions/velocity.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.18/cmrseq/plotting.py` & `cmrseq-0.19/cmrseq/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,19 +185,21 @@
 
     if format_axes:
         [ax.set_ylabel(l) for ax, l in zip(axes, [r"RF [$\mu$T]", "G [mT/m]",
                                                   "G [mT/m]", "G [mT/m]"])]
         axes[-1].set_xlabel("Time [ms]")
         grad_range = np.array([-seq._system_specs.max_grad.m_as("mT/m"),
                                 seq._system_specs.max_grad.m_as("mT/m")])
+        rf_range = np.array([-seq._system_specs.rf_peak_power.m_as("uT"),
+                                seq._system_specs.rf_peak_power.m_as("uT")])
         [ax.grid(True) for ax in axes]
         [ax.set_ylim(grad_range * 1.1) for ax in axes[1:]]
-        [ax.set_yticks(np.linspace(grad_range[0], grad_range[1], n_yticks)) for ax in axes[1:]]
+        [ax.set_yticks(np.linspace(*grad_range, n_yticks)) for ax in axes[1:]]
         [ax.yaxis.set_major_formatter(FormatStrFormatter('%3.2f')) for ax in axes]
-        axes[0].set_ylim([-110, 110]), axes[0].set_yticks(np.linspace(-100, 100, n_yticks))
+        axes[0].set_ylim(rf_range * 1.1), axes[0].set_yticks(np.linspace(*rf_range, n_yticks))
         if single_axis:
             [tick.set_verticalalignment("bottom") for tick in axes[0].get_yticklabels()]
             [tick.set_verticalalignment("top") for tick in axes[1].get_yticklabels()]
             axes[0].set_ylabel("RF" + r"[$\mu$T]", labelpad=20)
     return f
```

### Comparing `cmrseq-0.18/cmrseq/utils.py` & `cmrseq-0.19/cmrseq/utils.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.18/cmrseq.egg-info/PKG-INFO` & `cmrseq-0.19/cmrseq.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmrseq
-Version: 0.18
+Version: 0.19
 Summary: UNKNOWN
 Home-page: https://gitlab.ethz.ch/jweine/cmrseq
 Author: Jonathan Weine, Charles McGrath
 Author-email: weine@biomed.ee.ethz.ch, mcgrath@biomed.ee.ethz.ch
 License: UNKNOWN
 Project-URL: Documentation, https://people.ee.ethz.ch/~jweine/cmrseq/latest/index.html
 Project-URL: Source, https://gitlab.ethz.ch/jweine/cmrseq
```

### Comparing `cmrseq-0.18/cmrseq.egg-info/SOURCES.txt` & `cmrseq-0.19/cmrseq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmrseq-0.18/setup.py` & `cmrseq-0.19/setup.py`

 * *Files identical despite different names*

