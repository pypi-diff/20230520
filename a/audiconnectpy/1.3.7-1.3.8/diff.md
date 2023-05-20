# Comparing `tmp/audiconnectpy-1.3.7.tar.gz` & `tmp/audiconnectpy-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-1.3.7.tar", last modified: Thu May 18 12:35:08 2023, max compression
+gzip compressed data, was "audiconnectpy-1.3.8.tar", last modified: Sat May 20 12:00:47 2023, max compression
```

## Comparing `audiconnectpy-1.3.7.tar` & `audiconnectpy-1.3.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:35:08.847831 audiconnectpy-1.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 12:34:59.000000 audiconnectpy-1.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-18 12:34:59.000000 audiconnectpy-1.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-18 12:35:08.847831 audiconnectpy-1.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-18 12:34:59.000000 audiconnectpy-1.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:35:08.847831 audiconnectpy-1.3.7/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-18 12:34:59.000000 audiconnectpy-1.3.7/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-18 12:34:59.000000 audiconnectpy-1.3.7/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22631 2023-05-18 12:34:59.000000 audiconnectpy-1.3.7/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-18 12:34:59.000000 audiconnectpy-1.3.7/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-18 12:34:59.000000 audiconnectpy-1.3.7/audiconnectpy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    29017 2023-05-18 12:34:59.000000 audiconnectpy-1.3.7/audiconnectpy/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    32808 2023-05-18 12:34:59.000000 audiconnectpy-1.3.7/audiconnectpy/services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:35:08.847831 audiconnectpy-1.3.7/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-18 12:35:08.000000 audiconnectpy-1.3.7/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-18 12:35:08.000000 audiconnectpy-1.3.7/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 12:35:08.000000 audiconnectpy-1.3.7/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 12:35:08.000000 audiconnectpy-1.3.7/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-18 12:35:08.000000 audiconnectpy-1.3.7/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-18 12:34:59.000000 audiconnectpy-1.3.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 12:35:08.847831 audiconnectpy-1.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-18 12:35:08.000000 audiconnectpy-1.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:35:08.847831 audiconnectpy-1.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-18 12:34:59.000000 audiconnectpy-1.3.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:00:47.930325 audiconnectpy-1.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-20 12:00:36.000000 audiconnectpy-1.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-20 12:00:36.000000 audiconnectpy-1.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-20 12:00:47.930325 audiconnectpy-1.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-20 12:00:36.000000 audiconnectpy-1.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:00:47.930325 audiconnectpy-1.3.8/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-20 12:00:36.000000 audiconnectpy-1.3.8/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-20 12:00:36.000000 audiconnectpy-1.3.8/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22701 2023-05-20 12:00:36.000000 audiconnectpy-1.3.8/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-20 12:00:36.000000 audiconnectpy-1.3.8/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-20 12:00:36.000000 audiconnectpy-1.3.8/audiconnectpy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29017 2023-05-20 12:00:36.000000 audiconnectpy-1.3.8/audiconnectpy/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32065 2023-05-20 12:00:36.000000 audiconnectpy-1.3.8/audiconnectpy/services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:00:47.930325 audiconnectpy-1.3.8/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-20 12:00:47.000000 audiconnectpy-1.3.8/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-20 12:00:47.000000 audiconnectpy-1.3.8/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 12:00:47.000000 audiconnectpy-1.3.8/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 12:00:47.000000 audiconnectpy-1.3.8/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-20 12:00:47.000000 audiconnectpy-1.3.8/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-20 12:00:36.000000 audiconnectpy-1.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 12:00:47.930325 audiconnectpy-1.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-20 12:00:46.000000 audiconnectpy-1.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:00:47.930325 audiconnectpy-1.3.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-20 12:00:36.000000 audiconnectpy-1.3.8/tests/__init__.py
```

### Comparing `audiconnectpy-1.3.7/LICENSE` & `audiconnectpy-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.7/PKG-INFO` & `audiconnectpy-1.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.3.7
+Version: 1.3.8
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.3.7/README.md` & `audiconnectpy-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.7/audiconnectpy/api.py` & `audiconnectpy-1.3.8/audiconnectpy/api.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.7/audiconnectpy/auth.py` & `audiconnectpy-1.3.8/audiconnectpy/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,28 +82,29 @@
         raw_reply: bool = False,
         raw_rsp: bool = False,
         **kwargs: Any,
     ) -> Any:
         """Request url with method."""
         try:
             async with async_timeout.timeout(TIMEOUT):
