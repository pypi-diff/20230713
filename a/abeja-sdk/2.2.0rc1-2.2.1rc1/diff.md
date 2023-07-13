# Comparing `tmp/abeja_sdk-2.2.0rc1-py3-none-any.whl.zip` & `tmp/abeja_sdk-2.2.1rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 97799 bytes, number of entries: 93
+Zip file size: 97792 bytes, number of entries: 93
 -rw-r--r--  2.0 unx      200 b- defN 80-Jan-01 00:00 abeja/__init__.py
 -rw-r--r--  2.0 unx      263 b- defN 80-Jan-01 00:00 abeja/base_client.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 abeja/common/__init__.py
 -rw-r--r--  2.0 unx      406 b- defN 80-Jan-01 00:00 abeja/common/api_client.py
 -rw-r--r--  2.0 unx     2063 b- defN 80-Jan-01 00:00 abeja/common/auth.py
 -rw-r--r--  2.0 unx      714 b- defN 80-Jan-01 00:00 abeja/common/config.py
 -rw-r--r--  2.0 unx     8053 b- defN 80-Jan-01 00:00 abeja/common/connection.py
@@ -22,15 +22,15 @@
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 abeja/contrib/keras/__init__.py
 -rw-r--r--  2.0 unx      983 b- defN 80-Jan-01 00:00 abeja/contrib/keras/callbacks.py
 -rw-r--r--  2.0 unx      104 b- defN 80-Jan-01 00:00 abeja/datalake/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 abeja/datalake/api/__init__.py
 -rw-r--r--  2.0 unx    56688 b- defN 80-Jan-01 00:00 abeja/datalake/api/client.py
 -rw-r--r--  2.0 unx    18670 b- defN 80-Jan-01 00:00 abeja/datalake/channel.py
 -rw-r--r--  2.0 unx     1619 b- defN 80-Jan-01 00:00 abeja/datalake/client.py
--rw-r--r--  2.0 unx    20511 b- defN 80-Jan-01 00:00 abeja/datalake/file.py
+-rw-r--r--  2.0 unx    20592 b- defN 80-Jan-01 00:00 abeja/datalake/file.py
 -rw-r--r--  2.0 unx     1508 b- defN 80-Jan-01 00:00 abeja/datalake/metadata.py
 -rw-r--r--  2.0 unx       93 b- defN 80-Jan-01 00:00 abeja/datalake/storage_type.py
 -rw-r--r--  2.0 unx      104 b- defN 80-Jan-01 00:00 abeja/datasets/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 abeja/datasets/api/__init__.py
 -rw-r--r--  2.0 unx    37307 b- defN 80-Jan-01 00:00 abeja/datasets/api/client.py
 -rw-r--r--  2.0 unx      211 b- defN 80-Jan-01 00:00 abeja/datasets/base.py
 -rw-r--r--  2.0 unx     1557 b- defN 80-Jan-01 00:00 abeja/datasets/client.py
@@ -84,12 +84,12 @@
 -rw-r--r--  2.0 unx     2981 b- defN 80-Jan-01 00:00 abeja/training/statistics.py
 -rw-r--r--  2.0 unx       63 b- defN 80-Jan-01 00:00 abeja/triggers/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 abeja/triggers/api/__init__.py
 -rw-r--r--  2.0 unx    14857 b- defN 80-Jan-01 00:00 abeja/triggers/api/client.py
 -rw-r--r--  2.0 unx       51 b- defN 80-Jan-01 00:00 abeja/user/__init__.py
 -rw-r--r--  2.0 unx     1601 b- defN 80-Jan-01 00:00 abeja/user/user.py
 -rw-r--r--  2.0 unx      155 b- defN 80-Jan-01 00:00 abeja/version.py
