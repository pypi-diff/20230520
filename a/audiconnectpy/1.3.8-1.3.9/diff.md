# Comparing `tmp/audiconnectpy-1.3.8.tar.gz` & `tmp/audiconnectpy-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-1.3.8.tar", last modified: Sat May 20 12:00:47 2023, max compression
+gzip compressed data, was "audiconnectpy-1.3.9.tar", last modified: Sat May 20 13:41:46 2023, max compression
```

## Comparing `audiconnectpy-1.3.8.tar` & `audiconnectpy-1.3.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:00:47.930325 audiconnectpy-1.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-20 12:00:36.000000 audiconnectpy-1.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-20 12:00:36.000000 audiconnectpy-1.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-20 12:00:47.930325 audiconnectpy-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-20 12:00:36.000000 audiconnectpy-1.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:00:47.930325 audiconnectpy-1.3.8/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-20 12:00:36.000000 audiconnectpy-1.3.8/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-20 12:00:36.000000 audiconnectpy-1.3.8/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22701 2023-05-20 12:00:36.000000 audiconnectpy-1.3.8/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-20 12:00:36.000000 audiconnectpy-1.3.8/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-20 12:00:36.000000 audiconnectpy-1.3.8/audiconnectpy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    29017 2023-05-20 12:00:36.000000 audiconnectpy-1.3.8/audiconnectpy/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    32065 2023-05-20 12:00:36.000000 audiconnectpy-1.3.8/audiconnectpy/services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:00:47.930325 audiconnectpy-1.3.8/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-20 12:00:47.000000 audiconnectpy-1.3.8/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-20 12:00:47.000000 audiconnectpy-1.3.8/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 12:00:47.000000 audiconnectpy-1.3.8/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 12:00:47.000000 audiconnectpy-1.3.8/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-20 12:00:47.000000 audiconnectpy-1.3.8/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-20 12:00:36.000000 audiconnectpy-1.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 12:00:47.930325 audiconnectpy-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-20 12:00:46.000000 audiconnectpy-1.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:00:47.930325 audiconnectpy-1.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-20 12:00:36.000000 audiconnectpy-1.3.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:41:46.065297 audiconnectpy-1.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-20 13:41:36.000000 audiconnectpy-1.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-20 13:41:36.000000 audiconnectpy-1.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-20 13:41:46.061297 audiconnectpy-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-20 13:41:36.000000 audiconnectpy-1.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:41:46.061297 audiconnectpy-1.3.9/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-20 13:41:36.000000 audiconnectpy-1.3.9/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-20 13:41:36.000000 audiconnectpy-1.3.9/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22837 2023-05-20 13:41:36.000000 audiconnectpy-1.3.9/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-20 13:41:36.000000 audiconnectpy-1.3.9/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-20 13:41:36.000000 audiconnectpy-1.3.9/audiconnectpy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27196 2023-05-20 13:41:36.000000 audiconnectpy-1.3.9/audiconnectpy/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32069 2023-05-20 13:41:36.000000 audiconnectpy-1.3.9/audiconnectpy/services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:41:46.061297 audiconnectpy-1.3.9/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-20 13:41:46.000000 audiconnectpy-1.3.9/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-20 13:41:46.000000 audiconnectpy-1.3.9/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 13:41:46.000000 audiconnectpy-1.3.9/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 13:41:46.000000 audiconnectpy-1.3.9/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-20 13:41:46.000000 audiconnectpy-1.3.9/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-20 13:41:36.000000 audiconnectpy-1.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 13:41:46.065297 audiconnectpy-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-20 13:41:45.000000 audiconnectpy-1.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:41:46.061297 audiconnectpy-1.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-20 13:41:36.000000 audiconnectpy-1.3.9/tests/__init__.py
```

### Comparing `audiconnectpy-1.3.8/LICENSE` & `audiconnectpy-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.8/PKG-INFO` & `audiconnectpy-1.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.3.8
+Version: 1.3.9
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.3.8/README.md` & `audiconnectpy-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.8/audiconnectpy/api.py` & `audiconnectpy-1.3.9/audiconnectpy/api.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.8/audiconnectpy/auth.py` & `audiconnectpy-1.3.9/audiconnectpy/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 from .exceptions import (
     AudiException,
     HttpRequestError,
     ServiceNotFoundError,
     TimeoutExceededError,
 )
