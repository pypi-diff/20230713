# Comparing `tmp/LabelFusion-1.0.7-py3-none-any.whl.zip` & `tmp/LabelFusion-1.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
 Zip file size: 12980 bytes, number of entries: 14
--rw-r--r--  2.0 unx       83 b- defN 21-Mar-24 03:16 LabelFusion/__init__.py
--rw-r--r--  2.0 unx     1446 b- defN 21-Mar-24 03:16 LabelFusion/fusion_wrappers.py
--rw-r--r--  2.0 unx    21958 b- defN 21-Mar-24 03:16 LabelFusion/fusionator.py
--rw-r--r--  2.0 unx     1608 b- defN 21-Mar-24 03:16 LabelFusion/itkUtils.py
--rw-r--r--  2.0 unx      482 b- defN 21-Mar-24 03:16 LabelFusion/majority_voting.py
--rw-r--r--  2.0 unx     1758 b- defN 21-Mar-24 03:16 LabelFusion/simple.py
--rw-r--r--  2.0 unx     1312 b- defN 21-Mar-24 03:16 LabelFusion/utils.py
--rw-r--r--  2.0 unx     1112 b- defN 21-Mar-24 03:16 LabelFusion/wrapper.py
--rwxr-xr-x  2.0 unx     2156 b- defN 21-Mar-24 03:17 LabelFusion-1.0.7.data/scripts/fusion_run
--rw-r--r--  2.0 unx      277 b- defN 21-Mar-24 03:17 LabelFusion-1.0.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     4527 b- defN 21-Mar-24 03:17 LabelFusion-1.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Mar-24 03:17 LabelFusion-1.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 21-Mar-24 03:17 LabelFusion-1.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1151 b- defN 21-Mar-24 03:17 LabelFusion-1.0.7.dist-info/RECORD
+-rw-r--r--  2.0 unx       83 b- defN 21-Mar-24 11:10 LabelFusion/__init__.py
+-rw-r--r--  2.0 unx     1446 b- defN 21-Mar-24 11:10 LabelFusion/fusion_wrappers.py
+-rw-r--r--  2.0 unx    21958 b- defN 21-Mar-24 11:10 LabelFusion/fusionator.py
+-rw-r--r--  2.0 unx     1608 b- defN 21-Mar-24 11:10 LabelFusion/itkUtils.py
+-rw-r--r--  2.0 unx      482 b- defN 21-Mar-24 11:10 LabelFusion/majority_voting.py
+-rw-r--r--  2.0 unx     1758 b- defN 21-Mar-24 11:10 LabelFusion/simple.py
+-rw-r--r--  2.0 unx     1312 b- defN 21-Mar-24 11:10 LabelFusion/utils.py
+-rw-r--r--  2.0 unx     1112 b- defN 21-Mar-24 11:10 LabelFusion/wrapper.py
+-rwxr-xr-x  2.0 unx     2156 b- defN 21-Mar-24 11:11 LabelFusion-1.0.8.data/scripts/fusion_run
+-rw-r--r--  2.0 unx      277 b- defN 21-Mar-24 11:11 LabelFusion-1.0.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4527 b- defN 21-Mar-24 11:11 LabelFusion-1.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 21-Mar-24 11:11 LabelFusion-1.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 21-Mar-24 11:11 LabelFusion-1.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1151 b- defN 21-Mar-24 11:11 LabelFusion-1.0.8.dist-info/RECORD
 14 files, 37974 bytes uncompressed, 11066 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: LabelFusion/utils.py
 Comment: 
 
 Filename: LabelFusion/wrapper.py
 Comment: 
 
-Filename: LabelFusion-1.0.7.data/scripts/fusion_run
+Filename: LabelFusion-1.0.8.data/scripts/fusion_run
 Comment: 
 
-Filename: LabelFusion-1.0.7.dist-info/LICENSE
+Filename: LabelFusion-1.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: LabelFusion-1.0.7.dist-info/METADATA
+Filename: LabelFusion-1.0.8.dist-info/METADATA
 Comment: 
 
-Filename: LabelFusion-1.0.7.dist-info/WHEEL
+Filename: LabelFusion-1.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: LabelFusion-1.0.7.dist-info/top_level.txt
+Filename: LabelFusion-1.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: LabelFusion-1.0.7.dist-info/RECORD
+Filename: LabelFusion-1.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `LabelFusion-1.0.7.data/scripts/fusion_run` & `LabelFusion-1.0.8.data/scripts/fusion_run`

 * *Files identical despite different names*

## Comparing `LabelFusion-1.0.7.dist-info/METADATA` & `LabelFusion-1.0.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LabelFusion
-Version: 1.0.7
+Version: 1.0.8
 Summary: Label fusion strategies for multi-class labels.
 Home-page: https://github.com/FETS-AI/LabelFusion
 Author: Megh Bhalerao, Sarthak Pati
 Author-email: software@cbica.upenn.edu
 License: BSD-3-Clause License
 Keywords: semantic,segmentation,label-fusion,fusion
 Platform: UNKNOWN
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: LabelFusion Version: 1.0.7 Summary: Label fusion
+Metadata-Version: 2.1 Name: LabelFusion Version: 1.0.8 Summary: Label fusion
 strategies for multi-class labels. Home-page: https://github.com/FETS-AI/
 LabelFusion Author: Megh Bhalerao, Sarthak Pati Author-email:
 software@cbica.upenn.edu License: BSD-3-Clause License Keywords:
 semantic,segmentation,label-fusion,fusion Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: BSD License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
```