--rw-r--r--  2.0 unx    11344 b- defN 80-Jan-01 00:00 abeja_sdk-2.2.0rc1.dist-info/LICENSE
-?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 abeja_sdk-2.2.0rc1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1479 b- defN 16-Jan-01 00:00 abeja_sdk-2.2.0rc1.dist-info/METADATA
-?rw-r--r--  2.0 unx     7635 b- defN 16-Jan-01 00:00 abeja_sdk-2.2.0rc1.dist-info/RECORD
-93 files, 485397 bytes uncompressed, 85761 bytes compressed:  82.3%
+-rw-r--r--  2.0 unx    11344 b- defN 80-Jan-01 00:00 abeja_sdk-2.2.1rc1.dist-info/LICENSE
+?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 abeja_sdk-2.2.1rc1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1434 b- defN 16-Jan-01 00:00 abeja_sdk-2.2.1rc1.dist-info/METADATA
+?rw-r--r--  2.0 unx     7635 b- defN 16-Jan-01 00:00 abeja_sdk-2.2.1rc1.dist-info/RECORD
+93 files, 485433 bytes uncompressed, 85754 bytes compressed:  82.3%
```

## zipnote {}

```diff
@@ -261,20 +261,20 @@
 
 Filename: abeja/user/user.py
 Comment: 
 
 Filename: abeja/version.py
 Comment: 
 
-Filename: abeja_sdk-2.2.0rc1.dist-info/LICENSE
+Filename: abeja_sdk-2.2.1rc1.dist-info/LICENSE
 Comment: 
 
-Filename: abeja_sdk-2.2.0rc1.dist-info/WHEEL
+Filename: abeja_sdk-2.2.1rc1.dist-info/WHEEL
 Comment: 
 
-Filename: abeja_sdk-2.2.0rc1.dist-info/METADATA
+Filename: abeja_sdk-2.2.1rc1.dist-info/METADATA
 Comment: 
 
-Filename: abeja_sdk-2.2.0rc1.dist-info/RECORD
+Filename: abeja_sdk-2.2.1rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## abeja/datalake/file.py

```diff
@@ -510,14 +510,16 @@
             # and delegate it validation in list api.
             if self.start:
                 params['start'] = self.start
             if self.end:
                 params['end'] = self.end
             if self.sort:
                 params['sort'] = self.sort
+            if self.timezone:
+                params['timezone'] = self.timezone
 
         res = self._api.list_channel_files(self.channel_id, **params)
 
         self.next_page_token = res.get('next_page_token')
         self._is_first_page = False
 
         return [self._create_datalake_file(item) for item in res['files']]
```

## abeja/version.py

```diff
@@ -1,3 +1,3 @@
 # The VERSION value is rewritten by CI to the correct value at the time of deployment.
 # see: ${REPOSITORY_ROOT}/.circleci/config.yml
-VERSION = "2.2.0rc1"
+VERSION = "2.2.1rc1"
```

## Comparing `abeja_sdk-2.2.0rc1.dist-info/LICENSE` & `abeja_sdk-2.2.1rc1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `abeja_sdk-2.2.0rc1.dist-info/METADATA` & `abeja_sdk-2.2.1rc1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abeja-sdk
-Version: 2.2.0rc1
+Version: 2.2.1rc1
 Summary: ABEJA Platform Software Development Kit
 License: Apache-2.0
 Author: ABEJA Inc.
 Author-email: platform-support@abejainc.com
 Requires-Python: >=3.7,<3.12
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -27,9 +27,8 @@
 Requires-Dist: guzzle_sphinx_theme (==0.7.11); extra == "docs"
 Requires-Dist: importlib-metadata (>=2.0.0,<3.0.0); extra == "docs"
 Requires-Dist: protobuf (<4)
 Requires-Dist: requests (>=2.27.1)
 Requires-Dist: retrying (==1.3.4)
 Requires-Dist: tensorboardx (==2.5.1)
 Requires-Dist: tomlkit (==0.7.0)
-Requires-Dist: typing-extensions (==3.7.4.3)
 Requires-Dist: virtualenv (==20.0.34); extra == "docs"
```

## Comparing `abeja_sdk-2.2.0rc1.dist-info/RECORD` & `abeja_sdk-2.2.1rc1.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 abeja/contrib/keras/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 abeja/contrib/keras/callbacks.py,sha256=Y_IicimhgJiG_hCFdked85hIiMJhOetV1XxdikgvLhE,983
 abeja/datalake/__init__.py,sha256=YSFlQZsEmUR1JbxFaUqRV7sZYuDhWe4JRdqGe4SJOes,104
 abeja/datalake/api/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 abeja/datalake/api/client.py,sha256=EDdUsTKpa7WcfqCkBsz0OKcaSvphlDReej9tBQ1FRCk,56688
 abeja/datalake/channel.py,sha256=BGVVm_GZJuv_d1c5RYQW85F61yOUBlJ-Fp489mjPMC8,18670
 abeja/datalake/client.py,sha256=-DHuTAiNbGgovH_QriWySPVG0dnemH13UdE4XUnu_HY,1619
