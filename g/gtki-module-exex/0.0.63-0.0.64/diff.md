# Comparing `tmp/gtki_module_exex-0.0.63-py3-none-any.whl.zip` & `tmp/gtki_module_exex-0.0.64-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 6847 bytes, number of entries: 11
+Zip file size: 6856 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jun-09 04:59 gtki_module_exex/__init__.py
--rw-rw-rw-  2.0 fat    12132 b- defN 23-Jul-11 13:33 gtki_module_exex/main.py
+-rw-rw-rw-  2.0 fat    12165 b- defN 23-Jul-13 04:31 gtki_module_exex/main.py
 -rw-rw-rw-  2.0 fat     1431 b- defN 23-Jun-15 14:51 gtki_module_exex/mixins.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jun-09 05:22 gtki_module_exex/tests/__init__.py
 -rw-rw-rw-  2.0 fat     2251 b- defN 23-Jul-06 07:30 gtki_module_exex/tests/main_tests.py
 -rw-rw-rw-  2.0 fat     1007 b- defN 22-Jun-09 05:55 gtki_module_exex/tests/mixins_tests.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jul-11 13:34 gtki_module_exex-0.0.63.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      280 b- defN 23-Jul-11 13:34 gtki_module_exex-0.0.63.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-11 13:34 gtki_module_exex-0.0.63.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-11 13:34 gtki_module_exex-0.0.63.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      958 b- defN 23-Jul-11 13:34 gtki_module_exex-0.0.63.dist-info/RECORD
-11 files, 19259 bytes uncompressed, 5199 bytes compressed:  73.0%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jul-13 04:33 gtki_module_exex-0.0.64.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      280 b- defN 23-Jul-13 04:33 gtki_module_exex-0.0.64.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-13 04:33 gtki_module_exex-0.0.64.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-13 04:33 gtki_module_exex-0.0.64.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      958 b- defN 23-Jul-13 04:33 gtki_module_exex-0.0.64.dist-info/RECORD
+11 files, 19292 bytes uncompressed, 5208 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: gtki_module_exex/tests/main_tests.py
 Comment: 
 
 Filename: gtki_module_exex/tests/mixins_tests.py
 Comment: 
 
-Filename: gtki_module_exex-0.0.63.dist-info/LICENSE
+Filename: gtki_module_exex-0.0.64.dist-info/LICENSE
 Comment: 
 
-Filename: gtki_module_exex-0.0.63.dist-info/METADATA
+Filename: gtki_module_exex-0.0.64.dist-info/METADATA
 Comment: 
 
-Filename: gtki_module_exex-0.0.63.dist-info/WHEEL
+Filename: gtki_module_exex-0.0.64.dist-info/WHEEL
 Comment: 
 
-Filename: gtki_module_exex-0.0.63.dist-info/top_level.txt
+Filename: gtki_module_exex-0.0.64.dist-info/top_level.txt
 Comment: 
 
-Filename: gtki_module_exex-0.0.63.dist-info/RECORD
+Filename: gtki_module_exex-0.0.64.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gtki_module_exex/main.py

```diff
@@ -150,16 +150,17 @@
         self.create_day_header(day.strftime("%#d/%m/%Y"))
         self.set_column_width()
         start_row = self.set_column_names()
         new_row = start_row
         for tc in ["ТКО", "ПО", "Хвосты", "Прочее"]:
             new_row = self.operate_trash_cat(tc, day.strftime("%Y.%m.%d"),
                                              start_row=new_row)
-            amounts.append(new_row + 2)
-            new_row += 1
+            if new_row:
+                amounts.append(new_row + 2)
+                new_row += 1
         hyn_row = self.add_hyundai(day, new_row)
         if hyn_row:
             amounts.append(hyn_row + 2)
             new_row = hyn_row
         phys_row = self.add_phys(day, new_row + 2)
         if phys_row:
             amounts.append(phys_row + 2)
```

## Comparing `gtki_module_exex-0.0.63.dist-info/LICENSE` & `gtki_module_exex-0.0.64.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gtki_module_exex-0.0.63.dist-info/RECORD` & `gtki_module_exex-0.0.64.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 gtki_module_exex/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-gtki_module_exex/main.py,sha256=vCTFsxSrJ0GgfoSQMpYso7qbAur4VUGq7VzwJmBWcw8,12132
+gtki_module_exex/main.py,sha256=UeTprSXBUsaZMVfnVHb3PTuCMGY3_FnRgUIo6AXFilU,12165
 gtki_module_exex/mixins.py,sha256=nKYRHMoFYSva364Q2WyH30SefjAxi5xGXekgLmRAyXk,1431
 gtki_module_exex/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 gtki_module_exex/tests/main_tests.py,sha256=ZTo-ylgaHZCNeMuVtoktNdEzwioc9r6XU7EWCgpVfGw,2251
 gtki_module_exex/tests/mixins_tests.py,sha256=8oogAhtkQgyhB3sUEsIvQpvA1a7YrRPc76bDHKsxodI,1007
-gtki_module_exex-0.0.63.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-gtki_module_exex-0.0.63.dist-info/METADATA,sha256=7Fk84kOe9WCo7RuRzvrNSIY3fz65JYCjjSYJ1i62_MI,280
-gtki_module_exex-0.0.63.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-gtki_module_exex-0.0.63.dist-info/top_level.txt,sha256=5fDck53WZ0oTnmcblVZKn9XwbA-Uqijh0L93F1ml9Bc,17
-gtki_module_exex-0.0.63.dist-info/RECORD,,
+gtki_module_exex-0.0.64.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+gtki_module_exex-0.0.64.dist-info/METADATA,sha256=GEJBxrunDS7tznexr7sp-EzJfcAYyrq8wlcPKCyPN_A,280
+gtki_module_exex-0.0.64.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+gtki_module_exex-0.0.64.dist-info/top_level.txt,sha256=5fDck53WZ0oTnmcblVZKn9XwbA-Uqijh0L93F1ml9Bc,17
+gtki_module_exex-0.0.64.dist-info/RECORD,,
```

