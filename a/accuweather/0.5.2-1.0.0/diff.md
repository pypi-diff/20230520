# Comparing `tmp/accuweather-0.5.2.tar.gz` & `tmp/accuweather-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accuweather-0.5.2.tar", last modified: Mon May 15 20:45:59 2023, max compression
+gzip compressed data, was "accuweather-1.0.0.tar", last modified: Sat May 20 12:44:20 2023, max compression
```

## Comparing `accuweather-0.5.2.tar` & `accuweather-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:45:59.142764 accuweather-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-05-15 20:45:48.000000 accuweather-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-15 20:45:48.000000 accuweather-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-15 20:45:59.142764 accuweather-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-15 20:45:48.000000 accuweather-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:45:59.142764 accuweather-0.5.2/accuweather/
--rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-05-15 20:45:48.000000 accuweather-0.5.2/accuweather/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-15 20:45:48.000000 accuweather-0.5.2/accuweather/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-15 20:45:48.000000 accuweather-0.5.2/accuweather/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:45:48.000000 accuweather-0.5.2/accuweather/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:45:59.142764 accuweather-0.5.2/accuweather.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-15 20:45:59.000000 accuweather-0.5.2/accuweather.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-15 20:45:59.000000 accuweather-0.5.2/accuweather.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:45:59.000000 accuweather-0.5.2/accuweather.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 20:45:59.000000 accuweather-0.5.2/accuweather.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 20:45:59.000000 accuweather-0.5.2/accuweather.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-15 20:45:48.000000 accuweather-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-15 20:45:48.000000 accuweather-0.5.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 20:45:48.000000 accuweather-0.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 20:45:59.142764 accuweather-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-15 20:45:48.000000 accuweather-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:44:20.966207 accuweather-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-05-20 12:44:06.000000 accuweather-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-20 12:44:06.000000 accuweather-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-20 12:44:20.966207 accuweather-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-05-20 12:44:06.000000 accuweather-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:44:20.966207 accuweather-1.0.0/accuweather/
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-05-20 12:44:06.000000 accuweather-1.0.0/accuweather/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-20 12:44:06.000000 accuweather-1.0.0/accuweather/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-20 12:44:06.000000 accuweather-1.0.0/accuweather/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 12:44:06.000000 accuweather-1.0.0/accuweather/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-05-20 12:44:06.000000 accuweather-1.0.0/accuweather/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:44:20.966207 accuweather-1.0.0/accuweather.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-20 12:44:20.000000 accuweather-1.0.0/accuweather.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-20 12:44:20.000000 accuweather-1.0.0/accuweather.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 12:44:20.000000 accuweather-1.0.0/accuweather.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-20 12:44:20.000000 accuweather-1.0.0/accuweather.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-20 12:44:20.000000 accuweather-1.0.0/accuweather.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-20 12:44:06.000000 accuweather-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-20 12:44:06.000000 accuweather-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 12:44:20.966207 accuweather-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-20 12:44:06.000000 accuweather-1.0.0/setup.py
```

### Comparing `accuweather-0.5.2/LICENSE` & `accuweather-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `accuweather-0.5.2/PKG-INFO` & `accuweather-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: accuweather
-Version: 0.5.2
-Summary: Python wrapper for getting weather data from AccuWeather servers.
+Version: 1.0.0
+Summary: Python wrapper for getting weather data from AccuWeather API.
 Home-page: https://github.com/bieniu/accuweather
 Author: Maciej Bieniek
 License: Apache-2.0 License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -23,15 +23,15 @@
 [![PyPI][pypi-releases-shield]][pypi-releases]
 [![PyPI - Downloads][pypi-downloads]][pypi-statistics]
 [![Buy me a coffee][buy-me-a-coffee-shield]][buy-me-a-coffee]
 [![PayPal_Me][paypal-me-shield]][paypal-me]
 
 # accuweather
 
-Python wrapper for getting weather data from AccuWeather servers for Limited Trial package.
+Python wrapper for getting weather data from AccuWeather API.
 
 
 ## API key
 
 To generate API key go to https://developer.accuweather.com/user/register and after registration create an app.
 
 
@@ -49,43 +49,50 @@
     InvalidApiKeyError,
     InvalidCoordinatesError,
     RequestsExceededError,
 )
 
 LATITUDE = 52.0677904
 LONGITUDE = 19.4795644
-LOCATION_KEY = "268068"
 API_KEY = "xxxxx"
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 async def main():
     """Run main function."""
     async with ClientSession() as websession:
         try:
             accuweather = AccuWeather(
-                API_KEY, websession, latitude=LATITUDE, longitude=LONGITUDE
+                API_KEY,
+                websession,
+                latitude=LATITUDE,
+                longitude=LONGITUDE,
+                language="pl",
             )
             current_conditions = await accuweather.async_get_current_conditions()
-            forecast = await accuweather.async_get_forecast(metric=True)
-            forecast_hourly = await accuweather.async_get_forecast_hourly(metric=True)
+            forecast_daily = await accuweather.async_get_daily_forecast(
+                days=5, metric=True
+            )
+            forecast_hourly = await accuweather.async_get_hourly_forecast(
+                hours=12, metric=True
+            )
         except (
             ApiError,
             InvalidApiKeyError,
             InvalidCoordinatesError,
             ClientError,
             RequestsExceededError,
         ) as error:
             print(f"Error: {error}")
         else:
             print(f"Location: {accuweather.location_name} ({accuweather.location_key})")
             print(f"Requests remaining: {accuweather.requests_remaining}")
             print(f"Current: {current_conditions}")
-            print(f"Forecast: {forecast}")
+            print(f"Forecast: {forecast_daily}")
             print(f"Forecast hourly: {forecast_hourly}")
 
 
 loop = asyncio.new_event_loop()
 loop.run_until_complete(main())
 loop.close()
 ```
