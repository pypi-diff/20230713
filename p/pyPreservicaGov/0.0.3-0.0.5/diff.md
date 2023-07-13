# Comparing `tmp/pyPreservicaGov-0.0.3-py3-none-any.whl.zip` & `tmp/pyPreservicaGov-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 27721 bytes, number of entries: 25
--rw-rw-rw-  2.0 fat      341 b- defN 23-Jul-13 09:33 pyPreservicaGov/__init__.py
+Zip file size: 27800 bytes, number of entries: 25
+-rw-rw-rw-  2.0 fat      341 b- defN 23-Jul-13 14:39 pyPreservicaGov/__init__.py
 -rw-rw-rw-  2.0 fat      441 b- defN 23-Jul-13 11:04 pyPreservicaGov/__main__.py
 -rw-rw-rw-  2.0 fat    16453 b- defN 23-Jul-13 11:08 pyPreservicaGov/main.py
 -rw-rw-rw-  2.0 fat      133 b- defN 23-Jul-12 16:29 pyPreservicaGov/run.py
 -rw-rw-rw-  2.0 fat     6412 b- defN 23-Jul-13 11:00 pyPreservicaGov/schema.py
 -rw-rw-rw-  2.0 fat     4694 b- defN 23-Jul-12 13:53 pyPreservicaGov/images/committee.png
 -rw-rw-rw-  2.0 fat     2654 b- defN 23-Jul-12 13:53 pyPreservicaGov/images/meeting.png
 -rw-rw-rw-  2.0 fat     1151 b- defN 22-Jan-21 10:29 pyPreservicaGov/schema/mg-attachment-CMIS.xml
@@ -15,13 +15,13 @@
 -rw-rw-rw-  2.0 fat     1079 b- defN 22-Jan-21 09:42 pyPreservicaGov/schema/mg-committee-CMIS.xsl
 -rw-rw-rw-  2.0 fat      592 b- defN 22-Jan-21 09:39 pyPreservicaGov/schema/mg-committee-Index.xml
 -rw-rw-rw-  2.0 fat      287 b- defN 22-Jan-21 09:31 pyPreservicaGov/schema/mg-committee-schema.xsd
 -rw-rw-rw-  2.0 fat     1097 b- defN 22-Jan-21 10:05 pyPreservicaGov/schema/mg-meeting-CMIS.xml
 -rw-rw-rw-  2.0 fat     1097 b- defN 22-Jan-21 10:05 pyPreservicaGov/schema/mg-meeting-CMIS.xsl
 -rw-rw-rw-  2.0 fat     1457 b- defN 22-Jan-21 09:49 pyPreservicaGov/schema/mg-meeting-Index.xml
 -rw-rw-rw-  2.0 fat      279 b- defN 22-Jan-14 14:27 pyPreservicaGov/schema/mg-meeting-schema.xsd
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jul-13 14:35 pyPreservicaGov-0.0.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3015 b- defN 23-Jul-13 14:35 pyPreservicaGov-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-13 14:35 pyPreservicaGov-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 23-Jul-13 14:35 pyPreservicaGov-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2331 b- defN 23-Jul-13 14:35 pyPreservicaGov-0.0.3.dist-info/RECORD
-25 files, 59843 bytes uncompressed, 23859 bytes compressed:  60.1%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jul-13 14:39 pyPreservicaGov-0.0.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3316 b- defN 23-Jul-13 14:39 pyPreservicaGov-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-13 14:39 pyPreservicaGov-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Jul-13 14:39 pyPreservicaGov-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2331 b- defN 23-Jul-13 14:39 pyPreservicaGov-0.0.5.dist-info/RECORD
+25 files, 60144 bytes uncompressed, 23938 bytes compressed:  60.2%
```

## zipnote {}

```diff
@@ -54,23 +54,23 @@
 
 Filename: pyPreservicaGov/schema/mg-meeting-Index.xml
 Comment: 
 
 Filename: pyPreservicaGov/schema/mg-meeting-schema.xsd
 Comment: 
 
-Filename: pyPreservicaGov-0.0.3.dist-info/LICENSE
+Filename: pyPreservicaGov-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: pyPreservicaGov-0.0.3.dist-info/METADATA
+Filename: pyPreservicaGov-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: pyPreservicaGov-0.0.3.dist-info/WHEEL
+Filename: pyPreservicaGov-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: pyPreservicaGov-0.0.3.dist-info/top_level.txt
+Filename: pyPreservicaGov-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: pyPreservicaGov-0.0.3.dist-info/RECORD
+Filename: pyPreservicaGov-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyPreservicaGov/__init__.py

```diff
@@ -8,12 +8,12 @@
 
 from .main import PreservicaGov
 from .schema import Schema
 
 __author__ = "James Carr (drjamescarr@gmail.com)"
 
 # Version of the pyPreservica.Gov package
-__version__ = "0.0.3"
+__version__ = "0.0.5"
 
 __license__ = "Apache License Version 2.0"
```

## Comparing `pyPreservicaGov-0.0.3.dist-info/LICENSE` & `pyPreservicaGov-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyPreservicaGov-0.0.3.dist-info/METADATA` & `pyPreservicaGov-0.0.5.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPreservicaGov
-Version: 0.0.3
+Version: 0.0.5
 Summary: Python Library For Harvesting Modern.Gov Records into Preservica for Long Term Preservation
 Home-page: https://pyPreservicaGov.readthedocs.io/
 Author: James Carr
 Author-email: drjamescarr@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://pyPreservicaGov.readthedocs.io
 Project-URL: Source, https://github.com/carj/pyPreservica.Gov
