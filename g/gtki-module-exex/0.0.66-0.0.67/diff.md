# Comparing `tmp/gtki_module_exex-0.0.66-py3-none-any.whl.zip` & `tmp/gtki_module_exex-0.0.67-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 6858 bytes, number of entries: 11
+Zip file size: 6895 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jun-09 04:59 gtki_module_exex/__init__.py
--rw-rw-rw-  2.0 fat    12170 b- defN 23-Jul-13 11:49 gtki_module_exex/main.py
+-rw-rw-rw-  2.0 fat    12274 b- defN 23-Jul-13 11:55 gtki_module_exex/main.py
 -rw-rw-rw-  2.0 fat     1431 b- defN 23-Jun-15 14:51 gtki_module_exex/mixins.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jun-09 05:22 gtki_module_exex/tests/__init__.py
 -rw-rw-rw-  2.0 fat     2251 b- defN 23-Jul-06 07:30 gtki_module_exex/tests/main_tests.py
 -rw-rw-rw-  2.0 fat     1007 b- defN 22-Jun-09 05:55 gtki_module_exex/tests/mixins_tests.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jul-13 11:50 gtki_module_exex-0.0.66.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      280 b- defN 23-Jul-13 11:50 gtki_module_exex-0.0.66.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-13 11:50 gtki_module_exex-0.0.66.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-13 11:50 gtki_module_exex-0.0.66.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      958 b- defN 23-Jul-13 11:50 gtki_module_exex-0.0.66.dist-info/RECORD
-11 files, 19297 bytes uncompressed, 5210 bytes compressed:  73.0%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jul-13 11:56 gtki_module_exex-0.0.67.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      280 b- defN 23-Jul-13 11:56 gtki_module_exex-0.0.67.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-13 11:56 gtki_module_exex-0.0.67.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-13 11:56 gtki_module_exex-0.0.67.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      958 b- defN 23-Jul-13 11:56 gtki_module_exex-0.0.67.dist-info/RECORD
+11 files, 19401 bytes uncompressed, 5247 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: gtki_module_exex/tests/main_tests.py
 Comment: 
 
 Filename: gtki_module_exex/tests/mixins_tests.py
 Comment: 
 
-Filename: gtki_module_exex-0.0.66.dist-info/LICENSE
+Filename: gtki_module_exex-0.0.67.dist-info/LICENSE
 Comment: 
 
-Filename: gtki_module_exex-0.0.66.dist-info/METADATA
+Filename: gtki_module_exex-0.0.67.dist-info/METADATA
 Comment: 
 
-Filename: gtki_module_exex-0.0.66.dist-info/WHEEL
+Filename: gtki_module_exex-0.0.67.dist-info/WHEEL
 Comment: 
 
-Filename: gtki_module_exex-0.0.66.dist-info/top_level.txt
+Filename: gtki_module_exex-0.0.67.dist-info/top_level.txt
 Comment: 
 
-Filename: gtki_module_exex-0.0.66.dist-info/RECORD
+Filename: gtki_module_exex-0.0.67.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gtki_module_exex/main.py

```diff
@@ -69,14 +69,15 @@
 
     def create_day_header(self, day=None):
         merge_format = self.workbook.add_format({'align': 'center'})
         merge_format.set_font_size(14)
         self.worksheet.merge_range('A1:G1', day, merge_format)
 
     def operate_trash_cat(self, trash_cat, day, start_row):
+        print("WORKING WITH", trash_cat)
         records = self.ar_qdk.execute_method("get_daily_report_by_trash_cat",
                                              trash_cat=trash_cat,
                                              day=day,
                                              except_car_numbers=('Н370УЕ102'),
                                              get_response=True)
         if records['status']:
             records = records['info']
@@ -149,16 +150,18 @@
             day = datetime.datetime.now()
         self.create_day_header(day.strftime("%#d/%m/%Y"))
         self.set_column_width()
         start_row = self.set_column_names()
         new_row = start_row
         for tc in ["ТКО", "ПО", "Хвосты", "Прочее"]:
             response = self.operate_trash_cat(tc, day.strftime("%Y.%m.%d"),
-                                               start_row=new_row)
+                                            start_row=new_row)
+            print(response)
             if response:
+                new_row = response
                 amounts.append(response + 2)
                 new_row += 1
         hyn_row = self.add_hyundai(day, new_row)
         if hyn_row:
             amounts.append(hyn_row + 2)
             new_row = hyn_row
         phys_row = self.add_phys(day, new_row + 2)
```

## Comparing `gtki_module_exex-0.0.66.dist-info/LICENSE` & `gtki_module_exex-0.0.67.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gtki_module_exex-0.0.66.dist-info/RECORD` & `gtki_module_exex-0.0.67.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 gtki_module_exex/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-gtki_module_exex/main.py,sha256=U9-eYLQFLeGru95S3CaRseZDZjT7CtByXTel-KkvP1E,12170
+gtki_module_exex/main.py,sha256=rgnxyr0gBIZQkNjQEfSs6VCHvImzvzGvJhl01YM1soM,12274
 gtki_module_exex/mixins.py,sha256=nKYRHMoFYSva364Q2WyH30SefjAxi5xGXekgLmRAyXk,1431
 gtki_module_exex/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 gtki_module_exex/tests/main_tests.py,sha256=ZTo-ylgaHZCNeMuVtoktNdEzwioc9r6XU7EWCgpVfGw,2251
 gtki_module_exex/tests/mixins_tests.py,sha256=8oogAhtkQgyhB3sUEsIvQpvA1a7YrRPc76bDHKsxodI,1007
-gtki_module_exex-0.0.66.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-gtki_module_exex-0.0.66.dist-info/METADATA,sha256=4lLaccHIigWljU-kgAz8qtmyFewd4jTjRMotzQG8fyw,280
-gtki_module_exex-0.0.66.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-gtki_module_exex-0.0.66.dist-info/top_level.txt,sha256=5fDck53WZ0oTnmcblVZKn9XwbA-Uqijh0L93F1ml9Bc,17
-gtki_module_exex-0.0.66.dist-info/RECORD,,
+gtki_module_exex-0.0.67.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+gtki_module_exex-0.0.67.dist-info/METADATA,sha256=OFfTNM3dW727_K450m6jXVl3K9LYT-BIjPP4QF45BWg,280
+gtki_module_exex-0.0.67.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+gtki_module_exex-0.0.67.dist-info/top_level.txt,sha256=5fDck53WZ0oTnmcblVZKn9XwbA-Uqijh0L93F1ml9Bc,17
+gtki_module_exex-0.0.67.dist-info/RECORD,,
```