+                _LOGGER.debug("REQUEST HEADERS: %s", headers)
                 _LOGGER.debug("REQUEST: %s", url)
-                # _LOGGER.debug("HEADERS: %s", headers)
                 response = await self._session.request(
                     method, url, headers=headers, data=data, **kwargs
                 )
         except (asyncio.CancelledError, asyncio.TimeoutError) as error:
             raise TimeoutExceededError(
                 "Timeout occurred while connecting to Audi Connect."
             ) from error
         except (aiohttp.ClientError, socket.gaierror) as error:
             raise HttpRequestError(
                 "Error occurred while communicating with Audit Connect."
             ) from error
 
+        _LOGGER.debug("RESPONSE HEADERS: %s", response.headers)
         _LOGGER.debug(
             "RESPONSE: %s ,return_code '%s'",
             (await response.read()).decode("utf8"),
             response.status,
         )
 
         content_type = response.headers.get("Content-Type", "")
```

### Comparing `audiconnectpy-1.3.7/audiconnectpy/helpers.py` & `audiconnectpy-1.3.8/audiconnectpy/helpers.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.7/audiconnectpy/models.py` & `audiconnectpy-1.3.8/audiconnectpy/models.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.7/audiconnectpy/services.py` & `audiconnectpy-1.3.8/audiconnectpy/services.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,49 +50,47 @@
 
     async def async_get_vehicles(self) -> Any:
         """Get all vehicles."""
         url = await self._async_get_home_region("")
         data = await self._auth.get(
             f"{url}/usermanagement/users/v1/{self.brand}/{self.country}/vehicles"
         )
-        if not isinstance(data, ExtendedDict):
-            _LOGGER.warning("Format is incorrect %s", data)
+        data = data if data else ExtendedDict()
         return data
 
     async def async_get_vehicle_details(self, vin: str) -> Any:
         """Get vehicle data."""
         url = await self._async_get_home_region(vin.upper())
         accept = {
             "Accept": "application/vnd.vwg.mbb.vehicleDataDetail_v2_1_0+json, application/vnd.vwg.mbb.genericError_v1_0_2+json"
         }
         headers = await self._auth.async_get_headers(token_type="mbb", headers=accept)
         data = await self._auth.get(
             f"{url}/vehicleMgmt/vehicledata/v2/{self.brand}/{self.country}/vehicles/{vin.upper()}/",
             headers=headers,
         )
-        if not isinstance(data, ExtendedDict):
-            _LOGGER.warning("Format is incorrect %s", data)
+        data = data if data else ExtendedDict()
         return data
 
     async def async_get_vehicle(self, vin: str) -> VehicleDataResponse:
         """Get store data."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
             f"{url}/bs/vsr/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/status"
         )
-        if not isinstance(data, ExtendedDict):
-            _LOGGER.warning("Format is incorrect %s", data)
+        data = data if data else ExtendedDict()
         return VehicleDataResponse(data, self._spin is not None)
 
     async def async_refresh_vehicle_data(self, vin: str) -> None:
         """Refresh vehicle data."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.post(
             f"{url}/bs/vsr/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/requests"
         )
