# Comparing `tmp/cxmlinvbot-1.1.1.tar.gz` & `tmp/cxmlinvbot-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cxmlinvbot-1.1.1.tar", last modified: Mon May 29 15:40:35 2023, max compression
+gzip compressed data, was "cxmlinvbot-1.1.2.tar", last modified: Thu Jul 13 11:29:22 2023, max compression
```

## Comparing `cxmlinvbot-1.1.1.tar` & `cxmlinvbot-1.1.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 15:40:35.209355 cxmlinvbot-1.1.1/
--rw-rw-rw-   0        0        0      166 2023-05-29 15:40:35.208362 cxmlinvbot-1.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-29 15:40:34.586148 cxmlinvbot-1.1.1/cxmlinvbot/
--rw-rw-rw-   0        0        0        0 2023-05-06 08:44:56.000000 cxmlinvbot-1.1.1/cxmlinvbot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:40:34.606093 cxmlinvbot-1.1.1/cxmlinvbot/config/
--rw-rw-rw-   0        0        0        0 2023-04-19 13:14:10.000000 cxmlinvbot-1.1.1/cxmlinvbot/config/__init__.py
--rw-rw-rw-   0        0        0     1641 2023-05-29 13:29:14.000000 cxmlinvbot-1.1.1/cxmlinvbot/config/base.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:40:34.649975 cxmlinvbot-1.1.1/cxmlinvbot/errors/
--rw-rw-rw-   0        0        0        0 2023-05-06 10:19:45.000000 cxmlinvbot-1.1.1/cxmlinvbot/errors/__init__.py
--rw-rw-rw-   0        0        0      445 2023-05-13 12:28:57.000000 cxmlinvbot-1.1.1/cxmlinvbot/errors/errors.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:40:34.744329 cxmlinvbot-1.1.1/cxmlinvbot/filing/
--rw-rw-rw-   0        0        0        0 2023-05-06 10:19:57.000000 cxmlinvbot-1.1.1/cxmlinvbot/filing/__init__.py
--rw-rw-rw-   0        0        0     2349 2023-05-13 13:12:19.000000 cxmlinvbot-1.1.1/cxmlinvbot/filing/filing.py
--rw-rw-rw-   0        0        0      246 2023-05-06 11:05:58.000000 cxmlinvbot-1.1.1/cxmlinvbot/kill.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:40:34.803489 cxmlinvbot-1.1.1/cxmlinvbot/mail/
--rw-rw-rw-   0        0        0        0 2023-05-06 10:20:09.000000 cxmlinvbot-1.1.1/cxmlinvbot/mail/__init__.py
--rw-rw-rw-   0        0        0     3393 2023-05-10 18:39:23.000000 cxmlinvbot-1.1.1/cxmlinvbot/mail/mail.py
--rw-rw-rw-   0        0        0     9291 2023-05-29 15:04:38.000000 cxmlinvbot-1.1.1/cxmlinvbot/main.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:40:34.937710 cxmlinvbot-1.1.1/cxmlinvbot/mapping/
--rw-rw-rw-   0        0        0        0 2023-05-06 10:20:19.000000 cxmlinvbot-1.1.1/cxmlinvbot/mapping/__init__.py
--rw-rw-rw-   0        0        0     2142 2023-05-29 13:24:41.000000 cxmlinvbot-1.1.1/cxmlinvbot/mapping/action.py
--rw-rw-rw-   0        0        0     4712 2023-05-10 12:55:16.000000 cxmlinvbot-1.1.1/cxmlinvbot/mapping/headermapping.py
--rw-rw-rw-   0        0        0    14134 2023-05-29 15:13:38.000000 cxmlinvbot-1.1.1/cxmlinvbot/mapping/invoicedetailrequestmapping.py
--rw-rw-rw-   0        0        0    13884 2023-05-29 15:15:10.000000 cxmlinvbot-1.1.1/cxmlinvbot/mapping/invoicedetailrequestservicemapping.py
--rw-rw-rw-   0        0        0     1046 2023-05-13 12:27:38.000000 cxmlinvbot-1.1.1/cxmlinvbot/mapping/mapping.py
--rw-rw-rw-   0        0        0      464 2023-05-06 09:52:03.000000 cxmlinvbot-1.1.1/cxmlinvbot/mapping/profilerequestmapping.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:40:35.105129 cxmlinvbot-1.1.1/cxmlinvbot/objects/
--rw-rw-rw-   0        0        0        0 2023-04-19 11:11:56.000000 cxmlinvbot-1.1.1/cxmlinvbot/objects/__init__.py
--rw-rw-rw-   0        0        0     5144 2023-05-06 09:08:47.000000 cxmlinvbot-1.1.1/cxmlinvbot/objects/cxmlobject.py
--rw-rw-rw-   0        0        0     1359 2023-05-06 09:05:33.000000 cxmlinvbot-1.1.1/cxmlinvbot/objects/profileresponse.py
--rw-rw-rw-   0        0        0      803 2023-05-06 09:05:41.000000 cxmlinvbot-1.1.1/cxmlinvbot/objects/response.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:40:35.203371 cxmlinvbot-1.1.1/cxmlinvbot/unittests/
--rw-rw-rw-   0        0        0        0 2023-04-19 11:22:52.000000 cxmlinvbot-1.1.1/cxmlinvbot/unittests/__init__.py
--rw-rw-rw-   0        0        0     2231 2023-05-06 13:49:56.000000 cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_action.py
--rw-rw-rw-   0        0        0     2947 2023-05-06 09:06:03.000000 cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_cxmlobject.py
--rw-rw-rw-   0        0        0     1218 2023-05-13 12:30:12.000000 cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_errors.py
--rw-rw-rw-   0        0        0     2950 2023-05-13 13:26:20.000000 cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_filing.py
--rw-rw-rw-   0        0        0    24937 2023-05-29 15:37:28.000000 cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_main.py
--rw-rw-rw-   0        0        0     2183 2023-05-13 12:30:54.000000 cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_mapping.py
--rw-rw-rw-   0        0        0     2164 2023-05-06 09:46:38.000000 cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_profileresponse.py
--rw-rw-rw-   0        0        0     1123 2023-05-06 09:07:06.000000 cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_response.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:40:34.599111 cxmlinvbot-1.1.1/cxmlinvbot.egg-info/
--rw-rw-rw-   0        0        0      166 2023-05-29 15:40:34.000000 cxmlinvbot-1.1.1/cxmlinvbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1207 2023-05-29 15:40:34.000000 cxmlinvbot-1.1.1/cxmlinvbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 15:40:34.000000 cxmlinvbot-1.1.1/cxmlinvbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-29 15:40:34.000000 cxmlinvbot-1.1.1/cxmlinvbot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-29 15:40:34.000000 cxmlinvbot-1.1.1/cxmlinvbot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 15:40:35.210352 cxmlinvbot-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      671 2023-05-13 13:33:59.000000 cxmlinvbot-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:29:22.140000 cxmlinvbot-1.1.2/
+-rw-rw-rw-   0        0        0      166 2023-07-13 11:29:22.120772 cxmlinvbot-1.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-13 11:29:07.190000 cxmlinvbot-1.1.2/cxmlinvbot/
+-rw-rw-rw-   0        0        0        0 2023-05-06 08:44:56.000000 cxmlinvbot-1.1.2/cxmlinvbot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:29:12.970000 cxmlinvbot-1.1.2/cxmlinvbot/config/
+-rw-rw-rw-   0        0        0        0 2023-04-19 13:14:10.000000 cxmlinvbot-1.1.2/cxmlinvbot/config/__init__.py
+-rw-rw-rw-   0        0        0     1641 2023-07-13 11:23:30.000000 cxmlinvbot-1.1.2/cxmlinvbot/config/base.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:29:13.830000 cxmlinvbot-1.1.2/cxmlinvbot/errors/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:19:45.000000 cxmlinvbot-1.1.2/cxmlinvbot/errors/__init__.py
+-rw-rw-rw-   0        0        0      445 2023-05-13 12:28:57.000000 cxmlinvbot-1.1.2/cxmlinvbot/errors/errors.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:29:14.270000 cxmlinvbot-1.1.2/cxmlinvbot/filing/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:19:57.000000 cxmlinvbot-1.1.2/cxmlinvbot/filing/__init__.py
+-rw-rw-rw-   0        0        0     2349 2023-05-13 13:12:19.000000 cxmlinvbot-1.1.2/cxmlinvbot/filing/filing.py
+-rw-rw-rw-   0        0        0      246 2023-05-06 11:05:58.000000 cxmlinvbot-1.1.2/cxmlinvbot/kill.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:29:14.780000 cxmlinvbot-1.1.2/cxmlinvbot/mail/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:20:09.000000 cxmlinvbot-1.1.2/cxmlinvbot/mail/__init__.py
+-rw-rw-rw-   0        0        0     3393 2023-05-10 18:39:23.000000 cxmlinvbot-1.1.2/cxmlinvbot/mail/mail.py
+-rw-rw-rw-   0        0        0     9291 2023-05-29 15:04:38.000000 cxmlinvbot-1.1.2/cxmlinvbot/main.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:29:17.830000 cxmlinvbot-1.1.2/cxmlinvbot/mapping/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:20:19.000000 cxmlinvbot-1.1.2/cxmlinvbot/mapping/__init__.py
+-rw-rw-rw-   0        0        0     2142 2023-05-29 13:24:41.000000 cxmlinvbot-1.1.2/cxmlinvbot/mapping/action.py
+-rw-rw-rw-   0        0        0     4712 2023-05-10 12:55:16.000000 cxmlinvbot-1.1.2/cxmlinvbot/mapping/headermapping.py
+-rw-rw-rw-   0        0        0    14134 2023-06-30 13:25:39.000000 cxmlinvbot-1.1.2/cxmlinvbot/mapping/invoicedetailrequestmapping.py
+-rw-rw-rw-   0        0        0    13884 2023-06-30 13:25:50.000000 cxmlinvbot-1.1.2/cxmlinvbot/mapping/invoicedetailrequestservicemapping.py
+-rw-rw-rw-   0        0        0     1046 2023-05-13 12:27:38.000000 cxmlinvbot-1.1.2/cxmlinvbot/mapping/mapping.py
+-rw-rw-rw-   0        0        0      464 2023-05-06 09:52:03.000000 cxmlinvbot-1.1.2/cxmlinvbot/mapping/profilerequestmapping.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:29:18.890000 cxmlinvbot-1.1.2/cxmlinvbot/objects/
+-rw-rw-rw-   0        0        0        0 2023-04-19 11:11:56.000000 cxmlinvbot-1.1.2/cxmlinvbot/objects/__init__.py
+-rw-rw-rw-   0        0        0     5144 2023-05-06 09:08:47.000000 cxmlinvbot-1.1.2/cxmlinvbot/objects/cxmlobject.py
+-rw-rw-rw-   0        0        0     1359 2023-05-06 09:05:33.000000 cxmlinvbot-1.1.2/cxmlinvbot/objects/profileresponse.py
+-rw-rw-rw-   0        0        0      803 2023-05-06 09:05:41.000000 cxmlinvbot-1.1.2/cxmlinvbot/objects/response.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:29:21.000000 cxmlinvbot-1.1.2/cxmlinvbot/unittests/
+-rw-rw-rw-   0        0        0        0 2023-04-19 11:22:52.000000 cxmlinvbot-1.1.2/cxmlinvbot/unittests/__init__.py
+-rw-rw-rw-   0        0        0     2231 2023-05-06 13:49:56.000000 cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_action.py
+-rw-rw-rw-   0        0        0     2947 2023-05-06 09:06:03.000000 cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_cxmlobject.py
+-rw-rw-rw-   0        0        0     1218 2023-05-13 12:30:12.000000 cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_errors.py
+-rw-rw-rw-   0        0        0     2950 2023-05-13 13:26:20.000000 cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_filing.py
+-rw-rw-rw-   0        0        0    24937 2023-05-29 15:37:28.000000 cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_main.py
+-rw-rw-rw-   0        0        0     2183 2023-05-13 12:30:54.000000 cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_mapping.py
+-rw-rw-rw-   0        0        0     2164 2023-05-06 09:46:38.000000 cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_profileresponse.py
+-rw-rw-rw-   0        0        0     1123 2023-05-06 09:07:06.000000 cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_response.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:29:11.780000 cxmlinvbot-1.1.2/cxmlinvbot.egg-info/
+-rw-rw-rw-   0        0        0      166 2023-07-13 11:29:02.000000 cxmlinvbot-1.1.2/cxmlinvbot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1207 2023-07-13 11:29:03.000000 cxmlinvbot-1.1.2/cxmlinvbot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 11:29:02.000000 cxmlinvbot-1.1.2/cxmlinvbot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-13 11:29:02.000000 cxmlinvbot-1.1.2/cxmlinvbot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-13 11:29:02.000000 cxmlinvbot-1.1.2/cxmlinvbot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 11:29:22.191465 cxmlinvbot-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      671 2023-05-13 13:33:59.000000 cxmlinvbot-1.1.2/setup.py
```

### Comparing `cxmlinvbot-1.1.1/cxmlinvbot/config/base.py` & `cxmlinvbot-1.1.2/cxmlinvbot/config/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     PROD_COUPA_END_POINT    = 'https://cbre.coupahost.com/cxml/'
     TEST_COUPA_END_POINT    = 'https://cbre-test.coupahost.com/cxml/'
     PROD_INVOICE_END_POINT  = '%sinvoices/' % PROD_COUPA_END_POINT
     TEST_INVOICE_END_POINT  = '%sinvoices/' % TEST_COUPA_END_POINT
 
     # Miscellania...
     MAIL_PREAMBLE           = 'Pro Door Invoice Bot - '
