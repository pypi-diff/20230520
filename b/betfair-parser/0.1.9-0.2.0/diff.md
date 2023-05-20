# Comparing `tmp/betfair_parser-0.1.9.tar.gz` & `tmp/betfair_parser-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betfair_parser-0.1.9.tar", max compression
+gzip compressed data, was "betfair_parser-0.2.0.tar", max compression
```

## Comparing `betfair_parser-0.1.9.tar` & `betfair_parser-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,27 @@
--rw-r--r--   0        0        0        0 2022-04-10 23:57:27.532287 betfair_parser-0.1.9/betfair_parser/__init__.py
--rw-r--r--   0        0        0      717 2022-11-25 01:09:17.104913 betfair_parser-0.1.9/betfair_parser/constants.py
--rw-r--r--   0        0        0      555 2022-11-25 02:27:40.551221 betfair_parser-0.1.9/betfair_parser/core.py
--rw-r--r--   0        0        0        0 2022-04-10 23:57:27.532287 betfair_parser-0.1.9/betfair_parser/spec/__init__.py
--rw-r--r--   0        0        0        0 2022-11-25 01:09:17.104913 betfair_parser-0.1.9/betfair_parser/spec/api/__init__.py
--rw-r--r--   0        0        0      889 2022-11-25 01:09:17.104913 betfair_parser-0.1.9/betfair_parser/spec/api/account.py
--rw-r--r--   0        0        0     2693 2022-12-27 08:49:54.937768 betfair_parser-0.1.9/betfair_parser/spec/api/betting.py
--rw-r--r--   0        0        0      267 2022-12-21 22:27:33.117597 betfair_parser-0.1.9/betfair_parser/spec/api/core.py
--rw-r--r--   0        0        0      144 2022-11-25 01:09:17.104913 betfair_parser-0.1.9/betfair_parser/spec/api/error.py
--rw-r--r--   0        0        0     2793 2023-01-04 07:39:34.765066 betfair_parser-0.1.9/betfair_parser/spec/api/markets.py
--rw-r--r--   0        0        0      324 2022-11-25 01:09:17.104913 betfair_parser-0.1.9/betfair_parser/spec/streaming/__init__.py
--rw-r--r--   0        0        0        0 2022-11-25 01:09:17.104913 betfair_parser-0.1.9/betfair_parser/spec/streaming/core.py
--rw-r--r--   0        0        0     5587 2023-01-04 08:13:10.637906 betfair_parser-0.1.9/betfair_parser/spec/streaming/mcm.py
--rw-r--r--   0        0        0     1630 2022-12-27 08:49:54.941768 betfair_parser-0.1.9/betfair_parser/spec/streaming/ocm.py
--rw-r--r--   0        0        0      476 2022-12-27 08:49:54.941768 betfair_parser-0.1.9/betfair_parser/spec/streaming/status.py
--rw-r--r--   0        0        0      384 2023-01-04 08:24:50.739775 betfair_parser-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 betfair_parser-0.1.9/setup.py
--rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 betfair_parser-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-02-17 06:17:12.705223 betfair_parser-0.2.0/betfair_parser/__init__.py
+-rw-r--r--   0        0        0      919 2023-02-24 04:45:44.811742 betfair_parser-0.2.0/betfair_parser/core.py
+-rw-r--r--   0        0        0        0 2023-02-17 06:17:12.706435 betfair_parser-0.2.0/betfair_parser/spec/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 01:56:57.283786 betfair_parser-0.2.0/betfair_parser/spec/accounts/__init__.py
+-rw-r--r--   0        0        0     2589 2023-05-20 01:56:57.284082 betfair_parser-0.2.0/betfair_parser/spec/accounts/enums.py
+-rw-r--r--   0        0        0        0 2023-05-20 01:56:57.284124 betfair_parser-0.2.0/betfair_parser/spec/accounts/exceptions.py
+-rw-r--r--   0        0        0     2584 2023-05-20 01:56:57.284257 betfair_parser-0.2.0/betfair_parser/spec/accounts/operations.py
+-rw-r--r--   0        0        0    10884 2023-05-20 01:56:57.284389 betfair_parser-0.2.0/betfair_parser/spec/accounts/type_definitions.py
+-rw-r--r--   0        0        0        0 2023-05-20 01:56:57.284468 betfair_parser-0.2.0/betfair_parser/spec/betting/__init__.py
+-rw-r--r--   0        0        0    20267 2023-05-20 01:56:57.284702 betfair_parser-0.2.0/betfair_parser/spec/betting/enums.py
+-rw-r--r--   0        0        0     1811 2023-05-20 01:56:57.284819 betfair_parser-0.2.0/betfair_parser/spec/betting/exceptions.py
+-rw-r--r--   0        0        0     9434 2023-05-20 01:56:57.284942 betfair_parser-0.2.0/betfair_parser/spec/betting/listings.py
+-rw-r--r--   0        0        0     8003 2023-05-20 01:56:57.285056 betfair_parser-0.2.0/betfair_parser/spec/betting/orders.py
+-rw-r--r--   0        0        0    28629 2023-05-20 01:56:57.285245 betfair_parser-0.2.0/betfair_parser/spec/betting/type_definitions.py
+-rw-r--r--   0        0        0     5331 2023-05-20 01:56:57.285473 betfair_parser-0.2.0/betfair_parser/spec/common.py
+-rw-r--r--   0        0        0      717 2023-05-20 01:56:57.285784 betfair_parser-0.2.0/betfair_parser/spec/constants.py
+-rw-r--r--   0        0        0     3569 2023-05-20 01:56:57.285934 betfair_parser-0.2.0/betfair_parser/spec/error.py
+-rw-r--r--   0        0        0     1768 2023-05-20 01:56:57.286037 betfair_parser-0.2.0/betfair_parser/spec/heartbeat.py
+-rw-r--r--   0        0        0     3399 2023-05-20 01:56:57.286141 betfair_parser-0.2.0/betfair_parser/spec/navigation.py
+-rw-r--r--   0        0        0     2903 2023-05-20 01:56:57.286235 betfair_parser-0.2.0/betfair_parser/spec/race_status.py
+-rw-r--r--   0        0        0      324 2023-02-17 06:17:12.708820 betfair_parser-0.2.0/betfair_parser/spec/streaming/__init__.py
+-rw-r--r--   0        0        0     6274 2023-05-20 01:56:57.286455 betfair_parser-0.2.0/betfair_parser/spec/streaming/mcm.py
+-rw-r--r--   0        0        0     2241 2023-05-20 01:56:57.286612 betfair_parser-0.2.0/betfair_parser/spec/streaming/ocm.py
+-rw-r--r--   0        0        0     2416 2023-05-20 01:56:57.286756 betfair_parser-0.2.0/betfair_parser/spec/streaming/status.py
+-rw-r--r--   0        0        0     2148 2023-05-20 01:56:57.286841 betfair_parser-0.2.0/betfair_parser/strenums.py
+-rw-r--r--   0        0        0      645 2023-05-20 01:56:57.287292 betfair_parser-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      432 1970-01-01 00:00:00.000000 betfair_parser-0.2.0/PKG-INFO
```

### Comparing `betfair_parser-0.1.9/betfair_parser/constants.py` & `betfair_parser-0.2.0/betfair_parser/spec/constants.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.1.9/betfair_parser/spec/streaming/ocm.py` & `betfair_parser-0.2.0/betfair_parser/spec/streaming/ocm.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,70 +1,84 @@
 from typing import List, Literal, Optional
 
