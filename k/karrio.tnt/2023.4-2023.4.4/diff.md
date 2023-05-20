# Comparing `tmp/karrio.tnt-2023.4-py3-none-any.whl.zip` & `tmp/karrio.tnt-2023.4.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 13756 bytes, number of entries: 18
+Zip file size: 13746 bytes, number of entries: 18
 -rw-rw-r--  2.0 unx      525 b- defN 22-Nov-15 19:21 karrio/mappers/tnt/__init__.py
--rw-rw-r--  2.0 unx     1631 b- defN 23-Apr-01 12:45 karrio/mappers/tnt/mapper.py
--rw-rw-r--  2.0 unx     1019 b- defN 23-Apr-01 12:45 karrio/mappers/tnt/proxy.py
--rw-rw-r--  2.0 unx      481 b- defN 23-Apr-15 06:44 karrio/mappers/tnt/settings.py
+-rw-rw-r--  2.0 unx     1631 b- defN 23-Apr-23 04:04 karrio/mappers/tnt/mapper.py
+-rw-rw-r--  2.0 unx     1019 b- defN 23-Apr-23 04:04 karrio/mappers/tnt/proxy.py
+-rw-rw-r--  2.0 unx      481 b- defN 23-Apr-23 04:04 karrio/mappers/tnt/settings.py
 -rw-rw-r--  2.0 unx      322 b- defN 22-Nov-15 19:21 karrio/providers/tnt/__init__.py
 -rw-rw-r--  2.0 unx     3963 b- defN 22-Nov-15 19:21 karrio/providers/tnt/error.py
--rw-rw-r--  2.0 unx     5025 b- defN 23-Apr-01 15:18 karrio/providers/tnt/rate.py
--rw-rw-r--  2.0 unx     2405 b- defN 23-Apr-01 15:57 karrio/providers/tnt/tracking.py
+-rw-rw-r--  2.0 unx     5025 b- defN 23-Apr-23 04:04 karrio/providers/tnt/rate.py
+-rw-rw-r--  2.0 unx     2405 b- defN 23-Apr-23 04:04 karrio/providers/tnt/tracking.py
 -rw-rw-r--  2.0 unx     4079 b- defN 23-Jan-11 18:22 karrio/providers/tnt/units.py
--rw-rw-r--  2.0 unx      625 b- defN 23-Apr-15 06:44 karrio/providers/tnt/utils.py
+-rw-rw-r--  2.0 unx      625 b- defN 23-Apr-23 04:04 karrio/providers/tnt/utils.py
 -rw-rw-r--  2.0 unx       91 b- defN 22-Nov-15 19:21 karrio/providers/tnt/shipment/__init__.py
--rw-rw-r--  2.0 unx     2236 b- defN 23-Apr-01 15:18 karrio/providers/tnt/shipment/create.py
--rw-rw-r--  2.0 unx     4841 b- defN 23-Apr-01 13:47 karrio/providers/tnt/shipment/label.py
--rw-rw-r--  2.0 unx     6515 b- defN 23-Apr-01 13:47 karrio/providers/tnt/shipment/request.py
--rw-rw-r--  2.0 unx      956 b- defN 23-Apr-18 07:09 karrio.tnt-2023.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 07:09 karrio.tnt-2023.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Apr-18 07:09 karrio.tnt-2023.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1556 b- defN 23-Apr-18 07:09 karrio.tnt-2023.4.dist-info/RECORD
-18 files, 36369 bytes uncompressed, 11174 bytes compressed:  69.3%
+-rw-rw-r--  2.0 unx     2236 b- defN 23-Apr-23 04:04 karrio/providers/tnt/shipment/create.py
+-rw-rw-r--  2.0 unx     4713 b- defN 23-May-17 00:17 karrio/providers/tnt/shipment/label.py
+-rw-rw-r--  2.0 unx     6515 b- defN 23-Apr-23 04:04 karrio/providers/tnt/shipment/request.py
+-rw-rw-r--  2.0 unx      958 b- defN 23-May-20 11:14 karrio.tnt-2023.4.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-20 11:14 karrio.tnt-2023.4.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-May-20 11:14 karrio.tnt-2023.4.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1564 b- defN 23-May-20 11:14 karrio.tnt-2023.4.4.dist-info/RECORD
+18 files, 36251 bytes uncompressed, 11148 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: karrio/providers/tnt/shipment/label.py
 Comment: 
 
 Filename: karrio/providers/tnt/shipment/request.py
 Comment: 
 
