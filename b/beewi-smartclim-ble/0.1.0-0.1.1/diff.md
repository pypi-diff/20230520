# Comparing `tmp/beewi_smartclim_ble-0.1.0.tar.gz` & `tmp/beewi_smartclim_ble-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beewi_smartclim_ble-0.1.0.tar", max compression
+gzip compressed data, was "beewi_smartclim_ble-0.1.1.tar", max compression
```

## Comparing `beewi_smartclim_ble-0.1.0.tar` & `beewi_smartclim_ble-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-05-09 10:00:56.448175 beewi_smartclim_ble-0.1.0/LICENSE
--rw-r--r--   0        0        0     2477 2023-05-13 21:19:58.053147 beewi_smartclim_ble-0.1.0/README.md
--rw-r--r--   0        0        0     2256 2023-05-13 21:19:58.053147 beewi_smartclim_ble-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      101 2023-05-13 21:19:58.053147 beewi_smartclim_ble-0.1.0/src/smartclim_ble/__init__.py
--rw-r--r--   0        0        0     6718 2023-05-13 20:22:24.851408 beewi_smartclim_ble-0.1.0/src/smartclim_ble/parser.py
--rw-r--r--   0        0        0        0 2023-05-10 09:24:36.332678 beewi_smartclim_ble-0.1.0/src/smartclim_ble/py.typed
--rw-r--r--   0        0        0     3751 1970-01-01 00:00:00.000000 beewi_smartclim_ble-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-09 10:00:56.448175 beewi_smartclim_ble-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2477 2023-05-13 21:19:58.053147 beewi_smartclim_ble-0.1.1/README.md
+-rw-r--r--   0        0        0     2257 2023-05-20 12:32:27.853828 beewi_smartclim_ble-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-05-20 12:32:27.853828 beewi_smartclim_ble-0.1.1/src/smartclim_ble/__init__.py
+-rw-r--r--   0        0        0     6768 2023-05-20 12:32:27.853828 beewi_smartclim_ble-0.1.1/src/smartclim_ble/parser.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:24:36.332678 beewi_smartclim_ble-0.1.1/src/smartclim_ble/py.typed
+-rw-r--r--   0        0        0     3752 1970-01-01 00:00:00.000000 beewi_smartclim_ble-0.1.1/PKG-INFO
```

### Comparing `beewi_smartclim_ble-0.1.0/LICENSE` & `beewi_smartclim_ble-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `beewi_smartclim_ble-0.1.0/README.md` & `beewi_smartclim_ble-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `beewi_smartclim_ble-0.1.0/pyproject.toml` & `beewi_smartclim_ble-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "beewi-smartclim-ble"
-version = "0.1.0"
+version = "0.1.1"
 description = "Parser for the BeeWi SmartClim device"
 authors = ["f-davin <none@none.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/f-davin/hassis_beewi_smartclim.git"
 classifiers = [
-    "Development Status :: 1 - Planning",
+    "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries",
 ]
 packages = [
     { include = "smartclim_ble", from = "src" },
```

### Comparing `beewi_smartclim_ble-0.1.0/src/smartclim_ble/parser.py` & `beewi_smartclim_ble-0.1.1/src/smartclim_ble/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Parser for BeeWi SmartClim BLE devices"""
+"""Parser for BeeWi SmartClim BLE devices."""
 
 import re
 from dataclasses import dataclass
 from datetime import datetime
 
 from bleak import BleakClient
 from bleak.backends.device import BLEDevice
@@ -16,16 +16,16 @@
     serial: str = ""
     fw_revision: str = ""
     hw_revision: str = ""
     soft_revision: str = ""
 
 
 @dataclass
-class SensorData:
-    """Data to store the information about the sensor"""
+class SmartClimSensorData:
+    """Data to store the information about the sensor."""
 
     # Constants
     __CONNECTED_DATA_SIZE = 10
     __ADVERTISING_DATA_SIZE = 11
     __ADVERTISING_MANUFACTURING_DATA_KEY = 13
 
     name: str = ""
@@ -66,15 +66,15 @@
             temp = temp - 0xFFFF
         self.temperature = temp / 10.0
         self.humidity = raw_data[4 + offset]
         self.battery = raw_data[9 + offset]
 
     def supported_data(self, adv_data: AdvertisementData) -> bool:
         """
-        Check if the advertisement frame received correspond to BeeWi SmartClim frame
+        Check if the advertisement frame received correspond to BeeWi SmartClim frame.
 
         Args:
             adv_data (AdvertisementData): Frame received
 
         Returns:
             bool: True if corresponding, false otherwise
         """
@@ -90,15 +90,15 @@
                 and bytes_data[0] == 0x05
             ):
                 ret = True
         return ret
 
     def get_manufacturing_data(self, adv_data: AdvertisementData) -> bytearray:
         """
-        Get the manufacturing data from the manufacturing frame
+        Get the manufacturing data from the manufacturing frame.Z
 
         Args:
             adv_data (AdvertisementData): Frame with data
 
         Raises:
             Exception: Invalid data detected
 
@@ -114,15 +114,15 @@
 
 
 @dataclass
 class BeeWiSmartClimAdvertisement:
     """Class to realize the treatment of an advertising frame."""
 
     device: BLEDevice = None
-    readings: SensorData = SensorData()
+    readings: SmartClimSensorData = SmartClimSensorData()
 
     def __init__(
         self,
         device: BLEDevice = None,
         ad_data: AdvertisementData = None,
     ):
         """Constructor."""
@@ -175,17 +175,17 @@
         self.manufacturer_data.hw_revision = await self.device.read_gatt_char(
             self.UUID_HARDWARE_REV
         )
         self.manufacturer_data.soft_revision = await self.device.read_gatt_char(
             self.UUID_SOFTWARE_REV
         )
 
-    async def current_readings(self) -> SensorData:
+    async def current_readings(self) -> SmartClimSensorData:
         """Extract current readings from remote device"""
-        readings = SensorData()
+        readings = SmartClimSensorData()
         values = await self.device.read_gatt_char(self.UUID_GET_VALUES)
         readings.decode(values, False)
         self.last_values_read = datetime.now()
         return readings
 
     async def get_seconds_since_update(self) -> int:
         """
```

### Comparing `beewi_smartclim_ble-0.1.0/PKG-INFO` & `beewi_smartclim_ble-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: beewi-smartclim-ble
-Version: 0.1.0
+Version: 0.1.1
 Summary: Parser for the BeeWi SmartClim device
 Home-page: https://github.com/f-davin/hassis_beewi_smartclim.git
 License: MIT
 Author: f-davin
 Author-email: none@none.com
 Requires-Python: >=3.9,<4.0
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