-abeja/datalake/file.py,sha256=0zfqTHtxasT3Axi_vh8SGrT5zST-vmfepxwOmwifm6o,20511
+abeja/datalake/file.py,sha256=NXaZUJow2b6afv3uHSTQ-Hjp3KOA_q56OMx_pO8giRc,20592
 abeja/datalake/metadata.py,sha256=3XhkqK-gkftzh_z-rhQPWjO2knM_aSYA6dE-dAcR3P8,1508
 abeja/datalake/storage_type.py,sha256=zIBvqso8VroMHnhMWLbObitKdiQXqdVTbX2GByB0uSc,93
 abeja/datasets/__init__.py,sha256=Q7knz1k-y15RE4TKttLFfovcQCP8Q7I1SnvIXEexpK0,104
 abeja/datasets/api/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 abeja/datasets/api/client.py,sha256=MIVhsWEPG9gJP9ge1Lg80JXNDnxHG3ZqiKDpqqBGB-M,37307
 abeja/datasets/base.py,sha256=vhl2l92wcfPRK_o7X840oAf9c2a195MCmuJNZhXLKZk,211
 abeja/datasets/client.py,sha256=Yq3RyGMWanu8MQBsd5HOrdYTZlc6jt-iDmS6DPxNrD8,1557
@@ -82,12 +82,12 @@
 abeja/training/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 abeja/training/statistics.py,sha256=srEprLDKZSSTmgI3g7rBbDxQzFkDg8FN5OTFH1muwfU,2981
 abeja/triggers/__init__.py,sha256=1juY5YZuLTVcG2h614iwS16NiO-7xuEl62tEe-Hf56A,63
 abeja/triggers/api/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 abeja/triggers/api/client.py,sha256=ftNmiw7fxu43ChUCeNlieKUc3NNIUUccXI6AlDFDIX0,14857
 abeja/user/__init__.py,sha256=js-XQZRHXsGJZ-r9H-cLGQKa_YXmjjPmklnVe9Y12D8,51
 abeja/user/user.py,sha256=KAILiaZ1QaS2gMzFl2Vb1sBdhjKKctv8PYA6jDc1Two,1601
-abeja/version.py,sha256=2iD4ejsvq61jJAuNrS-cqqRh9st9A3iUDOt5MQmoU-I,155
-abeja_sdk-2.2.0rc1.dist-info/LICENSE,sha256=LasG9nAf8e8HZVQSsSkIKAm0s_kjYPGuk968yRClNSw,11344
-abeja_sdk-2.2.0rc1.dist-info/WHEEL,sha256=vxFmldFsRN_Hx10GDvsdv1wroKq8r5Lzvjp6GZ4OO8c,88
-abeja_sdk-2.2.0rc1.dist-info/METADATA,sha256=gAyqNS4OdO79ED-Z9LWiANcN5y0VuyLO24X1fkO1iX8,1479
-abeja_sdk-2.2.0rc1.dist-info/RECORD,,
+abeja/version.py,sha256=xfnGUXB-jD1ysWId5dygDFb3Y1dFSo4HbzQaWOV00VQ,155
+abeja_sdk-2.2.1rc1.dist-info/LICENSE,sha256=LasG9nAf8e8HZVQSsSkIKAm0s_kjYPGuk968yRClNSw,11344
+abeja_sdk-2.2.1rc1.dist-info/WHEEL,sha256=vxFmldFsRN_Hx10GDvsdv1wroKq8r5Lzvjp6GZ4OO8c,88
+abeja_sdk-2.2.1rc1.dist-info/METADATA,sha256=v0dt2rEu8k6dgCUsqb9yQFMMBYEpz15HAQpKT9qKej4,1434
+abeja_sdk-2.2.1rc1.dist-info/RECORD,,
```

