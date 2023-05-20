# Comparing `tmp/odoo_addons_oca_hr_expense-15.0.20230518.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_hr_expense-15.0.20230519.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1462 bytes, number of entries: 4
--rw-r--r--  2.0 unx     1234 b- defN 23-May-19 05:02 odoo_addons_oca_hr_expense-15.0.20230518.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-19 05:02 odoo_addons_oca_hr_expense-15.0.20230518.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-19 05:02 odoo_addons_oca_hr_expense-15.0.20230518.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      413 b- defN 23-May-19 05:02 odoo_addons_oca_hr_expense-15.0.20230518.0.dist-info/RECORD
-4 files, 1740 bytes uncompressed, 648 bytes compressed:  62.8%
+Zip file size: 1479 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     1380 b- defN 23-May-20 07:15 odoo_addons_oca_hr_expense-15.0.20230519.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-20 07:15 odoo_addons_oca_hr_expense-15.0.20230519.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-20 07:15 odoo_addons_oca_hr_expense-15.0.20230519.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      413 b- defN 23-May-20 07:15 odoo_addons_oca_hr_expense-15.0.20230519.1.dist-info/RECORD
+4 files, 1886 bytes uncompressed, 665 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_hr_expense-15.0.20230518.0.dist-info/METADATA
+Filename: odoo_addons_oca_hr_expense-15.0.20230519.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_hr_expense-15.0.20230518.0.dist-info/WHEEL
+Filename: odoo_addons_oca_hr_expense-15.0.20230519.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_hr_expense-15.0.20230518.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_hr_expense-15.0.20230519.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_hr_expense-15.0.20230518.0.dist-info/RECORD
+Filename: odoo_addons_oca_hr_expense-15.0.20230519.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_hr_expense-15.0.20230518.0.dist-info/METADATA` & `odoo_addons_oca_hr_expense-15.0.20230519.1.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-hr-expense
-Version: 15.0.20230518.0
+Version: 15.0.20230519.1
 Summary: Meta package for oca-hr-expense Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 15.0
 Requires-Dist: odoo-addon-hr-expense-advance-clearing (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-hr-expense-advance-clearing-sequence (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-hr-expense-cancel (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-hr-expense-exception (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-hr-expense-invoice (<15.1dev,>=15.0dev)
+Requires-Dist: odoo-addon-hr-expense-pay-to-vendor (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-hr-expense-payment (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-hr-expense-payment-widget-amount (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-hr-expense-petty-cash (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-hr-expense-portal (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-hr-expense-sequence (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-hr-expense-tax-adjust (<15.1dev,>=15.0dev)
+Requires-Dist: odoo-addon-hr-expense-tier-validation (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-sale-expense-cost-reinvoice (<15.1dev,>=15.0dev)
 Requires-Dist: odoo-addon-sale-expense-manual-reinvoice (<15.1dev,>=15.0dev)
 
 UNKNOWN
```

