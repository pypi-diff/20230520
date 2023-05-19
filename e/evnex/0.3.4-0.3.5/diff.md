# Comparing `tmp/evnex-0.3.4.tar.gz` & `tmp/evnex-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evnex-0.3.4.tar", max compression
+gzip compressed data, was "evnex-0.3.5.tar", max compression
```

## Comparing `evnex-0.3.4.tar` & `evnex-0.3.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2023-05-15 03:51:30.614979 evnex-0.3.4/LICENSE
--rw-r--r--   0        0        0     1792 2023-05-15 03:51:30.614979 evnex-0.3.4/README.md
--rw-r--r--   0        0        0       23 2023-05-15 03:51:30.614979 evnex-0.3.4/evnex/__init__.py
--rw-r--r--   0        0        0    18048 2023-05-15 03:51:30.614979 evnex-0.3.4/evnex/api.py
--rw-r--r--   0        0        0       51 2023-05-15 03:51:30.614979 evnex-0.3.4/evnex/errors.py
--rw-r--r--   0        0        0        0 2023-05-15 03:51:30.614979 evnex-0.3.4/evnex/schema/__init__.py
--rw-r--r--   0        0        0     3588 2023-05-15 03:51:30.614979 evnex-0.3.4/evnex/schema/charge_points.py
--rw-r--r--   0        0        0      117 2023-05-15 03:51:30.614979 evnex-0.3.4/evnex/schema/commands.py
--rw-r--r--   0        0        0       95 2023-05-15 03:51:30.614979 evnex-0.3.4/evnex/schema/cost.py
--rw-r--r--   0        0        0      650 2023-05-15 03:51:30.614979 evnex-0.3.4/evnex/schema/org.py
--rw-r--r--   0        0        0      439 2023-05-15 03:51:30.614979 evnex-0.3.4/evnex/schema/user.py
--rw-r--r--   0        0        0        0 2023-05-15 03:51:30.614979 evnex-0.3.4/evnex/schema/v3/__init__.py
--rw-r--r--   0        0        0     1472 2023-05-15 03:51:30.614979 evnex-0.3.4/evnex/schema/v3/charge_points.py
--rw-r--r--   0        0        0      156 2023-05-15 03:51:30.614979 evnex-0.3.4/evnex/schema/v3/commands.py
--rw-r--r--   0        0        0      273 2023-05-15 03:51:30.618979 evnex-0.3.4/evnex/schema/v3/cost.py
--rw-r--r--   0        0        0      608 2023-05-15 03:51:30.618979 evnex-0.3.4/evnex/schema/v3/generic.py
--rw-r--r--   0        0        0      338 2023-05-15 03:51:30.618979 evnex-0.3.4/evnex/schema/v3/relationships.py
--rw-r--r--   0        0        0      717 2023-05-15 03:51:30.618979 evnex-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     2615 1970-01-01 00:00:00.000000 evnex-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-19 23:05:52.533785 evnex-0.3.5/LICENSE
+-rw-r--r--   0        0        0     1792 2023-05-19 23:05:52.533785 evnex-0.3.5/README.md
+-rw-r--r--   0        0        0       23 2023-05-19 23:05:52.533785 evnex-0.3.5/evnex/__init__.py
+-rw-r--r--   0        0        0    18864 2023-05-19 23:05:52.533785 evnex-0.3.5/evnex/api.py
+-rw-r--r--   0        0        0       51 2023-05-19 23:05:52.533785 evnex-0.3.5/evnex/errors.py
+-rw-r--r--   0        0        0        0 2023-05-19 23:05:52.533785 evnex-0.3.5/evnex/schema/__init__.py
+-rw-r--r--   0        0        0     3588 2023-05-19 23:05:52.533785 evnex-0.3.5/evnex/schema/charge_points.py
+-rw-r--r--   0        0        0      117 2023-05-19 23:05:52.533785 evnex-0.3.5/evnex/schema/commands.py
+-rw-r--r--   0        0        0       95 2023-05-19 23:05:52.533785 evnex-0.3.5/evnex/schema/cost.py
+-rw-r--r--   0        0        0      650 2023-05-19 23:05:52.533785 evnex-0.3.5/evnex/schema/org.py
+-rw-r--r--   0        0        0      439 2023-05-19 23:05:52.533785 evnex-0.3.5/evnex/schema/user.py
+-rw-r--r--   0        0        0        0 2023-05-19 23:05:52.533785 evnex-0.3.5/evnex/schema/v3/__init__.py
+-rw-r--r--   0        0        0     2813 2023-05-19 23:05:52.533785 evnex-0.3.5/evnex/schema/v3/charge_points.py
+-rw-r--r--   0        0        0      156 2023-05-19 23:05:52.533785 evnex-0.3.5/evnex/schema/v3/commands.py
+-rw-r--r--   0        0        0      415 2023-05-19 23:05:52.533785 evnex-0.3.5/evnex/schema/v3/cost.py
+-rw-r--r--   0        0        0      608 2023-05-19 23:05:52.533785 evnex-0.3.5/evnex/schema/v3/generic.py
+-rw-r--r--   0        0        0      400 2023-05-19 23:05:52.533785 evnex-0.3.5/evnex/schema/v3/relationships.py
+-rw-r--r--   0        0        0      717 2023-05-19 23:05:52.537785 evnex-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     2615 1970-01-01 00:00:00.000000 evnex-0.3.5/PKG-INFO
```

### Comparing `evnex-0.3.4/LICENSE` & `evnex-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `evnex-0.3.4/README.md` & `evnex-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `evnex-0.3.4/evnex/api.py` & `evnex-0.3.5/evnex/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,25 +13,27 @@
 from evnex.errors import NotAuthorizedException
 from evnex.schema.charge_points import (
     EvnexChargePoint,
     EvnexChargePointDetail,
     EvnexChargePointLoadSchedule,
     EvnexChargePointOverrideConfig,
     EvnexChargePointSolarConfig,
-    EvnexChargePointTransaction,
     EvnexChargeProfileSegment,
+    EvnexChargePointTransaction,
+    EvnexGetChargePointTransactionsResponse,
     EvnexGetChargePointDetailResponse,
     EvnexGetChargePointsResponse,
-    EvnexGetChargePointTransactionsResponse,
 )
 from evnex.schema.commands import EvnexCommandResponse
 from evnex.schema.org import EvnexGetOrgInsightResponse, EvnexOrgInsightEntry
 from evnex.schema.user import EvnexGetUserResponse, EvnexUserDetail
 from evnex.schema.v3.charge_points import (
     EvnexChargePointDetail as EvnexChargePointDetailV3,
+    EvnexGetChargePointSessionsResponse,
+    EvnexChargePointSession,
 )
 from evnex.schema.v3.commands import EvnexCommandResponse as EvnexCommandResponseV3
 from evnex.schema.v3.generic import EvnexV3APIResponse
 
 logger = logging.getLogger("evnex.api")
 
 
