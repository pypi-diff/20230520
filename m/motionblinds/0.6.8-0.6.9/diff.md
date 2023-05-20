# Comparing `tmp/motionblinds-0.6.8.tar.gz` & `tmp/motionblinds-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\motionblinds-0.6.8.tar", last modified: Wed Jun  1 07:29:45 2022, max compression
+gzip compressed data, was "motionblinds-0.6.9.tar", last modified: Wed Jun 29 10:55:07 2022, max compression
```

## Comparing `motionblinds-0.6.8.tar` & `motionblinds-0.6.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-06-01 07:29:45.242513 motionblinds-0.6.8/
--rw-rw-rw-   0        0        0     1090 2022-02-23 14:14:50.000000 motionblinds-0.6.8/LICENSE
--rw-rw-rw-   0        0        0    26382 2022-06-01 07:29:45.242513 motionblinds-0.6.8/PKG-INFO
--rw-rw-rw-   0        0        0    25562 2022-05-13 10:17:38.000000 motionblinds-0.6.8/README.md
-drwxrwxrwx   0        0        0        0 2022-06-01 07:29:45.242513 motionblinds-0.6.8/motionblinds/
--rw-rw-rw-   0        0        0      812 2022-06-01 07:16:35.000000 motionblinds-0.6.8/motionblinds/__init__.py
--rw-rw-rw-   0        0        0     4658 2022-05-13 10:17:38.000000 motionblinds-0.6.8/motionblinds/async_motion_blinds.py
--rw-rw-rw-   0        0        0    64478 2022-06-01 06:39:19.000000 motionblinds-0.6.8/motionblinds/motion_blinds.py
-drwxrwxrwx   0        0        0        0 2022-06-01 07:29:45.242513 motionblinds-0.6.8/motionblinds.egg-info/
--rw-rw-rw-   0        0        0    26382 2022-06-01 07:29:44.000000 motionblinds-0.6.8/motionblinds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2022-06-01 07:29:44.000000 motionblinds-0.6.8/motionblinds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-01 07:29:44.000000 motionblinds-0.6.8/motionblinds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-06-01 07:29:44.000000 motionblinds-0.6.8/motionblinds.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2022-06-01 07:29:44.000000 motionblinds-0.6.8/motionblinds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-06-01 07:29:44.000000 motionblinds-0.6.8/motionblinds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-06-01 07:29:45.258139 motionblinds-0.6.8/setup.cfg
--rw-rw-rw-   0        0        0     1367 2022-06-01 07:16:42.000000 motionblinds-0.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-06-29 10:55:07.015624 motionblinds-0.6.9/
+-rw-rw-rw-   0        0        0     1069 2020-11-30 22:37:07.000000 motionblinds-0.6.9/LICENSE
+-rw-rw-rw-   0        0        0    26386 2022-06-29 10:55:07.015624 motionblinds-0.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0    25562 2022-05-07 11:47:51.000000 motionblinds-0.6.9/README.md
+drwxrwxrwx   0        0        0        0 2022-06-29 10:55:07.006623 motionblinds-0.6.9/motionblinds/
+-rw-rw-rw-   0        0        0      812 2022-06-29 10:52:45.000000 motionblinds-0.6.9/motionblinds/__init__.py
+-rw-rw-rw-   0        0        0     4658 2022-04-11 15:35:58.000000 motionblinds-0.6.9/motionblinds/async_motion_blinds.py
+-rw-rw-rw-   0        0        0    64834 2022-06-29 10:50:03.000000 motionblinds-0.6.9/motionblinds/motion_blinds.py
+drwxrwxrwx   0        0        0        0 2022-06-29 10:55:07.013627 motionblinds-0.6.9/motionblinds.egg-info/
+-rw-rw-rw-   0        0        0    26386 2022-06-29 10:55:05.000000 motionblinds-0.6.9/motionblinds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2022-06-29 10:55:06.000000 motionblinds-0.6.9/motionblinds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-06-29 10:55:05.000000 motionblinds-0.6.9/motionblinds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2020-11-13 15:16:09.000000 motionblinds-0.6.9/motionblinds.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2022-06-29 10:55:06.000000 motionblinds-0.6.9/motionblinds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2022-06-29 10:55:06.000000 motionblinds-0.6.9/motionblinds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-06-29 10:55:07.015624 motionblinds-0.6.9/setup.cfg
+-rw-rw-rw-   0        0        0     1367 2022-06-29 10:52:36.000000 motionblinds-0.6.9/setup.py
```

### Comparing `motionblinds-0.6.8/LICENSE` & `motionblinds-0.6.9/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2020 starkillerOG
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2020 starkillerOG
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `motionblinds-0.6.8/PKG-INFO` & `motionblinds-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motionblinds
-Version: 0.6.8
+Version: 0.6.9
 Summary: Python library for interfacing with Motion Blinds
 Home-page: https://github.com/starkillerOG/motion-blinds
 Author: starkillerOG
 Author-email: starkiller.og@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -314,7 +314,9 @@
 | "blind_1.battery_voltage" | {"T": double, "B": double}              | Return the current battery voltage of the blind in V                                                    |
 | "blind_1.battery_level"   | {"T": double, "B": double}              | Return the current battery level of the blind in %                                                      |
 | "blind_1.RSSI"            | int                                     | Return the radio connection strength of the blind to the gateway in dBm                                 |
 | "blind_1.wireless_mode"   | enum                                    | Return the wireless mode of the blind as a WirelessMode enum                                            |
 | "blind_1.wireless_name"   | string                                  | Return the wireless mode of the blind from WirelessMode enum                                            |
 | "blind_1.voltage_mode"    | enum                                    | Return the voltage mode of the blind as a VoltageMode enum                                              |
 | "blind_1.voltage_name"    | string                                  | Return the voltage mode of the blind from VoltageMode enum                                              |
+
+
```

