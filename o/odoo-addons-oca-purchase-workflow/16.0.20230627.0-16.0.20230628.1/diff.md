# Comparing `tmp/odoo_addons_oca_purchase_workflow-16.0.20230627.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_purchase_workflow-16.0.20230628.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1736 bytes, number of entries: 4
--rw-r--r--  2.0 unx     2772 b- defN 23-Jun-28 04:53 odoo_addons_oca_purchase_workflow-16.0.20230627.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-28 04:53 odoo_addons_oca_purchase_workflow-16.0.20230627.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-28 04:53 odoo_addons_oca_purchase_workflow-16.0.20230627.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      441 b- defN 23-Jun-28 04:53 odoo_addons_oca_purchase_workflow-16.0.20230627.0.dist-info/RECORD
-4 files, 3306 bytes uncompressed, 866 bytes compressed:  73.8%
+Zip file size: 1751 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     2910 b- defN 23-Jun-29 05:45 odoo_addons_oca_purchase_workflow-16.0.20230628.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-29 05:45 odoo_addons_oca_purchase_workflow-16.0.20230628.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-29 05:45 odoo_addons_oca_purchase_workflow-16.0.20230628.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      441 b- defN 23-Jun-29 05:45 odoo_addons_oca_purchase_workflow-16.0.20230628.1.dist-info/RECORD
+4 files, 3444 bytes uncompressed, 881 bytes compressed:  74.4%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_purchase_workflow-16.0.20230627.0.dist-info/METADATA
+Filename: odoo_addons_oca_purchase_workflow-16.0.20230628.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_purchase_workflow-16.0.20230627.0.dist-info/WHEEL
+Filename: odoo_addons_oca_purchase_workflow-16.0.20230628.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_purchase_workflow-16.0.20230627.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_purchase_workflow-16.0.20230628.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_purchase_workflow-16.0.20230627.0.dist-info/RECORD
+Filename: odoo_addons_oca_purchase_workflow-16.0.20230628.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_purchase_workflow-16.0.20230627.0.dist-info/METADATA` & `odoo_addons_oca_purchase_workflow-16.0.20230628.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-purchase-workflow
-Version: 16.0.20230627.0
+Version: 16.0.20230628.1
 Summary: Meta package for oca-purchase-workflow Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
@@ -20,23 +20,25 @@
 Requires-Dist: odoo-addon-purchase-force-invoiced (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-purchase-last-price-info (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-purchase-line-procurement-group (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-purchase-location-by-line (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-purchase-lot (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-purchase-merge (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-purchase-no-rfq (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-purchase-open-qty (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-purchase-order-approved (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-purchase-order-line-menu (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-purchase-order-no-zero-price (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-purchase-order-owner (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-purchase-order-product-recommendation (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-purchase-order-supplierinfo-update (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-purchase-order-type (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-purchase-order-type-dashboard (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-purchase-order-uninvoiced-amount (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-purchase-partner-incoterm (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-purchase-partner-selectable-option (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-purchase-request (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-purchase-request-tier-validation (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-purchase-requisition-tier-validation (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-purchase-security (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-purchase-stock-packaging (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-purchase-tag (<16.1dev,>=16.0dev)
```

