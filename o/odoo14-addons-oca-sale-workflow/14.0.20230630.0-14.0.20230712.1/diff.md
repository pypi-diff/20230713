# Comparing `tmp/odoo14_addons_oca_sale_workflow-14.0.20230630.0-py3-none-any.whl.zip` & `tmp/odoo14_addons_oca_sale_workflow-14.0.20230712.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 2475 bytes, number of entries: 4
--rw-r--r--  2.0 unx     6876 b- defN 23-Jul-02 05:03 odoo14_addons_oca_sale_workflow-14.0.20230630.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 05:03 odoo14_addons_oca_sale_workflow-14.0.20230630.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-02 05:03 odoo14_addons_oca_sale_workflow-14.0.20230630.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      433 b- defN 23-Jul-02 05:03 odoo14_addons_oca_sale_workflow-14.0.20230630.0.dist-info/RECORD
-4 files, 7402 bytes uncompressed, 1621 bytes compressed:  78.1%
+Zip file size: 2485 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     6967 b- defN 23-Jul-13 05:09 odoo14_addons_oca_sale_workflow-14.0.20230712.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-13 05:09 odoo14_addons_oca_sale_workflow-14.0.20230712.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-13 05:09 odoo14_addons_oca_sale_workflow-14.0.20230712.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      433 b- defN 23-Jul-13 05:09 odoo14_addons_oca_sale_workflow-14.0.20230712.1.dist-info/RECORD
+4 files, 7493 bytes uncompressed, 1631 bytes compressed:  78.2%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo14_addons_oca_sale_workflow-14.0.20230630.0.dist-info/METADATA
+Filename: odoo14_addons_oca_sale_workflow-14.0.20230712.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addons_oca_sale_workflow-14.0.20230630.0.dist-info/WHEEL
+Filename: odoo14_addons_oca_sale_workflow-14.0.20230712.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addons_oca_sale_workflow-14.0.20230630.0.dist-info/top_level.txt
+Filename: odoo14_addons_oca_sale_workflow-14.0.20230712.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addons_oca_sale_workflow-14.0.20230630.0.dist-info/RECORD
+Filename: odoo14_addons_oca_sale_workflow-14.0.20230712.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo14_addons_oca_sale_workflow-14.0.20230630.0.dist-info/METADATA` & `odoo14_addons_oca_sale_workflow-14.0.20230712.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addons-oca-sale-workflow
-Version: 14.0.20230630.0
+Version: 14.0.20230712.1
 Summary: Meta package for oca-sale-workflow Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
@@ -45,14 +45,15 @@
 Requires-Dist: odoo14-addon-sale-invoice-blocking
 Requires-Dist: odoo14-addon-sale-invoice-no-mail
 Requires-Dist: odoo14-addon-sale-invoice-plan
 Requires-Dist: odoo14-addon-sale-invoice-policy
 Requires-Dist: odoo14-addon-sale-isolated-quotation
 Requires-Dist: odoo14-addon-sale-last-price-info
 Requires-Dist: odoo14-addon-sale-mail-autosubscribe
+Requires-Dist: odoo14-addon-sale-manual-delivery
 Requires-Dist: odoo14-addon-sale-mrp-bom
 Requires-Dist: odoo14-addon-sale-order-archive
 Requires-Dist: odoo14-addon-sale-order-carrier-auto-assign
 Requires-Dist: odoo14-addon-sale-order-change-analytic-account
 Requires-Dist: odoo14-addon-sale-order-digitized-signature
 Requires-Dist: odoo14-addon-sale-order-disable-user-autosubscribe
 Requires-Dist: odoo14-addon-sale-order-general-discount
@@ -117,14 +118,15 @@
 Requires-Dist: odoo14-addon-sale-shipping-info-helper
 Requires-Dist: odoo14-addon-sale-start-end-dates
 Requires-Dist: odoo14-addon-sale-stock-delivery-address
 Requires-Dist: odoo14-addon-sale-stock-line-customer-ref
 Requires-Dist: odoo14-addon-sale-stock-picking-blocking
 Requires-Dist: odoo14-addon-sale-stock-picking-note
 Requires-Dist: odoo14-addon-sale-stock-reconcile-valuation-kit
+Requires-Dist: odoo14-addon-sale-substate
 Requires-Dist: odoo14-addon-sale-tier-validation
 Requires-Dist: odoo14-addon-sale-transaction-form-link
 Requires-Dist: odoo14-addon-sale-triple-discount
 Requires-Dist: odoo14-addon-sale-validity
 Requires-Dist: odoo14-addon-sale-wishlist
 Requires-Dist: odoo14-addon-sales-team-security
 Requires-Dist: odoo14-addon-sales-team-security-crm
```

