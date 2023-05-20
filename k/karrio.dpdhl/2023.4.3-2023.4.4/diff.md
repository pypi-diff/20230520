# Comparing `tmp/karrio.dpdhl-2023.4.3-py3-none-any.whl.zip` & `tmp/karrio.dpdhl-2023.4.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 14537 bytes, number of entries: 16
+Zip file size: 14772 bytes, number of entries: 16
 -rw-rw-r--  2.0 unx      558 b- defN 23-Apr-23 04:04 karrio/mappers/dpdhl/__init__.py
 -rw-rw-r--  2.0 unx     2030 b- defN 23-Apr-23 04:04 karrio/mappers/dpdhl/mapper.py
 -rw-rw-r--  2.0 unx     2431 b- defN 23-Apr-23 04:04 karrio/mappers/dpdhl/proxy.py
 -rw-rw-r--  2.0 unx     1021 b- defN 23-Apr-23 04:04 karrio/mappers/dpdhl/settings.py
 -rw-rw-r--  2.0 unx      313 b- defN 22-Nov-15 19:21 karrio/providers/dpdhl/__init__.py
--rw-rw-r--  2.0 unx     4884 b- defN 23-Apr-23 05:01 karrio/providers/dpdhl/error.py
+-rw-rw-r--  2.0 unx     4884 b- defN 23-Apr-24 04:01 karrio/providers/dpdhl/error.py
 -rw-rw-r--  2.0 unx     3657 b- defN 23-Apr-23 04:04 karrio/providers/dpdhl/tracking.py
--rw-rw-r--  2.0 unx     7670 b- defN 23-Apr-23 04:04 karrio/providers/dpdhl/units.py
--rw-rw-r--  2.0 unx     1684 b- defN 23-Apr-23 04:04 karrio/providers/dpdhl/utils.py
+-rw-rw-r--  2.0 unx     8251 b- defN 23-May-20 10:45 karrio/providers/dpdhl/units.py
+-rw-rw-r--  2.0 unx     1903 b- defN 23-May-17 00:17 karrio/providers/dpdhl/utils.py
 -rw-rw-r--  2.0 unx      226 b- defN 22-Nov-15 19:21 karrio/providers/dpdhl/shipment/__init__.py
 -rw-rw-r--  2.0 unx     2425 b- defN 23-Apr-23 04:04 karrio/providers/dpdhl/shipment/cancel.py
--rw-rw-r--  2.0 unx    19559 b- defN 23-Apr-23 04:04 karrio/providers/dpdhl/shipment/create.py
--rw-rw-r--  2.0 unx      994 b- defN 23-Apr-23 05:37 karrio.dpdhl-2023.4.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-23 05:37 karrio.dpdhl-2023.4.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Apr-23 05:37 karrio.dpdhl-2023.4.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1419 b- defN 23-Apr-23 05:37 karrio.dpdhl-2023.4.3.dist-info/RECORD
-16 files, 48970 bytes uncompressed, 12161 bytes compressed:  75.2%
+-rw-rw-r--  2.0 unx    19628 b- defN 23-May-17 00:17 karrio/providers/dpdhl/shipment/create.py
+-rw-rw-r--  2.0 unx      994 b- defN 23-May-20 11:14 karrio.dpdhl-2023.4.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-20 11:14 karrio.dpdhl-2023.4.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-May-20 11:14 karrio.dpdhl-2023.4.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1419 b- defN 23-May-20 11:14 karrio.dpdhl-2023.4.4.dist-info/RECORD
+16 files, 49839 bytes uncompressed, 12396 bytes compressed:  75.1%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: karrio/providers/dpdhl/shipment/cancel.py
 Comment: 
 
 Filename: karrio/providers/dpdhl/shipment/create.py
 Comment: 
 
-Filename: karrio.dpdhl-2023.4.3.dist-info/METADATA
+Filename: karrio.dpdhl-2023.4.4.dist-info/METADATA
 Comment: 
 
