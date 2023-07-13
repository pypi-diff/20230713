# Comparing `tmp/trviz-0.1.3.tar.gz` & `tmp/trviz-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trviz-0.1.3.tar", last modified: Mon Mar  6 18:56:06 2023, max compression
+gzip compressed data, was "trviz-1.0.1.tar", last modified: Thu Jul 13 19:03:44 2023, max compression
```

## Comparing `trviz-0.1.3.tar` & `trviz-1.0.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0 jonghun   (1000) jonghun   (1000)        0 2023-03-06 18:56:06.063865 trviz-0.1.3/
--rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)     1799 2022-08-05 22:54:44.000000 trviz-0.1.3/.gitignore
--rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)     1570 2022-08-26 22:12:56.000000 trviz-0.1.3/LICENSE.md
--rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)      131 2022-08-30 20:50:32.000000 trviz-0.1.3/MANIFEST.in
--rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)     2936 2023-03-06 18:56:06.063865 trviz-0.1.3/PKG-INFO
--rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)     2550 2023-03-06 18:55:06.000000 trviz-0.1.3/README.md
-drwxrwxrwx   0 jonghun   (1000) jonghun   (1000)        0 2023-03-06 18:56:05.850865 trviz-0.1.3/examples/
--rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)   213403 2023-02-24 18:24:41.000000 trviz-0.1.3/examples/SORL1_motif_map.png
-drwxrwxrwx   0 jonghun   (1000) jonghun   (1000)        0 2023-03-06 18:56:05.897863 trviz-0.1.3/examples/figures/
--rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)    49050 2022-12-10 00:12:00.000000 trviz-0.1.3/examples/figures/TRviz_main_figure.png
--rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)   403195 2022-09-16 05:13:43.000000 trviz-0.1.3/examples/figures/example_figure1_SORL1.png
--rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)   535112 2022-09-16 05:14:20.000000 trviz-0.1.3/examples/figures/example_figure2_VPS53.png
--rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)   124416 2023-01-04 18:49:31.000000 trviz-0.1.3/examples/test.png
--rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)     5319 2023-03-03 23:32:24.000000 trviz-0.1.3/examples/test_motif_map.png
--rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)      184 2023-01-03 18:41:57.000000 trviz-0.1.3/requirements.txt
--rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)       79 2023-03-06 18:56:06.066865 trviz-0.1.3/setup.cfg
--rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)      823 2023-03-06 18:43:58.000000 trviz-0.1.3/setup.py
-drwxrwxrwx   0 jonghun   (1000) jonghun   (1000)        0 2023-03-06 18:56:05.925864 trviz-0.1.3/tests/
--rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)        0 2022-08-29 21:55:36.000000 trviz-0.1.3/tests/__init__.py
--rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)     8275 2022-10-24 20:10:02.000000 trviz-0.1.3/tests/test_decomposer.py
-drwxrwxrwx   0 jonghun   (1000) jonghun   (1000)        0 2023-03-06 18:56:05.998864 trviz-0.1.3/trviz/
--rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)        0 2022-08-05 23:01:16.000000 trviz-0.1.3/trviz/__init__.py
--rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)    19470 2023-03-03 19:34:24.000000 trviz-0.1.3/trviz/decomposer.py
--rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)     6216 2023-01-18 18:48:06.000000 trviz-0.1.3/trviz/main.py
--rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)     7971 2023-02-16 23:51:01.000000 trviz-0.1.3/trviz/motif_aligner.py
--rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)     7610 2022-12-06 18:48:21.000000 trviz-0.1.3/trviz/motif_encoder.py
--rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)    15350 2023-01-18 18:48:06.000000 trviz-0.1.3/trviz/utils.py
--rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)    17841 2023-03-03 19:32:41.000000 trviz-0.1.3/trviz/visualizer.py
-drwxrwxrwx   0 jonghun   (1000) jonghun   (1000)        0 2023-03-06 18:56:06.052864 trviz-0.1.3/trviz.egg-info/
--rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)     2936 2023-03-06 18:56:05.000000 trviz-0.1.3/trviz.egg-info/PKG-INFO
--rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)      599 2023-03-06 18:56:05.000000 trviz-0.1.3/trviz.egg-info/SOURCES.txt
--rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)        1 2023-03-06 18:56:05.000000 trviz-0.1.3/trviz.egg-info/dependency_links.txt
--rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)       27 2023-03-06 18:56:05.000000 trviz-0.1.3/trviz.egg-info/requires.txt
--rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)       12 2023-03-06 18:56:05.000000 trviz-0.1.3/trviz.egg-info/top_level.txt
+drwxrwxrwx   0 jonghun   (1000) jonghun   (1000)        0 2023-07-13 19:03:44.823768 trviz-1.0.1/
+-rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)     1799 2022-08-05 22:54:44.000000 trviz-1.0.1/.gitignore
+-rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)     1570 2022-08-26 22:12:56.000000 trviz-1.0.1/LICENSE.md
+-rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)      131 2022-08-30 20:50:32.000000 trviz-1.0.1/MANIFEST.in
+-rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)     3191 2023-07-13 19:03:44.823768 trviz-1.0.1/PKG-INFO
+-rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)     2808 2023-07-07 04:38:15.000000 trviz-1.0.1/README.md
+drwxrwxrwx   0 jonghun   (1000) jonghun   (1000)        0 2023-07-13 19:03:44.611768 trviz-1.0.1/examples/
+-rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)   213403 2023-02-24 18:24:41.000000 trviz-1.0.1/examples/SORL1_motif_map.png
+drwxrwxrwx   0 jonghun   (1000) jonghun   (1000)        0 2023-07-13 19:03:44.657767 trviz-1.0.1/examples/figures/
+-rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)    49050 2022-12-10 00:12:00.000000 trviz-1.0.1/examples/figures/TRviz_main_figure.png
+-rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)   403195 2022-09-16 05:13:43.000000 trviz-1.0.1/examples/figures/example_figure1_SORL1.png
+-rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)   535112 2022-09-16 05:14:20.000000 trviz-1.0.1/examples/figures/example_figure2_VPS53.png
+-rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)   124416 2023-01-04 18:49:31.000000 trviz-1.0.1/examples/test.png
+-rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)     5319 2023-03-03 23:32:24.000000 trviz-1.0.1/examples/test_motif_map.png
+-rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)      203 2023-07-07 04:54:28.000000 trviz-1.0.1/requirements.txt
+-rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)       79 2023-07-13 19:03:44.826768 trviz-1.0.1/setup.cfg
+-rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)      823 2023-07-13 19:02:49.000000 trviz-1.0.1/setup.py
+drwxrwxrwx   0 jonghun   (1000) jonghun   (1000)        0 2023-07-13 19:03:44.686769 trviz-1.0.1/tests/
+-rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)        0 2022-08-29 21:55:36.000000 trviz-1.0.1/tests/__init__.py
+-rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)     8275 2022-10-24 20:10:02.000000 trviz-1.0.1/tests/test_decomposer.py
+drwxrwxrwx   0 jonghun   (1000) jonghun   (1000)        0 2023-07-13 19:03:44.761768 trviz-1.0.1/trviz/
+-rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)        0 2022-08-05 23:01:16.000000 trviz-1.0.1/trviz/__init__.py
+-rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)    19470 2023-03-03 19:34:24.000000 trviz-1.0.1/trviz/decomposer.py
+-rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)     8189 2023-07-13 18:52:52.000000 trviz-1.0.1/trviz/main.py
+-rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)     7971 2023-02-16 23:51:01.000000 trviz-1.0.1/trviz/motif_aligner.py
+-rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)     7610 2022-12-06 18:48:21.000000 trviz-1.0.1/trviz/motif_encoder.py
+-rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)    15477 2023-07-07 04:15:03.000000 trviz-1.0.1/trviz/utils.py
+-rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)    19656 2023-07-13 18:52:52.000000 trviz-1.0.1/trviz/visualizer.py
+drwxrwxrwx   0 jonghun   (1000) jonghun   (1000)        0 2023-07-13 19:03:44.812768 trviz-1.0.1/trviz.egg-info/
+-rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)     3191 2023-07-13 19:03:44.000000 trviz-1.0.1/trviz.egg-info/PKG-INFO
+-rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)      599 2023-07-13 19:03:44.000000 trviz-1.0.1/trviz.egg-info/SOURCES.txt
+-rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)        1 2023-07-13 19:03:44.000000 trviz-1.0.1/trviz.egg-info/dependency_links.txt
+-rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)       27 2023-07-13 19:03:44.000000 trviz-1.0.1/trviz.egg-info/requires.txt
+-rwxrwxrwx   0 jonghun   (1000) jonghun   (1000)       12 2023-07-13 19:03:44.000000 trviz-1.0.1/trviz.egg-info/top_level.txt
```

### Comparing `trviz-0.1.3/.gitignore` & `trviz-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `trviz-0.1.3/LICENSE.md` & `trviz-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `trviz-0.1.3/PKG-INFO` & `trviz-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trviz
-Version: 0.1.3
+Version: 1.0.1
 Summary: A python library for decomposing and visualizing tandem repeat sequences
 Home-page: https://github.com/Jong-hun-Park/trviz
 Author: Jonghun Park
 Author-email: jop002@eng.ucsd.edu
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -93,9 +93,12 @@
 tr_decomposer = Decomposer()
 tr_sequence = "ACCTTGACCTTGACCTTGACCTTG"
 motifs = ["ACCTTG"]
 tr_decomposer.decompose(tr_sequence, motifs)
 # >>> ["ACCTTG", "ACCTTG", "ACCTTG", "ACCTTG"]
 ``` 
 
+## Citation:
+Jonghun Park, Eli Kaufman, Paul N Valdmanis, Vineet Bafna, [TRviz: a Python library for decomposing and visualizing tandem repeat sequences](https://doi.org/10.1093/bioadv/vbad058), Bioinformatics Advances, Volume 3, Issue 1, 2023, vbad058 
+
 # Contact Us
 Please submit an issue on the [TRviz github](https://github.com/Jong-hun-Park/trviz/issues)
```

