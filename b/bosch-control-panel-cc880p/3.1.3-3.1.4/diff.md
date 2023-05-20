# Comparing `tmp/bosch-control-panel-cc880p-3.1.3.tar.gz` & `tmp/bosch-control-panel-cc880p-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bosch-control-panel-cc880p-3.1.3.tar", last modified: Sat May 20 17:17:14 2023, max compression
+gzip compressed data, was "bosch-control-panel-cc880p-3.1.4.tar", last modified: Sat May 20 17:38:26 2023, max compression
```

## Comparing `bosch-control-panel-cc880p-3.1.3.tar` & `bosch-control-panel-cc880p-3.1.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:17:14.319379 bosch-control-panel-cc880p-3.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-05-20 17:17:14.319379 bosch-control-panel-cc880p-3.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20428 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-20 17:17:14.319379 bosch-control-panel-cc880p-3.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:17:14.311379 bosch-control-panel-cc880p-3.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:17:14.307378 bosch-control-panel-cc880p-3.1.3/src/bosch/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:17:14.307378 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:17:14.311379 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:17:14.315379 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/cli/cmds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    18937 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/cp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:17:14.315379 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/models/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/models/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/models/cp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/models/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/models/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-20 17:16:56.000000 bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:17:14.319379 bosch-control-panel-cc880p-3.1.3/src/bosch_control_panel_cc880p.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-05-20 17:17:14.000000 bosch-control-panel-cc880p-3.1.3/src/bosch_control_panel_cc880p.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-20 17:17:14.000000 bosch-control-panel-cc880p-3.1.3/src/bosch_control_panel_cc880p.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 17:17:14.000000 bosch-control-panel-cc880p-3.1.3/src/bosch_control_panel_cc880p.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-20 17:17:14.000000 bosch-control-panel-cc880p-3.1.3/src/bosch_control_panel_cc880p.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-20 17:17:14.000000 bosch-control-panel-cc880p-3.1.3/src/bosch_control_panel_cc880p.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-20 17:17:14.000000 bosch-control-panel-cc880p-3.1.3/src/bosch_control_panel_cc880p.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:38:26.009485 bosch-control-panel-cc880p-3.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-05-20 17:38:26.009485 bosch-control-panel-cc880p-3.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20428 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-20 17:38:26.009485 bosch-control-panel-cc880p-3.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:38:26.001485 bosch-control-panel-cc880p-3.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:38:26.001485 bosch-control-panel-cc880p-3.1.4/src/bosch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:38:26.001485 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:38:26.005485 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:38:26.005485 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/cli/cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18926 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/cp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:38:26.005485 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/models/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/models/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/models/cp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/models/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/models/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-20 17:38:12.000000 bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:38:26.009485 bosch-control-panel-cc880p-3.1.4/src/bosch_control_panel_cc880p.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21111 2023-05-20 17:38:25.000000 bosch-control-panel-cc880p-3.1.4/src/bosch_control_panel_cc880p.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-20 17:38:26.000000 bosch-control-panel-cc880p-3.1.4/src/bosch_control_panel_cc880p.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 17:38:25.000000 bosch-control-panel-cc880p-3.1.4/src/bosch_control_panel_cc880p.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-20 17:38:25.000000 bosch-control-panel-cc880p-3.1.4/src/bosch_control_panel_cc880p.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-20 17:38:25.000000 bosch-control-panel-cc880p-3.1.4/src/bosch_control_panel_cc880p.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-20 17:38:25.000000 bosch-control-panel-cc880p-3.1.4/src/bosch_control_panel_cc880p.egg-info/top_level.txt
```

### Comparing `bosch-control-panel-cc880p-3.1.3/LICENSE` & `bosch-control-panel-cc880p-3.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.3/PKG-INFO` & `bosch-control-panel-cc880p-3.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bosch-control-panel-cc880p
-Version: 3.1.3
+Version: 3.1.4
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
-Metadata-Version: 2.1 Name: bosch-control-panel-cc880p Version: 3.1.3 Summary:
+Metadata-Version: 2.1 Name: bosch-control-panel-cc880p Version: 3.1.4 Summary:
 Library to interface with the old CC880p Bosch COntrol Panels Home-page: https:
 //github.com/hgomes88/bosch-control-panel-cc880p Author: Hugo Gomes Author-
 email: hgomes88@gmail.com Project-URL: Tracker, https://github.com/hgomes88/
 bosch-control-panel-cc880p/issues Project-URL: Download, https://pypi.org/
 project/bosch-control-panel-cc880p/ Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
```

### Comparing `bosch-control-panel-cc880p-3.1.3/README.md` & `bosch-control-panel-cc880p-3.1.4/README.md`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.3/setup.cfg` & `bosch-control-panel-cc880p-3.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/cli/cli.py` & `bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/cli/cli.py`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/cli/cmds.py` & `bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/cli/cmds.py`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/cli/parser.py` & `bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/cli/parser.py`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/cp.py` & `bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/cp.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,16 +254,16 @@
                 except EOFError:
                     _LOGGER.warning('Connection EOF')
                     raise
                 except (OSError):
                     _LOGGER.warning('Connection failed')
                     await self._close_connection()
                     raise
-                except BaseException as ex:
-                    _LOGGER.warning('Unexpected Error: %s', ex)
+                except BaseException:
+                    _LOGGER.exception('Unexpected Error:')
                     raise
                 else:
                     available = True
                     return resp
                 finally:
                     await self._update_availability(available)
         else:
```

### Comparing `bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/models/cp.py` & `bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/models/cp.py`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/models/requests.py` & `bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/models/requests.py`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/models/responses.py` & `bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/models/responses.py`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.3/src/bosch/control_panel/cc880p/utils.py` & `bosch-control-panel-cc880p-3.1.4/src/bosch/control_panel/cc880p/utils.py`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-3.1.3/src/bosch_control_panel_cc880p.egg-info/PKG-INFO` & `bosch-control-panel-cc880p-3.1.4/src/bosch_control_panel_cc880p.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bosch-control-panel-cc880p
-Version: 3.1.3
+Version: 3.1.4
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
-Metadata-Version: 2.1 Name: bosch-control-panel-cc880p Version: 3.1.3 Summary:
+Metadata-Version: 2.1 Name: bosch-control-panel-cc880p Version: 3.1.4 Summary:
 Library to interface with the old CC880p Bosch COntrol Panels Home-page: https:
 //github.com/hgomes88/bosch-control-panel-cc880p Author: Hugo Gomes Author-
 email: hgomes88@gmail.com Project-URL: Tracker, https://github.com/hgomes88/
 bosch-control-panel-cc880p/issues Project-URL: Download, https://pypi.org/
 project/bosch-control-panel-cc880p/ Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
```

### Comparing `bosch-control-panel-cc880p-3.1.3/src/bosch_control_panel_cc880p.egg-info/SOURCES.txt` & `bosch-control-panel-cc880p-3.1.4/src/bosch_control_panel_cc880p.egg-info/SOURCES.txt`

 * *Files identical despite different names*