-Filename: karrio.dpdhl-2023.4.3.dist-info/WHEEL
+Filename: karrio.dpdhl-2023.4.4.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.dpdhl-2023.4.3.dist-info/top_level.txt
+Filename: karrio.dpdhl-2023.4.4.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.dpdhl-2023.4.3.dist-info/RECORD
+Filename: karrio.dpdhl-2023.4.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/providers/dpdhl/units.py

```diff
@@ -1,11 +1,12 @@
 import typing
 import karrio.lib as lib
 import karrio.core.units as units
 import karrio.core.models as models
+import karrio.core.settings as settings
 
 
 class PackagingType(lib.Flag):
     """Carrier specific packaging type"""
 
     PACKAGE = "PACKAGE"
 
@@ -65,14 +66,15 @@
     FAS = "Free Alongside Ship"
     FCA = "Free Carrier"
     FOB = "Free On Board"
 
 
 class ConnectionConfig(lib.Enum):
     language_code = lib.OptionEnum("language_code")
+    service_suffix = lib.OptionEnum("service_suffix")
     shipping_options = lib.OptionEnum("shipping_options", list)
     shipping_services = lib.OptionEnum("shipping_services", list)
 
 
 class ShippingService(lib.Enum):
     """Carrier specific services"""
 
@@ -95,21 +97,31 @@
 
     @classmethod
     def account_suffix(
         cls: lib.Enum,
         account: str,
         service: str,
         options: units.Options,
+        settings: settings.Settings = None,
         is_international: bool = None,
     ):
         if len(account) > 10:
             return account
 
         _prefix = cls[service].value
-        _suffix = "01"
+        _svc_suffix = getattr(settings, "service_suffix", None)
+        _suffix = _svc_suffix if any(_svc_suffix or "") else "01"
+
+        if (
+            # is fixed suffix provided in settings use it
+            any(_svc_suffix or "")
+            # if not shipping options are defined, use default suffix
+            or options.has_content is False
+        ):
+            return f"{account}{_prefix}{_suffix}"
 
         if service == cls.V01PAK.name and (
             options.dpdhl_additional_insurance.state is not None
             or options.dpdhl_cash_on_delivery.state is not None
         ):
             _suffix = "03"
 
@@ -174,14 +186,15 @@
     dpdhl_endorsement = lib.OptionEnum("Endorsement", bool)
     dpdhl_go_green = lib.OptionEnum("GoGreen", bool)
     dpdhl_additional_insurance = lib.OptionEnum("AdditionalInsurance", float)
     dpdhl_bulky_goods = lib.OptionEnum("BulkyGoods", bool)
     dpdhl_cash_on_delivery = lib.OptionEnum("CashOnDelivery", float)
     dpdhl_premium = lib.OptionEnum("Premium", bool)
     dpdhl_parcel_outlet_routing = lib.OptionEnum("ParcelOutletRouting", bool)
+    dpdhl_packstation = lib.OptionEnum("Packstation")
 
     """ Unified Option type mapping """
     insurance = dpdhl_additional_insurance
     cash_on_dlivery = dpdhl_cash_on_delivery
     email_notification = dpdhl_notification
```

## karrio/providers/dpdhl/utils.py

```diff
@@ -1,7 +1,8 @@
+import typing
 import base64
 import karrio.lib as lib
 import karrio.core as core
 import dpdhl_lib.business_interface as dpdhl
 
 AuthentificationType = lib.mutate_xml_object_type(
     dpdhl.AuthentificationType,
@@ -47,18 +48,25 @@
 
         return lib.to_connection_config(
             self.config or {},
             option_type=ConnectionConfig,
         )
 
     @property
-    def language_code(self):
+    def language_code(self) -> str:
         return self.connection_config.language_code.state or "en"
 
     @property
+    def service_suffix(self) -> typing.Optional[str]:
+        return typing.cast(
+            typing.Optional[str],
+            self.connection_config.service_suffix.state,
+        )
+
+    @property
     def basic_authentication(self):
         pair = "%s:%s" % (
             (self.username, self.password)
             if self.test_mode
             else (self.app_id, self.app_token)
         )
         return base64.b64encode(pair.encode("utf-8")).decode("ascii")
```

