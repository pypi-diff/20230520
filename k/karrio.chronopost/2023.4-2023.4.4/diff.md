# Comparing `tmp/karrio.chronopost-2023.4-py3-none-any.whl.zip` & `tmp/karrio.chronopost-2023.4.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 11531 bytes, number of entries: 17
+Zip file size: 11523 bytes, number of entries: 17
 -rw-rw-r--  2.0 unx      482 b- defN 22-Nov-15 19:21 karrio/mappers/chronopost/__init__.py
--rw-rw-r--  2.0 unx     1910 b- defN 23-Apr-01 13:34 karrio/mappers/chronopost/mapper.py
--rw-rw-r--  2.0 unx     1742 b- defN 23-Apr-01 13:39 karrio/mappers/chronopost/proxy.py
--rw-rw-r--  2.0 unx      538 b- defN 23-Apr-15 06:44 karrio/mappers/chronopost/settings.py
+-rw-rw-r--  2.0 unx     1910 b- defN 23-Apr-23 04:04 karrio/mappers/chronopost/mapper.py
+-rw-rw-r--  2.0 unx     1742 b- defN 23-Apr-23 04:04 karrio/mappers/chronopost/proxy.py
+-rw-rw-r--  2.0 unx      538 b- defN 23-Apr-23 04:04 karrio/mappers/chronopost/settings.py
 -rw-rw-r--  2.0 unx      407 b- defN 22-Nov-15 19:21 karrio/providers/chronopost/__init__.py
 -rw-rw-r--  2.0 unx      678 b- defN 22-Nov-15 19:21 karrio/providers/chronopost/error.py
--rw-rw-r--  2.0 unx     3060 b- defN 23-Apr-01 15:18 karrio/providers/chronopost/rate.py
--rw-rw-r--  2.0 unx     2959 b- defN 23-Apr-01 15:19 karrio/providers/chronopost/tracking.py
+-rw-rw-r--  2.0 unx     3060 b- defN 23-Apr-23 04:04 karrio/providers/chronopost/rate.py
+-rw-rw-r--  2.0 unx     2959 b- defN 23-Apr-23 04:04 karrio/providers/chronopost/tracking.py
 -rw-rw-r--  2.0 unx     1663 b- defN 23-Jan-11 18:22 karrio/providers/chronopost/units.py
 -rw-rw-r--  2.0 unx      800 b- defN 23-Apr-15 02:55 karrio/providers/chronopost/utils.py
 -rw-rw-r--  2.0 unx      236 b- defN 22-Nov-15 19:21 karrio/providers/chronopost/shipment/__init__.py
--rw-rw-r--  2.0 unx     1733 b- defN 23-Apr-01 15:18 karrio/providers/chronopost/shipment/cancel.py
--rw-rw-r--  2.0 unx     8560 b- defN 23-Apr-01 15:18 karrio/providers/chronopost/shipment/create.py
--rw-rw-r--  2.0 unx     1013 b- defN 23-Apr-18 07:09 karrio.chronopost-2023.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 07:09 karrio.chronopost-2023.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Apr-18 07:09 karrio.chronopost-2023.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1580 b- defN 23-Apr-18 07:09 karrio.chronopost-2023.4.dist-info/RECORD
-17 files, 27460 bytes uncompressed, 8865 bytes compressed:  67.7%
+-rw-rw-r--  2.0 unx     1733 b- defN 23-Apr-23 04:04 karrio/providers/chronopost/shipment/cancel.py
+-rw-rw-r--  2.0 unx     8282 b- defN 23-May-17 00:17 karrio/providers/chronopost/shipment/create.py
+-rw-rw-r--  2.0 unx     1015 b- defN 23-May-20 11:14 karrio.chronopost-2023.4.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-20 11:14 karrio.chronopost-2023.4.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-May-20 11:14 karrio.chronopost-2023.4.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1588 b- defN 23-May-20 11:14 karrio.chronopost-2023.4.4.dist-info/RECORD
+17 files, 27192 bytes uncompressed, 8841 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -33,20 +33,20 @@
 
 Filename: karrio/providers/chronopost/shipment/cancel.py
 Comment: 
 
 Filename: karrio/providers/chronopost/shipment/create.py
 Comment: 
 
-Filename: karrio.chronopost-2023.4.dist-info/METADATA
+Filename: karrio.chronopost-2023.4.4.dist-info/METADATA
 Comment: 
 
-Filename: karrio.chronopost-2023.4.dist-info/WHEEL
+Filename: karrio.chronopost-2023.4.4.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.chronopost-2023.4.dist-info/top_level.txt
+Filename: karrio.chronopost-2023.4.4.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.chronopost-2023.4.dist-info/RECORD
+Filename: karrio.chronopost-2023.4.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/providers/chronopost/shipment/create.py

