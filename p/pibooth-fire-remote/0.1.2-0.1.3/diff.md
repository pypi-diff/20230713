# Comparing `tmp/pibooth_fire_remote-0.1.2-py3-none-any.whl.zip` & `tmp/pibooth_fire_remote-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,8 @@
-Zip file size: 3991 bytes, number of entries: 7
--rw-r--r--  2.0 unx     4015 b- defN 23-Jan-08 10:55 pibooth_fire_remote.py
--rw-r--r--  2.0 unx     1066 b- defN 23-Jan-08 11:05 pibooth_fire_remote-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1481 b- defN 23-Jan-08 11:05 pibooth_fire_remote-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-08 11:05 pibooth_fire_remote-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 23-Jan-08 11:05 pibooth_fire_remote-0.1.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 23-Jan-08 11:05 pibooth_fire_remote-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      632 b- defN 23-Jan-08 11:05 pibooth_fire_remote-0.1.2.dist-info/RECORD
-7 files, 7358 bytes uncompressed, 2851 bytes compressed:  61.3%
+Zip file size: 2800 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     1066 b- defN 23-Jul-13 19:36 pibooth_fire_remote-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1478 b- defN 23-Jul-13 19:36 pibooth_fire_remote-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-13 19:36 pibooth_fire_remote-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-Jul-13 19:36 pibooth_fire_remote-0.1.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-13 19:36 pibooth_fire_remote-0.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      552 b- defN 23-Jul-13 19:36 pibooth_fire_remote-0.1.3.dist-info/RECORD
+6 files, 3242 bytes uncompressed, 1780 bytes compressed:  45.1%
```

## zipnote {}

```diff
@@ -1,22 +1,19 @@
-Filename: pibooth_fire_remote.py
+Filename: pibooth_fire_remote-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: pibooth_fire_remote-0.1.2.dist-info/LICENSE
+Filename: pibooth_fire_remote-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: pibooth_fire_remote-0.1.2.dist-info/METADATA
+Filename: pibooth_fire_remote-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: pibooth_fire_remote-0.1.2.dist-info/WHEEL
+Filename: pibooth_fire_remote-0.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: pibooth_fire_remote-0.1.2.dist-info/entry_points.txt
+Filename: pibooth_fire_remote-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pibooth_fire_remote-0.1.2.dist-info/top_level.txt
-Comment: 
-
-Filename: pibooth_fire_remote-0.1.2.dist-info/RECORD
+Filename: pibooth_fire_remote-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pibooth_fire_remote-0.1.2.dist-info/LICENSE` & `pibooth_fire_remote-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pibooth_fire_remote-0.1.2.dist-info/METADATA` & `pibooth_fire_remote-0.1.3.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: pibooth-fire-remote
-Version: 0.1.2
+Version: 0.1.3
+Summary: UNKNOWN
 Home-page: https://github.com/chilipp89/pibooth-qr-download
 Author: P. Junietz
 License: MIT
 Keywords: Raspberry Pi,camera,photobooth,Bluetooth,Remote
 Platform: unix
 Platform: linux
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,17 +18,16 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Natural Language :: English
 Classifier: Topic :: Multimedia :: Graphics :: Capture :: Digital Camera
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
+Requires-Dist: evdev
 Requires-Dist: pibooth (>=2.0.0)
-Requires-Dist: evfev
 Requires-Dist: pygame
 
 # pibooth-fire-remote
 Remote Control with bluetooth Remote
 
 # Install
 pip install pibooth-fire-remote
@@ -53,7 +53,9 @@
 - enterBtn: Take Picture
 - settingsBtn: Open Menu
 - forward: Print
 
 
 
 
+
+
```

## Comparing `pibooth_fire_remote-0.1.2.dist-info/RECORD` & `pibooth_fire_remote-0.1.3.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,6 @@
-pibooth_fire_remote.py,sha256=81yNlTupv9scDJsafizfUyXNttnOhv6StPLxIuMrPMI,4015
-pibooth_fire_remote-0.1.2.dist-info/LICENSE,sha256=8MhKKX4jcdh7M60uTWf4zk_cdmFXMxHe26HsSJyZphU,1066
-pibooth_fire_remote-0.1.2.dist-info/METADATA,sha256=cDEl1Jefp5l0h9VHKWaErh1yXX92JobLVSpNJ24qTrw,1481
-pibooth_fire_remote-0.1.2.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-pibooth_fire_remote-0.1.2.dist-info/entry_points.txt,sha256=_3nuHjdNfa4xmkyNoHKHKuEM-Kd76WPP2i9YFh1Yhqg,52
-pibooth_fire_remote-0.1.2.dist-info/top_level.txt,sha256=uzVg30QGLIeuYlAgFLl7efJyUgD2uoKL2lOpC9oJGeY,20
-pibooth_fire_remote-0.1.2.dist-info/RECORD,,
+pibooth_fire_remote-0.1.3.dist-info/LICENSE,sha256=8MhKKX4jcdh7M60uTWf4zk_cdmFXMxHe26HsSJyZphU,1066
+pibooth_fire_remote-0.1.3.dist-info/METADATA,sha256=btkp-yXrx7N-00F-godXkZfRUGiRgYurGfyxgPclEsQ,1478
+pibooth_fire_remote-0.1.3.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+pibooth_fire_remote-0.1.3.dist-info/entry_points.txt,sha256=ExheM_w4JJMaMeao7ARgseEwDMsCCzTXD0F170rgR0U,53
+pibooth_fire_remote-0.1.3.dist-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+pibooth_fire_remote-0.1.3.dist-info/RECORD,,
```