-from .helpers import json_loads
+from .helpers import ExtendedDict, json_loads
 
 TIMEOUT = 120
 DELAY = 10
 HDR_XAPP_VERSION = "4.13.0"
 HDR_USER_AGENT = "myAudi-Android/4.13.0 (Build 800238275.2210271555) Android/11"
 MARKET_URL = "https://content.app.my.audi.com/service/mobileapp/configurations"
 CLIENT_ID = "09b6cbec-cd19-4589-82fd-363dfa8c24da@apps_vw-dilab_com"
@@ -96,36 +96,38 @@
                 "Timeout occurred while connecting to Audi Connect."
             ) from error
         except (aiohttp.ClientError, socket.gaierror) as error:
             raise HttpRequestError(
                 "Error occurred while communicating with Audit Connect."
             ) from error
 
+        content_type = response.headers.get("Content-Type", "")
+        contents = (await response.read()).decode("utf8")
+
         _LOGGER.debug("RESPONSE HEADERS: %s", response.headers)
-        _LOGGER.debug(
-            "RESPONSE: %s ,return_code '%s'",
-            (await response.read()).decode("utf8"),
-            response.status,
-        )
+        _LOGGER.debug("RESPONSE: %s ,return_code '%s'", contents, response.status)
 
-        content_type = response.headers.get("Content-Type", "")
         if response.status // 100 in [4, 5]:
-            contents = await response.read()
             response.close()
-            if content_type == "application/json":
-                raise ServiceNotFoundError(
-                    response.status, json.loads(contents.decode("utf8"))
-                )
-            raise ServiceNotFoundError(response.status, contents.decode("utf8"))
+            if "application/json" in content_type:
+                raise ServiceNotFoundError(response.status, json.loads(contents))
+            raise ServiceNotFoundError(response.status, contents)
 
         if raw_reply and raw_rsp is False:
             return response
 
         if "application/json" in content_type:
             rsp = await response.json(loads=json_loads)
+        elif (
+            headers
+            and "application/json" in headers.get("Accept", "")
+            and contents is None
+        ):
+            _LOGGER.debug("JSON FIX: Accept is JSON but Response is None")
+            rsp = ExtendedDict({})
         else:
             rsp = await response.text()
 
         if raw_reply and raw_rsp:
             return response, rsp
         return rsp
