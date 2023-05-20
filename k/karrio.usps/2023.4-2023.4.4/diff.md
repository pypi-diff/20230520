# Comparing `tmp/karrio.usps-2023.4-py3-none-any.whl.zip` & `tmp/karrio.usps-2023.4.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 18072 bytes, number of entries: 21
+Zip file size: 18073 bytes, number of entries: 21
 -rw-rw-r--  2.0 unx      450 b- defN 22-Nov-15 19:21 karrio/mappers/usps/__init__.py
--rw-rw-r--  2.0 unx     3442 b- defN 23-Apr-01 13:34 karrio/mappers/usps/mapper.py
--rw-rw-r--  2.0 unx     1969 b- defN 23-Apr-01 13:48 karrio/mappers/usps/proxy.py
--rw-rw-r--  2.0 unx      572 b- defN 23-Apr-15 06:44 karrio/mappers/usps/settings.py
+-rw-rw-r--  2.0 unx     3442 b- defN 23-Apr-23 04:04 karrio/mappers/usps/mapper.py
+-rw-rw-r--  2.0 unx     1969 b- defN 23-Apr-23 04:04 karrio/mappers/usps/proxy.py
+-rw-rw-r--  2.0 unx      572 b- defN 23-Apr-23 04:04 karrio/mappers/usps/settings.py
 -rw-rw-r--  2.0 unx      613 b- defN 22-Nov-15 19:21 karrio/providers/usps/__init__.py
 -rw-rw-r--  2.0 unx      722 b- defN 22-Nov-15 19:21 karrio/providers/usps/error.py
--rw-rw-r--  2.0 unx     6216 b- defN 23-Apr-01 15:18 karrio/providers/usps/rate.py
--rw-rw-r--  2.0 unx     3419 b- defN 23-Apr-01 15:18 karrio/providers/usps/tracking.py
+-rw-rw-r--  2.0 unx     6216 b- defN 23-Apr-23 04:04 karrio/providers/usps/rate.py
+-rw-rw-r--  2.0 unx     3419 b- defN 23-Apr-23 04:04 karrio/providers/usps/tracking.py
 -rw-rw-r--  2.0 unx    16295 b- defN 23-Mar-27 07:55 karrio/providers/usps/units.py
--rw-rw-r--  2.0 unx      734 b- defN 23-Apr-15 06:44 karrio/providers/usps/utils.py
+-rw-rw-r--  2.0 unx      734 b- defN 23-Apr-23 04:04 karrio/providers/usps/utils.py
 -rw-rw-r--  2.0 unx      286 b- defN 22-Nov-15 19:21 karrio/providers/usps/pickup/__init__.py
--rw-rw-r--  2.0 unx     1568 b- defN 23-Apr-01 15:18 karrio/providers/usps/pickup/cancel.py
--rw-rw-r--  2.0 unx     1926 b- defN 23-Apr-01 15:18 karrio/providers/usps/pickup/create.py
--rw-rw-r--  2.0 unx     2008 b- defN 23-Apr-01 15:18 karrio/providers/usps/pickup/update.py
+-rw-rw-r--  2.0 unx     1568 b- defN 23-Apr-23 04:04 karrio/providers/usps/pickup/cancel.py
+-rw-rw-r--  2.0 unx     1926 b- defN 23-Apr-23 04:04 karrio/providers/usps/pickup/create.py
+-rw-rw-r--  2.0 unx     2008 b- defN 23-Apr-23 04:04 karrio/providers/usps/pickup/update.py
 -rw-rw-r--  2.0 unx      198 b- defN 22-Nov-15 19:21 karrio/providers/usps/shipment/__init__.py
--rw-rw-r--  2.0 unx     1614 b- defN 23-Apr-01 15:18 karrio/providers/usps/shipment/cancel.py
--rw-rw-r--  2.0 unx     7701 b- defN 23-Apr-01 15:18 karrio/providers/usps/shipment/create.py
--rw-rw-r--  2.0 unx      964 b- defN 23-Apr-18 07:09 karrio.usps-2023.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 07:09 karrio.usps-2023.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Apr-18 07:09 karrio.usps-2023.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1859 b- defN 23-Apr-18 07:09 karrio.usps-2023.4.dist-info/RECORD
-21 files, 52655 bytes uncompressed, 14998 bytes compressed:  71.5%
+-rw-rw-r--  2.0 unx     1614 b- defN 23-Apr-23 04:04 karrio/providers/usps/shipment/cancel.py
+-rw-rw-r--  2.0 unx     7619 b- defN 23-May-17 00:17 karrio/providers/usps/shipment/create.py
+-rw-rw-r--  2.0 unx      966 b- defN 23-May-20 11:14 karrio.usps-2023.4.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-20 11:14 karrio.usps-2023.4.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-May-20 11:14 karrio.usps-2023.4.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1867 b- defN 23-May-20 11:14 karrio.usps-2023.4.4.dist-info/RECORD
+21 files, 52583 bytes uncompressed, 14983 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -45,20 +45,20 @@
 
 Filename: karrio/providers/usps/shipment/cancel.py
 Comment: 
 
 Filename: karrio/providers/usps/shipment/create.py
 Comment: 
 
