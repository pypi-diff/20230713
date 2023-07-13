# Comparing `tmp/nsqdriver-0.4.1-cp39-cp39-win_amd64.whl.zip` & `tmp/nsqdriver-0.4.2-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,19 @@
-Zip file size: 231179 bytes, number of entries: 18
--rw-rw-rw-  2.0 fat     8137 b- defN 23-Jul-10 06:36 nsqdriver/NS_CST.py
--rw-rw-rw-  2.0 fat    20142 b- defN 23-Jul-10 06:36 nsqdriver/NS_MCI.py
--rw-rw-rw-  2.0 fat    23950 b- defN 23-Jul-10 06:36 nsqdriver/NS_QSYNC.py
--rw-rw-rw-  2.0 fat      381 b- defN 23-Jul-10 06:36 nsqdriver/__init__.py
--rw-rw-rw-  2.0 fat      519 b- defN 23-Jul-10 06:36 nsqdriver/common.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-10 06:36 nsqdriver/compiler/__init__.py
--rw-rw-rw-  2.0 fat   214528 b- defN 23-Jul-10 06:38 nsqdriver/compiler/ns_wave.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     3975 b- defN 23-Jul-10 06:36 nsqdriver/compiler/ns_wave.pyi
--rw-rw-rw-  2.0 fat   272384 b- defN 23-Jul-10 06:38 nsqdriver/compiler/py_wave_asm.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      685 b- defN 23-Jul-10 06:36 nsqdriver/compiler/py_wave_asm.pyi
--rw-rw-rw-  2.0 fat    19745 b- defN 23-Jul-10 06:36 nsqdriver/wrapper/AWG_ADC.py
--rw-rw-rw-  2.0 fat    12555 b- defN 23-Jul-10 06:36 nsqdriver/wrapper/BD_NSMCI.py
--rw-rw-rw-  2.0 fat     6533 b- defN 23-Jul-10 06:36 nsqdriver/wrapper/ND_NSMCI.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-10 06:36 nsqdriver/wrapper/__init__.py
--rw-rw-rw-  2.0 fat     4465 b- defN 23-Jul-10 06:38 nsqdriver-0.4.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-10 06:38 nsqdriver-0.4.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Jul-10 06:37 nsqdriver-0.4.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1506 b- defN 23-Jul-10 06:38 nsqdriver-0.4.1.dist-info/RECORD
-18 files, 589615 bytes uncompressed, 228713 bytes compressed:  61.2%
+Zip file size: 227727 bytes, number of entries: 17
+-rw-rw-rw-  2.0 fat     8137 b- defN 23-Jul-13 05:37 nsqdriver/NS_CST.py
+-rw-rw-rw-  2.0 fat    20142 b- defN 23-Jul-13 05:37 nsqdriver/NS_MCI.py
+-rw-rw-rw-  2.0 fat    23950 b- defN 23-Jul-13 05:37 nsqdriver/NS_QSYNC.py
+-rw-rw-rw-  2.0 fat      381 b- defN 23-Jul-13 05:37 nsqdriver/__init__.py
+-rw-rw-rw-  2.0 fat      519 b- defN 23-Jul-13 05:37 nsqdriver/common.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-13 05:37 nsqdriver/compiler/__init__.py
+-rw-rw-rw-  2.0 fat   214528 b- defN 23-Jul-13 05:38 nsqdriver/compiler/ns_wave.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     3975 b- defN 23-Jul-13 05:37 nsqdriver/compiler/ns_wave.pyi
+-rw-rw-rw-  2.0 fat   272384 b- defN 23-Jul-13 05:39 nsqdriver/compiler/py_wave_asm.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      685 b- defN 23-Jul-13 05:37 nsqdriver/compiler/py_wave_asm.pyi
+-rw-rw-rw-  2.0 fat    19745 b- defN 23-Jul-13 05:37 nsqdriver/wrapper/AWG_ADC.py
+-rw-rw-rw-  2.0 fat     6533 b- defN 23-Jul-13 05:37 nsqdriver/wrapper/ND_NSMCI.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-13 05:37 nsqdriver/wrapper/__init__.py
+-rw-rw-rw-  2.0 fat     4465 b- defN 23-Jul-13 05:39 nsqdriver-0.4.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-13 05:39 nsqdriver-0.4.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Jul-13 05:38 nsqdriver-0.4.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1419 b- defN 23-Jul-13 05:39 nsqdriver-0.4.2.dist-info/RECORD
+17 files, 576973 bytes uncompressed, 225395 bytes compressed:  60.9%
```

## zipnote {}

```diff
@@ -27,29 +27,26 @@
 
 Filename: nsqdriver/compiler/py_wave_asm.pyi
 Comment: 
 
 Filename: nsqdriver/wrapper/AWG_ADC.py
 Comment: 
 
-Filename: nsqdriver/wrapper/BD_NSMCI.py
-Comment: 
-
 Filename: nsqdriver/wrapper/ND_NSMCI.py
 Comment: 
 
 Filename: nsqdriver/wrapper/__init__.py
 Comment: 
 
-Filename: nsqdriver-0.4.1.dist-info/METADATA
+Filename: nsqdriver-0.4.2.dist-info/METADATA
 Comment: 
 