### Comparing `trviz-0.1.3/README.md` & `trviz-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -146,15 +146,31 @@
 00000910: 6d6f 7469 6673 203d 205b 2241 4343 5454  motifs = ["ACCTT
 00000920: 4722 5d0d 0a74 725f 6465 636f 6d70 6f73  G"]..tr_decompos
 00000930: 6572 2e64 6563 6f6d 706f 7365 2874 725f  er.decompose(tr_
 00000940: 7365 7175 656e 6365 2c20 6d6f 7469 6673  sequence, motifs
 00000950: 290d 0a23 203e 3e3e 205b 2241 4343 5454  )..# >>> ["ACCTT
 00000960: 4722 2c20 2241 4343 5454 4722 2c20 2241  G", "ACCTTG", "A
 00000970: 4343 5454 4722 2c20 2241 4343 5454 4722  CCTTG", "ACCTTG"
-00000980: 5d0d 0a60 6060 200d 0a0d 0a23 2043 6f6e  ]..``` ....# Con
-00000990: 7461 6374 2055 730d 0a50 6c65 6173 6520  tact Us..Please 
-000009a0: 7375 626d 6974 2061 6e20 6973 7375 6520  submit an issue 
-000009b0: 6f6e 2074 6865 205b 5452 7669 7a20 6769  on the [TRviz gi
-000009c0: 7468 7562 5d28 6874 7470 733a 2f2f 6769  thub](https://gi
-000009d0: 7468 7562 2e63 6f6d 2f4a 6f6e 672d 6875  thub.com/Jong-hu
-000009e0: 6e2d 5061 726b 2f74 7276 697a 2f69 7373  n-Park/trviz/iss
-000009f0: 7565 7329 0d0a                           ues)..
+00000980: 5d0d 0a60 6060 200d 0a0d 0a23 2320 4369  ]..``` ....## Ci
+00000990: 7461 7469 6f6e 3a0d 0a4a 6f6e 6768 756e  tation:..Jonghun
+000009a0: 2050 6172 6b2c 2045 6c69 204b 6175 666d   Park, Eli Kaufm
+000009b0: 616e 2c20 5061 756c 204e 2056 616c 646d  an, Paul N Valdm
+000009c0: 616e 6973 2c20 5669 6e65 6574 2042 6166  anis, Vineet Baf
+000009d0: 6e61 2c20 5b54 5276 697a 3a20 6120 5079  na, [TRviz: a Py
+000009e0: 7468 6f6e 206c 6962 7261 7279 2066 6f72  thon library for
+000009f0: 2064 6563 6f6d 706f 7369 6e67 2061 6e64   decomposing and
+00000a00: 2076 6973 7561 6c69 7a69 6e67 2074 616e   visualizing tan
+00000a10: 6465 6d20 7265 7065 6174 2073 6571 7565  dem repeat seque
+00000a20: 6e63 6573 5d28 6874 7470 733a 2f2f 646f  nces](https://do
+00000a30: 692e 6f72 672f 3130 2e31 3039 332f 6269  i.org/10.1093/bi
+00000a40: 6f61 6476 2f76 6261 6430 3538 292c 2042  oadv/vbad058), B
+00000a50: 696f 696e 666f 726d 6174 6963 7320 4164  ioinformatics Ad
+00000a60: 7661 6e63 6573 2c20 566f 6c75 6d65 2033  vances, Volume 3
+00000a70: 2c20 4973 7375 6520 312c 2032 3032 332c  , Issue 1, 2023,
+00000a80: 2076 6261 6430 3538 200d 0a0d 0a23 2043   vbad058 ....# C
+00000a90: 6f6e 7461 6374 2055 730d 0a50 6c65 6173  ontact Us..Pleas
+00000aa0: 6520 7375 626d 6974 2061 6e20 6973 7375  e submit an issu
+00000ab0: 6520 6f6e 2074 6865 205b 5452 7669 7a20  e on the [TRviz 
+00000ac0: 6769 7468 7562 5d28 6874 7470 733a 2f2f  github](https://
+00000ad0: 6769 7468 7562 2e63 6f6d 2f4a 6f6e 672d  github.com/Jong-
+00000ae0: 6875 6e2d 5061 726b 2f74 7276 697a 2f69  hun-Park/trviz/i
+00000af0: 7373 7565 7329 0d0a                      ssues)..
```

### Comparing `trviz-0.1.3/examples/SORL1_motif_map.png` & `trviz-1.0.1/examples/SORL1_motif_map.png`

 * *Files identical despite different names*

### Comparing `trviz-0.1.3/examples/figures/TRviz_main_figure.png` & `trviz-1.0.1/examples/figures/TRviz_main_figure.png`

 * *Files identical despite different names*

### Comparing `trviz-0.1.3/examples/figures/example_figure1_SORL1.png` & `trviz-1.0.1/examples/figures/example_figure1_SORL1.png`

 * *Files identical despite different names*

### Comparing `trviz-0.1.3/examples/figures/example_figure2_VPS53.png` & `trviz-1.0.1/examples/figures/example_figure2_VPS53.png`

 * *Files identical despite different names*

### Comparing `trviz-0.1.3/examples/test.png` & `trviz-1.0.1/examples/test.png`

 * *Files identical despite different names*

### Comparing `trviz-0.1.3/examples/test_motif_map.png` & `trviz-1.0.1/examples/test_motif_map.png`

 * *Files identical despite different names*

### Comparing `trviz-0.1.3/tests/test_decomposer.py` & `trviz-1.0.1/tests/test_decomposer.py`

 * *Files identical despite different names*

### Comparing `trviz-0.1.3/trviz/decomposer.py` & `trviz-1.0.1/trviz/decomposer.py`

 * *Files identical despite different names*

### Comparing `trviz-0.1.3/trviz/motif_aligner.py` & `trviz-1.0.1/trviz/motif_aligner.py`

 * *Files identical despite different names*

### Comparing `trviz-0.1.3/trviz/motif_encoder.py` & `trviz-1.0.1/trviz/motif_encoder.py`

 * *Files identical despite different names*

### Comparing `trviz-0.1.3/trviz/utils.py` & `trviz-1.0.1/trviz/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,21 +89,23 @@
         if sample_id in sample_ids:
             sorted_sample_ids.append(sample_id)
             sorted_aligned_vntrs.append(aligned_vntrs[sample_ids.index(sample_id)])
 
     return sorted_sample_ids, sorted_aligned_vntrs
 
 
