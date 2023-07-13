# Comparing `tmp/coolpandas-0.4.0.tar.gz` & `tmp/coolpandas-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolpandas-0.4.0.tar", last modified: Wed May 31 23:26:25 2023, max compression
+gzip compressed data, was "coolpandas-0.4.1.tar", last modified: Thu Jul 13 09:35:41 2023, max compression
```

## Comparing `coolpandas-0.4.0.tar` & `coolpandas-0.4.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:26:25.188072 coolpandas-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-31 23:26:16.000000 coolpandas-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-31 23:26:25.188072 coolpandas-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-31 23:26:16.000000 coolpandas-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:26:25.180071 coolpandas-0.4.0/coolpandas/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:26:25.184071 coolpandas-0.4.0/coolpandas/connect/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/connect/redshift.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:26:25.184071 coolpandas-0.4.0/coolpandas/eda/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/eda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/eda/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/eda/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/eda/duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/eda/features_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/eda/geo_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/eda/missing_values.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/eda/random_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/eda/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/eda/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/eda/value_counts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:26:25.184071 coolpandas-0.4.0/coolpandas/evaluate/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/evaluate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/evaluate/confusion_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:26:25.188072 coolpandas-0.4.0/coolpandas/plot/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/plot/barplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/plot/boxplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/plot/distplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/plot/geoplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/plot/lineplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/plot/mapplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/plot/style.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:26:25.188072 coolpandas-0.4.0/coolpandas/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/stats/effect.py
--rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/stats/ttest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:26:25.188072 coolpandas-0.4.0/coolpandas/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/transform/bin.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/transform/epoch.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/transform/missing_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/transform/outliers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:26:25.188072 coolpandas-0.4.0/coolpandas/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-31 23:26:16.000000 coolpandas-0.4.0/coolpandas/utils/random_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:26:25.184071 coolpandas-0.4.0/coolpandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-31 23:26:25.000000 coolpandas-0.4.0/coolpandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-31 23:26:25.000000 coolpandas-0.4.0/coolpandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 23:26:25.000000 coolpandas-0.4.0/coolpandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-31 23:26:25.000000 coolpandas-0.4.0/coolpandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 23:26:25.000000 coolpandas-0.4.0/coolpandas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-31 23:26:16.000000 coolpandas-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 23:26:25.188072 coolpandas-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:35:41.181844 coolpandas-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-13 09:35:20.000000 coolpandas-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-13 09:35:41.181844 coolpandas-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-13 09:35:20.000000 coolpandas-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:35:41.177844 coolpandas-0.4.1/coolpandas/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:35:41.177844 coolpandas-0.4.1/coolpandas/connect/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/connect/redshift.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:35:41.177844 coolpandas-0.4.1/coolpandas/eda/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/eda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/eda/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/eda/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/eda/duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/eda/features_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/eda/geo_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/eda/missing_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/eda/random_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/eda/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/eda/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/eda/value_counts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:35:41.177844 coolpandas-0.4.1/coolpandas/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/evaluate/confusion_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:35:41.177844 coolpandas-0.4.1/coolpandas/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/plot/barplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/plot/boxplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/plot/distplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/plot/geoplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/plot/lineplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/plot/mapplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/plot/style.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:35:41.181844 coolpandas-0.4.1/coolpandas/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/stats/effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/stats/ttest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:35:41.181844 coolpandas-0.4.1/coolpandas/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/transform/bin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/transform/epoch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/transform/missing_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/transform/outliers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:35:41.181844 coolpandas-0.4.1/coolpandas/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-13 09:35:20.000000 coolpandas-0.4.1/coolpandas/utils/random_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:35:41.177844 coolpandas-0.4.1/coolpandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-13 09:35:41.000000 coolpandas-0.4.1/coolpandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-13 09:35:41.000000 coolpandas-0.4.1/coolpandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:35:41.000000 coolpandas-0.4.1/coolpandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-13 09:35:41.000000 coolpandas-0.4.1/coolpandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 09:35:41.000000 coolpandas-0.4.1/coolpandas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-13 09:35:20.000000 coolpandas-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 09:35:41.181844 coolpandas-0.4.1/setup.cfg
```

### Comparing `coolpandas-0.4.0/LICENSE` & `coolpandas-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.0/PKG-INFO` & `coolpandas-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coolpandas
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Python package for Exploratory Data Analysis.
 Author-email: Avel Docquin <adocquin@outlook.com>
 Project-URL: Homepage, https://github.com/adocquin/coolpandas
 Project-URL: Bug Tracker, https://github.com/adocquin/coolpandas/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `coolpandas-0.4.0/README.md` & `coolpandas-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.0/coolpandas/connect/redshift.py` & `coolpandas-0.4.1/coolpandas/connect/redshift.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.0/coolpandas/eda/__init__.py` & `coolpandas-0.4.1/coolpandas/eda/__init__.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.0/coolpandas/eda/correlation.py` & `coolpandas-0.4.1/coolpandas/eda/correlation.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.0/coolpandas/eda/distribution.py` & `coolpandas-0.4.1/coolpandas/eda/distribution.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.0/coolpandas/eda/duplicates.py` & `coolpandas-0.4.1/coolpandas/eda/duplicates.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.0/coolpandas/eda/features_type.py` & `coolpandas-0.4.1/coolpandas/eda/features_type.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.0/coolpandas/eda/geo_distance.py` & `coolpandas-0.4.1/coolpandas/eda/geo_distance.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.0/coolpandas/eda/missing_values.py` & `coolpandas-0.4.1/coolpandas/eda/missing_values.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.0/coolpandas/eda/shape.py` & `coolpandas-0.4.1/coolpandas/eda/shape.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.0/coolpandas/eda/summary.py` & `coolpandas-0.4.1/coolpandas/eda/summary.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.0/coolpandas/eda/value_counts.py` & `coolpandas-0.4.1/coolpandas/eda/value_counts.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.0/coolpandas/evaluate/confusion_matrix.py` & `coolpandas-0.4.1/coolpandas/evaluate/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.0/coolpandas/plot/barplot.py` & `coolpandas-0.4.1/coolpandas/plot/barplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.0/coolpandas/plot/boxplot.py` & `coolpandas-0.4.1/coolpandas/plot/boxplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.0/coolpandas/plot/distplot.py` & `coolpandas-0.4.1/coolpandas/plot/distplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.0/coolpandas/plot/geoplot.py` & `coolpandas-0.4.1/coolpandas/plot/geoplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.0/coolpandas/plot/lineplot.py` & `coolpandas-0.4.1/coolpandas/plot/lineplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.0/coolpandas/plot/mapplot.py` & `coolpandas-0.4.1/coolpandas/plot/mapplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.0/coolpandas/plot/style.py` & `coolpandas-0.4.1/coolpandas/plot/style.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.0/coolpandas/stats/effect.py` & `coolpandas-0.4.1/coolpandas/stats/effect.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.0/coolpandas/stats/ttest.py` & `coolpandas-0.4.1/coolpandas/stats/ttest.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.0/coolpandas/transform/bin.py` & `coolpandas-0.4.1/coolpandas/transform/bin.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.0/coolpandas/transform/missing_values.py` & `coolpandas-0.4.1/coolpandas/transform/missing_values.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.0/coolpandas/transform/outliers.py` & `coolpandas-0.4.1/coolpandas/transform/outliers.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.0/coolpandas.egg-info/PKG-INFO` & `coolpandas-0.4.1/coolpandas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coolpandas
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Python package for Exploratory Data Analysis.
 Author-email: Avel Docquin <adocquin@outlook.com>
 Project-URL: Homepage, https://github.com/adocquin/coolpandas
 Project-URL: Bug Tracker, https://github.com/adocquin/coolpandas/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `coolpandas-0.4.0/coolpandas.egg-info/SOURCES.txt` & `coolpandas-0.4.1/coolpandas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.0/pyproject.toml` & `coolpandas-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coolpandas"
-version = "0.4.0"
+version = "0.4.1"
 authors = [
   { name="Avel Docquin", email="adocquin@outlook.com" },
   ]
 description = "A Python package for Exploratory Data Analysis."
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
```

