# Comparing `tmp/omniplate-0.9.92.tar.gz` & `tmp/omniplate-0.9.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniplate-0.9.92.tar", max compression
+gzip compressed data, was "omniplate-0.9.93.tar", max compression
```

## Comparing `omniplate-0.9.92.tar` & `omniplate-0.9.93.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      244 2022-05-26 16:08:15.786293 omniplate-0.9.92/README.md
--rw-r--r--   0        0        0        0 2023-05-15 08:36:42.000000 omniplate-0.9.92/om_code/__init__.py
--rw-r--r--   0        0        0     3383 2023-06-21 10:39:14.000000 omniplate-0.9.92/om_code/admin.py
--rw-r--r--   0        0        0     1289 2023-04-24 14:56:03.000000 omniplate-0.9.92/om_code/clogger.py
--rw-r--r--   0        0        0    24576 2023-06-21 10:49:59.000000 omniplate-0.9.92/om_code/corrections.py
--rw-r--r--   0        0        0     1380 2023-01-30 16:21:38.000000 omniplate-0.9.92/om_code/dilution_data_lucia.tsv
--rw-r--r--   0        0        0     1893 2023-01-30 16:21:38.000000 omniplate-0.9.92/om_code/dilution_data_xiao.tsv
--rw-r--r--   0        0        0     7681 2023-06-10 14:52:08.000000 omniplate-0.9.92/om_code/getfitnesspenalty.py
--rw-r--r--   0        0        0     3470 2023-06-10 16:06:46.000000 omniplate-0.9.92/om_code/loaddata.py
--rw-r--r--   0        0        0     5187 2023-06-10 14:52:08.000000 omniplate-0.9.92/om_code/midlog.py
--rw-r--r--   0        0        0     2577 2023-05-26 11:17:09.000000 omniplate-0.9.92/om_code/old_analyseOldTecan.py
--rw-r--r--   0        0        0     1771 2023-05-26 11:17:09.000000 omniplate-0.9.92/om_code/old_analyseSunrise.py
--rw-r--r--   0        0        0     2609 2023-05-26 11:17:09.000000 omniplate-0.9.92/om_code/old_analyseTecan.py
--rw-r--r--   0        0        0      435 2022-05-26 16:08:15.904220 omniplate-0.9.92/om_code/omerrors.py
--rw-r--r--   0        0        0    11860 2023-06-20 18:31:25.138985 omniplate-0.9.92/om_code/omfitderiv.py
--rw-r--r--   0        0        0     3925 2023-06-10 14:52:08.000000 omniplate-0.9.92/om_code/omgenutils.py
--rw-r--r--   0        0        0    11471 2023-06-20 17:42:50.408709 omniplate-0.9.92/om_code/omplot.py
--rw-r--r--   0        0        0     6794 2023-06-21 13:56:46.000000 omniplate-0.9.92/om_code/omstats.py
--rw-r--r--   0        0        0     4211 2023-06-10 16:06:35.000000 omniplate-0.9.92/om_code/parseplate.py
--rw-r--r--   0        0        0     6068 2023-06-10 14:52:08.000000 omniplate-0.9.92/om_code/runfitderiv.py
--rw-r--r--   0        0        0     4597 2023-06-22 15:26:16.248601 omniplate-0.9.92/om_code/sunder.py
--rw-r--r--   0        0        0    93755 2023-06-22 13:02:45.132194 omniplate-0.9.92/omniplate/Omniplate.py
--rw-r--r--   0        0        0       44 2022-05-26 16:08:15.902667 omniplate-0.9.92/omniplate/__init__.py
--rw-r--r--   0        0        0     1118 2023-06-22 14:16:05.982462 omniplate-0.9.92/pyproject.toml
--rw-r--r--   0        0        0     1501 1970-01-01 00:00:00.000000 omniplate-0.9.92/PKG-INFO
+-rw-r--r--   0        0        0      244 2022-05-26 16:08:15.000000 omniplate-0.9.93/README.md
+-rw-r--r--   0        0        0        0 2023-05-15 08:36:42.000000 omniplate-0.9.93/om_code/__init__.py
+-rw-r--r--   0        0        0     3383 2023-06-21 10:39:14.000000 omniplate-0.9.93/om_code/admin.py
+-rw-r--r--   0        0        0     1289 2023-04-24 14:56:03.000000 omniplate-0.9.93/om_code/clogger.py
+-rw-r--r--   0        0        0    24576 2023-06-21 10:49:59.000000 omniplate-0.9.93/om_code/corrections.py
+-rw-r--r--   0        0        0     1380 2023-01-30 16:21:38.000000 omniplate-0.9.93/om_code/dilution_data_lucia.tsv
+-rw-r--r--   0        0        0     1893 2023-01-30 16:21:38.000000 omniplate-0.9.93/om_code/dilution_data_xiao.tsv
+-rw-r--r--   0        0        0     7681 2023-06-10 14:52:08.000000 omniplate-0.9.93/om_code/getfitnesspenalty.py
+-rw-r--r--   0        0        0     3470 2023-06-10 16:06:46.000000 omniplate-0.9.93/om_code/loaddata.py
+-rw-r--r--   0        0        0     5187 2023-06-10 14:52:08.000000 omniplate-0.9.93/om_code/midlog.py
+-rw-r--r--   0        0        0     2577 2023-05-26 11:17:09.000000 omniplate-0.9.93/om_code/old_analyseOldTecan.py
+-rw-r--r--   0        0        0     1771 2023-05-26 11:17:09.000000 omniplate-0.9.93/om_code/old_analyseSunrise.py
+-rw-r--r--   0        0        0     2609 2023-05-26 11:17:09.000000 omniplate-0.9.93/om_code/old_analyseTecan.py
+-rw-r--r--   0        0        0      435 2022-05-26 16:08:15.000000 omniplate-0.9.93/om_code/omerrors.py
+-rw-r--r--   0        0        0    11860 2023-06-20 18:31:25.000000 omniplate-0.9.93/om_code/omfitderiv.py
+-rw-r--r--   0        0        0     3925 2023-06-10 14:52:08.000000 omniplate-0.9.93/om_code/omgenutils.py
+-rw-r--r--   0        0        0    11471 2023-06-20 17:42:50.000000 omniplate-0.9.93/om_code/omplot.py
+-rw-r--r--   0        0        0     6794 2023-06-21 13:56:46.000000 omniplate-0.9.93/om_code/omstats.py
+-rw-r--r--   0        0        0     4211 2023-06-10 16:06:35.000000 omniplate-0.9.93/om_code/parseplate.py
+-rw-r--r--   0        0        0     6068 2023-06-10 14:52:08.000000 omniplate-0.9.93/om_code/runfitderiv.py
+-rw-r--r--   0        0        0     4607 2023-07-13 15:38:23.276104 omniplate-0.9.93/om_code/sunder.py
+-rw-r--r--   0        0        0    93755 2023-07-13 15:41:59.798123 omniplate-0.9.93/omniplate/Omniplate.py
+-rw-r--r--   0        0        0       44 2022-05-26 16:08:15.000000 omniplate-0.9.93/omniplate/__init__.py
+-rw-r--r--   0        0        0     1118 2023-07-13 15:42:15.648949 omniplate-0.9.93/pyproject.toml
+-rw-r--r--   0        0        0     1501 1970-01-01 00:00:00.000000 omniplate-0.9.93/PKG-INFO
```

### Comparing `omniplate-0.9.92/om_code/admin.py` & `omniplate-0.9.93/om_code/admin.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.92/om_code/clogger.py` & `omniplate-0.9.93/om_code/clogger.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.92/om_code/corrections.py` & `omniplate-0.9.93/om_code/corrections.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.92/om_code/dilution_data_lucia.tsv` & `omniplate-0.9.93/om_code/dilution_data_lucia.tsv`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.92/om_code/dilution_data_xiao.tsv` & `omniplate-0.9.93/om_code/dilution_data_xiao.tsv`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.92/om_code/getfitnesspenalty.py` & `omniplate-0.9.93/om_code/getfitnesspenalty.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.92/om_code/loaddata.py` & `omniplate-0.9.93/om_code/loaddata.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.92/om_code/midlog.py` & `omniplate-0.9.93/om_code/midlog.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.92/om_code/old_analyseOldTecan.py` & `omniplate-0.9.93/om_code/old_analyseOldTecan.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.92/om_code/old_analyseSunrise.py` & `omniplate-0.9.93/om_code/old_analyseSunrise.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.92/om_code/old_analyseTecan.py` & `omniplate-0.9.93/om_code/old_analyseTecan.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.92/om_code/omfitderiv.py` & `omniplate-0.9.93/om_code/omfitderiv.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.92/om_code/omgenutils.py` & `omniplate-0.9.93/om_code/omgenutils.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.92/om_code/omplot.py` & `omniplate-0.9.93/om_code/omplot.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.92/om_code/omstats.py` & `omniplate-0.9.93/om_code/omstats.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.92/om_code/parseplate.py` & `omniplate-0.9.93/om_code/parseplate.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.92/om_code/runfitderiv.py` & `omniplate-0.9.93/om_code/runfitderiv.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.92/om_code/sunder.py` & `omniplate-0.9.93/om_code/sunder.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 
 def getset(
     self,
     label,
     labelincludes,
     labelexcludes,
     labeltype,
-    nomedia,
-    nonull,
+    nomedia=True,
+    nonull=True,
 ):
     """Find user-specified list of experiments, conditions, or strains."""
     all_labels = getall_labels(self, labeltype, nomedia, nonull)
     if label != "all":
         # prioritise explicitly specified labels
         labels = gu.makelist(label)
         # check user's choice exists