-def sort(aligned_vntrs, sample_ids, symbol_to_motif, sample_order_file, method='lexicographically'):
+def sort(aligned_vntrs, sample_ids, symbol_to_motif, sample_order_file, method='motif_count'):
     """ Sort the aligned and encoded tandem repeats """
-    if method == 'lexicographically':
+    if method == 'name':
         return zip(*sorted(list(zip(sample_ids, aligned_vntrs)), key=lambda x: x[0]))
-    if method == 'simulated_annealing':
+    elif method == 'motif_count':
+        return zip(*sorted(list(zip(sample_ids, aligned_vntrs)), key=lambda x: len(x[1].replace('-', ''))))
+    elif method == 'simulated_annealing':
         return sort_by_simulated_annealing_optimized(aligned_vntrs, sample_ids, symbol_to_motif)
-    if method == 'manually':
+    elif method == 'manually':
         return sort_by_manually(aligned_vntrs, sample_ids, sample_order_file)
     else:
         raise ValueError("Please check the rearrangement method. {}".format(method))
 
 
 def get_levenshtein_distance(s1, s2):
     """
```

### Comparing `trviz-0.1.3/trviz/visualizer.py` & `trviz-1.0.1/trviz/visualizer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from typing import List, Tuple, Dict
-import re
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.colors import ListedColormap
 
 from trviz.utils import PRIVATE_MOTIF_LABEL
 
 
@@ -51,15 +50,15 @@
             raise ValueError("Symbol to color is not set.")
 
         if figure_size is not None:
             fig, ax = plt.subplots(figsize=figure_size)
         else:
             max_motif_length = len(max(symbol_to_motif.values(), key=len))
             w = len(symbol_to_motif) // 10 + 5 if len(symbol_to_motif) > 50 else len(symbol_to_motif) // 5 + 1
-            h = max_motif_length // 10 + max_motif_length if max_motif_length > 50 else max_motif_length // 5 + 1
+            h = max_motif_length // 4 + 1 if max_motif_length > 50 else max_motif_length // 3 + 1
             if h * dpi > 2 ** 16:
                 h = 2 ** 15 // dpi * 0.75  # "Weight and Height must be less than 2^16"
             fig, ax = plt.subplots(figsize=(w, h))
         ax.set_aspect('equal')
 
         max_motif_length = len(max(symbol_to_motif.values(), key=len))
         # TODO: sort by the frequency
@@ -109,88 +108,102 @@
             length=0)  # labels along the bottom edge are on
 
         # Hide xticks
         ax.set_xticks([])
 
         # No frame
         ax.set_frame_on(False)
-        # ax.spines['top'].set_visible(False)
-        # ax.spines['right'].set_visible(False)
-        # ax.spines['bottom'].set_visible(False)
-        # ax.spines['left'].set_visible(False)
 
         fig.tight_layout()
         fig.savefig(file_name, dpi=dpi, bbox_inches='tight', pad_inches=0)
         plt.close(fig)
 
     def trplot(self,
                aligned_labeled_repeats: List[str],
                sample_ids: List[str],
                figure_size: Tuple[int, int] = None,
                output_name: str = None,
-               dpi: int = 500,
+               dpi: int = 300,
                alpha: float = 0.6,
                box_line_width: float = 0,
-               xtick_degrees: int = 90,
                hide_xticks: bool = False,
                hide_yticks: bool = False,
-               symbol_to_motif: Dict = None,
+               symbol_to_motif: Dict[str, str] = None,
                sort_by_clustering: bool = True,
-               hide_dendrogram: bool = False,
-               population_data = None,
-               sample_as_row = False,
-               xlable_size = 8,
-               ylable_size = 8,
+               hide_dendrogram: bool = True,
+               population_data: str = None,
+               motif_marks: Dict[str, str] = None,
+               allele_as_row: bool = True,
+               xlabel_size: int = 8,
+               ylabel_size: int = 8,
+               xlabel_rotation: int = 0,
+               ylabel_rotation: int = 0,
                private_motif_color: str = 'black',
-               frame_on = {'top': False, 'bottom': True, 'right': False, 'left': True},
+               frame_on: Dict[str, bool] = None,
                debug: bool = False
                ):
         """
         Generate a plot showing the variations in tandem repeat sequences.
         A distinct color is assigned to each motif.
         For private motifs (with low frequency), the same color (in black by default) may be assigned.
 
         :param aligned_labeled_repeats: aligned and encoded tandem repeat sequences.
         :param sample_ids: sample IDs
         :param figure_size: figure size
         :param output_name: output file name
         :param dpi: DPI for the plot
         :param alpha: alpha value for the plot
         :param box_line_width: line width for box edges
