# Comparing `tmp/coolpandas-0.4.3.tar.gz` & `tmp/coolpandas-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolpandas-0.4.3.tar", last modified: Thu Jul 13 14:39:05 2023, max compression
+gzip compressed data, was "coolpandas-0.4.4.tar", last modified: Thu Jul 13 15:05:31 2023, max compression
```

## Comparing `coolpandas-0.4.3.tar` & `coolpandas-0.4.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:39:05.905328 coolpandas-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-13 14:38:39.000000 coolpandas-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-13 14:39:05.905328 coolpandas-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-13 14:38:39.000000 coolpandas-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:39:05.897327 coolpandas-0.4.3/coolpandas/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:39:05.897327 coolpandas-0.4.3/coolpandas/connect/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/connect/redshift.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:39:05.901327 coolpandas-0.4.3/coolpandas/eda/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/eda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/eda/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/eda/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/eda/duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/eda/features_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/eda/geo_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/eda/missing_values.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/eda/random_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/eda/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/eda/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/eda/value_counts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:39:05.901327 coolpandas-0.4.3/coolpandas/evaluate/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/evaluate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/evaluate/confusion_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:39:05.901327 coolpandas-0.4.3/coolpandas/plot/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/plot/barplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/plot/boxplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/plot/distplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/plot/geoplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/plot/lineplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/plot/mapplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/plot/scatterplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/plot/style.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:39:05.901327 coolpandas-0.4.3/coolpandas/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/stats/effect.py
--rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/stats/ttest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:39:05.901327 coolpandas-0.4.3/coolpandas/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/transform/bin.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/transform/epoch.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/transform/missing_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/transform/outliers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:39:05.905328 coolpandas-0.4.3/coolpandas/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-13 14:38:39.000000 coolpandas-0.4.3/coolpandas/utils/random_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:39:05.897327 coolpandas-0.4.3/coolpandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-13 14:39:05.000000 coolpandas-0.4.3/coolpandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-13 14:39:05.000000 coolpandas-0.4.3/coolpandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:39:05.000000 coolpandas-0.4.3/coolpandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-13 14:39:05.000000 coolpandas-0.4.3/coolpandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 14:39:05.000000 coolpandas-0.4.3/coolpandas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-13 14:38:39.000000 coolpandas-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 14:39:05.905328 coolpandas-0.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:05:31.852748 coolpandas-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-13 15:05:08.000000 coolpandas-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-13 15:05:31.852748 coolpandas-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-13 15:05:08.000000 coolpandas-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:05:31.844748 coolpandas-0.4.4/coolpandas/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:05:31.848748 coolpandas-0.4.4/coolpandas/connect/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/connect/redshift.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:05:31.848748 coolpandas-0.4.4/coolpandas/eda/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/eda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/eda/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/eda/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/eda/duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/eda/features_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/eda/geo_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/eda/missing_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/eda/random_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/eda/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/eda/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/eda/value_counts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:05:31.848748 coolpandas-0.4.4/coolpandas/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/evaluate/confusion_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:05:31.848748 coolpandas-0.4.4/coolpandas/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/plot/barplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/plot/boxplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/plot/distplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/plot/geoplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/plot/lineplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/plot/mapplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/plot/scatterplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/plot/style.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:05:31.848748 coolpandas-0.4.4/coolpandas/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/stats/effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/stats/ttest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:05:31.852748 coolpandas-0.4.4/coolpandas/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/transform/bin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/transform/epoch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/transform/missing_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/transform/outliers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:05:31.852748 coolpandas-0.4.4/coolpandas/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-13 15:05:08.000000 coolpandas-0.4.4/coolpandas/utils/random_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:05:31.848748 coolpandas-0.4.4/coolpandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-13 15:05:31.000000 coolpandas-0.4.4/coolpandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-13 15:05:31.000000 coolpandas-0.4.4/coolpandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:05:31.000000 coolpandas-0.4.4/coolpandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-13 15:05:31.000000 coolpandas-0.4.4/coolpandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 15:05:31.000000 coolpandas-0.4.4/coolpandas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-13 15:05:08.000000 coolpandas-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 15:05:31.852748 coolpandas-0.4.4/setup.cfg
```

### Comparing `coolpandas-0.4.3/LICENSE` & `coolpandas-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.3/PKG-INFO` & `coolpandas-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coolpandas
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Python package for Exploratory Data Analysis.
 Author-email: Avel Docquin <adocquin@outlook.com>
 Project-URL: Homepage, https://github.com/adocquin/coolpandas
 Project-URL: Bug Tracker, https://github.com/adocquin/coolpandas/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `coolpandas-0.4.3/README.md` & `coolpandas-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.3/coolpandas/connect/redshift.py` & `coolpandas-0.4.4/coolpandas/connect/redshift.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.3/coolpandas/eda/__init__.py` & `coolpandas-0.4.4/coolpandas/eda/__init__.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.3/coolpandas/eda/correlation.py` & `coolpandas-0.4.4/coolpandas/eda/correlation.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.3/coolpandas/eda/distribution.py` & `coolpandas-0.4.4/coolpandas/eda/distribution.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.3/coolpandas/eda/duplicates.py` & `coolpandas-0.4.4/coolpandas/eda/duplicates.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.3/coolpandas/eda/features_type.py` & `coolpandas-0.4.4/coolpandas/eda/features_type.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.3/coolpandas/eda/geo_distance.py` & `coolpandas-0.4.4/coolpandas/eda/geo_distance.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.3/coolpandas/eda/missing_values.py` & `coolpandas-0.4.4/coolpandas/eda/missing_values.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.3/coolpandas/eda/shape.py` & `coolpandas-0.4.4/coolpandas/eda/shape.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.3/coolpandas/eda/summary.py` & `coolpandas-0.4.4/coolpandas/eda/summary.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.3/coolpandas/eda/value_counts.py` & `coolpandas-0.4.4/coolpandas/eda/value_counts.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.3/coolpandas/evaluate/confusion_matrix.py` & `coolpandas-0.4.4/coolpandas/evaluate/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.3/coolpandas/plot/barplot.py` & `coolpandas-0.4.4/coolpandas/plot/barplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.3/coolpandas/plot/boxplot.py` & `coolpandas-0.4.4/coolpandas/plot/boxplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.3/coolpandas/plot/distplot.py` & `coolpandas-0.4.4/coolpandas/plot/distplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.3/coolpandas/plot/geoplot.py` & `coolpandas-0.4.4/coolpandas/plot/geoplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.3/coolpandas/plot/lineplot.py` & `coolpandas-0.4.4/coolpandas/plot/lineplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.3/coolpandas/plot/mapplot.py` & `coolpandas-0.4.4/coolpandas/plot/mapplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.3/coolpandas/plot/scatterplot.py` & `coolpandas-0.4.4/coolpandas/plot/scatterplot.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,9 +33,8 @@
         y=y_axis,
         title=format_title(title, subtitle=subtitle),
         template=custom_template,
         width=800,
         height=400,
         **kwargs,
     )