```diff
@@ -64,17 +64,15 @@
     request = lib.Envelope(
         Body=lib.Body(
             chronopost.shippingMultiParcelV5(
                 esdValue=None,
                 headerValue=settings.header_value,
                 shipperValue=(
                     chronopost.shipperValue(
-                        shipperAdress1=lib.text(
-                            shipper.street_number, shipper.address_line1
-                        ),
+                        shipperAdress1=shipper.street,
                         shipperAdress2=shipper.address_line2,
                         shipperCity=shipper.city,
                         shipperContactName=shipper.person_name,
                         shipperCountry=shipper.country_code,
                         shipperCountryName=shipper.country_name,
                         shipperEmail=shipper.email,
                         shipperMobilePhone=shipper.phone_number,
@@ -82,17 +80,15 @@
                         shipperName2=shipper.company_name,
                         shipperPreAlert=0,
                         shipperCivility="M",
                         shipperZipCode=shipper.postal_code,
                     ),
                 ),
                 customerValue=chronopost.customerValue(
-                    customerAdress1=lib.text(
-                        recipient.street_number, recipient.address_line1
-                    ),
+                    customerAdress1=recipient.street,
                     customerAdress2=recipient.address_line2,
                     customerCity=recipient.city,
                     customerContactName=recipient.person_name,
                     customerCountry=recipient.country_code,
                     customerCountryName=recipient.country_name,
                     customerEmail=recipient.email,
                     customerMobilePhone=recipient.phone_number,
@@ -101,17 +97,15 @@
                     customerPreAlert=0,
                     customerZipCode=recipient.postal_code,
                     printAsSender=None,
                     customerCivility="M",
                 ),
                 recipientValue=(
                     chronopost.recipientValue(
-                        recipientAdress1=lib.text(
-                            recipient.street_number, recipient.address_line1
-                        ),
+                        recipientAdress1=recipient.street,
                         recipientAdress2=recipient.address_line2,
                         recipientCity=recipient.city,
                         recipientContactName=recipient.person_name,
                         recipientCountry=recipient.country_code,
                         recipientCountryName=recipient.country_name,
                         recipientEmail=recipient.email,
                         recipientMobilePhone=recipient.phone_number,
```

## Comparing `karrio.chronopost-2023.4.dist-info/METADATA` & `karrio.chronopost-2023.4.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karrio.chronopost
-Version: 2023.4
+Version: 2023.4.4
 Summary: Karrio - Chronopost Shipping Extension
 Home-page: https://github.com/karrioapi/karrio
 Author: karrio
 Author-email: hello@karrio.io
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

## Comparing `karrio.chronopost-2023.4.dist-info/RECORD` & `karrio.chronopost-2023.4.4.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -6,12 +6,12 @@
 karrio/providers/chronopost/error.py,sha256=5Kt8vVCN0fj0Add9tCii66fBfr3dWTCJ0DVaOMxf_D0,678
 karrio/providers/chronopost/rate.py,sha256=UxmtY5CW65abZYQP4KErhG0eeNE4EZHNf3XbNLANNGQ,3060
 karrio/providers/chronopost/tracking.py,sha256=atAPqxxIDsFL45oW2P7BGAflLE_9HQabn6DFE_6sO68,2959
 karrio/providers/chronopost/units.py,sha256=jZVxZgO_1N2w3inhf5_GRoGJ-UHvPL2DKC2LSyGlxyc,1663
 karrio/providers/chronopost/utils.py,sha256=U8a36xPS4zNIAWWeJMxE2S9zoJ8oxnGEWR3UF1s3olE,800
 karrio/providers/chronopost/shipment/__init__.py,sha256=Qps1uXAaxVmDCPV54GVgnGfzqy51KZlDBBiSt5Z4QqY,236
 karrio/providers/chronopost/shipment/cancel.py,sha256=IZ4hHC3piisGhdxZRxvZh_7pBfzNDNA3H9Fn52S2EsE,1733
-karrio/providers/chronopost/shipment/create.py,sha256=bcIHVEUjnMbVyyOuPZXdi8dcJyYJb7RJgcJqhqDtnLI,8560
-karrio.chronopost-2023.4.dist-info/METADATA,sha256=us-nnx6xm2pMhE_Gtd6-SyohyZpvsLG72eUMOpsZKak,1013
-karrio.chronopost-2023.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-karrio.chronopost-2023.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
-karrio.chronopost-2023.4.dist-info/RECORD,,
+karrio/providers/chronopost/shipment/create.py,sha256=Q6eceVj4qr_zjOBD0ltRnEITavKgUdQ4BDaLzrep8BM,8282
+karrio.chronopost-2023.4.4.dist-info/METADATA,sha256=-2afB_dHnD3nb9dH1gLckuuH19jQ6-USgsat61QMGWY,1015
+karrio.chronopost-2023.4.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+karrio.chronopost-2023.4.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
+karrio.chronopost-2023.4.4.dist-info/RECORD,,
```

