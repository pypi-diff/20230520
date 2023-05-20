# Comparing `tmp/quinten-cli-1.1.3.tar.gz` & `tmp/quinten-cli-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quinten-cli-1.1.3.tar", last modified: Mon Apr 24 18:31:42 2023, max compression
+gzip compressed data, was "quinten-cli-1.1.4.tar", last modified: Sat May 20 19:44:00 2023, max compression
```

## Comparing `quinten-cli-1.1.3.tar` & `quinten-cli-1.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-04-24 18:31:42.385105 quinten-cli-1.1.3/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1069 2023-04-24 18:30:39.000000 quinten-cli-1.1.3/LICENSE
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      603 2023-04-24 18:31:42.385105 quinten-cli-1.1.3/PKG-INFO
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      294 2023-04-24 18:30:39.000000 quinten-cli-1.1.3/README.md
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-04-24 18:31:42.385105 quinten-cli-1.1.3/cli/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      925 2023-04-24 18:30:39.000000 quinten-cli-1.1.3/cli/__init__.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      157 2023-04-24 18:30:39.000000 quinten-cli-1.1.3/cli/env.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      625 2023-04-24 18:30:39.000000 quinten-cli-1.1.3/cli/input_interface.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      741 2023-04-24 18:30:39.000000 quinten-cli-1.1.3/cli/install.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1241 2023-04-24 18:30:39.000000 quinten-cli-1.1.3/cli/output_interface.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1483 2023-04-24 18:30:39.000000 quinten-cli-1.1.3/cli/progress.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     5097 2023-04-24 18:31:06.000000 quinten-cli-1.1.3/cli/run.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      366 2023-04-24 18:30:39.000000 quinten-cli-1.1.3/cli/status.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      586 2023-04-24 18:31:21.000000 quinten-cli-1.1.3/pyproject.toml
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-04-24 18:31:42.385105 quinten-cli-1.1.3/quinten_cli.egg-info/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      603 2023-04-24 18:31:42.000000 quinten-cli-1.1.3/quinten_cli.egg-info/PKG-INFO
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      418 2023-04-24 18:31:42.000000 quinten-cli-1.1.3/quinten_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)        1 2023-04-24 18:31:42.000000 quinten-cli-1.1.3/quinten_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       44 2023-04-24 18:31:42.000000 quinten-cli-1.1.3/quinten_cli.egg-info/entry_points.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       74 2023-04-24 18:31:42.000000 quinten-cli-1.1.3/quinten_cli.egg-info/requires.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)        4 2023-04-24 18:31:42.000000 quinten-cli-1.1.3/quinten_cli.egg-info/top_level.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       38 2023-04-24 18:31:42.385105 quinten-cli-1.1.3/setup.cfg
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-04-24 18:31:42.385105 quinten-cli-1.1.3/tests/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      322 2023-04-24 18:30:39.000000 quinten-cli-1.1.3/tests/test_api.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      937 2023-04-24 18:30:39.000000 quinten-cli-1.1.3/tests/test_progress_ui.py
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-05-20 19:44:00.539976 quinten-cli-1.1.4/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1069 2023-05-20 19:23:25.000000 quinten-cli-1.1.4/LICENSE
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      603 2023-05-20 19:44:00.539976 quinten-cli-1.1.4/PKG-INFO
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      294 2023-05-20 19:23:25.000000 quinten-cli-1.1.4/README.md
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-05-20 19:44:00.539976 quinten-cli-1.1.4/cli/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      925 2023-05-20 19:23:25.000000 quinten-cli-1.1.4/cli/__init__.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      157 2023-05-20 19:23:25.000000 quinten-cli-1.1.4/cli/env.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      625 2023-05-20 19:23:25.000000 quinten-cli-1.1.4/cli/input_interface.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      741 2023-05-20 19:23:25.000000 quinten-cli-1.1.4/cli/install.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1241 2023-05-20 19:23:25.000000 quinten-cli-1.1.4/cli/output_interface.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1526 2023-05-20 19:43:16.000000 quinten-cli-1.1.4/cli/progress.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     5097 2023-05-20 19:23:25.000000 quinten-cli-1.1.4/cli/run.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      366 2023-05-20 19:23:25.000000 quinten-cli-1.1.4/cli/status.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      586 2023-05-20 19:37:43.000000 quinten-cli-1.1.4/pyproject.toml
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-05-20 19:44:00.539976 quinten-cli-1.1.4/quinten_cli.egg-info/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      603 2023-05-20 19:44:00.000000 quinten-cli-1.1.4/quinten_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      418 2023-05-20 19:44:00.000000 quinten-cli-1.1.4/quinten_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)        1 2023-05-20 19:44:00.000000 quinten-cli-1.1.4/quinten_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       44 2023-05-20 19:44:00.000000 quinten-cli-1.1.4/quinten_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       74 2023-05-20 19:44:00.000000 quinten-cli-1.1.4/quinten_cli.egg-info/requires.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)        4 2023-05-20 19:44:00.000000 quinten-cli-1.1.4/quinten_cli.egg-info/top_level.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       38 2023-05-20 19:44:00.539976 quinten-cli-1.1.4/setup.cfg
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-05-20 19:44:00.539976 quinten-cli-1.1.4/tests/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      322 2023-05-20 19:23:25.000000 quinten-cli-1.1.4/tests/test_api.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1249 2023-05-20 19:37:23.000000 quinten-cli-1.1.4/tests/test_progress_ui.py
```

### Comparing `quinten-cli-1.1.3/LICENSE` & `quinten-cli-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `quinten-cli-1.1.3/PKG-INFO` & `quinten-cli-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quinten-cli
-Version: 1.1.3
+Version: 1.1.4
 Author-email: Quinten Roets <qdr2104@columbia.edu>
 License: MIT
 Project-URL: Source Code, https://github.com/quintenroets/cli
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
```