-Filename: karrio.usps-2023.4.dist-info/METADATA
+Filename: karrio.usps-2023.4.4.dist-info/METADATA
 Comment: 
 
-Filename: karrio.usps-2023.4.dist-info/WHEEL
+Filename: karrio.usps-2023.4.4.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.usps-2023.4.dist-info/top_level.txt
+Filename: karrio.usps-2023.4.4.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.usps-2023.4.dist-info/RECORD
+Filename: karrio.usps-2023.4.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/providers/usps/shipment/create.py

```diff
@@ -89,26 +89,26 @@
         ImageParameters=ImageParametersType(
             ImageParameter=label_format,
             LabelSequence=LabelSequenceType(PackageNumber=1, TotalPackages=1),
         ),
         FromName=shipper.person_name,
         FromFirm=shipper.company_name or "N/A",
         FromAddress1=shipper.address_line2 or "",
-        FromAddress2=lib.text(shipper.street_number, shipper.address_line1),
+        FromAddress2=shipper.street,
         FromCity=shipper.city,
         FromState=shipper.state_code,
         FromZip5=lib.to_zip5(shipper.postal_code) or "",
         FromZip4=lib.to_zip4(shipper.postal_code) or "",
         FromPhone=shipper.phone_number,
         POZipCode=None,
         AllowNonCleansedOriginAddr=False,
         ToName=recipient.person_name,
         ToFirm=recipient.company_name or "N/A",
         ToAddress1=recipient.address_line2,
-        ToAddress2=lib.text(recipient.street_number, recipient.address_line1),
+        ToAddress2=recipient.street,
         ToCity=recipient.city,
         ToState=recipient.state_code,
         ToZip5=lib.to_zip5(recipient.postal_code) or "",
         ToZip4=lib.to_zip4(recipient.postal_code) or "",
         ToPhone=recipient.phone_number,
         POBox=None,
         ToContactPreference=None,
```

## Comparing `karrio.usps-2023.4.dist-info/METADATA` & `karrio.usps-2023.4.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karrio.usps
-Version: 2023.4
+Version: 2023.4.4
 Summary: Karrio - USPS Shipping extension
 Home-page: https://github.com/karrioapi/karrio
 Author: karrio
 Author-email: hello@karrio.io
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

## Comparing `karrio.usps-2023.4.dist-info/RECORD` & `karrio.usps-2023.4.4.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 karrio/providers/usps/utils.py,sha256=EB5z8FZrk24So3s267pv2TeCtOeKB8zAqzOG4Ba9Ypc,734
 karrio/providers/usps/pickup/__init__.py,sha256=YTFtc6O-bbi1NhsYbug5vag4GmbmvXms88lGbSWeZ0E,286
 karrio/providers/usps/pickup/cancel.py,sha256=BBewXX3WNjO_aQIoY6h2O4H14cHApe3fsGzeOhBFkZg,1568
 karrio/providers/usps/pickup/create.py,sha256=MtoEZXmbJpPe3q5nZB8XkeFHwWYJa5ykpvMD7EaP67s,1926
 karrio/providers/usps/pickup/update.py,sha256=4xDQRQ36aWlgpu_TEIJp1D_6Zmi6Hznk6__APuD5bAw,2008
 karrio/providers/usps/shipment/__init__.py,sha256=ZGECAADplncp0tiq9F_mawDECcgZS_kOCVMIzVfTnKE,198
 karrio/providers/usps/shipment/cancel.py,sha256=Noo8-0R1sJIzLaGN1Dx6eF0qT_PDIbkQvisbgV7zbh0,1614
-karrio/providers/usps/shipment/create.py,sha256=toiPyAlVef0LAnBqnhmH2UEMsKUCceQLu3-uosQmSoM,7701
-karrio.usps-2023.4.dist-info/METADATA,sha256=rRhwuhmpls2ORGNrrTil977FC0tBxgp59jsiUazXq-E,964
-karrio.usps-2023.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-karrio.usps-2023.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
-karrio.usps-2023.4.dist-info/RECORD,,
+karrio/providers/usps/shipment/create.py,sha256=R6FPF3UJv5pR2hAbupegBGhDJxaiUN4kCD2Lz-FnpVM,7619
+karrio.usps-2023.4.4.dist-info/METADATA,sha256=3AmCoo5601EPWHRe8RLtrTc5cRmm1HaoMM45fK0RqOE,966
+karrio.usps-2023.4.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+karrio.usps-2023.4.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
+karrio.usps-2023.4.4.dist-info/RECORD,,
```