-        :param xtick_degrees: xtick degree (default is 90)
         :param hide_xticks: if true, hide xticks
         :param hide_yticks: if true, hide yticks
+        :param symbol_to_motif: a dictionary mapping symbols to motifs
+        :param sort_by_clustering: if true, sort the samples by clustering
+        :param hide_dendrogram: if true, hide the dendrogram
+        :param population_data: population data file name
+        :param motif_marks: a dictionary mapping sample to motif marks
+        :param allele_as_row: if true, plot allele as row (default is true)
+        :param xlabel_size: x label size (default is 8)
+        :param ylabel_size: y label size (default is 8)
+        :param xlabel_rotation: x label rotation (default is 0)
+        :param ylabel_rotation: y label rotation (default is 0)
         :param private_motif_color: the color for private motifs. Default is black
-        :param debug: if true, print verbse information.
+        :param frame_on: a dictionary mapping sample to frame on.
+                         Default is {'top': False, 'bottom': True, 'right': False, 'left': True}
+        :param debug: if true, print verbose information.
         """
 
-        fig, ax_main = plt.subplots(figsize=figure_size)  # width and height in inch
+        if motif_marks is not None:
+            if len(motif_marks) != len(sample_ids):
+                raise ValueError("The length of motif_marks must be the same as the number of samples")
 
+        fig, ax_main = plt.subplots(figsize=figure_size)  # width and height in inch
         max_repeat_count = len(aligned_labeled_repeats[0])
         if figure_size is None:
-            w = len(sample_ids) // 10 + 5 if len(sample_ids) > 50 else 5
-            h = max_repeat_count // 10 + max_repeat_count if max_repeat_count > 50 else max_repeat_count // 5 + 2
+            if allele_as_row:
+                h = len(sample_ids) // 5 + 2 if len(sample_ids) > 50 else 5
+                w = max_repeat_count // 5 + 2 if max_repeat_count > 50 else max_repeat_count // 5 + 2
+            else:
+                w = len(sample_ids) // 5 + 2 if len(sample_ids) > 50 else 5
+                h = max_repeat_count // 5 + 2 if max_repeat_count > 50 else max_repeat_count // 5 + 2
             if h * dpi > 2**16:
                 h = 2**15 // dpi * 0.75  # "Weight and Height must be less than 2^16"
             fig, ax_main = plt.subplots(figsize=(w, h))
 
         # Add clustering
         if sort_by_clustering:
             if symbol_to_motif is None:
                 raise ValueError("symbol_to_motif must be provided when sort_by_clustering is True")
-
             sorted_sample_ids, sorted_aligned_labeled_repeats = self.add_dendrogram(fig,
                                                                                     aligned_labeled_repeats,
                                                                                     sample_ids,
                                                                                     symbol_to_motif,
                                                                                     hide_dendrogram)
             if debug:
                 print("Sort by clustering")
                 print('\n'.join(sorted_sample_ids))
-
         else:
             # Already sorted in some way
             sorted_sample_ids, sorted_aligned_labeled_repeats = sample_ids, aligned_labeled_repeats
             if debug:
                 print("No clustering")
 
         # Set symbol to color map
@@ -198,29 +211,48 @@
         unique_label_count = len(unique_labels)
         symbol_to_color = self.get_symbol_to_color_map(alpha, unique_label_count, unique_labels)
         self.set_symbol_to_color_map(symbol_to_color)
 
         box_height = 1.0
         box_width = 1.0
         for allele_index, allele in enumerate(sorted_aligned_labeled_repeats):
-            box_position = [allele_index, 0]
+            motif_index = 0
+            if allele_as_row:
+                box_position = [allele_index, len(sorted_aligned_labeled_repeats) - allele_index - 1]
+            else:  # each column is an allele
+                box_position = [allele_index, 0]
+
             for box_index, symbol in enumerate(allele):
-                box_position[1] = box_height * box_index
+                if allele_as_row:
+                    box_position[0] = box_width * box_index  # move x position
+                else:
+                    box_position[1] = box_height * box_index
                 fcolor = symbol_to_color[symbol]
+                hatch_pattern = None
+
                 if symbol == '-':  # For gaps, color them as white blocks
                     fcolor = (1, 1, 1, 1)
+                else:  # Not a gap
+                    if motif_marks is not None:
+                        motif_mark = motif_marks[sorted_sample_ids[allele_index]][motif_index]
+                        if motif_mark == 'I':  # introns
+                            hatch_pattern = 'xxx'
+                    motif_index += 1
+
                 if symbol == PRIVATE_MOTIF_LABEL:
                     fcolor = private_motif_color
                 ax_main.add_patch(plt.Rectangle(box_position, box_width, box_height,
-                                           linewidth=box_line_width + 0.1,
-                                           facecolor=fcolor,
-                                           edgecolor="white"))
+                                                linewidth=box_line_width + 0.1,
+                                                facecolor=fcolor,
+                                                edgecolor="white",
+                                                hatch=hatch_pattern, ))
 
         # population_data = "../../HPRC_metadata/sample_metadata.tsv"
         if population_data is not None:
+            # TODO: need to be fixed when allele_as_row is True (the below works only for allele as column)
             ax_bottom = fig.add_axes([0.125, 0.07, 0.775, 0.03])  # xmin, ymin, dx, dy
             box_height = 1.0
             box_width = 1.0
             population_color_map = self.get_population_colormap(population_data)
             for allele_index, allele in enumerate(sorted_aligned_labeled_repeats):
                 sample_id = sorted_sample_ids[allele_index]
                 if sample_id.find('-') != -1:
@@ -237,54 +269,54 @@
             ax_bottom.set_xticklabels(sorted_sample_ids, ha='center', rotation=xtick_degrees)
             ax_bottom.set_yticks([])
             ax_bottom.set_frame_on(False)
             # ax_bottom.tick_params(axis='x', which='both', length=0)  # if don't want the ticks
 
             ax_main.set_xlim(right=len(sorted_aligned_labeled_repeats))
             ax_main.set_xticks([])
+
+        if allele_as_row:
+            ax_main.set_ylim(top=len(sorted_aligned_labeled_repeats))
+            ax_main.set_yticks([x + 0.5 for x in range(len(aligned_labeled_repeats))])
+            ax_main.set_yticklabels(sorted_sample_ids[::-1], ha='right', rotation=ylabel_rotation)
+
+            labels = [x for x in range(1, max_repeat_count + 1)]
+            ax_main.set_xticks(labels, labels, rotation=xlabel_rotation)
         else:
             ax_main.set_xlim(right=len(sorted_aligned_labeled_repeats))
             ax_main.set_xticks([x + 0.5 for x in range(len(aligned_labeled_repeats))])
-            ax_main.set_xticklabels(sorted_sample_ids, ha='center', rotation=xtick_degrees)
+            ax_main.set_xticklabels(sorted_sample_ids, ha='center', rotation=xlabel_rotation)
 
-        ax_main.set_yticks([y for y in range(1, max_repeat_count + 1)])
-        sample_as_row = True
-        if sample_as_row:
-            # y-tick right and rotate
-            ax_main.set_yticklabels(([y for y in range(1, max_repeat_count + 1)]), rotation=90, ha='center')
-            ax_main.yaxis.tick_right()
-            frame_on['right'] = True
-            frame_on['left'] = False
-        else:
-            ax_main.set_yticklabels(([y for y in range(1, max_repeat_count + 1)]))
+            labels = [y for y in range(1, max_repeat_count + 1)]
+            ax_main.set_yticks(labels, labels=labels, rotation=ylabel_rotation)
 
-        ax_main.tick_params(axis='y', which='major', pad=6.5)
-        # ax_main.tick_params(axis='both', which='major', labelsize=8)
-        ax_main.tick_params(axis='y', which='major', labelsize=ylable_size)
-        ax_main.tick_params(axis='y', which='minor', labelsize=ylable_size)
-        # ax_main.tick_params(axis='x', which='major', labelsize=xlabel_size)
-        # ax_main.tick_params(axis='x', which='minor', labelsize=xlabel_size)
+        ax_main.tick_params(axis='y', which='major', labelsize=ylabel_size)
+        ax_main.tick_params(axis='y', which='minor', labelsize=ylabel_size)
+        ax_main.tick_params(axis='x', which='major', labelsize=xlabel_size)
+        ax_main.tick_params(axis='x', which='minor', labelsize=xlabel_size)
 
         if hide_xticks:
             ax_main.set_xticks([])
         if hide_yticks:
             ax_main.set_yticks([])
 
         # Frame
+        if frame_on is None:  # Set default
+            frame_on = {'top': False, 'bottom': True, 'right': False, 'left': True}
+
         ax_main.spines['top'].set_visible(frame_on['top'])
         ax_main.spines['right'].set_visible(frame_on['right'])
         ax_main.spines['bottom'].set_visible(frame_on['bottom'])
         ax_main.spines['left'].set_visible(frame_on['left'])
 
         if output_name is not None:
-            # fig.set_size_inches(w, h)  # Because the figure size is changed after adding axes
-            # if re.match(".*", tweet):
-            #     fig.savefig(f"{output_name}", dpi=dpi, bbox_inches='tight')
-            # else:
-            fig.savefig(f"{output_name}.pdf", dpi=800, bbox_inches='tight')
+            if '.' not in output_name:
+                fig.savefig(f"{output_name}.pdf", dpi=dpi, bbox_inches='tight')
+            else:
+                fig.savefig(f"{output_name}", dpi=dpi, bbox_inches='tight')
         else:
             fig.savefig("test_trplot.png", dpi=dpi, bbox_inches='tight')
 
         plt.close(fig)
 
     def add_dendrogram(self, fig, aligned_labeled_repeats, sample_ids, symbol_to_motif, hide_clustering):
         """