### Comparing `quinten-cli-1.1.3/cli/__init__.py` & `quinten-cli-1.1.4/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `quinten-cli-1.1.3/cli/input_interface.py` & `quinten-cli-1.1.4/cli/input_interface.py`

 * *Files identical despite different names*

### Comparing `quinten-cli-1.1.3/cli/install.py` & `quinten-cli-1.1.4/cli/install.py`

 * *Files identical despite different names*

### Comparing `quinten-cli-1.1.3/cli/output_interface.py` & `quinten-cli-1.1.4/cli/output_interface.py`

 * *Files identical despite different names*

### Comparing `quinten-cli-1.1.3/cli/progress.py` & `quinten-cli-1.1.4/cli/progress.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import sys
 
 
 def get_progress():
-    from rich.progress import TextColumn  # noqa: autoimport
-    from rich.progress import (BarColumn, Progress,  # noqa: autoimport
-                               TimeRemainingColumn)
+    from rich.progress import TimeRemainingColumn  # noqa: autoimport
+    from rich.progress import BarColumn, Progress, TextColumn  # noqa: autoimport
 
     columns = [TextColumn("[progress.description]{task.description}")]
+
+    column_message = (
+        "[progress.completed]{task.completed}/[progress.total]"
+        "{task.total:>0.0f} {task.fields[unit]}"
+    )
     columns.extend(
         (
-            TextColumn(
-                "[progress.completed]{task.completed}/[progress.total]{task.total:>0.0f} {task.fields[unit]}"
-            ),
+            TextColumn(column_message),
             BarColumn(bar_width=1000),  # shrinks depending on other columns
             TextColumn("[progress.percentage]{task.percentage:>3.0f}%"),
             TimeRemainingColumn(),
         )
     )
     return Progress(*columns)
 
@@ -28,18 +30,19 @@
     @property
     def prog(cls):
         if cls._prog is None:
             cls._prog = get_progress()
         return cls._prog
 
 
-def progress(sequence, description="", unit="it", total=None):
+def progress(sequence, description="", unit="it", total=None, cleanup=False):
     # classmethod properties require python 3.9
     prog = ProgressManager.prog() if sys.version_info < (3, 9) else ProgressManager.prog
     prog.__enter__()
 
     task_id = prog.add_task(description=description, unit=unit)
     ProgressManager.busy_amount += 1
     yield from prog.track(sequence, total, task_id, description)
     ProgressManager.busy_amount -= 1
-    if ProgressManager.busy_amount == 0:
-        pass  # prog.__exit__(None, None, None)  # disable for now to fix issue of progress appearing twice
+    # cleanup False by default because it makes completed progressbar appear twice
+    if ProgressManager.busy_amount == 0 and cleanup:
+        prog.__exit__(None, None, None)
```

### Comparing `quinten-cli-1.1.3/cli/run.py` & `quinten-cli-1.1.4/cli/run.py`

 * *Files identical despite different names*

### Comparing `quinten-cli-1.1.3/pyproject.toml` & `quinten-cli-1.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "quinten-cli"
-version = "1.1.3"
+version = "1.1.4"
 description = ""
 authors = [{name = "Quinten Roets", email = "qdr2104@columbia.edu"}]
 license = {text = "MIT"}
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
     "python-dotenv",
```

### Comparing `quinten-cli-1.1.3/quinten_cli.egg-info/PKG-INFO` & `quinten-cli-1.1.4/quinten_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quinten-cli
-Version: 1.1.3
+Version: 1.1.4
 Author-email: Quinten Roets <qdr2104@columbia.edu>
 License: MIT
 Project-URL: Source Code, https://github.com/quintenroets/cli
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
```

### Comparing `quinten-cli-1.1.3/tests/test_progress_ui.py` & `quinten-cli-1.1.4/tests/test_progress_ui.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,53 @@
 import time
 
 import pytest
 
 import cli
 
+SLEEP_INTERVAL = 0.01
+ITERATIONS = 200
+
+
+def sleep():
+    time.sleep(SLEEP_INTERVAL)
+
 
 @pytest.mark.skip(reason="requires manual inspection")
 def test_progress():
-    items = cli.progress(range(200), description="counting", unit="items")
+    items = cli.progress(range(ITERATIONS), description="counting", unit="items")
+    for i in items:
+        sleep()
+
+
+@pytest.mark.skip(reason="requires manual inspection")
+def test_progress_with_cleanup():
+    items = cli.progress(range(ITERATIONS), description="counting", unit="items")
     for i in items:
-        time.sleep(0.01)
+        sleep()
 
 
 @pytest.mark.skip(reason="requires manual inspection")
 def test_progress_double():
-    for i in cli.progress(range(10), description="outer loop", unit="items"):
-        time.sleep(0.1)
+    for i in cli.progress(range(ITERATIONS), description="outer loop", unit="items"):
+        sleep()
         if i == 4:
-            for j in cli.progress(range(10), description="inner loop"):
-                time.sleep(0.1)
+            for j in cli.progress(range(ITERATIONS), description="inner loop"):
+                sleep()
 
 
 @pytest.mark.skip(reason="requires manual inspection")
 def test_progress_with_status():
-    for i in cli.progress(range(10), "advance"):
-        time.sleep(0.1)
+    for i in cli.progress(range(ITERATIONS), "advance"):
+        sleep()
         with cli.status("waiting"):
-            time.sleep(0.1)
+            sleep()
 
     with cli.status("waiting"):
-        time.sleep(5)
+        sleep()
 
 
 if __name__ == "__main__":
     test_progress()
+    test_progress_with_cleanup()
     test_progress_double()
     test_progress_with_status()
```