@@ -47,28 +47,36 @@
 
 The second section contains the security tag which should be assigned to the records as they are ingested. For example 
 records which can be published immediately on the Preservica access portal should be set to "public".
 
 The site_name parameter should point to the URL of the Modern.Gov system you would like to harvest.
 
 parent.folder should be the UUID of the Preservica collection the Committee folders will be ingested into. 
+
+The committee.FromDate and committee.ToDate parameters specify the date range of meetings which will be harvested.
     
     [credentials]
     username=test@test.com
     password=1234567
     server=uk.preservica.com
     
     [Modern.Gov]
     security.tag=open
     site_name=https://democracy.local_authority.gov.uk/
     parent.folder=372d2881-7cce-4c2e-99f7-386c3cf4a922
     committee.FromDate=01/01/1980
     committee.ToDate=01/01/2024
 
 
+Once the credentials.properties has been updated you can run pyPreservica.Gov again directly from the command line
+to start the harvest process.
+
+        $ python -m  pyPreservicaGov
+
+
 ## License
 
 The package is available as open source under the terms of the Apache License 2.0
 
 
 ## Installation
```

## Comparing `pyPreservicaGov-0.0.3.dist-info/RECORD` & `pyPreservicaGov-0.0.5.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-pyPreservicaGov/__init__.py,sha256=dPYCFp4KakZmHpjalLQX2IHbZvX6w26AZeaEYuwN6GA,341
+pyPreservicaGov/__init__.py,sha256=m0nrywCUfxV3AmIequgDkAdJiOKrx1ha7kEOHcZ2y_U,341
 pyPreservicaGov/__main__.py,sha256=gaCYC_PJ5XjrO9vDE949gtdug44WpVMTARzPGOrAM5k,441
 pyPreservicaGov/main.py,sha256=ry5oQFT2OOtTAOeYUPPOKEuiux6ZGNebFxsac41Y22E,16453
 pyPreservicaGov/run.py,sha256=QCj7bwtZpd5Ih9se61h0FZ_fWGtlZ02pLySHdVRiDcE,133
 pyPreservicaGov/schema.py,sha256=agdXO5oieGdw63PUqQpmoSo2ZPphRY8YjZlDScnPCJ4,6412
 pyPreservicaGov/images/committee.png,sha256=2DXy2GT2QSAEup3vTabiidIW1tHVHQh9ZbQNhV7qadc,4694
 pyPreservicaGov/images/meeting.png,sha256=kTkm_3JUOG3C_ONjeRIEWOptgdcPp24W5o-Nn4MBdHs,2654
 pyPreservicaGov/schema/mg-attachment-CMIS.xml,sha256=e-Ed28zyezS_AuC1ymi99ov3PvG-pKj7AaP3PkfNpk4,1151
@@ -14,12 +14,12 @@
 pyPreservicaGov/schema/mg-committee-CMIS.xsl,sha256=hTR7WG_FVe3fgWNz7ME_A177ZRUizCtGYEJ7ZiMHxvQ,1079
 pyPreservicaGov/schema/mg-committee-Index.xml,sha256=QmYhwFP9VI1x4pEIuQ4TOCTaPoJFBNMnGvPNtfo_iJw,592
 pyPreservicaGov/schema/mg-committee-schema.xsd,sha256=imprsweRqJtGZ4cWEZ2dkjwuLs8bBxG6bYn4dGzyrGg,287
 pyPreservicaGov/schema/mg-meeting-CMIS.xml,sha256=qxfHS1NqFcPJukOhjl4fUPYMdyAJpJg11VWzGhThD4A,1097
 pyPreservicaGov/schema/mg-meeting-CMIS.xsl,sha256=qxfHS1NqFcPJukOhjl4fUPYMdyAJpJg11VWzGhThD4A,1097
 pyPreservicaGov/schema/mg-meeting-Index.xml,sha256=8vr3AaVK8cvzxQxut8mLC82lOrzjWNkL13EPxluKz4c,1457
 pyPreservicaGov/schema/mg-meeting-schema.xsd,sha256=TYhELIbdE8Dpy2NbMEKd3E9K8wZR_HFOqkkP8jHrzDE,279
-pyPreservicaGov-0.0.3.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-pyPreservicaGov-0.0.3.dist-info/METADATA,sha256=4M31zqJ7_jmUQsz8cbbEF0UWRQHkLq4VhxdgGZpRYoc,3015
-pyPreservicaGov-0.0.3.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-pyPreservicaGov-0.0.3.dist-info/top_level.txt,sha256=GQzyUbcXfdtq_JEpso-xSlWZfeImZE_ZYpZam1ZlDpc,16
-pyPreservicaGov-0.0.3.dist-info/RECORD,,
+pyPreservicaGov-0.0.5.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+pyPreservicaGov-0.0.5.dist-info/METADATA,sha256=u8ukKZzaSDKx6V3TN56YbS0KGZUzd44WcR7jl9u8xe8,3316
+pyPreservicaGov-0.0.5.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+pyPreservicaGov-0.0.5.dist-info/top_level.txt,sha256=GQzyUbcXfdtq_JEpso-xSlWZfeImZE_ZYpZam1ZlDpc,16
+pyPreservicaGov-0.0.5.dist-info/RECORD,,
```

