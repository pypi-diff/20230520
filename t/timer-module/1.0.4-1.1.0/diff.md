# Comparing `tmp/timer-module-1.0.4.tar.gz` & `tmp/timer-module-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\shady\Desktop\Python Projects\timer_module\dist\tmp1zun8h0h\timer-module-1.0.4.tar", last modified: Sun Feb 12 02:06:39 2023, max compression
+gzip compressed data, was "timer-module-1.1.0.tar", last modified: Sat May 20 04:32:06 2023, max compression
```

## Comparing `timer-module-1.0.4.tar` & `timer-module-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-02-12 02:06:39.000000 timer-module-1.0.4/
--rw-rw-rw-   0        0        0     1091 2023-02-11 02:09:32.000000 timer-module-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     2373 2023-02-12 02:06:39.000000 timer-module-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1804 2023-02-12 02:05:34.000000 timer-module-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-02-12 02:06:39.000000 timer-module-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      906 2023-02-12 02:04:58.000000 timer-module-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-12 02:06:39.000000 timer-module-1.0.4/timer_module/
--rw-rw-rw-   0        0        0     8222 2023-02-11 01:27:49.000000 timer-module-1.0.4/timer_module/profiler.py
--rw-rw-rw-   0        0        0     1459 2023-02-11 01:27:34.000000 timer-module-1.0.4/timer_module/timer.py
--rw-rw-rw-   0        0        0      127 2023-02-11 01:35:27.000000 timer-module-1.0.4/timer_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-12 02:06:39.000000 timer-module-1.0.4/timer_module.egg-info/
--rw-rw-rw-   0        0        0        1 2023-02-12 02:06:39.000000 timer-module-1.0.4/timer_module.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2373 2023-02-12 02:06:39.000000 timer-module-1.0.4/timer_module.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       17 2023-02-12 02:06:39.000000 timer-module-1.0.4/timer_module.egg-info/requires.txt
--rw-rw-rw-   0        0        0      277 2023-02-12 02:06:39.000000 timer-module-1.0.4/timer_module.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       13 2023-02-12 02:06:39.000000 timer-module-1.0.4/timer_module.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 04:32:06.229749 timer-module-1.1.0/
+-rw-rw-rw-   0        0        0     1091 2023-02-11 02:09:32.000000 timer-module-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2428 2023-05-20 04:32:06.228748 timer-module-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1859 2023-05-20 04:26:53.000000 timer-module-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-20 04:32:06.229749 timer-module-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      922 2023-05-20 04:31:19.000000 timer-module-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 04:32:06.202187 timer-module-1.1.0/timer_module/
+-rw-rw-rw-   0        0        0      127 2023-05-20 02:26:45.000000 timer-module-1.1.0/timer_module/__init__.py
+-rw-rw-rw-   0        0        0      494 2023-05-20 04:26:53.000000 timer-module-1.1.0/timer_module/converters.py
+-rw-rw-rw-   0        0        0    10558 2023-05-20 04:26:53.000000 timer-module-1.1.0/timer_module/profiler.py
+-rw-rw-rw-   0        0        0     1356 2023-05-20 04:26:53.000000 timer-module-1.1.0/timer_module/stdio.py
+-rw-rw-rw-   0        0        0     1459 2023-02-11 01:27:34.000000 timer-module-1.1.0/timer_module/timer.py
+drwxrwxrwx   0        0        0        0 2023-05-20 04:32:06.227747 timer-module-1.1.0/timer_module.egg-info/
+-rw-rw-rw-   0        0        0     2428 2023-05-20 04:32:06.000000 timer-module-1.1.0/timer_module.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-05-20 04:32:06.000000 timer-module-1.1.0/timer_module.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 04:32:06.000000 timer-module-1.1.0/timer_module.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-20 04:32:06.000000 timer-module-1.1.0/timer_module.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-20 04:32:06.000000 timer-module-1.1.0/timer_module.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `timer-module-1.0.4/LICENSE` & `timer-module-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timer-module-1.0.4/PKG-INFO` & `timer-module-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timer-module
-Version: 1.0.4
+Version: 1.1.0
 Summary: Timer Module with performance profiling features
 Home-page: https://github.com/syn-chromatic/timer-module
 Author: syn-chromatic
 Author-email: synchromatic.github@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,28 +12,28 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ___
-## Prerequisite:
+## 📋 Prerequisite:
 ```
 Requires Python >= 3.10
 TimeProfiler makes use of new features from Python's typing module.
 ```
 
 ___
-## Installation:
+## 🛠️ Installation:
 ```
 pip install timer-module
 ```
 
 ___
-## Timer Usage:
+## 🖥️ Timer Usage:
 ```python
 import time
 from timer_module import TimerModule
 
 timer_module = TimerModule().start()
 
 timer_module.pause()
@@ -42,31 +42,31 @@
 timer_module.start()
 time.sleep(2)
 
 time_seconds = timer_module.get_time()
 print(time_seconds)
 ```
 
-#### set the timer
+#### Set the timer
 ```python
 timer_module = TimerModule().set_time(5).start()
 ```
 
-#### refresh time (keeps timer state)
+#### Refresh time (preserves timer state):
 ```python
 timer_module.refresh()
 ```
 
-#### reset time (resets everyting)
+#### Reset time (resets everyting)
 ```python
 timer_module.reset()
 ```
 
 ___
-## Profiler Usage:
+## 🖥️ Profiler Usage:
 TimeProfiler also includes a "function_profiler" and "async_function_profiler", in a class the asynchronous methods are handled automatically, but for functions you need to select the appropriate decorator.
 
 ```python
 import time
 from timer_module import TimeProfiler
 
 # You only need this line to profile the entire class 