-Filename: karrio.tnt-2023.4.dist-info/METADATA
+Filename: karrio.tnt-2023.4.4.dist-info/METADATA
 Comment: 
 
-Filename: karrio.tnt-2023.4.dist-info/WHEEL
+Filename: karrio.tnt-2023.4.4.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.tnt-2023.4.dist-info/top_level.txt
+Filename: karrio.tnt-2023.4.4.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.tnt-2023.4.dist-info/RECORD
+Filename: karrio.tnt-2023.4.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/providers/tnt/shipment/label.py

```diff
@@ -36,28 +36,26 @@
                 consignmentIdentity=consignmentIdentityType(
                     consignmentNumber=cast(CREATE, activity.CREATE).CONNUMBER,
                     customerReference=payload.reference,
                 ),
                 collectionDateTime=None,
                 sender=nameAndAddressRequestType(
                     name=recipient.contact,
-                    addressLine1=lib.text(shipper.street_number, shipper.address_line1),
+                    addressLine1=shipper.street,
                     addressLine2=shipper.address_line2,
                     addressLine3=None,
                     town=shipper.city,
                     exactMatch=None,
                     province=shipper.state_code,
                     postcode=shipper.postal_code,
                     country=shipper.country_code,
                 ),
                 delivery=nameAndAddressRequestType(
                     name=recipient.contact,
-                    addressLine1=lib.text(
-                        recipient.street_number, recipient.address_line1
-                    ),
+                    addressLine1=recipient.street,
                     addressLine2=recipient.address_line2,
                     addressLine3=None,
                     town=recipient.city,
                     exactMatch=None,
                     province=recipient.state_code,
                     postcode=recipient.postal_code,
                     country=recipient.country_code,
```

## Comparing `karrio.tnt-2023.4.dist-info/METADATA` & `karrio.tnt-2023.4.4.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karrio.tnt
-Version: 2023.4
+Version: 2023.4.4
 Summary: Karrio - TNT Shipping extension
 Home-page: https://github.com/karrioapi/karrio
 Author: karrio
 Author-email: hello@karrio.io
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

## Comparing `karrio.tnt-2023.4.dist-info/RECORD` & `karrio.tnt-2023.4.4.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 karrio/providers/tnt/error.py,sha256=SkoXTZ9HO0-D8xE5x6ikS2HYQdIoCq5wWvTysyTvWjM,3963
 karrio/providers/tnt/rate.py,sha256=b2furEIFdKdLmi8KJXVAxZMmqyqw9BTSXgH1glzdGRo,5025
 karrio/providers/tnt/tracking.py,sha256=96jtTWBhtsjYOdWVRsaRaN1gHbm5tiWPAEgUuV5qP1o,2405
 karrio/providers/tnt/units.py,sha256=3HP4Ve6GXlK_zLzKXFzLIlZr1O5l5_1Hye2Dyy0VJfM,4079
 karrio/providers/tnt/utils.py,sha256=U9QGLpRj8QozSaDvBdxllhywSwPP1NQolLbhoVKHK5A,625
 karrio/providers/tnt/shipment/__init__.py,sha256=UPOD_hgNR9l8Mlkq4f0fB2Znl_iZLDLf2i1b-v2Hw9A,91
 karrio/providers/tnt/shipment/create.py,sha256=_ZKiaqqh8BMeaorlmlxjsRRwW-mIKw-1mnE1xb7iD3Q,2236
-karrio/providers/tnt/shipment/label.py,sha256=By2Sjj2T2dNz7id8GtHBfsl2P-lG1PLtiBKkEToGICI,4841
+karrio/providers/tnt/shipment/label.py,sha256=dJ4rjoi3UNyOQ8YHYPLPWFF010OU738c7PQNS7PjtXw,4713
 karrio/providers/tnt/shipment/request.py,sha256=hFsJB_c8GLWkQTV3S8vRymMrisPsR3MD5psrznZoQ_0,6515
-karrio.tnt-2023.4.dist-info/METADATA,sha256=5nn7f0rO4eYPJNnLXpuJGWaGr-Ldg08OFY-Raww3JlM,956
-karrio.tnt-2023.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-karrio.tnt-2023.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
-karrio.tnt-2023.4.dist-info/RECORD,,
+karrio.tnt-2023.4.4.dist-info/METADATA,sha256=Qz_keMEoTBoo2dJ9-oAZpJGwNOipr142FDCBAtd4KBg,958
+karrio.tnt-2023.4.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+karrio.tnt-2023.4.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
+karrio.tnt-2023.4.4.dist-info/RECORD,,
```