@@ -292,26 +294,44 @@
     @retry(
         wait=wait_random_exponential(multiplier=1, max=60),
         retry=retry_if_not_exception_type((ValidationError, NotAuthorizedException)),
     )
     async def get_charge_point_transactions(
         self, charge_point_id: str
     ) -> list[EvnexChargePointTransaction]:
+        warn(
+            "This method is deprecated. See get_charge_point_sessions",
+            DeprecationWarning,
+            stacklevel=2,
+        )
         # Similar to f'https://client-api.evnex.io/v3/charge-points/{charge_point_id}/sessions',
 
         r = await self.httpx_client.get(
             f"https://client-api.evnex.io/v2/apps/charge-points/{charge_point_id}/transactions",
             headers=self._common_headers,
         )
         json_data = await self._check_api_response(r)
-
         return EvnexGetChargePointTransactionsResponse(**json_data).data.items
 
     @retry(
         wait=wait_random_exponential(multiplier=1, max=60),
+        retry=retry_if_not_exception_type((ValidationError, NotAuthorizedException)),
+    )
+    async def get_charge_point_sessions(
+        self, charge_point_id: str
+    ) -> list[EvnexChargePointSession]:
+        r = await self.httpx_client.get(
+            f"https://client-api.evnex.io/v3/charge-points/{charge_point_id}/sessions",
+            headers=self._common_headers,
+        )
+        json_data = await self._check_api_response(r)
+        return EvnexGetChargePointSessionsResponse.parse_obj(json_data).data
+
+    @retry(
+        wait=wait_random_exponential(multiplier=1, max=60),
         retry=retry_if_not_exception_type(
             (ValidationError, NotAuthorizedException, ReadTimeout)
         ),
     )
     async def stop_charge_point(
         self,
         charge_point_id: str,
```

### Comparing `evnex-0.3.4/evnex/schema/charge_points.py` & `evnex-0.3.5/evnex/schema/charge_points.py`

 * *Files identical despite different names*

### Comparing `evnex-0.3.4/evnex/schema/org.py` & `evnex-0.3.5/evnex/schema/org.py`

 * *Files identical despite different names*

### Comparing `evnex-0.3.4/evnex/schema/v3/generic.py` & `evnex-0.3.5/evnex/schema/v3/generic.py`

 * *Files identical despite different names*

### Comparing `evnex-0.3.4/pyproject.toml` & `evnex-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "evnex"
-version = "0.3.4"
+version = "0.3.5"
 description = "A Python wrapper for the EVNEX Cloud API"
 authors = ["Brian Thorne <brian@hardbyte.nz>"]
 readme = "README.md"
 repository = "https://github.com/hardbyte/python-evnex"
 license = "Apache-2.0"
 
 [tool.poetry.urls]
```

### Comparing `evnex-0.3.4/PKG-INFO` & `evnex-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evnex
-Version: 0.3.4
+Version: 0.3.5
 Summary: A Python wrapper for the EVNEX Cloud API
 Home-page: https://github.com/hardbyte/python-evnex
 License: Apache-2.0
 Author: Brian Thorne
 Author-email: brian@hardbyte.nz
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