+        data = data if data else ExtendedDict()
         request_id: str = data.getr("CurrentVehicleDataResponse.requestId")
         await self.async_check_request_succeeded(
             f"{url}/bs/vsr/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/requests/{request_id}/jobstatus",
             "refresh vehicle data",
             REQUEST_SUCCESSFUL,
             REQUEST_FAILED,
             "requestStatusResponse.status",
@@ -100,52 +98,49 @@
 
     async def async_get_stored_position(self, vin: str) -> PositionDataResponse:
         """Get position data."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
             f"{url}/bs/cf/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/position"
         )
-        if not isinstance(data, ExtendedDict):
-            _LOGGER.warning("Format is incorrect %s", data)
+        data = data if data else ExtendedDict()
         return PositionDataResponse(data)
 
     async def async_get_destinations(self, vin: str) -> DestinationDataResponse:
         """Get destination data."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
             f"{url}/destinationfeedservice/mydestinations/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/destinations"
         )
-        if not isinstance(data, ExtendedDict):
-            _LOGGER.warning("Format is incorrect %s", data)
+        data = data if data else ExtendedDict()
         return DestinationDataResponse(data)
 
     async def async_get_history(self, vin: str) -> HistoryDataResponse:
         """Get history data."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
             f"{url}/bs/dwap/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/history"
         )
-        if not isinstance(data, ExtendedDict):
-            _LOGGER.warning("Format is incorrect %s", data)
+        data = data if data else ExtendedDict()
         return HistoryDataResponse(data)
 
     async def async_get_vehicule_users(self, vin: str) -> UsersDataResponse:
         """Get ufers of vehicle."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(f"{url}/bs/uic/v1/{vin.upper()}/users")
+        data = data if data else ExtendedDict()
         return UsersDataResponse(data)
 
     async def async_get_charger(self, vin: str) -> ChargerDataResponse:
         """Get charger data."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
             f"{url}/bs/batterycharge/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/charger"
         )
-        if not isinstance(data, ExtendedDict):
-            _LOGGER.warning("Format is incorrect %s", data)
+        data = data if data else ExtendedDict()
         return ChargerDataResponse(data)
 
     async def async_get_tripdata(
         self, vin: str, kind: Literal["short", "long", "cyclic"]
     ) -> tuple[TripDataResponse, TripDataResponse]:
         """Get trip data."""
         if kind not in ["short", "long", "cyclic"]:
@@ -160,16 +155,15 @@
                 "%Y-%m-%dT%H:%M:%SZ"
             ),
         }
         data = await self._auth.get(
             f"{url}/bs/tripstatistics/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/tripdata/{kind}",
             params=params,
         )
-        if not isinstance(data, ExtendedDict):
-            _LOGGER.warning("Format is incorrect %s", data)
+        data = data if data else ExtendedDict()
         td_sorted = sorted(
             data.getr("tripDataList.tripData"),
             key=lambda k: k["overallMileage"],  # type: ignore[no-any-return]
             reverse=True,
         )
         td_current = td_sorted[0]
         td_reset_trip = {}
@@ -187,57 +181,52 @@
 
     async def async_get_operations_list(self, vin: str) -> Any:
         """Get operation data."""
         url = await self._async_get_home_region_setter(vin.upper())
         data = await self._auth.get(
             f"{url}/rolesrights/operationlist/v3/vehicles/{vin.upper()}"
         )
-        if not isinstance(data, ExtendedDict):
-            _LOGGER.warning("Format is incorrect %s", data)
+        data = data if data else ExtendedDict()
         return data
 
     async def async_get_climater(self, vin: str) -> ClimaterDataResponse:
         """Get climater data."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
             f"{url}/bs/climatisation/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/climater"
         )
-        if not isinstance(data, ExtendedDict):
-            _LOGGER.warning("Format is incorrect %s", data)
+        data = data if data else ExtendedDict()
         return ClimaterDataResponse(data)
 
     async def async_get_preheater(self, vin: str) -> PreheaterDataResponse:
         """Get Heater/Ventilation data."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
             f"{url}/bs/rs/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/status"
         )
-        if not isinstance(data, ExtendedDict):
-            _LOGGER.warning("Format is incorrect %s", data)
+        data = data if data else ExtendedDict()
         return PreheaterDataResponse(data)
 
     async def async_get_climater_timer(self, vin: str) -> Any:
         """Get timer."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
             f"{url}/bs/departuretimer/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/timer"
         )