-    VERSION                 = '1.1.1'
+    VERSION                 = '1.1.2'
 
     # Testing widgets...
     SAMPLE_PATH             = '%sResources\\cXML\\1.2.057\\Samples\\' % EnvConfig.PROJECT_ROOT
     XML_SAMPLES             = {
         'ProfileResponse'           : '%sprofileresponse.xml' % SAMPLE_PATH,
         'ProfileResponseNoDTD'      : '%sprofileresponsenodtd.xml' % SAMPLE_PATH,
         'ProfileResponseInvalidXML' : '%sprofileresponseinvalidxml.xml' % SAMPLE_PATH,
```

### Comparing `cxmlinvbot-1.1.1/cxmlinvbot/filing/filing.py` & `cxmlinvbot-1.1.2/cxmlinvbot/filing/filing.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.1/cxmlinvbot/mail/mail.py` & `cxmlinvbot-1.1.2/cxmlinvbot/mail/mail.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.1/cxmlinvbot/main.py` & `cxmlinvbot-1.1.2/cxmlinvbot/main.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.1/cxmlinvbot/mapping/action.py` & `cxmlinvbot-1.1.2/cxmlinvbot/mapping/action.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.1/cxmlinvbot/mapping/headermapping.py` & `cxmlinvbot-1.1.2/cxmlinvbot/mapping/headermapping.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.1/cxmlinvbot/mapping/invoicedetailrequestmapping.py` & `cxmlinvbot-1.1.2/cxmlinvbot/mapping/invoicedetailrequestmapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     #'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Extrinsic',
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/GrossAmount/Money',
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/NetAmount/Money',
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/DueAmount/Money',
   ]
 
   FIELD_TO_ACTION_MAPS = HeaderMapping.FIELD_TO_ACTION_MAPS + [dict(
-    BillToAddressID=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact@addressID', '357106'),
+    BillToAddressID=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact@addressID', '437805'),
     ContactName=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/Name', 'CBRE MANAGED SERVICES LIMITED'),
     POAddressLine1=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/Street', '61 SOUTHWARK STREET'),
     POCity=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/City', 'London'),
     POPostalCode=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/PostalCode', 'SE1 0HL'),
     POCountry=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/Country@isoCountryCode', 'GB'),
     # This first set of fields come directly from the CSV and in the same order
     #SAVATRegNO=cxmlinvbot.mapping.action.Default(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/Extrinsic',
```

### Comparing `cxmlinvbot-1.1.1/cxmlinvbot/mapping/invoicedetailrequestservicemapping.py` & `cxmlinvbot-1.1.2/cxmlinvbot/mapping/invoicedetailrequestservicemapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail/TaxAmount/Money',
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/GrossAmount/Money',
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/NetAmount/Money',
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/DueAmount/Money',
   ]
 
   FIELD_TO_ACTION_MAPS = HeaderMapping.FIELD_TO_ACTION_MAPS + [dict(
-    BillToAddressID=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact@addressID', '357106'),
+    BillToAddressID=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact@addressID', '437805'),
     ContactName=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/Name', 'CBRE MANAGED SERVICES LIMITED'),
     POAddressLine1=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/Street', '61 SOUTHWARK STREET'),
     POCity=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/City', 'London'),
     POPostalCode=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/PostalCode', 'SE1 0HL'),
     POCountry=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/Country@isoCountryCode', 'GB'),
     # This first set of fields come directly from the CSV and in the same order
     #SAVATRegNO=cxmlinvbot.mapping.action.Default(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/Extrinsic',
```

### Comparing `cxmlinvbot-1.1.1/cxmlinvbot/mapping/mapping.py` & `cxmlinvbot-1.1.2/cxmlinvbot/mapping/mapping.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.1/cxmlinvbot/objects/cxmlobject.py` & `cxmlinvbot-1.1.2/cxmlinvbot/objects/cxmlobject.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.1/cxmlinvbot/objects/profileresponse.py` & `cxmlinvbot-1.1.2/cxmlinvbot/objects/profileresponse.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.1/cxmlinvbot/objects/response.py` & `cxmlinvbot-1.1.2/cxmlinvbot/objects/response.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_action.py` & `cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_action.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_cxmlobject.py` & `cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_cxmlobject.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_errors.py` & `cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_errors.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_filing.py` & `cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_filing.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_main.py` & `cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_main.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_mapping.py` & `cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_profileresponse.py` & `cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_profileresponse.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.1/cxmlinvbot/unittests/test_response.py` & `cxmlinvbot-1.1.2/cxmlinvbot/unittests/test_response.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.1/cxmlinvbot.egg-info/SOURCES.txt` & `cxmlinvbot-1.1.2/cxmlinvbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.1.1/setup.py` & `cxmlinvbot-1.1.2/setup.py`

 * *Files identical despite different names*