## karrio/providers/dpdhl/shipment/create.py

```diff
@@ -65,21 +65,23 @@
         initializer=provider_units.shipping_options_initializer,
     )
 
     account_number = provider_units.ServicePrefix.account_suffix(
         settings.account_number,
         service=service,
         options=options,
+        settings=settings,
         is_international=shipper.country_code != recipient.country_code,
     )
     return_account_number = (
         provider_units.ServicePrefix.account_suffix(
             options.return_account_number.state,
             service=service,
             options=options,
+            settings=settings,
             is_international=shipper.country_code != recipient.country_code,
         )
         if options.return_account_number.state is not None
         else account_number
     )
 
     request = lib.Envelope(
@@ -216,26 +218,21 @@
                                     if options.email_notification.state
                                     else None
                                 ),
                                 BankData=None,
                             ),
                             Shipper=dpdhl.ShipperType(
                                 Name=dpdhl.NameType(
-                                    *lib.join(
-                                        shipper.person_name,
-                                        shipper.company_name or " ",
-                                    )
+                                    name1=shipper.address_line1,
+                                    name2=shipper.address_line2,
+                                    name3=None,
                                 ),
                                 Address=dpdhl.NativeAddressTypeNew(
-                                    streetName=(
-                                        shipper.street_name or shipper.address_line1
-                                    ),
-                                    streetNumber=(
-                                        shipper.street_number or shipper.address_line2
-                                    ),
+                                    streetName=shipper.street_name,
+                                    streetNumber=shipper.street_number,
                                     addressAddition=None,
                                     dispatchingInformation=None,
                                     zip=dpdhl.ZipType(shipper.postal_code),
                                     city=shipper.city,
                                     province=shipper.state_code,
                                     Origin=dpdhl.CountryType(
                                         country=shipper.country_name,
@@ -250,25 +247,27 @@
                                     )
                                     if shipper.has_contact_info
                                     else None
                                 ),
                             ),
                             ShipperReference=payload.reference,
                             Receiver=dpdhl.ReceiverType(
-                                name1=(recipient.person_name or recipient.company_name),
+                                name1=recipient.address_line1,
                                 Address=dpdhl.ReceiverNativeAddressType(
-                                    name2=recipient.company_name,
+                                    name2=(
+                                        options.dpdhl_packstation.state
+                                        or recipient.address_line2
+                                    ),
                                     name3=None,
                                     streetName=(
-                                        recipient.street_name or recipient.address_line1
-                                    ),
-                                    streetNumber=(
-                                        recipient.street_number
-                                        or recipient.address_line2
+                                        recipient.street_name
+                                        if (options.dpdhl_packstation.state is None)
+                                        else "Packstation"
                                     ),
+                                    streetNumber=recipient.street_number,
                                     addressAddition=None,
                                     dispatchingInformation=None,
                                     zip=dpdhl.ZipType(recipient.postal_code),
                                     city=recipient.city,
                                     province=recipient.state_code,
                                     Origin=dpdhl.CountryType(
                                         country=recipient.country_name,
@@ -277,15 +276,18 @@
                                 ),
                                 Packstation=None,
                                 Postfiliale=None,
                                 Communication=(
                                     dpdhl.CommunicationType(
                                         phone=recipient.phone_number,
                                         email=recipient.email,
-                                        contactPerson=recipient.person_name,
+                                        contactPerson=(
+                                            recipient.person_name
+                                            or recipient.company_name
+                                        ),
                                     )
                                     if recipient.has_contact_info
                                     else None
                                 ),
                             ),
                             ReturnReceiver=None,
                             ExportDocument=(
```