-        if not isinstance(data, ExtendedDict):
-            _LOGGER.warning("Format is incorrect %s", data)
+        data = data if data else ExtendedDict()
         return data
 
     async def async_get_capabilities(self, vin: str) -> VehicleDataResponse:
         """Get capabilities."""
         url = "https://emea.bff.cariad.digital"
         headers = await self._auth.async_get_headers(token_type="idk")
         data = await self._auth.get(
             f"{url}/vehicle/v1/vehicles/{vin.upper()}/capabilities", headers=headers
         )
-        if not isinstance(data, ExtendedDict):
-            _LOGGER.warning("Format is incorrect %s", data)
+        data = data if data else ExtendedDict()
         return VehicleDataResponse(data, self._spin is not None)
 
     async def async_get_vehicle_information(self) -> Any:
         """Get vehicle information."""
         headers = await self._auth.async_get_headers(
             token_type="audi",
             headers={
@@ -251,109 +240,102 @@
         }
         resp = await self._auth.post(
             "https://app-api.live-my.audi.com/vgql/v1/graphql",
             data=data,
             headers=headers,
             allow_redirects=False,
         )
+        resp = resp if resp else ExtendedDict()
         if "data" not in resp:
             raise AudiException("Invalid json in vehicle information")
         return resp
 
     async def async_get_honkflash(self, vin: str) -> Any:
         """Get Honk & Flash status."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
             f"{url}/bs/rhf/v1/{self.brand}/{self.country}/configuration"
         )
-        if not isinstance(data, ExtendedDict):
-            _LOGGER.warning("Format is incorrect %s", data)
+        data = data if data else ExtendedDict()
         return data
 
     async def async_get_personal_data(self) -> Any:
         """Get Honk & Flash status."""
         url = f"{self._auth.profil_url}/customers/{self._auth.user_id}"
         headers = await self._auth.async_get_headers(token_type="idk")
         data = await self._auth.get(f"{url}/personalData", headers=headers)
-        if not isinstance(data, ExtendedDict):
-            _LOGGER.warning("Format is incorrect %s", data)
+        data = data if data else ExtendedDict()
         return data
 
     async def async_get_real_car_data(self) -> Any:
         """Get Honk & Flash status."""
         url = f"{self._auth.profil_url}/customers/{self._auth.user_id}"
         headers = await self._auth.async_get_headers(token_type="idk")
         data = await self._auth.get(f"{url}/realCarData", headers=headers)
-        if not isinstance(data, ExtendedDict):
-            _LOGGER.warning("Format is incorrect %s", data)
+        data = data if data else ExtendedDict()
         return data
 
     async def async_get_mbb_status(self) -> Any:
         """Get Honk & Flash status."""
         url = f"{self._auth.profil_url}/customers/{self._auth.user_id}"
         headers = await self._auth.async_get_headers(token_type="idk")
         data = await self._auth.get(f"{url}/mbbStatusData", headers=headers)
-        if not isinstance(data, ExtendedDict):
-            _LOGGER.warning("Format is incorrect %s", data)
+        data = data if data else ExtendedDict()
         return data
 
     async def async_get_identity_data(self) -> Any:
         """Get Honk & Flash status."""
         url = f"{self._auth.profil_url}/customers/{self._auth.user_id}"
         headers = await self._auth.async_get_headers(token_type="idk")
         data = await self._auth.get(f"{url}/identityData", headers=headers)
-        if not isinstance(data, ExtendedDict):
-            _LOGGER.warning("Format is incorrect %s", data)
+        data = data if data else ExtendedDict()
         return data
 
     # async def async_get_users(self, vin: str) -> Any:
     #     """Get users."""
     #     url = "https://userinformationservice.apps.emea.vwapps.io/iaa"
     #     headers = await self._auth.async_get_headers(token_type="idk")
     #     data = await self._auth.get(f"{url}/uic/v1/vin/{vin.upper()}/users", headers=headers)
+    #     data = data if data else ExtendedDict()
     #     return data
 
     async def async_get_fences(self, vin: str) -> Any:
         """Get fences."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
             f"{url}/bs/geofencing/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/geofencingAlerts"
         )
