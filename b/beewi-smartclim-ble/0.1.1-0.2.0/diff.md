# Comparing `tmp/beewi_smartclim_ble-0.1.1.tar.gz` & `tmp/beewi_smartclim_ble-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beewi_smartclim_ble-0.1.1.tar", max compression
+gzip compressed data, was "beewi_smartclim_ble-0.2.0.tar", max compression
```

## Comparing `beewi_smartclim_ble-0.1.1.tar` & `beewi_smartclim_ble-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-05-09 10:00:56.448175 beewi_smartclim_ble-0.1.1/LICENSE
--rw-r--r--   0        0        0     2477 2023-05-13 21:19:58.053147 beewi_smartclim_ble-0.1.1/README.md
--rw-r--r--   0        0        0     2257 2023-05-20 12:32:27.853828 beewi_smartclim_ble-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      122 2023-05-20 12:32:27.853828 beewi_smartclim_ble-0.1.1/src/smartclim_ble/__init__.py
--rw-r--r--   0        0        0     6768 2023-05-20 12:32:27.853828 beewi_smartclim_ble-0.1.1/src/smartclim_ble/parser.py
--rw-r--r--   0        0        0        0 2023-05-10 09:24:36.332678 beewi_smartclim_ble-0.1.1/src/smartclim_ble/py.typed
--rw-r--r--   0        0        0     3752 1970-01-01 00:00:00.000000 beewi_smartclim_ble-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-20 15:16:55.204539 beewi_smartclim_ble-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2477 2023-05-20 15:16:55.204539 beewi_smartclim_ble-0.2.0/README.md
+-rw-r--r--   0        0        0     2257 2023-05-20 15:16:56.276544 beewi_smartclim_ble-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-05-20 15:16:56.220544 beewi_smartclim_ble-0.2.0/src/smartclim_ble/__init__.py
+-rw-r--r--   0        0        0     6707 2023-05-20 15:16:55.204539 beewi_smartclim_ble-0.2.0/src/smartclim_ble/parser.py
+-rw-r--r--   0        0        0        0 2023-05-20 15:16:55.204539 beewi_smartclim_ble-0.2.0/src/smartclim_ble/py.typed
+-rw-r--r--   0        0        0     3752 1970-01-01 00:00:00.000000 beewi_smartclim_ble-0.2.0/PKG-INFO
```

### Comparing `beewi_smartclim_ble-0.1.1/LICENSE` & `beewi_smartclim_ble-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `beewi_smartclim_ble-0.1.1/README.md` & `beewi_smartclim_ble-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `beewi_smartclim_ble-0.1.1/pyproject.toml` & `beewi_smartclim_ble-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beewi-smartclim-ble"
-version = "0.1.1"
+version = "0.2.0"
 description = "Parser for the BeeWi SmartClim device"
 authors = ["f-davin <none@none.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/f-davin/hassis_beewi_smartclim.git"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
```

### Comparing `beewi_smartclim_ble-0.1.1/src/smartclim_ble/parser.py` & `beewi_smartclim_ble-0.2.0/src/smartclim_ble/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,62 +131,61 @@
         if device and ad_data:
             self.readings.name = device.name
             data = self.readings.get_manufacturing_data(ad_data)
             self.readings.decode(data, True)
 
 
 class BeeWiSmartClim:
-    # Param return value if no data
-    AR4_NO_DATA_FOR_PARAM = -1
-
-    UUID_MANUFACTURER_NAME = "00002a29-0000-1000-8000-00805f9b34fb"  # Handle 0x0025
-    UUID_SOFTWARE_REV = "00002a28-0000-1000-8000-00805f9b34fb"  # Handle 0x0023
-    UUID_SERIAL_NUMBER = "00002a25-0000-1000-8000-00805f9b34fb"  # Handle 0x001d
-    UUID_MODEL = "00002a24-0000-1000-8000-00805f9b34fb"  # Handle 0x001b
-    UUID_FIRMWARE_REV = "00002a26-0000-1000-8000-00805f9b34fb"  # Handle 0x001f
-    UUID_HARDWARE_REV = "00002a27-0000-1000-8000-00805f9b34fb"  # Handle 0X0021
-    UUID_GET_VALUES = "a8b3fb43-4834-4051-89d0-3de95cddd318"  # Handle 0x003f
+    __UUID_MANUFACTURER_NAME = "00002a29-0000-1000-8000-00805f9b34fb"  # Handle 0x0025
+    __UUID_SOFTWARE_REV = "00002a28-0000-1000-8000-00805f9b34fb"  # Handle 0x0023
+    __UUID_SERIAL_NUMBER = "00002a25-0000-1000-8000-00805f9b34fb"  # Handle 0x001d
+    __UUID_MODEL = "00002a24-0000-1000-8000-00805f9b34fb"  # Handle 0x001b
+    __UUID_FIRMWARE_REV = "00002a26-0000-1000-8000-00805f9b34fb"  # Handle 0x001f
+    __UUID_HARDWARE_REV = "00002a27-0000-1000-8000-00805f9b34fb"  # Handle 0X0021
+    __UUID_GET_VALUES = "a8b3fb43-4834-4051-89d0-3de95cddd318"  # Handle 0x003f
 
     # Regexp
-    REGEX_MAC = "([0-9a-f]{2}[:-]){5}([0-9a-f]{2})"
-    REGEX_UUID = "[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}"
-    REGEX_ADDR = f"({REGEX_MAC})|({REGEX_UUID})"
+    __REGEX_MAC = "([0-9a-f]{2}[:-]){5}([0-9a-f]{2})"
+    __REGEX_ID = r"^\d{18}$"
+    __REGEX_ADDR = f"({__REGEX_MAC})|({__REGEX_ID})"
 
     def __init__(self, address: str):
-        if not re.match(self.REGEX_ADDR, address.lower()):
+        if not re.match(self.__REGEX_ADDR, address.lower()):
             raise Exception("Invalid device address")
 
         self.address = address
         self.device = BleakClient(address)
         self.reading: bool = True
         self.manufacturer_data: ManufacturerData = ManufacturerData()
         self.last_values_read: datetime = datetime.now()
 
-    async def read_manufactoring_data(self) -> None:
+    async def read_manufacturing_data(self) -> None:
         """Read the data from the manufacturer."""
-        manufacturer = await self.device.read_gatt_char(self.UUID_MANUFACTURER_NAME)
+        manufacturer = await self.device.read_gatt_char(self.__UUID_MANUFACTURER_NAME)
         self.manufacturer_data.manufacturer = manufacturer
-        self.manufacturer_data.model = await self.device.read_gatt_char(self.UUID_MODEL)
+        self.manufacturer_data.model = await self.device.read_gatt_char(
+            self.__UUID_MODEL
+        )
         self.manufacturer_data.serial = await self.device.read_gatt_char(
-            self.UUID_SERIAL_NUMBER
+            self.__UUID_SERIAL_NUMBER
         )
         self.manufacturer_data.fw_revision = await self.device.read_gatt_char(
-            self.UUID_FIRMWARE_REV
+            self.__UUID_FIRMWARE_REV
         )
         self.manufacturer_data.hw_revision = await self.device.read_gatt_char(
-            self.UUID_HARDWARE_REV
+            self.__UUID_HARDWARE_REV
         )
         self.manufacturer_data.soft_revision = await self.device.read_gatt_char(
-            self.UUID_SOFTWARE_REV
+            self.__UUID_SOFTWARE_REV
         )
 
     async def current_readings(self) -> SmartClimSensorData:
         """Extract current readings from remote device"""
         readings = SmartClimSensorData()
-        values = await self.device.read_gatt_char(self.UUID_GET_VALUES)
+        values = await self.device.read_gatt_char(self.__UUID_GET_VALUES)
         readings.decode(values, False)
         self.last_values_read = datetime.now()
         return readings
 
     async def get_seconds_since_update(self) -> int:
         """
         Get the value for how long (in seconds) has passed since last
```

### Comparing `beewi_smartclim_ble-0.1.1/PKG-INFO` & `beewi_smartclim_ble-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beewi-smartclim-ble
-Version: 0.1.1
+Version: 0.2.0
 Summary: Parser for the BeeWi SmartClim device
 Home-page: https://github.com/f-davin/hassis_beewi_smartclim.git
 License: MIT
 Author: f-davin
 Author-email: none@none.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

