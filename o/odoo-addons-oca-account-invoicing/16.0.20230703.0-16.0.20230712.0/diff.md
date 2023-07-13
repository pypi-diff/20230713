# Comparing `tmp/odoo_addons_oca_account_invoicing-16.0.20230703.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_account_invoicing-16.0.20230712.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1672 bytes, number of entries: 4
--rw-r--r--  2.0 unx     2167 b- defN 23-Jul-04 02:46 odoo_addons_oca_account_invoicing-16.0.20230703.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 02:46 odoo_addons_oca_account_invoicing-16.0.20230703.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-04 02:46 odoo_addons_oca_account_invoicing-16.0.20230703.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      441 b- defN 23-Jul-04 02:46 odoo_addons_oca_account_invoicing-16.0.20230703.0.dist-info/RECORD
-4 files, 2701 bytes uncompressed, 802 bytes compressed:  70.3%
+Zip file size: 1691 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     2251 b- defN 23-Jul-13 02:46 odoo_addons_oca_account_invoicing-16.0.20230712.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-13 02:46 odoo_addons_oca_account_invoicing-16.0.20230712.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-13 02:46 odoo_addons_oca_account_invoicing-16.0.20230712.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      441 b- defN 23-Jul-13 02:46 odoo_addons_oca_account_invoicing-16.0.20230712.0.dist-info/RECORD
+4 files, 2785 bytes uncompressed, 821 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_account_invoicing-16.0.20230703.0.dist-info/METADATA
+Filename: odoo_addons_oca_account_invoicing-16.0.20230712.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_account_invoicing-16.0.20230703.0.dist-info/WHEEL
+Filename: odoo_addons_oca_account_invoicing-16.0.20230712.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_account_invoicing-16.0.20230703.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_account_invoicing-16.0.20230712.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_account_invoicing-16.0.20230703.0.dist-info/RECORD
+Filename: odoo_addons_oca_account_invoicing-16.0.20230712.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_account_invoicing-16.0.20230703.0.dist-info/METADATA` & `odoo_addons_oca_account_invoicing-16.0.20230712.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-account-invoicing
-Version: 16.0.20230703.0
+Version: 16.0.20230712.0
 Summary: Meta package for oca-account-invoicing Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
@@ -22,14 +22,15 @@
 Requires-Dist: odoo-addon-account-invoice-transmit-method (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-invoice-triple-discount (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-menu-invoice-refund (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-move-tier-validation (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-receipt-journal (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-receipt-send (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-tax-change (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-account-tax-group-widget-base-amount (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-invoicing-mode (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-invoicing-mode-at-shipping (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-partner-invoicing-mode-monthly (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-purchase-stock-picking-return-invoicing (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-sale-order-invoicing-grouping-criteria (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-stock-picking-return-refund-option (<16.1dev,>=16.0dev)
```

