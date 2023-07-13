# Comparing `tmp/table_recognition_metric-0.0.2-py3-none-any.whl.zip` & `tmp/table_recognition_metric-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4997 bytes, number of entries: 7
--rw-r--r--  2.0 unx      117 b- defN 23-Jul-12 11:32 table_recognition_metric/__init__.py
--rw-r--r--  2.0 unx     5674 b- defN 23-Jul-12 11:32 table_recognition_metric/main.py
--rw-r--r--  2.0 unx     4047 b- defN 23-Jul-12 11:32 table_recognition_metric-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 11:32 table_recognition_metric-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       81 b- defN 23-Jul-12 11:32 table_recognition_metric-0.0.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       25 b- defN 23-Jul-12 11:32 table_recognition_metric-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      659 b- defN 23-Jul-12 11:32 table_recognition_metric-0.0.2.dist-info/RECORD
-7 files, 10695 bytes uncompressed, 3801 bytes compressed:  64.5%
+Zip file size: 5052 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      117 b- defN 23-Jul-13 14:01 table_recognition_metric/__init__.py
+-rw-r--r--  2.0 unx     5674 b- defN 23-Jul-13 14:01 table_recognition_metric/main.py
+-rw-r--r--  2.0 unx     4289 b- defN 23-Jul-13 14:01 table_recognition_metric-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-13 14:01 table_recognition_metric-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       81 b- defN 23-Jul-13 14:01 table_recognition_metric-0.0.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       25 b- defN 23-Jul-13 14:01 table_recognition_metric-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      659 b- defN 23-Jul-13 14:01 table_recognition_metric-0.0.3.dist-info/RECORD
+7 files, 10937 bytes uncompressed, 3856 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: table_recognition_metric/__init__.py
 Comment: 
 
 Filename: table_recognition_metric/main.py
 Comment: 
 
-Filename: table_recognition_metric-0.0.2.dist-info/METADATA
+Filename: table_recognition_metric-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: table_recognition_metric-0.0.2.dist-info/WHEEL
+Filename: table_recognition_metric-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: table_recognition_metric-0.0.2.dist-info/entry_points.txt
+Filename: table_recognition_metric-0.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: table_recognition_metric-0.0.2.dist-info/top_level.txt
+Filename: table_recognition_metric-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: table_recognition_metric-0.0.2.dist-info/RECORD
+Filename: table_recognition_metric-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `table_recognition_metric-0.0.2.dist-info/METADATA` & `table_recognition_metric-0.0.3.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: table-recognition-metric
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tool of computing the TEDS of table recognition
 Home-page: https://github.com/SWHL/TableRecognitionMetric
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Keywords: ocr, table-recognition
 Platform: Any
@@ -20,14 +20,15 @@
 Requires-Dist: lxml (>=4.9.3)
 Requires-Dist: levenshtein
 
 ## table_recognition_metric
 <p align="left">
     <a href=""><img src="https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg"></a>
     <a href=""><img src="https://img.shields.io/badge/python->=3.6,<3.12-aff.svg"></a>
+    <a href="https://pypi.org/project/table_recognition_metric/"><img alt="PyPI" src="https://img.shields.io/pypi/v/table_recognition_metric"></a>
     <a href="https://pepy.tech/project/table-recognition-metric"><img src="https://static.pepy.tech/personalized-badge/table-recognition-metric?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads"></a>
 <a href="https://semver.org/"><img alt="SemVer2.0" src="https://img.shields.io/badge/SemVer-2.0-brightgreen"></a>
     <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
 
 ### 1. Install package by pypi.
 ```bash
@@ -57,7 +58,9 @@
 gt_html = '<html><body><table><tr><td>购买方</td><td colspan="5">纳税人识别号地址、电记开户行及账号</td><td>密码区</td><td colspan="4"></td></tr><tr><td colspan="2">货物或应税劳务、服务名称理肤泉清痘旅行装控油祛痘调节水油平衡理肤泉特安舒缓修护乳40ml合计</td><td>规格型号</td><td>单位</td><td>11</td><td colspan="3"></td><td></td><td>税率17%17%</td><td></td></tr><tr><td colspan="2">价税合计（大写）</td><td colspan="9"></td></tr><tr><td>销售方</td><td colspan="5">纳税人识别号地址、电话开户行及账号</td><td>备注</td><td colspan="4"></td></tr></table></body></html>'
 pred_html = '<html><body><table><tr><td>购买方</td><td colspan="5">纳税人识别号地址、电记开户行及账号</td><td>密码区</td><td colspan="4"></td></tr><tr><td colspan="2">货物或应税劳务、服务名称理肤泉清痘旅行装控油祛痘调节水油平衡理肤泉特安舒缓修护乳40ml合计</td><td>规格型号</td><td>单位</td><td>11</td><td colspan="3"></td><td></td><td>税率17%17%</td><td></td></tr><tr><td colspan="2">价税合计（大写）</td><td colspan="9"></td></tr><tr><td>销售方</td><td colspan="5">纳税人识别号地址、电话开户行及账号</td><td>备注</td><td colspan="4"></td></tr></table></body></html>'
 
 score = teds(gt_html, pred_html)
 print(score)
 ```
 
+### See details for [TableRecognitionMetric](https://github.com/SWHL/TableRecognitionMetric).
+
```

### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: table-recognition-metric Version: 0.0.2 Summary:
+Metadata-Version: 2.1 Name: table-recognition-metric Version: 0.0.3 Summary:
 Tool of computing the TEDS of table recognition Home-page: https://github.com/
 SWHL/TableRecognitionMetric Author: SWHL Author-email: liekkaskono@163.com
 License: Apache-2.0 Keywords: ocr, table-recognition Platform: Any Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Python: >=3.6,<3.12 Description-Content-Type: text/markdown Requires-Dist:
 apted (>=1.0.3) Requires-Dist: lxml (>=4.9.3) Requires-Dist: levenshtein ##
 table_recognition_metric
 [https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg] [https://
-img.shields.io/badge/python->=3.6,<3.12-aff.svg] [https://static.pepy.tech/
-personalized-badge/table-recognition-
+img.shields.io/badge/python->=3.6,<3.12-aff.svg] [PyPI] [https://
+static.pepy.tech/personalized-badge/table-recognition-
 metric?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads]
 [SemVer2.0] [https://img.shields.io/badge/code%20style-black-000000.svg]
 ### 1. Install package by pypi. ```bash pip install table_recognition_metric
 ``` ### 2. Run by command line. - Usage: ```bash $ table_recognition_metric -
 h usage: table_recognition_metric [-h] [-gt GT_HTML] [-pred PRED_HTML] optional
 arguments: -h, --help show this help message and exit -gt GT_HTML, --gt_html
 GT_HTML -pred PRED_HTML, --pred_html PRED_HTM ``` - Example: ```bash $
@@ -30,8 +30,9 @@
 ä»·ç¨åè®¡ï¼å¤§åï¼
 éåçº³ç¨äººè¯å«å·å°åãçµè¯å¼æ·è¡åè´¦å·                                           å¤æ³¨
 ' pred_html = '
 è´­ä¹çº³ç¨äººè¯å«å·å°åãçµè®°å¼æ·è¡åè´¦å·                                           å¯ç åº
 è´§ç©æåºç¨å³å¡ãæå¡åç§°çè¤æ³æ¸çæè¡è£æ§æ²�è§æ ¼�å�11�æ°´æ²�ç¨ç17%17%�è¤æ³ç¹å®èç¼ä¿®æ¤ä¹³40mlåè®¡
 ä»·ç¨åè®¡ï¼å¤§åï¼
 éåçº³ç¨äººè¯å«å·å°åãçµè¯å¼æ·è¡åè´¦å·                                           å¤æ³¨
-' score = teds(gt_html, pred_html) print(score) ```
+' score = teds(gt_html, pred_html) print(score) ``` ### See details for
+[TableRecognitionMetric](https://github.com/SWHL/TableRecognitionMetric).
```

## Comparing `table_recognition_metric-0.0.2.dist-info/RECORD` & `table_recognition_metric-0.0.3.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 table_recognition_metric/__init__.py,sha256=miYoIfaMmCPxPrImXPNAjFQBKjiUc6YlshLo8m4Avh4,117
 table_recognition_metric/main.py,sha256=IzfE2MXfavGuWj8zk25fiSftzyYYv39jSkVF0DHp-P0,5674
-table_recognition_metric-0.0.2.dist-info/METADATA,sha256=9w2DgYYHWzEfvKJigjJvQYjj02fHtOy4qRG4_RuC-vY,4047
-table_recognition_metric-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-table_recognition_metric-0.0.2.dist-info/entry_points.txt,sha256=fp9hx8Jmu2GwIA9PHpiTXg7hPjnUpldswOHmwUWJhfg,81
-table_recognition_metric-0.0.2.dist-info/top_level.txt,sha256=ojlGPRBOcj5veGfh4md1Xk45NHy9sskT44ef0fLKrxk,25
-table_recognition_metric-0.0.2.dist-info/RECORD,,
+table_recognition_metric-0.0.3.dist-info/METADATA,sha256=4As2ahFzeVaTa7NRBXzAqfJb96dvsom0GTVLWiShK5Y,4289
+table_recognition_metric-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+table_recognition_metric-0.0.3.dist-info/entry_points.txt,sha256=fp9hx8Jmu2GwIA9PHpiTXg7hPjnUpldswOHmwUWJhfg,81
+table_recognition_metric-0.0.3.dist-info/top_level.txt,sha256=ojlGPRBOcj5veGfh4md1Xk45NHy9sskT44ef0fLKrxk,25
+table_recognition_metric-0.0.3.dist-info/RECORD,,
```

