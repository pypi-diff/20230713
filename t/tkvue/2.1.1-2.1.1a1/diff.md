# Comparing `tmp/tkvue-2.1.1-py3-none-any.whl.zip` & `tmp/tkvue-2.1.1a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 196208 bytes, number of entries: 10
--rw-r--r--  2.0 unx    31759 b- defN 23-Jul-12 18:27 tkvue/__init__.py
--rw-rw-rw-  2.0 unx   170486 b- defN 23-Jul-12 18:27 tkvue/tests/preloader.gif
--rw-rw-rw-  2.0 unx      814 b- defN 23-Jul-12 18:27 tkvue/tests/python_icon.png
--rw-rw-rw-  2.0 unx    23217 b- defN 23-Jul-12 18:27 tkvue/tests/test_tkvue.py
--rw-rw-rw-  2.0 unx    26523 b- defN 23-Jul-12 18:27 tkvue-2.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     6250 b- defN 23-Jul-12 18:27 tkvue-2.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 18:27 tkvue-2.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 23-Jul-12 18:27 tkvue-2.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Jul-12 18:27 tkvue-2.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      794 b- defN 23-Jul-12 18:27 tkvue-2.1.1.dist-info/RECORD
-10 files, 259988 bytes uncompressed, 194864 bytes compressed:  25.0%
+Zip file size: 196235 bytes, number of entries: 10
+-rw-r--r--  2.0 unx    31759 b- defN 23-Jul-12 18:21 tkvue/__init__.py
+-rw-rw-rw-  2.0 unx   170486 b- defN 22-Nov-09 20:32 tkvue/tests/preloader.gif
+-rw-rw-rw-  2.0 unx      814 b- defN 22-Nov-09 20:32 tkvue/tests/python_icon.png
+-rw-rw-rw-  2.0 unx    23217 b- defN 23-Jul-12 18:21 tkvue/tests/test_tkvue.py
+-rw-rw-rw-  2.0 unx    26523 b- defN 23-Jul-12 18:21 tkvue-2.1.1a1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6252 b- defN 23-Jul-12 18:21 tkvue-2.1.1a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 18:21 tkvue-2.1.1a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-Jul-12 18:21 tkvue-2.1.1a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-12 18:21 tkvue-2.1.1a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      806 b- defN 23-Jul-12 18:21 tkvue-2.1.1a1.dist-info/RECORD
+10 files, 260002 bytes uncompressed, 194867 bytes compressed:  25.1%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: tkvue/tests/python_icon.png
 Comment: 
 
 Filename: tkvue/tests/test_tkvue.py
 Comment: 
 
-Filename: tkvue-2.1.1.dist-info/LICENSE
+Filename: tkvue-2.1.1a1.dist-info/LICENSE
 Comment: 
 
-Filename: tkvue-2.1.1.dist-info/METADATA
+Filename: tkvue-2.1.1a1.dist-info/METADATA
 Comment: 
 
-Filename: tkvue-2.1.1.dist-info/WHEEL
+Filename: tkvue-2.1.1a1.dist-info/WHEEL
 Comment: 
 
-Filename: tkvue-2.1.1.dist-info/entry_points.txt
+Filename: tkvue-2.1.1a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: tkvue-2.1.1.dist-info/top_level.txt
+Filename: tkvue-2.1.1a1.dist-info/top_level.txt
 Comment: 
 
-Filename: tkvue-2.1.1.dist-info/RECORD
+Filename: tkvue-2.1.1a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `tkvue-2.1.1.dist-info/LICENSE` & `tkvue-2.1.1a1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tkvue-2.1.1.dist-info/METADATA` & `tkvue-2.1.1a1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkvue
-Version: 2.1.1
+Version: 2.1.1a1
 Summary: Declarative Tkinter UI using makup language with reactive data binding
 Home-page: https://gitlab.com/ikus-soft/tkvue
 Author: IKUS Software inc.
 Author-email: support@ikus-soft.com
 Maintainer: Patrik Dufresne
 Maintainer-email: patrik@ikus-soft.com
 License: LGPLv3
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tkvue Version: 2.1.1 Summary: Declarative Tkinter
+Metadata-Version: 2.1 Name: tkvue Version: 2.1.1a1 Summary: Declarative Tkinter
 UI using makup language with reactive data binding Home-page: https://
 gitlab.com/ikus-soft/tkvue Author: IKUS Software inc. Author-email:
 support@ikus-soft.com Maintainer: Patrik Dufresne Maintainer-email:
 patrik@ikus-soft.com License: LGPLv3 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: X11 Applications Classifier: Environment :: Win32
 (MS Windows) Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: End Users/Desktop Classifier: License :: OSI Approved :: GNU Lesser
```

## Comparing `tkvue-2.1.1.dist-info/RECORD` & `tkvue-2.1.1a1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 tkvue/__init__.py,sha256=EKCfF5iy3hv1ECtXfORb2ajPuWDeYbALcTSzHKXSBIk,31759
 tkvue/tests/preloader.gif,sha256=4WubudKMAoutzmKtq4PR70A8DoCy5GC_fdVn08FRItc,170486
 tkvue/tests/python_icon.png,sha256=TNB4Jv9uPJYDC9CxCVUv6q5Fu6mlSx2Skuk68ckAcqQ,814
 tkvue/tests/test_tkvue.py,sha256=ou_M6PUEyTeVlPOA0UfTAaW4OyZigxjcXX7m86Cnv7A,23217
-tkvue-2.1.1.dist-info/LICENSE,sha256=wOyDtdXHKbVMd0kW1v8xZvyrYk9MeGP2-70glJMR9nc,26523
-tkvue-2.1.1.dist-info/METADATA,sha256=BB-7wDfx9n_iisHTiWGm54pYyYZK5WMdjcZBRf8UaXs,6250
-tkvue-2.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-tkvue-2.1.1.dist-info/entry_points.txt,sha256=8VY5M0e9X8hXWRDu4nXU60waEEcTmLS5mRgxCmcVE88,47
-tkvue-2.1.1.dist-info/top_level.txt,sha256=anZORAc3YItPGY-GYRZ9zA_9cHsS-bhOtuYTL0R6ffU,6
-tkvue-2.1.1.dist-info/RECORD,,
+tkvue-2.1.1a1.dist-info/LICENSE,sha256=wOyDtdXHKbVMd0kW1v8xZvyrYk9MeGP2-70glJMR9nc,26523
+tkvue-2.1.1a1.dist-info/METADATA,sha256=nv1HTIIoROWtnQdmDY_hZzgGW2DwmdwCfajhtoCe7nI,6252
+tkvue-2.1.1a1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+tkvue-2.1.1a1.dist-info/entry_points.txt,sha256=8VY5M0e9X8hXWRDu4nXU60waEEcTmLS5mRgxCmcVE88,47
+tkvue-2.1.1a1.dist-info/top_level.txt,sha256=anZORAc3YItPGY-GYRZ9zA_9cHsS-bhOtuYTL0R6ffU,6
+tkvue-2.1.1a1.dist-info/RECORD,,
```