-        if not isinstance(data, ExtendedDict):
-            _LOGGER.warning("Format is incorrect %s", data)
+        data = data if data else ExtendedDict()
         return data
 
     async def async_get_fences_config(self, vin: str) -> Any:
         """Get fences configuration."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
             f"{url}/bs/geofencing/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/geofencingConfiguration"
         )
-        if not isinstance(data, ExtendedDict):
-            _LOGGER.warning("Format is incorrect %s", data)
+        data = data if data else ExtendedDict()
         return data
 
     async def async_get_speed_alert(self, vin: str) -> Any:
         """Get speed alert."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
             f"{url}/bs/speedalert/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/speedAlerts"
         )
-        if not isinstance(data, ExtendedDict):
-            _LOGGER.warning("Format is incorrect %s", data)
+        data = data if data else ExtendedDict()
         return data
 
     async def async_get_speed_config(self, vin: str) -> Any:
         """Get speed alert configuration."""
         url = await self._async_get_home_region(vin.upper())
         data = await self._auth.get(
             f"{url}/bs/speedalert/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/speedAlertConfiguration"
         )
-        if not isinstance(data, ExtendedDict):
-            _LOGGER.warning("Format is incorrect %s", data)
+        data = data if data else ExtendedDict()
         return data
 
     async def async_lock(self, vin: str, lock: bool) -> None:
         """Set lock."""
         # OpenHab "lock","unlock"
         url = await self._async_get_home_region(vin.upper())
         data = '<?xml version="1.0" encoding= "UTF-8" ?>'
@@ -370,15 +352,15 @@
 
         rsp = await self._auth.post(
             f"{url}/bs/rlu/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/actions",
             headers=headers,
             data=data,
             use_json=False,
         )
