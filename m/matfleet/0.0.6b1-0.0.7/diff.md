# Comparing `tmp/matfleet-0.0.6b1-py3-none-any.whl.zip` & `tmp/matfleet-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 77429 bytes, number of entries: 59
+Zip file size: 77407 bytes, number of entries: 59
 -rw-r--r--  2.0 unx      345 b- defN 23-Apr-26 13:17 matfleet/__init__.py
 -rw-r--r--  2.0 unx      356 b- defN 23-Apr-26 00:46 matfleet/constant.py
 -rw-r--r--  2.0 unx     1399 b- defN 23-Apr-26 00:46 matfleet/get_doc.py
 -rw-r--r--  2.0 unx      322 b- defN 23-Apr-26 00:46 matfleet/core/__init__.py
 -rw-r--r--  2.0 unx      313 b- defN 23-Apr-26 00:46 matfleet/core/general_plot/__init__.py
 -rw-r--r--  2.0 unx     2041 b- defN 23-Apr-26 00:46 matfleet/core/general_plot/alkuser_hist.py
 -rw-r--r--  2.0 unx     2224 b- defN 23-Apr-26 00:46 matfleet/core/general_plot/data_smooth.py
@@ -49,13 +49,13 @@
 -rw-r--r--  2.0 unx     8252 b- defN 23-Apr-26 00:46 matfleet/vasp/xdatcar.py
 -rw-r--r--  2.0 unx     3384 b- defN 23-Apr-26 00:46 matfleet/vasp/xsf.py
 -rw-r--r--  2.0 unx      330 b- defN 23-Apr-26 00:46 matfleet/vasp/unit_test/__init__.py
 -rw-r--r--  2.0 unx     2051 b- defN 23-Apr-26 00:46 matfleet/vasp/unit_test/test_plt.py
 -rw-r--r--  2.0 unx     1790 b- defN 23-Apr-26 00:46 matfleet/vasp/unit_test/test_poscar.py
 -rw-r--r--  2.0 unx     2207 b- defN 23-Apr-26 00:46 matfleet/vasp/unit_test/test_xdatcar.py
 -rw-r--r--  2.0 unx      924 b- defN 23-Apr-26 00:46 matfleet/vasp/unit_test/test_xsf.py
--rw-r--r--  2.0 unx     1433 b- defN 23-Jul-13 09:20 matfleet-0.0.6b1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-13 09:20 matfleet-0.0.6b1.dist-info/WHEEL
--rwxrwxrwx  2.0 unx       74 b- defN 23-Jul-13 09:20 matfleet-0.0.6b1.dist-info/entry_points.txt
--rwxrwxrwx  2.0 unx        9 b- defN 23-Jul-13 09:20 matfleet-0.0.6b1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5111 b- defN 23-Jul-13 09:20 matfleet-0.0.6b1.dist-info/RECORD
-59 files, 194396 bytes uncompressed, 69273 bytes compressed:  64.4%
+-rw-r--r--  2.0 unx     1431 b- defN 23-Jul-13 09:17 matfleet-0.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-13 09:17 matfleet-0.0.7.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx       74 b- defN 23-Jul-13 09:17 matfleet-0.0.7.dist-info/entry_points.txt
+-rwxrwxrwx  2.0 unx        9 b- defN 23-Jul-13 09:17 matfleet-0.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     5101 b- defN 23-Jul-13 09:17 matfleet-0.0.7.dist-info/RECORD
+59 files, 194384 bytes uncompressed, 69271 bytes compressed:  64.4%
```

## zipnote {}

```diff
@@ -156,23 +156,23 @@
 
 Filename: matfleet/vasp/unit_test/test_xdatcar.py
 Comment: 
 
 Filename: matfleet/vasp/unit_test/test_xsf.py
 Comment: 
 
-Filename: matfleet-0.0.6b1.dist-info/METADATA
+Filename: matfleet-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: matfleet-0.0.6b1.dist-info/WHEEL
+Filename: matfleet-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: matfleet-0.0.6b1.dist-info/entry_points.txt
+Filename: matfleet-0.0.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: matfleet-0.0.6b1.dist-info/top_level.txt
+Filename: matfleet-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: matfleet-0.0.6b1.dist-info/RECORD
+Filename: matfleet-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `matfleet-0.0.6b1.dist-info/METADATA` & `matfleet-0.0.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matfleet
-Version: 0.0.6b1
+Version: 0.0.7
 Summary: test
 Home-page: https://gitee.com/alkemiems/matfleet
 Author: Guanjie Wang
 Author-email: gjwang@buaa.edu.cn
 License: MIT
 Description-Content-Type: text/markdown
```

## Comparing `matfleet-0.0.6b1.dist-info/RECORD` & `matfleet-0.0.7.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -48,12 +48,12 @@
 matfleet/vasp/xdatcar.py,sha256=lq5vWyF7ZfczsEIlW7Dl5Dk-tXUQYp48jSIRqq1lJ3c,8252
 matfleet/vasp/xsf.py,sha256=l9BGAlJm5yLuAYnNX79rV3bPIDRDJzOz6P1hbjMHn0E,3384
 matfleet/vasp/unit_test/__init__.py,sha256=AyETtTR_DsZjiOeyTvG_8WmyLDJiw3J-4OCYT-VSYNA,330
 matfleet/vasp/unit_test/test_plt.py,sha256=jBdilDX6aZzkGPS0ILgXChdBAg7J6_MTaSOnfDwbmL0,2051
 matfleet/vasp/unit_test/test_poscar.py,sha256=ahHMiN_6PK1oxQ0ZiAMzULnzWj7JytzFwmeIk3GCydg,1790
 matfleet/vasp/unit_test/test_xdatcar.py,sha256=5YYzQuJey9yZX5l3MBSR9fjJwgdsWw4Bl3WP7DbMTew,2207
 matfleet/vasp/unit_test/test_xsf.py,sha256=SnMo5-If_ZtHpuYr1mCdNQ_YqlcPAI_pJVJhGseCHIg,924
-matfleet-0.0.6b1.dist-info/METADATA,sha256=mCgyAR0Ke96UbkInwF1R_fzddinvV3n3sDW7SnGfkbE,1433
-matfleet-0.0.6b1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-matfleet-0.0.6b1.dist-info/entry_points.txt,sha256=k8e-ij5k7oxLCDanRBh7RVpbDm_l5EN8_lr2Y0zQHt0,74
-matfleet-0.0.6b1.dist-info/top_level.txt,sha256=BcmhB-73MgSM7c3Pf5xiAEwrx1SatziFSftm-eTAE1Q,9
-matfleet-0.0.6b1.dist-info/RECORD,,
+matfleet-0.0.7.dist-info/METADATA,sha256=iI3V5xpwdqMRej0w6YLOMthJi4RNmGSISbW71nKRTXI,1431
+matfleet-0.0.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+matfleet-0.0.7.dist-info/entry_points.txt,sha256=k8e-ij5k7oxLCDanRBh7RVpbDm_l5EN8_lr2Y0zQHt0,74
+matfleet-0.0.7.dist-info/top_level.txt,sha256=BcmhB-73MgSM7c3Pf5xiAEwrx1SatziFSftm-eTAE1Q,9
+matfleet-0.0.7.dist-info/RECORD,,
```

