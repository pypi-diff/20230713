# Comparing `tmp/scutls-0.3.1.tar.gz` & `tmp/scutls-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scutls-0.3.1.tar", max compression
+gzip compressed data, was "scutls-0.3.2.tar", max compression
```

## Comparing `scutls-0.3.1.tar` & `scutls-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      601 2023-07-12 18:14:59.152132 scutls-0.3.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-12 18:15:20.548026 scutls-0.3.1/scutls/__init__.py
--rw-r--r--   0        0        0     7560 2023-07-12 14:28:04.640198 scutls-0.3.1/scutls/arguments.py
--rw-r--r--   0        0        0   214034 2022-07-12 15:06:20.917130 scutls-0.3.1/scutls/assets/genome_ensembl_107_54_54_54.json
--rw-r--r--   0        0        0     1014 2022-07-12 14:34:04.505244 scutls-0.3.1/scutls/assets/genome_ensembl_release_all.txt
--rw-r--r--   0        0        0       50 2022-07-12 18:12:25.707935 scutls-0.3.1/scutls/assets/genome_ensembl_release_use.txt
--rw-r--r--   0        0        0    41218 2022-06-20 13:34:43.299412 scutls-0.3.1/scutls/assets/genome_ucsc.json
--rw-r--r--   0        0        0     2269 2023-07-08 04:35:05.254780 scutls-0.3.1/scutls/bam.py
--rw-r--r--   0        0        0     5820 2023-06-21 04:19:39.366335 scutls-0.3.1/scutls/barcode.py
--rw-r--r--   0        0        0     1381 2023-07-08 04:30:45.312955 scutls-0.3.1/scutls/cli.py
--rw-r--r--   0        0        0     7682 2023-05-08 14:35:07.521838 scutls-0.3.1/scutls/download.py
--rw-r--r--   0        0        0     4984 2023-06-29 04:31:23.564846 scutls-0.3.1/scutls/fastq.py
--rw-r--r--   0        0        0    14108 2023-07-12 18:14:00.283583 scutls-0.3.1/scutls/util.py
--rw-r--r--   0        0        0      946 1970-01-01 00:00:00.000000 scutls-0.3.1/setup.py
--rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 scutls-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      601 2023-07-13 03:56:30.293056 scutls-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-13 04:04:57.949309 scutls-0.3.2/scutls/__init__.py
+-rw-r--r--   0        0        0     7560 2023-07-12 14:28:04.640198 scutls-0.3.2/scutls/arguments.py
+-rw-r--r--   0        0        0   214034 2022-07-12 15:06:20.917130 scutls-0.3.2/scutls/assets/genome_ensembl_107_54_54_54.json
+-rw-r--r--   0        0        0     1014 2022-07-12 14:34:04.505244 scutls-0.3.2/scutls/assets/genome_ensembl_release_all.txt
+-rw-r--r--   0        0        0       50 2022-07-12 18:12:25.707935 scutls-0.3.2/scutls/assets/genome_ensembl_release_use.txt
+-rw-r--r--   0        0        0    41218 2022-06-20 13:34:43.299412 scutls-0.3.2/scutls/assets/genome_ucsc.json
+-rw-r--r--   0        0        0     2269 2023-07-08 04:35:05.254780 scutls-0.3.2/scutls/bam.py
+-rw-r--r--   0        0        0     5820 2023-06-21 04:19:39.366335 scutls-0.3.2/scutls/barcode.py
+-rw-r--r--   0        0        0     1381 2023-07-08 04:30:45.312955 scutls-0.3.2/scutls/cli.py
+-rw-r--r--   0        0        0     7682 2023-05-08 14:35:07.521838 scutls-0.3.2/scutls/download.py
+-rw-r--r--   0        0        0     4984 2023-06-29 04:31:23.564846 scutls-0.3.2/scutls/fastq.py
+-rw-r--r--   0        0        0    14186 2023-07-13 03:48:31.653526 scutls-0.3.2/scutls/util.py
+-rw-r--r--   0        0        0      946 1970-01-01 00:00:00.000000 scutls-0.3.2/setup.py
+-rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 scutls-0.3.2/PKG-INFO
```

### Comparing `scutls-0.3.1/pyproject.toml` & `scutls-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scutls"
-version = "0.3.1"
+version = "0.3.2"
 description = "Single-cell data processing utility tools"
 authors = ["Kai Hu <kai.hu@umassmed.edu>"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 importlib-resources = "^5.8.0"
 wget = "^3.2"
```

### Comparing `scutls-0.3.1/scutls/arguments.py` & `scutls-0.3.2/scutls/arguments.py`

 * *Files identical despite different names*

### Comparing `scutls-0.3.1/scutls/assets/genome_ensembl_107_54_54_54.json` & `scutls-0.3.2/scutls/assets/genome_ensembl_107_54_54_54.json`

 * *Files identical despite different names*

### Comparing `scutls-0.3.1/scutls/assets/genome_ensembl_release_all.txt` & `scutls-0.3.2/scutls/assets/genome_ensembl_release_all.txt`

 * *Files identical despite different names*

### Comparing `scutls-0.3.1/scutls/assets/genome_ucsc.json` & `scutls-0.3.2/scutls/assets/genome_ucsc.json`

 * *Files identical despite different names*

### Comparing `scutls-0.3.1/scutls/bam.py` & `scutls-0.3.2/scutls/bam.py`

 * *Files identical despite different names*

### Comparing `scutls-0.3.1/scutls/barcode.py` & `scutls-0.3.2/scutls/barcode.py`

 * *Files identical despite different names*

### Comparing `scutls-0.3.1/scutls/cli.py` & `scutls-0.3.2/scutls/cli.py`

 * *Files identical despite different names*

### Comparing `scutls-0.3.1/scutls/download.py` & `scutls-0.3.2/scutls/download.py`

 * *Files identical despite different names*

### Comparing `scutls-0.3.1/scutls/fastq.py` & `scutls-0.3.2/scutls/fastq.py`

 * *Files identical despite different names*

### Comparing `scutls-0.3.1/scutls/util.py` & `scutls-0.3.2/scutls/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,20 +320,21 @@
                 if alignment.reference_start > ref_coordinate:
                     # alignment does not span ref_pos
                     res.append(alignment.query_name + ",NA")
                 elif alignment.reference_start == ref_coordinate:
                     res.append(alignment.query_name + "," + str(alignment.query_alignment_start))
                 else:
                     ref_pos  = alignment.reference_start
-                    read_pos = alignment.query_alignment_start
+                    # read_pos = alignment.query_alignment_start # soft clip also consume query, will double count if set like this
+                    read_pos = 0
                     for i, v in enumerate(alignment.cigartuples):
                         query_consume, ref_consume = cigar_consume(v)
                         ref_pos_tem = ref_pos + ref_consume 
                         read_pos_tem = read_pos + query_consume
-                        
+
                         if ref_pos_tem < ref_coordinate:
                             ref_pos = ref_pos_tem
                             read_pos = read_pos_tem
                         elif ref_pos_tem >= ref_coordinate:
                             if read_pos == read_pos_tem:
                                 res.append(alignment.query_name + "," + str(read_pos))
                                 break
```

### Comparing `scutls-0.3.1/setup.py` & `scutls-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'wget>=3.2,<4.0']
 
 entry_points = \
 {'console_scripts': ['scutls = scutls.arguments:main']}
 
 setup_kwargs = {
     'name': 'scutls',
-    'version': '0.3.1',
+    'version': '0.3.2',
     'description': 'Single-cell data processing utility tools',
     'long_description': 'None',
     'author': 'Kai Hu',
     'author_email': 'kai.hu@umassmed.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `scutls-0.3.1/PKG-INFO` & `scutls-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scutls
-Version: 0.3.1
+Version: 0.3.2
 Summary: Single-cell data processing utility tools
 Author: Kai Hu
 Author-email: kai.hu@umassmed.edu
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