@@ -349,20 +381,17 @@
                                    (0.337, 0.706, 0.914),
                                    (0, 0.620, 0.451),
                                    (0.941, 0.894, 0.259),
                                    (0, 0.447, 0.698),
                                    (0.835, 0.369, 0),
                                    (0.8, 0.475, 0.655)])
         else:
-            cmap = plt.cm.get_cmap('hsv', unique_symbol_count + 1)
-            # Setting alpha values
-            temp_cmap = cmap(np.arange(cmap.N))
-            temp_cmap[:, -1] = alpha
-            # Update color map
-            cmap = ListedColormap(temp_cmap)
+            import distinctipy
+            cmap = distinctipy.get_colors(unique_symbol_count, pastel_factor=0.9, rng=777)
+            cmap = ListedColormap(cmap)
 
         symbol_to_color = {r: cmap(i) for i, r in enumerate(list(unique_symbols))}
         return symbol_to_color
 
     def set_symbol_to_color_map(self, symbol_to_color):
         self.symbol_to_color = symbol_to_color
```

### Comparing `trviz-0.1.3/trviz.egg-info/PKG-INFO` & `trviz-1.0.1/trviz.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trviz
-Version: 0.1.3
+Version: 1.0.1
 Summary: A python library for decomposing and visualizing tandem repeat sequences
 Home-page: https://github.com/Jong-hun-Park/trviz
 Author: Jonghun Park
 Author-email: jop002@eng.ucsd.edu
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -93,9 +93,12 @@
 tr_decomposer = Decomposer()
 tr_sequence = "ACCTTGACCTTGACCTTGACCTTG"
 motifs = ["ACCTTG"]
 tr_decomposer.decompose(tr_sequence, motifs)
 # >>> ["ACCTTG", "ACCTTG", "ACCTTG", "ACCTTG"]
 ``` 
 
+## Citation:
+Jonghun Park, Eli Kaufman, Paul N Valdmanis, Vineet Bafna, [TRviz: a Python library for decomposing and visualizing tandem repeat sequences](https://doi.org/10.1093/bioadv/vbad058), Bioinformatics Advances, Volume 3, Issue 1, 2023, vbad058 
+
 # Contact Us
 Please submit an issue on the [TRviz github](https://github.com/Jong-hun-Park/trviz/issues)
```

### Comparing `trviz-0.1.3/trviz.egg-info/SOURCES.txt` & `trviz-1.0.1/trviz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

