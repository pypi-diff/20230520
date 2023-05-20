# Comparing `tmp/karrio.dhl_poland-2023.4-py3-none-any.whl.zip` & `tmp/karrio.dhl_poland-2023.4.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 12013 bytes, number of entries: 16
+Zip file size: 12025 bytes, number of entries: 16
 -rw-rw-r--  2.0 unx      583 b- defN 22-Nov-15 19:21 karrio/mappers/dhl_poland/__init__.py
--rw-rw-r--  2.0 unx     2033 b- defN 23-Apr-01 13:34 karrio/mappers/dhl_poland/mapper.py
--rw-rw-r--  2.0 unx     2063 b- defN 23-Apr-01 12:45 karrio/mappers/dhl_poland/proxy.py
--rw-rw-r--  2.0 unx      871 b- defN 23-Apr-15 06:44 karrio/mappers/dhl_poland/settings.py
+-rw-rw-r--  2.0 unx     2033 b- defN 23-Apr-23 04:04 karrio/mappers/dhl_poland/mapper.py
+-rw-rw-r--  2.0 unx     2063 b- defN 23-Apr-23 04:04 karrio/mappers/dhl_poland/proxy.py
+-rw-rw-r--  2.0 unx      871 b- defN 23-Apr-23 04:04 karrio/mappers/dhl_poland/settings.py
 -rw-rw-r--  2.0 unx      328 b- defN 22-Nov-15 19:21 karrio/providers/dhl_poland/__init__.py
 -rw-rw-r--  2.0 unx      621 b- defN 22-Nov-15 19:21 karrio/providers/dhl_poland/error.py
--rw-rw-r--  2.0 unx     2894 b- defN 23-Apr-01 15:18 karrio/providers/dhl_poland/tracking.py
+-rw-rw-r--  2.0 unx     2894 b- defN 23-Apr-23 04:04 karrio/providers/dhl_poland/tracking.py
 -rw-rw-r--  2.0 unx     4184 b- defN 23-Mar-27 07:55 karrio/providers/dhl_poland/units.py
 -rw-rw-r--  2.0 unx     1851 b- defN 23-Apr-15 02:55 karrio/providers/dhl_poland/utils.py
 -rw-rw-r--  2.0 unx      236 b- defN 22-Nov-15 19:21 karrio/providers/dhl_poland/shipment/__init__.py
--rw-rw-r--  2.0 unx     1565 b- defN 23-Apr-01 15:18 karrio/providers/dhl_poland/shipment/cancel.py
--rw-rw-r--  2.0 unx    13627 b- defN 23-Apr-01 15:18 karrio/providers/dhl_poland/shipment/create.py
--rw-rw-r--  2.0 unx     1026 b- defN 23-Apr-18 07:10 karrio.dhl_poland-2023.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 07:10 karrio.dhl_poland-2023.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Apr-18 07:10 karrio.dhl_poland-2023.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1490 b- defN 23-Apr-18 07:10 karrio.dhl_poland-2023.4.dist-info/RECORD
-16 files, 33471 bytes uncompressed, 9493 bytes compressed:  71.6%
+-rw-rw-r--  2.0 unx     1565 b- defN 23-Apr-23 04:04 karrio/providers/dhl_poland/shipment/cancel.py
+-rw-rw-r--  2.0 unx    13453 b- defN 23-May-17 00:17 karrio/providers/dhl_poland/shipment/create.py
+-rw-rw-r--  2.0 unx     1028 b- defN 23-May-20 11:14 karrio.dhl_poland-2023.4.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-20 11:14 karrio.dhl_poland-2023.4.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-May-20 11:14 karrio.dhl_poland-2023.4.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1498 b- defN 23-May-20 11:14 karrio.dhl_poland-2023.4.4.dist-info/RECORD
+16 files, 33307 bytes uncompressed, 9489 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: karrio/providers/dhl_poland/shipment/cancel.py
 Comment: 
 
 Filename: karrio/providers/dhl_poland/shipment/create.py
 Comment: 
 
-Filename: karrio.dhl_poland-2023.4.dist-info/METADATA
+Filename: karrio.dhl_poland-2023.4.4.dist-info/METADATA
 Comment: 
 
-Filename: karrio.dhl_poland-2023.4.dist-info/WHEEL
+Filename: karrio.dhl_poland-2023.4.4.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.dhl_poland-2023.4.dist-info/top_level.txt
+Filename: karrio.dhl_poland-2023.4.4.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.dhl_poland-2023.4.dist-info/RECORD
+Filename: karrio.dhl_poland-2023.4.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/providers/dhl_poland/shipment/create.py