```

### Comparing `accuweather-0.5.2/README.md` & `accuweather-1.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [![PyPI][pypi-releases-shield]][pypi-releases]
 [![PyPI - Downloads][pypi-downloads]][pypi-statistics]
 [![Buy me a coffee][buy-me-a-coffee-shield]][buy-me-a-coffee]
 [![PayPal_Me][paypal-me-shield]][paypal-me]
 
 # accuweather
 
-Python wrapper for getting weather data from AccuWeather servers for Limited Trial package.
+Python wrapper for getting weather data from AccuWeather API.
 
 
 ## API key
 
 To generate API key go to https://developer.accuweather.com/user/register and after registration create an app.
 
 
@@ -28,43 +28,50 @@
     InvalidApiKeyError,
     InvalidCoordinatesError,
     RequestsExceededError,
 )
 
 LATITUDE = 52.0677904
 LONGITUDE = 19.4795644
-LOCATION_KEY = "268068"
 API_KEY = "xxxxx"
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 async def main():
     """Run main function."""
     async with ClientSession() as websession:
         try:
             accuweather = AccuWeather(
-                API_KEY, websession, latitude=LATITUDE, longitude=LONGITUDE
+                API_KEY,
+                websession,
+                latitude=LATITUDE,
+                longitude=LONGITUDE,
+                language="pl",
             )
             current_conditions = await accuweather.async_get_current_conditions()
-            forecast = await accuweather.async_get_forecast(metric=True)
-            forecast_hourly = await accuweather.async_get_forecast_hourly(metric=True)
+            forecast_daily = await accuweather.async_get_daily_forecast(
+                days=5, metric=True
+            )
+            forecast_hourly = await accuweather.async_get_hourly_forecast(
+                hours=12, metric=True
+            )
         except (
             ApiError,
             InvalidApiKeyError,
             InvalidCoordinatesError,
             ClientError,
             RequestsExceededError,
         ) as error:
             print(f"Error: {error}")
         else:
             print(f"Location: {accuweather.location_name} ({accuweather.location_key})")
             print(f"Requests remaining: {accuweather.requests_remaining}")
             print(f"Current: {current_conditions}")
-            print(f"Forecast: {forecast}")
+            print(f"Forecast: {forecast_daily}")
             print(f"Forecast hourly: {forecast_hourly}")
 
 
 loop = asyncio.new_event_loop()
 loop.run_until_complete(main())
 loop.close()
 ```
```

### Comparing `accuweather-0.5.2/accuweather/exceptions.py` & `accuweather-1.0.0/accuweather/exceptions.py`

 * *Files identical despite different names*