-import msgspec
+from betfair_parser.spec.common import BaseMessage
 
 
-class MatchedOrder(msgspec.Struct, frozen=True, array_like=True):
+class MatchedOrder(BaseMessage, array_like=True, frozen=True):
     price: float
     size: float
 
 
-class UnmatchedOrder(msgspec.Struct, frozen=True):
+class UnmatchedOrder(BaseMessage, frozen=True):
     """
     https://docs.developer.betfair.com/display/1smk3cen4v3lu3yomq5qye0ni/Exchange+Stream+API
     """
 
     id: str
     p: float
     s: float
     side: Literal["B", "L"]
     status: Literal["E", "EC"]
     pt: str
     ot: str
     pd: int
-    rac: str
-    rc: str
-    rfo: str
-    rfs: str
+    rfo: Optional[str] = None
+    rfs: Optional[str] = None
+    rc: Optional[str] = None
+    rac: Optional[str] = None
     md: Optional[int] = None
     cd: Optional[int] = None
     ld: Optional[int] = None
     avp: Optional[float] = None
     sm: Optional[float] = None
     sr: Optional[float] = None
     sl: Optional[float] = None
     sc: Optional[float] = None
     sv: Optional[float] = None
 
 
-class OrderChanges(msgspec.Struct):
+class StrategyMatched(BaseMessage, frozen=True):
+    mb: Optional[List[MatchedOrder]] = []
+    ml: Optional[List[MatchedOrder]] = []
+
+
+class OrderChanges(BaseMessage, frozen=True):
     """
     https://docs.developer.betfair.com/display/1smk3cen4v3lu3yomq5qye0ni/Exchange+Stream+API
     """
 
     id: int
     fullImage: Optional[bool] = False
     hc: Optional[float] = None
     uo: Optional[List[UnmatchedOrder]] = []
     mb: Optional[List[MatchedOrder]] = []
     ml: Optional[List[MatchedOrder]] = []
+    smc: Optional[dict[str, StrategyMatched]] = None
 
 
-class OrderAccountChange(msgspec.Struct):
+class OrderAccountChange(BaseMessage, frozen=True):
     """
     https://docs.developer.betfair.com/display/1smk3cen4v3lu3yomq5qye0ni/Exchange+Stream+API
     """
 
     id: str
+    accountId: Optional[int] = None
     fullImage: Optional[bool] = False
-    orc: Optional[List[OrderChanges]] = []
+    orc: List[OrderChanges] = []
+    closed: Optional[bool] = None
 
 
-class OCM(msgspec.Struct, tag_field="op", tag=str.lower):
+class OCM(BaseMessage, tag_field="op", tag=str.lower, frozen=True):
     """
     https://docs.developer.betfair.com/display/1smk3cen4v3lu3yomq5qye0ni/Exchange+Stream+API
     """
 
     id: int
     clk: str
     pt: int
     oc: List[OrderAccountChange] = []
+    initialClk: Optional[str] = None
+    status: Optional[int] = None
+    conflateMs: Optional[int] = None
+    heartbeatMs: Optional[int] = None
+    ct: Optional[Literal["HEARTBEAT", "SUB_IMAGE"]] = None
+    con: Optional[bool] = None
```