-Filename: nsqdriver-0.4.1.dist-info/WHEEL
+Filename: nsqdriver-0.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: nsqdriver-0.4.1.dist-info/top_level.txt
+Filename: nsqdriver-0.4.2.dist-info/top_level.txt
 Comment: 
 
-Filename: nsqdriver-0.4.1.dist-info/RECORD
+Filename: nsqdriver-0.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nsqdriver/__init__.py

```diff
@@ -1,10 +1,10 @@
 from .NS_MCI import Driver as MCIDriver
 from .NS_QSYNC import Driver as QSYNCDriver
 from .NS_CST import Driver as CSTDriver
 from .compiler.ns_wave import InsChannel
 from .compiler.py_wave_asm import nsw_config, AssemblyError
 
-version_pack = (0, 4, 1)
+version_pack = (0, 4, 2)
 
 __version__ = '.'.join(str(_) for _ in version_pack)
 __all__ = ['MCIDriver', 'QSYNCDriver', 'CSTDriver', 'InsChannel']
```

## Comparing `nsqdriver-0.4.1.dist-info/METADATA` & `nsqdriver-0.4.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsqdriver
-Version: 0.4.1
+Version: 0.4.2
 Summary: Naishu Q series quantum measurement and control equipment driver interface
 Home-page: https://g2hoyqcmh4.feishu.cn/wiki/wikcnzvyMd82DLZUe2NsI6HxsFc
 Author: Naishu Technology
 Author-email: jilianyi@naishu.tech
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
 Classifier: Operating System :: MacOS :: MacOS X
```

## Comparing `nsqdriver-0.4.1.dist-info/RECORD` & `nsqdriver-0.4.2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 nsqdriver/NS_CST.py,sha256=zA5YcM65v66EqwBnplDvA6HM0I-y8damDOerE2CKyZE,8137
 nsqdriver/NS_MCI.py,sha256=dyjqAhIHwfPQgh7GRiYISRYi3I3BIVbnSjXij-Y-T1I,20142
 nsqdriver/NS_QSYNC.py,sha256=2tKMeRb5S4pHPD_CWfVTVPJFNRwo0OLwyevEgD6izDg,23950
-nsqdriver/__init__.py,sha256=Z8Wi2UWn4pDu2rsGYljshMmDeximrJOyMsDYAa7n8IU,381
+nsqdriver/__init__.py,sha256=pdL_TL58PRJzSH4UKO3Mu_ArmI0JKsM7ujOK61bjC4A,381
 nsqdriver/common.py,sha256=5BRActb9TgNdVwWtfuZ_gki47H1WbABzYr5XbxLKlh4,519
 nsqdriver/compiler/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-nsqdriver/compiler/ns_wave.cp39-win_amd64.pyd,sha256=kVU_vO_kgoa0EAnkLROWWfCR_HjvrLtwkcKoOQJlmZU,214528
+nsqdriver/compiler/ns_wave.cp39-win_amd64.pyd,sha256=d7ewm1_u6gFefusl81yRr8cwnR1OuHXHudspz9prbmo,214528
 nsqdriver/compiler/ns_wave.pyi,sha256=axQaxrMaKRPx8k9sDVlRj3SjR03AmXUDzkVW4D_2RJw,3975
-nsqdriver/compiler/py_wave_asm.cp39-win_amd64.pyd,sha256=7lskEV8d6UDaM9M_uLeBmeI2vllWkqAC_2g2q6AY-ps,272384
+nsqdriver/compiler/py_wave_asm.cp39-win_amd64.pyd,sha256=U4GY5kmOXCIboX7iEGJfooNPYNzT7f8MMhbnDyJgA0g,272384
 nsqdriver/compiler/py_wave_asm.pyi,sha256=PqEZuNt83CCu_FJUczUjStowOz2TBgvfIytGanFPHuQ,685
 nsqdriver/wrapper/AWG_ADC.py,sha256=I4nPtbQTHxqAqFuXTHb_oDLW-ycRxSUpBUyD67eq_dA,19745
-nsqdriver/wrapper/BD_NSMCI.py,sha256=BdMFvBDiAX8pms3RdfA8d4hjSMOG6yjo5uZjWEr7t6o,12555
 nsqdriver/wrapper/ND_NSMCI.py,sha256=e0j7BUdfrhfYb1GqBPlO4vSoZPXTKyictXy1nPvoMFE,6533
 nsqdriver/wrapper/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-nsqdriver-0.4.1.dist-info/METADATA,sha256=IyaNA0VcxY4N23x2CiCjMHyzP-nvzSO6iR_Sl17plmU,4465
-nsqdriver-0.4.1.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-nsqdriver-0.4.1.dist-info/top_level.txt,sha256=o7EbQoFO6BoaG3KGbS9Lg_aRheZSY5KYzoYuI9vx-AI,10
-nsqdriver-0.4.1.dist-info/RECORD,,
+nsqdriver-0.4.2.dist-info/METADATA,sha256=3TMmkVeHqWtCwulFHh4Fe-NDtPBOTVInIghcJaF1wGg,4465
+nsqdriver-0.4.2.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+nsqdriver-0.4.2.dist-info/top_level.txt,sha256=o7EbQoFO6BoaG3KGbS9Lg_aRheZSY5KYzoYuI9vx-AI,10
+nsqdriver-0.4.2.dist-info/RECORD,,
```