-
+        rsp = rsp if rsp else ExtendedDict()
         request_id = rsp.getr("rluActionResponse.requestId")
         await self.async_check_request_succeeded(
             f"{url}/bs/rlu/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/requests/{request_id}/status",
             "lock vehicle" if lock else "unlock vehicle",
             REQUEST_SUCCESSFUL,
             REQUEST_FAILED,
             "requestStatusResponse.status",
@@ -421,14 +403,15 @@
 
         rsp = await self._auth.post(
             f"{url}/bs/climatisation/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/climater/actions",
             headers=headers,
             data=data,
             use_json=False,
         )
+        rsp = rsp if rsp else ExtendedDict()
         actionid = rsp.getr("action.actionId")
         await self.async_check_request_succeeded(
             f"{url}/bs/climatisation/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/climater/actions/{actionid}",
             "start climatisation" if start else "stop climatisation",
             SUCCEEDED,
             FAILED,
             "action.actionState",
@@ -465,14 +448,15 @@
         # headers = await self._auth.async_get_action_headers("application/json", None)
         rsp = await self._auth.post(
             f"{url}/bs/climatisation/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/climater/actions",
             headers=headers,
             data=data,
             use_json=False,
         )
+        rsp = rsp if rsp else ExtendedDict()
         actionid = rsp.getr("action.actionId")
         await self.async_check_request_succeeded(
             f"{url}/bs/climatisation/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/climater/actions/{actionid}",
             "set target temperature",
             SUCCEEDED,
             FAILED,
             "action.actionState",
@@ -571,15 +555,15 @@
         )
         rsp = await self._auth.post(
             f"{url}/bs/batterycharge/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/charger/actions",
             headers=headers,
             data=data,
             use_json=False,
         )
-
+        rsp = rsp if rsp else ExtendedDict()
         actionid = rsp.getr("action.actionId")
         await self.async_check_request_succeeded(
             f"{url}/bs/batterycharge/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/charger/actions/{actionid}",
             "start charger" if start else "stop charger",
             SUCCEEDED,
             FAILED,
             "action.actionState",
@@ -595,14 +579,15 @@
         )
         rsp = await self._auth.post(
             f"{url}/bs/batterycharge/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/charger/actions",
             headers=headers,
             data=data,
             use_json=False,
         )
+        rsp = rsp if rsp else ExtendedDict()
         actionid = rsp.getr("action.actionId")
         await self.async_check_request_succeeded(
             f"{url}/bs/batterycharge/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/charger/actions/{actionid}",
             "set charger max current",
             SUCCEEDED,
             FAILED,
             "action.actionState",
@@ -626,14 +611,15 @@
         )
         rsp = await self._auth.post(
             f"{url}/bs/climatisation/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/climater/actions",
             headers=headers,
             data=data,
             use_json=False,
         )
+        rsp = rsp if rsp else ExtendedDict()
         actionid = rsp.getr("action.actionId")
         await self.async_check_request_succeeded(
             f"{url}/bs/climatisation/v1/{self.brand}/{self.country}/vehicles/{vin.upper()}/climater/actions/{actionid}",
             "start window heating" if start else "stop window heating",
             SUCCEEDED,
             FAILED,
             "action.actionState",
@@ -710,14 +696,15 @@
         """Fill region."""
         self._home_region[vin] = "https://msg.volkswagen.de/fs-car"
         self._home_region_setter[vin] = "https://mal-1a.prd.ece.vwg-connect.com/api"
         try:
             rsp = await self._auth.get(
                 f"{self._home_region_setter[vin]}/cs/vds/v1/vehicles/{vin}/homeRegion"
             )
+            rsp = rsp if rsp else ExtendedDict()
             uri = rsp.getr("homeRegion.baseUri.content")
             if uri and uri != self._home_region_setter[vin]:
                 self._home_region[vin] = uri.replace("mal-", "fal-").replace(
                     "/api", "/fs-car"
                 )
                 self._home_region_setter[vin] = uri
         except Exception:  # pylint: disable=broad-except
@@ -744,15 +731,15 @@
 
         # Challenge
         headers = await self._auth.async_get_headers(token_type="mbb", okhttp=True)
         rsp = await self._auth.get(
             f"{url}/rolesrights/authorization/v2/vehicles/{vin.upper()}/services/{action}/security-pin-auth-requested",
             headers=headers,
         )
-
+        rsp = rsp if rsp else ExtendedDict()
         sec_token = rsp.getr("securityPinAuthInfo.securityToken")
         challenge: str = rsp.getr(
             "securityPinAuthInfo.securityPinTransmission.challenge"
         )
 
         # Response
         security_pin_hash = self._generate_security_pin_hash(challenge)
```

### Comparing `audiconnectpy-1.3.7/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-1.3.8/audiconnectpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.3.7
+Version: 1.3.8
 Summary: Provides asynchronous authentication and access to Audi Connect
 Home-page: https://github.com/cyr-ius/audiconnectpy/tree/master/audiconnectpy
 Author: cyr-ius
 Author-email: cyr-ius@ipocus.net
 License: GPL-3
 Keywords: connect,async
 Classifier: Programming Language :: Python
```

### Comparing `audiconnectpy-1.3.7/pyproject.toml` & `audiconnectpy-1.3.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.3.7/setup.py` & `audiconnectpy-1.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="audiconnectpy",
-    version="1.3.7",
+    version="1.3.8",
     packages=find_packages(),
     author="cyr-ius",
     author_email="cyr-ius@ipocus.net",
     description="Provides asynchronous authentication and access to Audi Connect",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["aiohttp>=3.8.1", "beautifulsoup4>=4.11.2"],
```