```

### Comparing `audiconnectpy-1.3.8/audiconnectpy/helpers.py` & `audiconnectpy-1.3.9/audiconnectpy/helpers.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.8/audiconnectpy/models.py` & `audiconnectpy-1.3.9/audiconnectpy/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Definition class."""
 from __future__ import annotations
 
 import logging
 from dataclasses import dataclass
 from datetime import datetime as dt
-from typing import TYPE_CHECKING, Any, Literal
+from typing import TYPE_CHECKING, Literal
 
 from .exceptions import HttpRequestError, ServiceNotFoundError, TimeoutExceededError
 from .helpers import ExtendedDict, retry
 
 if TYPE_CHECKING:
     from .services import AudiService
 
@@ -125,27 +125,27 @@
 
     @property
     def is_supported(self) -> bool:
         """Supported status."""
         return self.attributes is not None
 
     @property
-    def attributes(self) -> Any:
+    def attributes(self) -> ExtendedDict:
         """Attributes properties."""
         return self._vehicle_data
 
-    def _get_attributes(self) -> dict[str, Any]:
-        attrs: dict[str, Any] = {"last_access": dt.now()}
+    def _get_attributes(self) -> ExtendedDict:
+        attrs = ExtendedDict({"last_access": dt.now()})
 
         default = self.data.getr("CurrentVehicleDataByRequestResponse.vehicleData.data")
         vehicle_data = self.data.getr(
             "StoredVehicleDataResponse.vehicleData.data", default
         )
         if vehicle_data is None:
-            return attrs
+            return ExtendedDict(attrs)
 
         for raw_data in vehicle_data:
             for raw_field in raw_data.get("field", {}):
                 ids = raw_field.get("id")
                 value = raw_field.get("value")
                 unit = raw_field.get("unit")
                 if ids == "0x0101010001":
@@ -173,16 +173,16 @@
 
         # Append meta sensors
         attrs.update(self._metadatas(attrs))
 
         return attrs
 
     @staticmethod
-    def _metadatas(attrs: dict[str, Any]) -> dict[str, Any]:
-        metadatas: dict[str, Any] = {}
+    def _metadatas(attrs: ExtendedDict) -> ExtendedDict:
+        metadatas = ExtendedDict({})
 
         # Windows open status
         left_check: int | None = attrs.get("state_left_front_window")
         left_rear_check: int | None = attrs.get("state_left_rear_window")
         right_check: int | None = attrs.get("state_right_front_window")
         right_rear_check: int | None = attrs.get("state_right_rear_window")
         if None not in [left_check, left_rear_check, right_check, right_rear_check]:
@@ -267,264 +267,222 @@
     """Preheater class."""
 
     data: ExtendedDict
 
     @property
     def is_supported(self) -> bool:
         """Supported status."""
-        if not isinstance(self.data, ExtendedDict):
-            _LOGGER.warning("Preheater format is incorrect %s", self.data)  # type: ignore
         return self.data.getr("statusResponse.climatisationStateReport") is not None
 
     @property
-    def attributes(self) -> dict[str, Any]:
+    def attributes(self) -> ExtendedDict:
         """Attributes properties."""
-        attrs: dict[str, Any] = {}
-        if isinstance(self.data, ExtendedDict):
-            report: ExtendedDict = self.data.getr(
-                "statusResponse.climatisationStateReport", {}
-            )
-            attrs = {
-                "preheater_state": report,
-                "preheater_active": report.get("climatisationState"),
-                "preheater_duration": report.get("climatisationDuration"),
-                "preheater_remaining": report.get("remainingClimateTime"),
-            }
-        return attrs
+        report: ExtendedDict = self.data.getr(
+            "statusResponse.climatisationStateReport", {}
+        )
+        attrs = {
+            "preheater_state": report,
+            "preheater_active": report.get("climatisationState"),
+            "preheater_duration": report.get("climatisationDuration"),
+            "preheater_remaining": report.get("remainingClimateTime"),
+        }
+        return ExtendedDict(attrs)
 
 
 @dataclass
 class ChargerDataResponse:
     """Charger class."""
 
     data: ExtendedDict
 
     @property
     def is_supported(self) -> bool:
         """Supported status."""
-        if not isinstance(self.data, ExtendedDict):
-            _LOGGER.warning("Charger format is incorrect %s", self.data)  # type: ignore
         return (
             self.data.getr("charger.settings") is not None
             or self.data.getr("charger.status") is not None
         )
 
     @property
-    def attributes(self) -> dict[str, Any]:
+    def attributes(self) -> ExtendedDict:
         """Attributes properties."""
-        attrs = {}
-        if isinstance(self.data, ExtendedDict):
-            settings = self.data.getr("charger.settings", {})
-            status = self.data.getr("charger.status", {})
-            charging = status.get("chargingStatusData", {})
-            cruising = status.get("cruisingRangeStatusData", {})
-            attrs = {
-                "max_charge_current": settings.getr("maxChargeCurrent.content"),
-                "charging_state": charging.getr("chargingState.content"),
-                "actual_charge_rate": charging.getr("actualChargeRate.content"),
-                "actual_charge_rate_unit": charging.getr("chargeRateUnit.content"),
-                "charging_power": charging.getr("chargingPower.content"),
-                "charging_mode": charging.getr("chargingMode.content"),
-                "energy_flow": charging.getr("energyFlow.content"),
-                "primary_engine_type": cruising.getr("engineTypeFirstEngine.content"),
-                "secondary_engine_type": cruising.getr(
-                    "engineTypeSecondEngine.content"
-                ),
-                "hybrid_range": cruising.getr("hybridRange.content"),
-                "primary_engine_range": cruising.getr("primaryEngineRange.content"),
-                "secondary_engine_range": cruising.getr("secondaryEngineRange.content"),
-                "state_of_charge": status.getr(
-                    "batteryStatusData.stateOfCharge.content"
-                ),
-                "plug_state": status.getr("plugStatusData.plugState.content"),
-                "plug_lock": status.getr("plugStatusData.lockState.content"),
-                "remaining_charging_time": status.getr(
-                    "batteryStatusData.remainingChargingTime.content"
-                ),
-            }
-        return attrs
+        settings = self.data.getr("charger.settings", {})
+        status = self.data.getr("charger.status", {})
+        charging = status.get("chargingStatusData", {})
+        cruising = status.get("cruisingRangeStatusData", {})
+        attrs = {
+            "max_charge_current": settings.getr("maxChargeCurrent.content"),
+            "charging_state": charging.getr("chargingState.content"),
+            "actual_charge_rate": charging.getr("actualChargeRate.content"),
+            "actual_charge_rate_unit": charging.getr("chargeRateUnit.content"),
+            "charging_power": charging.getr("chargingPower.content"),
+            "charging_mode": charging.getr("chargingMode.content"),
+            "energy_flow": charging.getr("energyFlow.content"),
+            "primary_engine_type": cruising.getr("engineTypeFirstEngine.content"),
+            "secondary_engine_type": cruising.getr("engineTypeSecondEngine.content"),
+            "hybrid_range": cruising.getr("hybridRange.content"),
+            "primary_engine_range": cruising.getr("primaryEngineRange.content"),
+            "secondary_engine_range": cruising.getr("secondaryEngineRange.content"),
+            "state_of_charge": status.getr("batteryStatusData.stateOfCharge.content"),
+            "plug_state": status.getr("plugStatusData.plugState.content"),
+            "plug_lock": status.getr("plugStatusData.lockState.content"),
+            "remaining_charging_time": status.getr(
+                "batteryStatusData.remainingChargingTime.content"
+            ),
+        }
+        return ExtendedDict(attrs)
 
 
 @dataclass
 class ClimaterDataResponse:
     """Climater class."""
 
     data: ExtendedDict
 
     @property
     def is_supported(self) -> bool:
         """Supported status."""
-        if not isinstance(self.data, ExtendedDict):
-            _LOGGER.warning("Climater format is incorrect %s", self.data)  # type: ignore
         return (
             self.data.getr("climater.settings") is not None
             or self.data.getr("climater.status") is not None
         )
 
     @property
-    def attributes(self) -> dict[str, Any]:
+    def attributes(self) -> ExtendedDict:
         """Attributes properties."""
-        attrs = {}
-        if isinstance(self.data, ExtendedDict):
-            settings = self.data.getr("climater.settings")
-            status = self.data.getr("climater.status")
-            attrs = {
-                "climatisation_state": status.getr(
-                    "climatisationStatusData.climatisationState.content"
-                ),
-                "outdoor_temperature": status.getr(
-                    "temperatureStatusData.outdoorTemperature.content"
-                ),
-                "climatisation_heater_src": settings.getr("heaterSource.content"),
-                "climatisation_target_temp": settings.getr("targetTemperature.content"),
-            }
-        return attrs
+        settings = self.data.getr("climater.settings", {})
+        status = self.data.getr("climater.status", {})
+        attrs = {
+            "climatisation_state": status.getr(
+                "climatisationStatusData.climatisationState.content"
+            ),
+            "outdoor_temperature": status.getr(
+                "temperatureStatusData.outdoorTemperature.content"
+            ),
+            "climatisation_heater_src": settings.getr("heaterSource.content"),
+            "climatisation_target_temp": settings.getr("targetTemperature.content"),
+        }
+        return ExtendedDict(attrs)
 
 
 @dataclass
 class DestinationDataResponse:
     """Destination."""
 
     data: ExtendedDict
 
     @property
     def is_supported(self) -> bool:
         """Supported status."""
         return self.attributes is not None
 
     @property
-    def attributes(self) -> dict[str, Any]:
+    def attributes(self) -> ExtendedDict:
         """Attributes properties."""
         attrs = self.data
-        return attrs
+        return ExtendedDict(attrs)
 
 
 @dataclass
 class HistoryDataResponse:
     """Destination."""
 
     data: ExtendedDict
 
     @property
     def is_supported(self) -> bool:
         """Supported status."""
         return self.attributes is not None
 
     @property
-    def attributes(self) -> dict[str, Any]:
+    def attributes(self) -> ExtendedDict:
         """Attributes properties."""
         attrs = self.data
-        return attrs
+        return ExtendedDict(attrs)
 
 
 @dataclass
 class UsersDataResponse:
     """Destination."""
 
     data: ExtendedDict
 
     @property
     def is_supported(self) -> bool:
         """Supported status."""
         return self.attributes is not None
 
     @property
-    def attributes(self) -> dict[str, Any]:
+    def attributes(self) -> ExtendedDict:
         """Attributes properties."""
         attrs = self.data
-        return attrs
+        return ExtendedDict(attrs)
 
 
 @dataclass
 class PositionDataResponse:
     """Position class."""
 
     data: ExtendedDict
 
     @property
     def is_supported(self) -> bool:
         """Supported status."""
-        if not isinstance(self.data, ExtendedDict):
-            _LOGGER.warning("Position format is incorrect %s", self.data)  # type: ignore
         return self.data.getr("findCarResponse.Position") is not None
 
     @property
-    def attributes(self) -> dict[str, Any]:
+    def attributes(self) -> ExtendedDict:
         """Attributes properties."""
-        attrs = {}
-        if isinstance(self.data, ExtendedDict) and (
-            coordinate := self.data.getr("findCarResponse.Position.carCoordinate")
-        ):
-            timestamp = self.data.getr("findCarResponse.Position.timestampCarSentUTC")
-            attrs = {
-                "position": {
-                    "latitude": coordinate["latitude"] / 1000000,
-                    "longitude": coordinate["longitude"] / 1000000,
+        coordinate = self.data.getr("findCarResponse.Position.carCoordinate", {})
+        timestamp = self.data.getr("findCarResponse.Position.timestampCarSentUTC")
+        attrs = {
+            "position": ExtendedDict(
+                {
+                    "latitude": coordinate.get("latitude", 0) / 1000000,
+                    "longitude": coordinate.get("longitude", 0) / 1000000,
                     "timestamp": timestamp,
                     "parktime": self.data.getr(
                         "findCarResponse.parkingTimeUTC", timestamp
                     ),
                 }
-            }
-        else:
-            _LOGGER.warning("Position format is incorrect %s", self.data)
-        return attrs
+            )
+        }
+        return ExtendedDict(attrs)
 
 
 @dataclass
 class TripDataResponse:
     """Trip class."""
 
     data: ExtendedDict
 
     @property
     def is_supported(self) -> bool:
         """Supported status."""
-        return self.data is not None
+        return self.data.get("tripID") is not None
 
     @property
-    def attributes(self) -> dict[str, Any]:
+    def attributes(self) -> ExtendedDict:
         """Attributes properties."""
-        trip_id = self.data["tripID"]
-        average_electricengine_consumption = (
-            (float(self.data["averageElectricEngineConsumption"]) / 10)
-            if "averageElectricEngineConsumption" in self.data
-            else None
-        )
-        average_fuel_consumption = (
-            float(self.data["averageFuelConsumption"]) / 10
-            if "averageFuelConsumption" in self.data
-            else None
-        )
-        average_speed = (
-            int(self.data["averageSpeed"]) if "averageSpeed" in self.data else None
-        )
-        mileage = int(self.data["mileage"]) if "mileage" in self.data else None
-        start_mileage = (
-            int(self.data["startMileage"]) if "startMileage" in self.data else None
-        )
-        travel_time = (
-            int(self.data["traveltime"]) if "traveltime" in self.data else None
-        )
-        timestamp = self.data["timestamp"] if "timestamp" in self.data else None
-        overall_mileage = (
-            int(self.data["overallMileage"]) if "overallMileage" in self.data else None
-        )
-
-        return {
-            "tripID": trip_id,
-            "averageElectricEngineConsumption": average_electricengine_consumption,
-            "averageFuelConsumption": average_fuel_consumption,
-            "averageSpeed": average_speed,
-            "mileage": mileage,
-            "startMileage": start_mileage,
-            "traveltime": travel_time,
-            "timestamp": timestamp,
-            "overallMileage": overall_mileage,
+        attrs = {
+            "tripID": self.data.get("tripID"),
+            "averageElectricEngineConsumption": (
+                float(self.data.get("averageElectricEngineConsumption", 0)) / 10
+            ),
+            "averageFuelConsumption": (
+                float(self.data.get("averageFuelConsumption", 0)) / 10
+            ),
+            "averageSpeed": int(self.data.get("averageSpeed", 0)),
+            "mileage": int(self.data.get("mileage", 0)),
+            "startMileage": int(self.data.get("startMileage", 0)),
+            "traveltime": int(self.data.get("traveltime", 0)),
+            "timestamp": self.data.get("timestamp"),
+            "overallMileage": int(self.data.get("overallMileage", 0)),
         }
+        return ExtendedDict(attrs)
 
 
 class Vehicle:
     """Vehicle class."""
 
     def __init__(self, data: ExtendedDict, audi_service: AudiService) -> None:
         """Initialize."""
```

### Comparing `audiconnectpy-1.3.8/audiconnectpy/services.py` & `audiconnectpy-1.3.9/audiconnectpy/services.py`

 * *Files 1% similar despite different names*

```diff
@@ -622,32 +622,28 @@
             "start window heating" if start else "stop window heating",
             SUCCEEDED,
             FAILED,
             "action.actionState",
         )
 
     async def set_control_duration(self, vin: str, duration: int) -> None:
-        """Set max current."""
+        """Set control duration."""
         self._control_duration[vin] = duration
 
     async def async_set_honkflash(
         self, vin: str, mode: Literal["honk", "flash"], duration: int = 15
     ) -> None:
         """Set honk and flash light."""
         # OpenHab "FLASH_ONLY","HONK_AND_FLASH"
         url = await self._async_get_home_region(vin.upper())
         rsp_position = await self._auth.get(
             f"{url}/bs/cf/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/position"
         )
-        position = (
-            rsp_position.get("findCarResponse", {})
-            .get("Position", {})
-            .get("carCoordinate")
-        )
-
+        rsp_position = rsp_position if rsp_position else ExtendedDict()
+        position = rsp_position.get("findCarResponse.Position.carCoordinate")
         headers = await self._auth.async_get_action_headers("application/json", None)
         data = {
             "honkAndFlashRequest": {
                 "serviceOperationCode": "HONK_AND_FLASH"
                 if mode == "honk"
                 else "FLASH_ONLY",
                 "serviceDuration": duration,
```

### Comparing `audiconnectpy-1.3.8/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-1.3.9/audiconnectpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.3.8
+Version: 1.3.9
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.3.8/pyproject.toml` & `audiconnectpy-1.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.8/setup.py` & `audiconnectpy-1.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="audiconnectpy",
-    version="1.3.8",
+    version="1.3.9",
     packages=find_packages(),
     author="cyr-ius",
     author_email="cyr-ius@ipocus.net",
     description="Provides asynchronous authentication and access to Audi Connect",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["aiohttp>=3.8.1", "beautifulsoup4>=4.11.2"],
```