### Comparing `motionblinds-0.6.8/README.md` & `motionblinds-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `motionblinds-0.6.8/motionblinds/__init__.py` & `motionblinds-0.6.9/motionblinds/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # Set default logging handler to avoid "No handler found" warnings.
 import logging
 
 logging.getLogger(__name__)
 
 __title__ = "motion-blinds"
-__version__ = "0.6.8"
+__version__ = "0.6.9"
 
 # Import motion_blinds module
 from .motion_blinds import MotionGateway
 from .motion_blinds import MotionMulticast
 from .motion_blinds import MotionDiscovery
 from .motion_blinds import BlindType
 from .motion_blinds import WirelessMode
```

### Comparing `motionblinds-0.6.8/motionblinds/async_motion_blinds.py` & `motionblinds-0.6.9/motionblinds/async_motion_blinds.py`

 * *Files identical despite different names*

### Comparing `motionblinds-0.6.8/motionblinds/motion_blinds.py` & `motionblinds-0.6.9/motionblinds/motion_blinds.py`

 * *Files 0% similar despite different names*

```diff
@@ -503,14 +503,20 @@
             if response.get("actionResult") is not None:
                 _LOGGER.error(
                     "Received actionResult: '%s', when sending message: '%s', got response: '%s'",
                     response.get("actionResult"),
                     log_hide(message),
                     log_hide(response),
                 )
+                if response.get("token") is not None:
+                    # check for token change
+                    if self._token != response["token"]:
+                        _LOGGER.warning("Gateway token has changed from actionResult.")
+                        self._token = response["token"]
+                        self._access_token = None
 
         if single_response:
             return responses[0]
 
         return responses
 
     def _read_subdevice(self, mac, device_type):
```

### Comparing `motionblinds-0.6.8/motionblinds.egg-info/PKG-INFO` & `motionblinds-0.6.9/motionblinds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motionblinds
-Version: 0.6.8
+Version: 0.6.9
 Summary: Python library for interfacing with Motion Blinds
 Home-page: https://github.com/starkillerOG/motion-blinds
 Author: starkillerOG
 Author-email: starkiller.og@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -314,7 +314,9 @@
 | "blind_1.battery_voltage" | {"T": double, "B": double}              | Return the current battery voltage of the blind in V                                                    |
 | "blind_1.battery_level"   | {"T": double, "B": double}              | Return the current battery level of the blind in %                                                      |
 | "blind_1.RSSI"            | int                                     | Return the radio connection strength of the blind to the gateway in dBm                                 |
 | "blind_1.wireless_mode"   | enum                                    | Return the wireless mode of the blind as a WirelessMode enum                                            |
 | "blind_1.wireless_name"   | string                                  | Return the wireless mode of the blind from WirelessMode enum                                            |
 | "blind_1.voltage_mode"    | enum                                    | Return the voltage mode of the blind as a VoltageMode enum                                              |
 | "blind_1.voltage_name"    | string                                  | Return the voltage mode of the blind from VoltageMode enum                                              |
+
+
```

### Comparing `motionblinds-0.6.8/setup.py` & `motionblinds-0.6.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(name='motionblinds',
-      version='0.6.8',
+      version='0.6.9',
       description='Python library for interfacing with Motion Blinds',
       long_description=README,
       long_description_content_type="text/markdown",
       url='https://github.com/starkillerOG/motion-blinds',
       author='starkillerOG',
       author_email='starkiller.og@gmail.com',
       license='MIT',
```

