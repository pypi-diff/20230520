# Comparing `tmp/circuitpython-bma220-0.3.0.tar.gz` & `tmp/circuitpython-bma220-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-bma220-0.3.0.tar", last modified: Fri May 19 16:13:07 2023, max compression
+gzip compressed data, was "circuitpython-bma220-0.4.0.tar", last modified: Sat May 20 17:19:25 2023, max compression
```

## Comparing `circuitpython-bma220-0.3.0.tar` & `circuitpython-bma220-0.4.0.tar`

### file list

```diff
@@ -1,50 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:13:07.996886 circuitpython-bma220-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:13:07.988886 circuitpython-bma220-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:13:07.988886 circuitpython-bma220-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-19 16:13:07.996886 circuitpython-bma220-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:13:07.992886 circuitpython-bma220-0.3.0/bma220/
--rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-05-19 16:12:58.000000 circuitpython-bma220-0.3.0/bma220/bma220.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-19 16:12:58.000000 circuitpython-bma220-0.3.0/bma220/bma220_const.py
--rw-r--r--   0 runner    (1001) docker     (123)    11195 2023-05-19 16:12:58.000000 circuitpython-bma220-0.3.0/bma220/bma220_slope.py
--rw-r--r--   0 runner    (1001) docker     (123)    13356 2023-05-19 16:12:58.000000 circuitpython-bma220-0.3.0/bma220/bma220_tap_sensing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:13:07.992886 circuitpython-bma220-0.3.0/circuitpython_bma220.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-19 16:13:07.000000 circuitpython-bma220-0.3.0/circuitpython_bma220.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-19 16:13:07.000000 circuitpython-bma220-0.3.0/circuitpython_bma220.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:13:07.000000 circuitpython-bma220-0.3.0/circuitpython_bma220.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-19 16:13:07.000000 circuitpython-bma220-0.3.0/circuitpython_bma220.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 16:13:07.000000 circuitpython-bma220-0.3.0/circuitpython_bma220.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:13:07.992886 circuitpython-bma220-0.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:13:07.992886 circuitpython-bma220-0.3.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:13:07.996886 circuitpython-bma220-0.3.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-19 16:12:58.000000 circuitpython-bma220-0.3.0/examples/bma220_acc_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-19 16:12:58.000000 circuitpython-bma220-0.3.0/examples/bma220_double_tap_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-19 16:12:58.000000 circuitpython-bma220-0.3.0/examples/bma220_filter_bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-19 16:12:58.000000 circuitpython-bma220-0.3.0/examples/bma220_latched_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-19 16:12:58.000000 circuitpython-bma220-0.3.0/examples/bma220_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-19 16:12:58.000000 circuitpython-bma220-0.3.0/examples/bma220_sleep_duration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-19 16:12:58.000000 circuitpython-bma220-0.3.0/examples/bma220_slope_slope_sign.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-19 16:12:58.000000 circuitpython-bma220-0.3.0/examples/bma220_slope_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-19 16:12:58.000000 circuitpython-bma220-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-19 16:12:46.000000 circuitpython-bma220-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 16:13:07.996886 circuitpython-bma220-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:19:25.950941 circuitpython-bma220-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:19:25.942941 circuitpython-bma220-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:19:25.946941 circuitpython-bma220-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-20 17:19:25.950941 circuitpython-bma220-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:19:25.946941 circuitpython-bma220-0.4.0/bma220/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/bma220/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/bma220/bma220.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/bma220/bma220_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/bma220/bma220_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11195 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/bma220/bma220_slope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13356 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/bma220/bma220_tap_sensing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:19:25.950941 circuitpython-bma220-0.4.0/circuitpython_bma220.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-20 17:19:25.000000 circuitpython-bma220-0.4.0/circuitpython_bma220.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-20 17:19:25.000000 circuitpython-bma220-0.4.0/circuitpython_bma220.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 17:19:25.000000 circuitpython-bma220-0.4.0/circuitpython_bma220.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-20 17:19:25.000000 circuitpython-bma220-0.4.0/circuitpython_bma220.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-20 17:19:25.000000 circuitpython-bma220-0.4.0/circuitpython_bma220.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:19:25.950941 circuitpython-bma220-0.4.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:19:25.950941 circuitpython-bma220-0.4.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:19:25.950941 circuitpython-bma220-0.4.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/examples/bma220_acc_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/examples/bma220_double_tap_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/examples/bma220_filter_bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/examples/bma220_latched_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/examples/bma220_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/examples/bma220_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/examples/bma220_sleep_duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/examples/bma220_slope_slope_sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/examples/bma220_slope_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-20 17:19:17.000000 circuitpython-bma220-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-20 17:19:07.000000 circuitpython-bma220-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 17:19:25.950941 circuitpython-bma220-0.4.0/setup.cfg
```

### Comparing `circuitpython-bma220-0.3.0/.github/workflows/build.yml` & `circuitpython-bma220-0.4.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.3.0/.github/workflows/release_gh.yml` & `circuitpython-bma220-0.4.0/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.3.0/.gitignore` & `circuitpython-bma220-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.3.0/.pre-commit-config.yaml` & `circuitpython-bma220-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.3.0/.pylintrc` & `circuitpython-bma220-0.4.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.3.0/LICENSE` & `circuitpython-bma220-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.3.0/PKG-INFO` & `circuitpython-bma220-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-bma220
-Version: 0.3.0
+Version: 0.4.0
 Summary: BMA220 Bosch Circuitpython Driver library
 Author-email: "Jose D. Montoya" <jlib@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_BMA220
 Keywords: sensor,blinka,circuitpython,micropython,bma220,acceleration,digital,bosch,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-bma220-0.3.0/README.rst` & `circuitpython-bma220-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.3.0/bma220/bma220.py` & `circuitpython-bma220-0.4.0/bma220/bma220.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 try:
     from busio import I2C
     from typing import Tuple
 except ImportError:
     pass
 
 
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __repo__ = "https://github.com/jposada202020/CircuitPython_BMA220.git"
 
 
 _REG_WHOAMI = const(0x00)
 _FILTER_CONF = const(0x20)
 _ACC_RANGE = const(0x22)
 _SLEEP_CONF = const(0x0F)