## Comparing `karrio.dpdhl-2023.4.3.dist-info/METADATA` & `karrio.dpdhl-2023.4.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karrio.dpdhl
-Version: 2023.4.3
+Version: 2023.4.4
 Summary: Karrio - Deutsche Post DHL Shipping extension
 Home-page: https://github.com/karrioapi/karrio
 Author: karrio
 Author-email: hello@karrio.io
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

## Comparing `karrio.dpdhl-2023.4.3.dist-info/RECORD` & `karrio.dpdhl-2023.4.4.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 karrio/mappers/dpdhl/__init__.py,sha256=hI9K0SVajo90niTvmU5BP9iV2QoOFh8tEbtZfVRax_c,558
 karrio/mappers/dpdhl/mapper.py,sha256=PX1mAMSFl8JmtAQ-SaKr8xDrV0eybOXzNLJbrUGKLfM,2030
 karrio/mappers/dpdhl/proxy.py,sha256=29jmjAngUb4FkLHu3bTB4leP7VxDROBb78-s8aAj4nk,2431
 karrio/mappers/dpdhl/settings.py,sha256=nRq7QoFa8Amrg1glJy_UmZ9fQUxuseC8KNKPltbifm0,1021
 karrio/providers/dpdhl/__init__.py,sha256=XtaZQrNssm_oho6v6SAYEH3cViuOZ3VFAPhHgW6f-yw,313
 karrio/providers/dpdhl/error.py,sha256=IKFlWE1FbfeNf6TjeB3L_lraLX716XpoDKCe87kgcDc,4884
 karrio/providers/dpdhl/tracking.py,sha256=Qn2luGRnyIlJkaa2JSRjlawLVq-jMnAkfFGRcJFugqc,3657
-karrio/providers/dpdhl/units.py,sha256=DDQX6MIFiYqMXl6exNkXfRbolbRD2czyMqeAcvMSk1w,7670
-karrio/providers/dpdhl/utils.py,sha256=Hdf1-fC0uK3SlNJlVb5ZlHshn2nC6hH61wO-EFvvCws,1684
+karrio/providers/dpdhl/units.py,sha256=6o2FddsCw2K49EwskglkMVWAjGODsgaaXFrlnnqdmc4,8251
+karrio/providers/dpdhl/utils.py,sha256=dDS7xkLYtrAeh89S5BnP3He3NmQXi8iSpCJ-BzuUjPI,1903
 karrio/providers/dpdhl/shipment/__init__.py,sha256=5tF7dih8kTSVa5pw4UXU8_byCMnuvtsJIz_h7VAOOyY,226
 karrio/providers/dpdhl/shipment/cancel.py,sha256=1Z_h5EUUNLS7LAiLLU04dkEPufmXSJGavvn543FGxQE,2425
-karrio/providers/dpdhl/shipment/create.py,sha256=AKmTE_tcKX3n7wStuyFZGJXU5H8J40WgqZqLVSV96gg,19559
-karrio.dpdhl-2023.4.3.dist-info/METADATA,sha256=5SrdVdSxeyoi-ghiVWx7BuWSTqHNCuo7Kfer8NpDCWI,994
-karrio.dpdhl-2023.4.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-karrio.dpdhl-2023.4.3.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
-karrio.dpdhl-2023.4.3.dist-info/RECORD,,
+karrio/providers/dpdhl/shipment/create.py,sha256=KinIFL3yosgs4v7nXHMy5XNDzjAI1XYrtvCu3GqnfYQ,19628
+karrio.dpdhl-2023.4.4.dist-info/METADATA,sha256=2F5rrzY3oaqKNnKn2vwFRh4BK3JNeAhV4-m2jkdsdUA,994
+karrio.dpdhl-2023.4.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+karrio.dpdhl-2023.4.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
+karrio.dpdhl-2023.4.4.dist-info/RECORD,,
```