### Comparing `accuweather-0.5.2/accuweather.egg-info/PKG-INFO` & `accuweather-1.0.0/accuweather.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: accuweather
-Version: 0.5.2
-Summary: Python wrapper for getting weather data from AccuWeather servers.
+Version: 1.0.0
+Summary: Python wrapper for getting weather data from AccuWeather API.
 Home-page: https://github.com/bieniu/accuweather
 Author: Maciej Bieniek
 License: Apache-2.0 License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -23,15 +23,15 @@
 [![PyPI][pypi-releases-shield]][pypi-releases]
 [![PyPI - Downloads][pypi-downloads]][pypi-statistics]
 [![Buy me a coffee][buy-me-a-coffee-shield]][buy-me-a-coffee]
 [![PayPal_Me][paypal-me-shield]][paypal-me]
 
 # accuweather
 
-Python wrapper for getting weather data from AccuWeather servers for Limited Trial package.
+Python wrapper for getting weather data from AccuWeather API.
 
 
 ## API key
 
 To generate API key go to https://developer.accuweather.com/user/register and after registration create an app.
 
 
@@ -49,43 +49,50 @@
     InvalidApiKeyError,
     InvalidCoordinatesError,
     RequestsExceededError,
 )
 
 LATITUDE = 52.0677904
 LONGITUDE = 19.4795644
-LOCATION_KEY = "268068"
 API_KEY = "xxxxx"
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 async def main():
     """Run main function."""
     async with ClientSession() as websession:
         try:
             accuweather = AccuWeather(
-                API_KEY, websession, latitude=LATITUDE, longitude=LONGITUDE
+                API_KEY,
+                websession,
+                latitude=LATITUDE,
+                longitude=LONGITUDE,
+                language="pl",
             )
             current_conditions = await accuweather.async_get_current_conditions()
-            forecast = await accuweather.async_get_forecast(metric=True)
-            forecast_hourly = await accuweather.async_get_forecast_hourly(metric=True)
+            forecast_daily = await accuweather.async_get_daily_forecast(
+                days=5, metric=True
+            )
+            forecast_hourly = await accuweather.async_get_hourly_forecast(
+                hours=12, metric=True
+            )
         except (
             ApiError,
             InvalidApiKeyError,
             InvalidCoordinatesError,
             ClientError,
             RequestsExceededError,
         ) as error:
             print(f"Error: {error}")
         else:
             print(f"Location: {accuweather.location_name} ({accuweather.location_key})")
             print(f"Requests remaining: {accuweather.requests_remaining}")
             print(f"Current: {current_conditions}")
-            print(f"Forecast: {forecast}")
+            print(f"Forecast: {forecast_daily}")
             print(f"Forecast hourly: {forecast_hourly}")
 
 
 loop = asyncio.new_event_loop()
 loop.run_until_complete(main())
 loop.close()
 ```
```

### Comparing `accuweather-0.5.2/pyproject.toml` & `accuweather-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -79,17 +79,14 @@
     "FBT001",   # Boolean positional arg in function definition
     "FBT002",   # Boolean default value in function definition
     "PT023",    # Use `@pytest.mark.asyncio()` over `@pytest.mark.asyncio`
     "TRY003",   # Avoid specifying long messages outside the exception class
 ]
 
 [tool.ruff.per-file-ignores]
-"const.py" = [
-    "E501",      # Line too long
-]
 "tests/*" = [
     "PLR2004",  # Magic value used in comparison
     "S101",     # Use of `assert` detected
 ]
 "example.py" = [
     "T201",      # `print` found
 ]
```

### Comparing `accuweather-0.5.2/setup.py` & `accuweather-1.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Setup module for accuweather."""
 from pathlib import Path
 
 from setuptools import setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "0.5.2"
+VERSION = "1.0.0"
 
 with open("requirements.txt", encoding="utf-8") as file:
     requirements = file.read().splitlines()
 
 setup(
     name="accuweather",
     version=VERSION,
     author="Maciej Bieniek",
-    description="Python wrapper for getting weather data from AccuWeather servers.",
+    description="Python wrapper for getting weather data from AccuWeather API.",
     long_description=README_FILE.read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     include_package_data=True,
     url="https://github.com/bieniu/accuweather",
     license="Apache-2.0 License",
     packages=["accuweather"],
     package_data={"accuweather": ["py.typed"]},
```