```

### Comparing `circuitpython-bma220-0.3.0/bma220/bma220_const.py` & `circuitpython-bma220-0.4.0/bma220/bma220_const.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 * Author(s): Jose D. Montoya
 
 
 """
 
 from micropython import const
 
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __repo__ = "https://github.com/jposada202020/CircuitPython_BMA220.git"
 
 # pylint: disable=duplicate-code
 # Acceleration range
 ACC_RANGE_2 = const(0b00)
 ACC_RANGE_4 = const(0b01)
 ACC_RANGE_8 = const(0b10)
@@ -90,10 +90,7 @@
     LATCH_FOR_050S,
     LATCH_FOR_1S,
     LATCH_FOR_2S,
     LATCH_FOR_4S,
     LATCH_FOR_8S,
     LATCHED,
 )
-
-# class names:
-#     pass
```

### Comparing `circuitpython-bma220-0.3.0/bma220/bma220_slope.py` & `circuitpython-bma220-0.4.0/bma220/bma220_slope.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from bma220.bma220 import BMA220
 
 try:
     from typing import Tuple
 except ImportError:
     pass
 
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __repo__ = "https://github.com/jposada202020/CircuitPython_BMA220.git"
 
 _CONF = const(0x1A)
 _SLOPE_INFO = const(0x12)
 _SLOPE_INFO2 = const(0x16)
 _INTERRUPTS = const(0x18)
```

### Comparing `circuitpython-bma220-0.3.0/bma220/bma220_tap_sensing.py` & `circuitpython-bma220-0.4.0/bma220/bma220_tap_sensing.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from bma220.bma220 import BMA220
 
 try:
     from typing import Tuple
 except ImportError:
     pass
 
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __repo__ = "https://github.com/jposada202020/CircuitPython_BMA220.git"
 
 _CONF = const(0x1A)
 _TT_INFO = const(0x10)
 _TT_INFO2 = const(0x16)
 _INTERRUPTS = const(0x18)
```

### Comparing `circuitpython-bma220-0.3.0/circuitpython_bma220.egg-info/PKG-INFO` & `circuitpython-bma220-0.4.0/circuitpython_bma220.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-bma220
-Version: 0.3.0
+Version: 0.4.0
 Summary: BMA220 Bosch Circuitpython Driver library
 Author-email: "Jose D. Montoya" <jlib@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_BMA220
 Keywords: sensor,blinka,circuitpython,micropython,bma220,acceleration,digital,bosch,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-bma220-0.3.0/circuitpython_bma220.egg-info/SOURCES.txt` & `circuitpython-bma220-0.4.0/circuitpython_bma220.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 README.rst
 pyproject.toml
 requirements.txt
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
 .github/workflows/release_gh.yml
 .github/workflows/release_pypi.yml
+bma220/__init__.py
 bma220/bma220.py
 bma220/bma220_const.py
+bma220/bma220_orientation.py
 bma220/bma220_slope.py
 bma220/bma220_tap_sensing.py
 circuitpython_bma220.egg-info/PKG-INFO
 circuitpython_bma220.egg-info/SOURCES.txt
 circuitpython_bma220.egg-info/dependency_links.txt
 circuitpython_bma220.egg-info/requires.txt
 circuitpython_bma220.egg-info/top_level.txt
@@ -30,11 +32,12 @@
 docs/_static/extra_css.css.license
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/bma220_acc_range.py
 examples/bma220_double_tap_test.py
 examples/bma220_filter_bandwidth.py
 examples/bma220_latched_mode.py
+examples/bma220_orientation.py
 examples/bma220_simpletest.py
 examples/bma220_sleep_duration.py
 examples/bma220_slope_slope_sign.py
 examples/bma220_slope_test.py
```

### Comparing `circuitpython-bma220-0.3.0/docs/_static/Logo.png` & `circuitpython-bma220-0.4.0/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.3.0/docs/_static/favicon.ico` & `circuitpython-bma220-0.4.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.3.0/docs/conf.py` & `circuitpython-bma220-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.3.0/docs/examples.rst` & `circuitpython-bma220-0.4.0/docs/examples.rst`

 * *Files 4% similar despite different names*

```diff
@@ -60,12 +60,21 @@
 .. literalinclude:: ../examples/bma220_slope_slope_sign.py
     :caption: examples/bma220_slope_slope_sign.py
     :linenos:
 
 Double Tap Example
 --------------------
 
-Example showing the Double Tap Setting
+Example showing the Double Tap Mode
 
 .. literalinclude:: ../examples/bma220_double_tap_test.py
     :caption: examples/bma220_double_tap_test.py
     :linenos:
+
+Orientation Mode Example
+-------------------------
+
+Example showing the Orientation Mode
+
+.. literalinclude:: ../examples/bma220_orientation.py
+    :caption: examples/bma220_orientation.py
+    :linenos:
```

### Comparing `circuitpython-bma220-0.3.0/examples/bma220_acc_range.py` & `circuitpython-bma220-0.4.0/examples/bma220_acc_range.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.3.0/examples/bma220_double_tap_test.py` & `circuitpython-bma220-0.4.0/examples/bma220_double_tap_test.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.3.0/examples/bma220_filter_bandwidth.py` & `circuitpython-bma220-0.4.0/examples/bma220_filter_bandwidth.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.3.0/examples/bma220_latched_mode.py` & `circuitpython-bma220-0.4.0/examples/bma220_latched_mode.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.3.0/examples/bma220_sleep_duration.py` & `circuitpython-bma220-0.4.0/examples/bma220_sleep_duration.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.3.0/examples/bma220_slope_slope_sign.py` & `circuitpython-bma220-0.4.0/examples/bma220_slope_slope_sign.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bma220-0.3.0/pyproject.toml` & `circuitpython-bma220-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-bma220"
 description = "BMA220 Bosch Circuitpython Driver library"
-version = "0.3.0"
+version = "0.4.0"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "jlib@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_BMA220"}
 keywords = [
     "sensor",
```