@@ -98,10 +98,11 @@
 
 
 ec = ExampleClass()
 ec.method_1()
 ```
 
 #### Output:
-![](https://raw.githubusercontent.com/syn-chromatic/timer-module/main/examples/profiler_output.png)
+![profiler_output](https://github.com/syn-chromatic/timer-module/assets/68112904/155f7515-fc5a-480b-b7eb-d1e710acae3f)
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `timer-module-1.0.4/README.md` & `timer-module-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ___
-## Prerequisite:
+## 📋 Prerequisite:
 ```
 Requires Python >= 3.10
 TimeProfiler makes use of new features from Python's typing module.
 ```
 
 ___
-## Installation:
+## 🛠️ Installation:
 ```
 pip install timer-module
 ```
 
 ___
-## Timer Usage:
+## 🖥️ Timer Usage:
 ```python
 import time
 from timer_module import TimerModule
 
 timer_module = TimerModule().start()
 
 timer_module.pause()
@@ -25,31 +25,31 @@
 timer_module.start()
 time.sleep(2)
 
 time_seconds = timer_module.get_time()
 print(time_seconds)
 ```
 
-#### set the timer
+#### Set the timer
 ```python
 timer_module = TimerModule().set_time(5).start()
 ```
 
-#### refresh time (keeps timer state)
+#### Refresh time (preserves timer state):
 ```python
 timer_module.refresh()
 ```
 
-#### reset time (resets everyting)
+#### Reset time (resets everyting)
 ```python
 timer_module.reset()
 ```
 
 ___
-## Profiler Usage:
+## 🖥️ Profiler Usage:
 TimeProfiler also includes a "function_profiler" and "async_function_profiler", in a class the asynchronous methods are handled automatically, but for functions you need to select the appropriate decorator.
 
 ```python
 import time
 from timer_module import TimeProfiler
 
 # You only need this line to profile the entire class 
@@ -81,8 +81,9 @@
 
 
 ec = ExampleClass()
 ec.method_1()
 ```
 
 #### Output:
-![](https://raw.githubusercontent.com/syn-chromatic/timer-module/main/examples/profiler_output.png)
+![profiler_output](https://github.com/syn-chromatic/timer-module/assets/68112904/155f7515-fc5a-480b-b7eb-d1e710acae3f)
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `timer-module-1.0.4/setup.py` & `timer-module-1.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from setuptools import setup, find_packages
 
-VERSION = "1.0.4"
+VERSION = "1.1.0"
 DESCRIPTION = "Timer Module with performance profiling features"
 
 root = Path(__file__).parent
-long_description = (root / "README.md").read_text()
+long_description = (root / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="timer-module",
     author="syn-chromatic",
     author_email="synchromatic.github@gmail.com",
     url="https://github.com/syn-chromatic/timer-module",
     version=VERSION,
```

### Comparing `timer-module-1.0.4/timer_module/timer.py` & `timer-module-1.1.0/timer_module/timer.py`

 * *Files identical despite different names*

### Comparing `timer-module-1.0.4/timer_module.egg-info/PKG-INFO` & `timer-module-1.1.0/timer_module.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timer-module
-Version: 1.0.4
+Version: 1.1.0
 Summary: Timer Module with performance profiling features
 Home-page: https://github.com/syn-chromatic/timer-module
 Author: syn-chromatic
 Author-email: synchromatic.github@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,28 +12,28 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ___
-## Prerequisite:
+## 📋 Prerequisite:
 ```
 Requires Python >= 3.10
 TimeProfiler makes use of new features from Python's typing module.
 ```
 
 ___
-## Installation:
+## 🛠️ Installation:
 ```
 pip install timer-module
 ```
 
 ___
-## Timer Usage:
+## 🖥️ Timer Usage:
 ```python
 import time
 from timer_module import TimerModule
 
 timer_module = TimerModule().start()
 
 timer_module.pause()
@@ -42,31 +42,31 @@
 timer_module.start()
 time.sleep(2)
 
 time_seconds = timer_module.get_time()
 print(time_seconds)
 ```
 
-#### set the timer
+#### Set the timer
 ```python
 timer_module = TimerModule().set_time(5).start()
 ```
 
-#### refresh time (keeps timer state)
+#### Refresh time (preserves timer state):
 ```python
 timer_module.refresh()
 ```
 
-#### reset time (resets everyting)
+#### Reset time (resets everyting)
 ```python
 timer_module.reset()
 ```
 
 ___
-## Profiler Usage:
+## 🖥️ Profiler Usage:
 TimeProfiler also includes a "function_profiler" and "async_function_profiler", in a class the asynchronous methods are handled automatically, but for functions you need to select the appropriate decorator.
 
 ```python
 import time
 from timer_module import TimeProfiler
 
 # You only need this line to profile the entire class 
@@ -98,10 +98,11 @@
 
 
 ec = ExampleClass()
 ec.method_1()
 ```
 
 #### Output:
-![](https://raw.githubusercontent.com/syn-chromatic/timer-module/main/examples/profiler_output.png)
+![profiler_output](https://github.com/syn-chromatic/timer-module/assets/68112904/155f7515-fc5a-480b-b7eb-d1e710acae3f)
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