```diff
@@ -155,19 +155,17 @@
                             )
                             else None
                         ),
                         address=dhl.Address(
                             name=(shipper.company_name or shipper.person_name),
                             postalCode=(shipper.postal_code or "").replace("-", ""),
                             city=shipper.city,
-                            street=lib.text(
-                                shipper.address_line1, shipper.address_line2
-                            ),
+                            street=shipper.address_line1,
                             houseNumber=(shipper.street_number or "N/A"),
-                            apartmentNumber=shipper.suite,
+                            apartmentNumber=shipper.address_line2,
                         ),
                     ),
                     receiver=dhl.ReceiverAddressat(
                         preaviso=(
                             dhl.PreavisoContact(
                                 personName=recipient.person_name,
                                 phoneNumber=recipient.phone_number,
@@ -202,19 +200,17 @@
                             isPackstation=None,
                             isPostfiliale=None,
                             postnummer=None,
                             addressType=("C" if recipient.residential else "B"),
                             name=(recipient.company_name or recipient.person_name),
                             postalCode=(recipient.postal_code or "").replace("-", ""),
                             city=recipient.city,
-                            street=lib.text(
-                                recipient.address_line1, recipient.address_line2
-                            ),
+                            street=recipient.address_line1,
                             houseNumber=(shipper.street_number or "N/A"),
-                            apartmentNumber=shipper.suite,
+                            apartmentNumber=recipient.address_line2,
                         ),
                     ),
                     neighbour=None,
                 ),
                 pieceList=dhl.ArrayOfPackage(
                     item=[
                         dhl.Package(
```

## Comparing `karrio.dhl_poland-2023.4.dist-info/METADATA` & `karrio.dhl_poland-2023.4.4.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karrio.dhl-poland
-Version: 2023.4
+Version: 2023.4.4
 Summary: Karrio - DHL Parcel Poland Shipping Extension
 Home-page: https://github.com/karrioapi/karrio
 Author: karrio
 Author-email: hello@karrio.io
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

## Comparing `karrio.dhl_poland-2023.4.dist-info/RECORD` & `karrio.dhl_poland-2023.4.4.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -5,12 +5,12 @@
 karrio/providers/dhl_poland/__init__.py,sha256=oLgXPC778tlkc-zFag7y40sBkgvf5IsTtt10FZ_e9Xk,328
 karrio/providers/dhl_poland/error.py,sha256=OXxiuVdmtW55THG8Uv0UTDC-wXoj_CENVRLK6niV6vs,621
 karrio/providers/dhl_poland/tracking.py,sha256=s90aAKkmrk1EbC1n_BKHMrc-H-y5-uznsMTE4hgElKU,2894
 karrio/providers/dhl_poland/units.py,sha256=KAQi3dkmsn4U5ghOCyg6uF2BmCSZUfVyTrA7XpXnWQY,4184
 karrio/providers/dhl_poland/utils.py,sha256=ETUe5XsIYzsQCX6seeZ-exzXWyWf87-qGY474x10lmQ,1851
 karrio/providers/dhl_poland/shipment/__init__.py,sha256=kH1OP9BIPNfzxj6k41NI5TGBQX6CZ9y0qinn3BkL9xI,236
 karrio/providers/dhl_poland/shipment/cancel.py,sha256=kUhh8IVU4j3QPTOy9SLnBsYtfKJesN1Wfo8xuqEKvHk,1565
-karrio/providers/dhl_poland/shipment/create.py,sha256=wCYrVq93jezD5YkbeJLJtY2ccPhwMdvebofGD09mfwc,13627
-karrio.dhl_poland-2023.4.dist-info/METADATA,sha256=dUe30wn3QMD9sckPa3mMgOZiaP9UlK3O3qZpbFzUplk,1026
-karrio.dhl_poland-2023.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-karrio.dhl_poland-2023.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
-karrio.dhl_poland-2023.4.dist-info/RECORD,,
+karrio/providers/dhl_poland/shipment/create.py,sha256=qbqpjAE-xU3duAowQYFimDyRX0LahoVAot0_XitR72U,13453
+karrio.dhl_poland-2023.4.4.dist-info/METADATA,sha256=citJXbTPjXNaH_pNNy3vpJS6VAcx3Z_ob4DXHJJ1Zmg,1028
+karrio.dhl_poland-2023.4.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+karrio.dhl_poland-2023.4.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
+karrio.dhl_poland-2023.4.4.dist-info/RECORD,,
```

