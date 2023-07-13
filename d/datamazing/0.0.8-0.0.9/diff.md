# Comparing `tmp/datamazing-0.0.8.tar.gz` & `tmp/datamazing-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamazing-0.0.8.tar", max compression
+gzip compressed data, was "datamazing-0.0.9.tar", max compression
```

## Comparing `datamazing-0.0.8.tar` & `datamazing-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       21 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/__init__.py
--rw-r--r--   0        0        0      295 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pandas/__init__.py
--rw-r--r--   0        0        0      267 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pandas/datacollection/__init__.py
--rw-r--r--   0        0        0      126 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pandas/testing/__init__.py
--rw-r--r--   0        0        0      826 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pandas/testing/assertions.py
--rw-r--r--   0        0        0     3818 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pandas/testing/data.py
--rw-r--r--   0        0        0        0 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pandas/transformations/__init__.py
--rw-r--r--   0        0        0      649 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pandas/transformations/basic.py
--rw-r--r--   0        0        0     2763 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pandas/transformations/grouping.py
--rw-r--r--   0        0        0      868 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pandas/transformations/resampling.py
--rw-r--r--   0        0        0      660 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pandas/types.py
--rw-r--r--   0        0        0      184 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pyspark/__init__.py
--rw-r--r--   0        0        0       92 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pyspark/testing/__init__.py
--rw-r--r--   0        0        0      153 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pyspark/testing/assertions.py
--rw-r--r--   0        0        0     2070 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pyspark/testing/data.py
--rw-r--r--   0        0        0        0 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pyspark/transformations/__init__.py
--rw-r--r--   0        0        0      540 2023-07-11 13:08:32.740400 datamazing-0.0.8/datamazing/pyspark/transformations/grouping.py
--rw-r--r--   0        0        0      708 2023-07-11 13:08:32.740400 datamazing-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 datamazing-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       21 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/__init__.py
+-rw-r--r--   0        0        0      295 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pandas/__init__.py
+-rw-r--r--   0        0        0      267 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pandas/datacollection/__init__.py
+-rw-r--r--   0        0        0      126 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pandas/testing/__init__.py
+-rw-r--r--   0        0        0      826 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pandas/testing/assertions.py
+-rw-r--r--   0        0        0     3818 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pandas/testing/data.py
+-rw-r--r--   0        0        0        0 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pandas/transformations/__init__.py
+-rw-r--r--   0        0        0      649 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pandas/transformations/basic.py
+-rw-r--r--   0        0        0     2781 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pandas/transformations/grouping.py
+-rw-r--r--   0        0        0      868 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pandas/transformations/resampling.py
+-rw-r--r--   0        0        0      660 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pandas/types.py
+-rw-r--r--   0        0        0      184 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pyspark/__init__.py
+-rw-r--r--   0        0        0       92 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pyspark/testing/__init__.py
+-rw-r--r--   0        0        0      153 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pyspark/testing/assertions.py
+-rw-r--r--   0        0        0     2070 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pyspark/testing/data.py
+-rw-r--r--   0        0        0        0 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pyspark/transformations/__init__.py
+-rw-r--r--   0        0        0      540 2023-07-12 07:04:04.108982 datamazing-0.0.9/datamazing/pyspark/transformations/grouping.py
+-rw-r--r--   0        0        0      708 2023-07-12 07:04:04.108982 datamazing-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 datamazing-0.0.9/PKG-INFO
```

### Comparing `datamazing-0.0.8/datamazing/pandas/testing/assertions.py` & `datamazing-0.0.9/datamazing/pandas/testing/assertions.py`

 * *Files identical despite different names*

### Comparing `datamazing-0.0.8/datamazing/pandas/testing/data.py` & `datamazing-0.0.9/datamazing/pandas/testing/data.py`

 * *Files identical despite different names*

### Comparing `datamazing-0.0.8/datamazing/pandas/transformations/basic.py` & `datamazing-0.0.9/datamazing/pandas/transformations/basic.py`

 * *Files identical despite different names*

### Comparing `datamazing-0.0.8/datamazing/pandas/transformations/grouping.py` & `datamazing-0.0.9/datamazing/pandas/transformations/grouping.py`

 * *Files 7% similar despite different names*

```diff
@@ -68,15 +68,15 @@
                 case the values will be inferred from the
                 pivoting column.
         """
 
         df = self.df.set_index(_concat(self.by, on))
 
         if values:
-            by_vals = df.index.to_frame(index=False)[_list(self.by)]
+            by_vals = df.index.to_frame(index=False)[_list(self.by)].drop_duplicates()
             on_vals = pd.DataFrame(values, columns=_list(on))
             cross_vals = by_vals.merge(on_vals, how="cross")
             df = df.reindex(pd.MultiIndex.from_frame(cross_vals))
 
         df = df.unstack(on)
 
         df.columns = df.columns.map(
```

### Comparing `datamazing-0.0.8/datamazing/pandas/transformations/resampling.py` & `datamazing-0.0.9/datamazing/pandas/transformations/resampling.py`

 * *Files identical despite different names*

### Comparing `datamazing-0.0.8/datamazing/pandas/types.py` & `datamazing-0.0.9/datamazing/pandas/types.py`

 * *Files identical despite different names*

### Comparing `datamazing-0.0.8/datamazing/pyspark/testing/data.py` & `datamazing-0.0.9/datamazing/pyspark/testing/data.py`

 * *Files identical despite different names*

### Comparing `datamazing-0.0.8/datamazing/pyspark/transformations/grouping.py` & `datamazing-0.0.9/datamazing/pyspark/transformations/grouping.py`

 * *Files identical despite different names*

### Comparing `datamazing-0.0.8/pyproject.toml` & `datamazing-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datamazing"
-version = "0.0.8"
+version = "0.0.9"
 description = "Package for working with pandas Dataset, but wit specialized functions used for Energinet"
 authors = ["Mikkel Ladekarl Folmersen Nygaard <mny@energinet.dk>", "Ulrik Christensen <uch@energinet.dk>"]
 packages = [
     { include = "datamazing" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `datamazing-0.0.8/PKG-INFO` & `datamazing-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamazing
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package for working with pandas Dataset, but wit specialized functions used for Energinet
 Author: Mikkel Ladekarl Folmersen Nygaard
 Author-email: mny@energinet.dk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