-    fig.update_traces(width=0.5)
     return fig
```

### Comparing `coolpandas-0.4.3/coolpandas/plot/style.py` & `coolpandas-0.4.4/coolpandas/plot/style.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.3/coolpandas/stats/effect.py` & `coolpandas-0.4.4/coolpandas/stats/effect.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.3/coolpandas/stats/ttest.py` & `coolpandas-0.4.4/coolpandas/stats/ttest.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.3/coolpandas/transform/bin.py` & `coolpandas-0.4.4/coolpandas/transform/bin.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.3/coolpandas/transform/missing_values.py` & `coolpandas-0.4.4/coolpandas/transform/missing_values.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.3/coolpandas/transform/outliers.py` & `coolpandas-0.4.4/coolpandas/transform/outliers.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.3/coolpandas.egg-info/PKG-INFO` & `coolpandas-0.4.4/coolpandas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coolpandas
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Python package for Exploratory Data Analysis.
 Author-email: Avel Docquin <adocquin@outlook.com>
 Project-URL: Homepage, https://github.com/adocquin/coolpandas
 Project-URL: Bug Tracker, https://github.com/adocquin/coolpandas/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `coolpandas-0.4.3/coolpandas.egg-info/SOURCES.txt` & `coolpandas-0.4.4/coolpandas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.3/pyproject.toml` & `coolpandas-0.4.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coolpandas"
-version = "0.4.3"
+version = "0.4.4"
 authors = [
   { name="Avel Docquin", email="adocquin@outlook.com" },
   ]
 description = "A Python package for Exploratory Data Analysis."
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
```

