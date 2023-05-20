# Comparing `tmp/karrio.dpd-2023.4-py3-none-any.whl.zip` & `tmp/karrio.dpd-2023.4.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 13293 bytes, number of entries: 15
--rw-rw-r--  2.0 unx      462 b- defN 23-Mar-30 19:14 karrio/mappers/dpd/__init__.py
--rw-rw-r--  2.0 unx     1576 b- defN 23-Apr-01 12:45 karrio/mappers/dpd/mapper.py
--rw-rw-r--  2.0 unx     1855 b- defN 23-Apr-01 12:45 karrio/mappers/dpd/proxy.py
--rw-rw-r--  2.0 unx     1270 b- defN 23-Apr-15 06:44 karrio/mappers/dpd/settings.py
+Zip file size: 13309 bytes, number of entries: 15
+-rw-rw-r--  2.0 unx      462 b- defN 23-Apr-23 04:04 karrio/mappers/dpd/__init__.py
+-rw-rw-r--  2.0 unx     1576 b- defN 23-Apr-23 04:04 karrio/mappers/dpd/mapper.py
+-rw-rw-r--  2.0 unx     1855 b- defN 23-Apr-23 04:04 karrio/mappers/dpd/proxy.py
+-rw-rw-r--  2.0 unx     1270 b- defN 23-Apr-23 04:04 karrio/mappers/dpd/settings.py
 -rw-rw-r--  2.0 unx      242 b- defN 23-Mar-27 07:55 karrio/providers/dpd/__init__.py
 -rw-rw-r--  2.0 unx     1037 b- defN 23-Mar-27 07:55 karrio/providers/dpd/error.py
--rw-rw-r--  2.0 unx     4241 b- defN 23-Apr-01 15:19 karrio/providers/dpd/tracking.py
+-rw-rw-r--  2.0 unx     4241 b- defN 23-Apr-23 04:04 karrio/providers/dpd/tracking.py
 -rw-rw-r--  2.0 unx     7720 b- defN 23-Mar-27 07:55 karrio/providers/dpd/units.py
 -rw-rw-r--  2.0 unx     3990 b- defN 23-Mar-27 07:55 karrio/providers/dpd/utils.py
 -rw-rw-r--  2.0 unx      104 b- defN 23-Mar-27 07:55 karrio/providers/dpd/shipment/__init__.py
--rw-rw-r--  2.0 unx    22002 b- defN 23-Apr-01 15:18 karrio/providers/dpd/shipment/create.py
--rw-rw-r--  2.0 unx      950 b- defN 23-Apr-18 07:10 karrio.dpd-2023.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-18 07:10 karrio.dpd-2023.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Apr-18 07:10 karrio.dpd-2023.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1283 b- defN 23-Apr-18 07:10 karrio.dpd-2023.4.dist-info/RECORD
-15 files, 46831 bytes uncompressed, 11151 bytes compressed:  76.2%
+-rw-rw-r--  2.0 unx    21830 b- defN 23-May-17 00:17 karrio/providers/dpd/shipment/create.py
+-rw-rw-r--  2.0 unx      952 b- defN 23-May-20 11:14 karrio.dpd-2023.4.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-20 11:14 karrio.dpd-2023.4.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-May-20 11:14 karrio.dpd-2023.4.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1291 b- defN 23-May-20 11:14 karrio.dpd-2023.4.4.dist-info/RECORD
+15 files, 46669 bytes uncompressed, 11151 bytes compressed:  76.1%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: karrio/providers/dpd/shipment/__init__.py
 Comment: 
 
 Filename: karrio/providers/dpd/shipment/create.py
 Comment: 
 
-Filename: karrio.dpd-2023.4.dist-info/METADATA
+Filename: karrio.dpd-2023.4.4.dist-info/METADATA
 Comment: 
 
-Filename: karrio.dpd-2023.4.dist-info/WHEEL
+Filename: karrio.dpd-2023.4.4.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.dpd-2023.4.dist-info/top_level.txt
+Filename: karrio.dpd-2023.4.4.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.dpd-2023.4.dist-info/RECORD
+Filename: karrio.dpd-2023.4.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/providers/dpd/shipment/create.py

```diff
@@ -268,18 +268,15 @@
                                             idDocType=None,
                                             idDocNumber=None,
                                             webSite=None,
                                             referenceNumber=None,
                                             destinationCountryRegistration=None,
                                         ),
                                         commercialInvoiceConsignor=dpd.address(
-                                            name1=(
-                                                shipper.person_name
-                                                or shipper.company_name
-                                            ),
+                                            name1=shipper.contact,
                                             name2=shipper.company_name,
                                             street=shipper.address_line1,
                                             houseNo=shipper.street_number,
                                             street2=shipper.address_line2,
                                             state=shipper.state_code,
                                             country=shipper.country_code,
                                             zipCode=shipper.postal_code,
```

## Comparing `karrio.dpd-2023.4.dist-info/METADATA` & `karrio.dpd-2023.4.4.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karrio.dpd
-Version: 2023.4
+Version: 2023.4.4
 Summary: Karrio - DPD Shipping Extension
 Home-page: https://github.com/karrioapi/karrio
 Author: karrio
 Author-email: hello@karrio.io
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

## Comparing `karrio.dpd-2023.4.dist-info/RECORD` & `karrio.dpd-2023.4.4.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -4,12 +4,12 @@
 karrio/mappers/dpd/settings.py,sha256=yWSi4yXm-NJ86C7hmTTP0IXemSKNiqbeJLZcprT3LYM,1270
 karrio/providers/dpd/__init__.py,sha256=q84FCmlbGI4Wo94ixjqQL4Mkeo08V1zj1PF0wizJYvs,242
 karrio/providers/dpd/error.py,sha256=XBuROolEZedFyV9rCukYSZvRQDi9RjChbrmOTS7Tlv0,1037
 karrio/providers/dpd/tracking.py,sha256=ds_bML0xPjrYsJiZH-01ehdJwE1VXqu1Dw4sCvzk90k,4241
 karrio/providers/dpd/units.py,sha256=a1mDI8DyRgOqb2syhh9iNmF7slcrVcq0uuwIhUw-Hkw,7720
 karrio/providers/dpd/utils.py,sha256=ec-58iGrCmirgAIKtyRKIfVEHReqzRmm78Ca1lV41v0,3990
 karrio/providers/dpd/shipment/__init__.py,sha256=60BkyUw1p_8mF9wiv-lO30Pt73BZ1GblL8wcZsUViCo,104
-karrio/providers/dpd/shipment/create.py,sha256=E1srCfOsGpmUmnZtVdA_8XJK-2IoLslxrqFx2Pv4jw4,22002
-karrio.dpd-2023.4.dist-info/METADATA,sha256=aIiqTvCPlbp7Pp4A0Zc6k0e5uBtbw_UbeoVWCRcGZa4,950
-karrio.dpd-2023.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-karrio.dpd-2023.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
-karrio.dpd-2023.4.dist-info/RECORD,,
+karrio/providers/dpd/shipment/create.py,sha256=YctaCjvs502jR07TlMTk-uY5WCcCMDMtn-rmNaESw0Q,21830
+karrio.dpd-2023.4.4.dist-info/METADATA,sha256=ah14ZjXamSWTilE2flTLVUsJUXKZbRKNFEcYhQ3XVb0,952
+karrio.dpd-2023.4.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+karrio.dpd-2023.4.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
+karrio.dpd-2023.4.4.dist-info/RECORD,,
```

