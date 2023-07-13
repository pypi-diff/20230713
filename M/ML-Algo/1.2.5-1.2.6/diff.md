# Comparing `tmp/ML-Algo-1.2.5.tar.gz` & `tmp/ML-Algo-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ML-Algo-1.2.5.tar", last modified: Wed Jul 12 13:33:22 2023, max compression
+gzip compressed data, was "ML-Algo-1.2.6.tar", last modified: Thu Jul 13 06:49:07 2023, max compression
```

## Comparing `ML-Algo-1.2.5.tar` & `ML-Algo-1.2.6.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 13:33:22.768912 ML-Algo-1.2.5/
-drwxrwxrwx   0        0        0        0 2023-07-12 13:33:22.753914 ML-Algo-1.2.5/ML_Algo/
--rw-rw-rw-   0        0        0     2031 2023-07-12 10:08:06.000000 ML-Algo-1.2.5/ML_Algo/DataCleaning.py
--rw-rw-rw-   0        0        0     1629 2023-07-12 13:17:21.000000 ML-Algo-1.2.5/ML_Algo/FetchData.py
--rw-rw-rw-   0        0        0      710 2023-07-12 13:32:32.000000 ML-Algo-1.2.5/ML_Algo/Predictions.py
--rw-rw-rw-   0        0        0     2487 2023-07-12 13:21:48.000000 ML-Algo-1.2.5/ML_Algo/Series_Data.py
--rw-rw-rw-   0        0        0      842 2023-07-12 09:46:19.000000 ML-Algo-1.2.5/ML_Algo/Series_Time.py
--rw-rw-rw-   0        0        0        0 2023-07-12 12:37:23.000000 ML-Algo-1.2.5/ML_Algo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 13:33:22.765777 ML-Algo-1.2.5/ML_Algo.egg-info/
--rw-rw-rw-   0        0        0      164 2023-07-12 13:33:22.000000 ML-Algo-1.2.5/ML_Algo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-07-12 13:33:22.000000 ML-Algo-1.2.5/ML_Algo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 13:33:22.000000 ML-Algo-1.2.5/ML_Algo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-12 13:33:22.000000 ML-Algo-1.2.5/ML_Algo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-12 13:33:22.000000 ML-Algo-1.2.5/ML_Algo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      164 2023-07-12 13:33:22.767892 ML-Algo-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-12 13:33:22.768912 ML-Algo-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0      288 2023-07-12 13:32:40.000000 ML-Algo-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 06:49:07.382434 ML-Algo-1.2.6/
+drwxrwxrwx   0        0        0        0 2023-07-13 06:49:07.368728 ML-Algo-1.2.6/ML_Algo/
+-rw-rw-rw-   0        0        0     2031 2023-07-12 10:08:06.000000 ML-Algo-1.2.6/ML_Algo/DataCleaning.py
+-rw-rw-rw-   0        0        0     1629 2023-07-12 13:17:21.000000 ML-Algo-1.2.6/ML_Algo/FetchData.py
+-rw-rw-rw-   0        0        0      710 2023-07-12 13:32:32.000000 ML-Algo-1.2.6/ML_Algo/Predictions.py
+-rw-rw-rw-   0        0        0     2487 2023-07-12 13:21:48.000000 ML-Algo-1.2.6/ML_Algo/Series_Data.py
+-rw-rw-rw-   0        0        0      842 2023-07-12 09:46:19.000000 ML-Algo-1.2.6/ML_Algo/Series_Time.py
+-rw-rw-rw-   0        0        0     2124 2023-07-13 06:48:22.000000 ML-Algo-1.2.6/ML_Algo/TestRun.py
+-rw-rw-rw-   0        0        0        0 2023-07-12 12:37:23.000000 ML-Algo-1.2.6/ML_Algo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 06:49:07.379432 ML-Algo-1.2.6/ML_Algo.egg-info/
+-rw-rw-rw-   0        0        0     2155 2023-07-13 06:49:07.000000 ML-Algo-1.2.6/ML_Algo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-07-13 06:49:07.000000 ML-Algo-1.2.6/ML_Algo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 06:49:07.000000 ML-Algo-1.2.6/ML_Algo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-13 06:49:07.000000 ML-Algo-1.2.6/ML_Algo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-13 06:49:07.000000 ML-Algo-1.2.6/ML_Algo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2155 2023-07-13 06:49:07.381433 ML-Algo-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-13 06:49:07.382434 ML-Algo-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      895 2023-07-13 06:47:24.000000 ML-Algo-1.2.6/setup.py
```

### Comparing `ML-Algo-1.2.5/ML_Algo/DataCleaning.py` & `ML-Algo-1.2.6/ML_Algo/DataCleaning.py`

 * *Files identical despite different names*

### Comparing `ML-Algo-1.2.5/ML_Algo/FetchData.py` & `ML-Algo-1.2.6/ML_Algo/FetchData.py`

 * *Files identical despite different names*

### Comparing `ML-Algo-1.2.5/ML_Algo/Predictions.py` & `ML-Algo-1.2.6/ML_Algo/Predictions.py`

 * *Files identical despite different names*

### Comparing `ML-Algo-1.2.5/ML_Algo/Series_Data.py` & `ML-Algo-1.2.6/ML_Algo/Series_Data.py`

 * *Files identical despite different names*

### Comparing `ML-Algo-1.2.5/ML_Algo/Series_Time.py` & `ML-Algo-1.2.6/ML_Algo/Series_Time.py`

 * *Files identical despite different names*