```

### Comparing `omniplate-0.9.92/omniplate/Omniplate.py` & `omniplate-0.9.93/omniplate/Omniplate.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import om_code.omgenutils as gu
 import om_code.omplot as omplot
 import om_code.sunder as sunder
 import pandas as pd
 import seaborn as sns
 from om_code.runfitderiv import runfitderiv
 
-version = "0.9.92"
+version = "0.9.93"
 
 plt.rcParams["figure.max_open_warning"] = 0
 sns.set()
 
 
 class platereader:
     """
```

### Comparing `omniplate-0.9.92/pyproject.toml` & `omniplate-0.9.93/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omniplate"
-version = "0.9.92"
+version = "0.9.93"
 description = "For analysing and meta-analysing plate-reader data"
 authors = ["Peter Swain <peter.swain@ed.ac.uk>"]
 
 license = "MIT"
 readme = "README.md"
 homepage = "https://swainlab.bio.ed.ac.uk/software/omniplate"
 repository = "https://git.ecdf.ed.ac.uk/pswain/omniplate"
```

### Comparing `omniplate-0.9.92/PKG-INFO` & `omniplate-0.9.93/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniplate
-Version: 0.9.92
+Version: 0.9.93
 Summary: For analysing and meta-analysing plate-reader data
 Home-page: https://swainlab.bio.ed.ac.uk/software/omniplate
 License: MIT
 Keywords: omniplate,systems biology,bioinformatics,plate readers
 Author: Peter Swain
 Author-email: peter.swain@ed.ac.uk
 Requires-Python: >=3.8,<3.11
```

