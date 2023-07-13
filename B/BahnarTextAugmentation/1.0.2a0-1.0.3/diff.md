# Comparing `tmp/BahnarTextAugmentation-1.0.2a0.tar.gz` & `tmp/BahnarTextAugmentation-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BahnarTextAugmentation-1.0.2a0.tar", last modified: Wed Jul 12 08:09:00 2023, max compression
+gzip compressed data, was "BahnarTextAugmentation-1.0.3.tar", last modified: Thu Jul 13 14:30:10 2023, max compression
```

## Comparing `BahnarTextAugmentation-1.0.2a0.tar` & `BahnarTextAugmentation-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-12 08:09:00.340092 BahnarTextAugmentation-1.0.2a0/
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      130 2023-07-12 08:09:00.340092 BahnarTextAugmentation-1.0.2a0/PKG-INFO
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-11 06:49:41.000000 BahnarTextAugmentation-1.0.2a0/README.md
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)       38 2023-07-12 08:09:00.340092 BahnarTextAugmentation-1.0.2a0/setup.cfg
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      779 2023-07-12 08:08:47.000000 BahnarTextAugmentation-1.0.2a0/setup.py
-drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-12 08:09:00.336092 BahnarTextAugmentation-1.0.2a0/src/
-drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-12 08:09:00.340092 BahnarTextAugmentation-1.0.2a0/src/BahnarTextAugmentation/
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     5743 2023-07-12 06:59:53.000000 BahnarTextAugmentation-1.0.2a0/src/BahnarTextAugmentation/EDA.py
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     1779 2023-07-12 07:56:32.000000 BahnarTextAugmentation-1.0.2a0/src/BahnarTextAugmentation/MTLCombination.py
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      929 2023-07-12 07:00:13.000000 BahnarTextAugmentation-1.0.2a0/src/BahnarTextAugmentation/SentenceBoundary.py
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     4885 2023-07-12 07:56:17.000000 BahnarTextAugmentation-1.0.2a0/src/BahnarTextAugmentation/Single.py
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     2117 2023-07-12 07:00:05.000000 BahnarTextAugmentation-1.0.2a0/src/BahnarTextAugmentation/Word2Vec.py
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)       45 2023-07-12 08:02:09.000000 BahnarTextAugmentation-1.0.2a0/src/BahnarTextAugmentation/__init__.py
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)       42 2023-07-12 08:08:56.000000 BahnarTextAugmentation-1.0.2a0/src/BahnarTextAugmentation/_version.py
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     1611 2023-07-12 08:08:31.000000 BahnarTextAugmentation-1.0.2a0/src/BahnarTextAugmentation/utils.py
-drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-12 08:09:00.340092 BahnarTextAugmentation-1.0.2a0/src/BahnarTextAugmentation.egg-info/
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      130 2023-07-12 08:09:00.000000 BahnarTextAugmentation-1.0.2a0/src/BahnarTextAugmentation.egg-info/PKG-INFO
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      583 2023-07-12 08:09:00.000000 BahnarTextAugmentation-1.0.2a0/src/BahnarTextAugmentation.egg-info/SOURCES.txt
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)        1 2023-07-12 08:09:00.000000 BahnarTextAugmentation-1.0.2a0/src/BahnarTextAugmentation.egg-info/dependency_links.txt
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      101 2023-07-12 08:09:00.000000 BahnarTextAugmentation-1.0.2a0/src/BahnarTextAugmentation.egg-info/requires.txt
--rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)       23 2023-07-12 08:09:00.000000 BahnarTextAugmentation-1.0.2a0/src/BahnarTextAugmentation.egg-info/top_level.txt
+drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-13 14:30:10.938602 BahnarTextAugmentation-1.0.3/
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      140 2023-07-13 14:30:10.938602 BahnarTextAugmentation-1.0.3/PKG-INFO
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-11 06:49:41.000000 BahnarTextAugmentation-1.0.3/README.md
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)       38 2023-07-13 14:30:10.938602 BahnarTextAugmentation-1.0.3/setup.cfg
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      855 2023-07-13 14:29:38.000000 BahnarTextAugmentation-1.0.3/setup.py
+drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-13 14:30:10.926605 BahnarTextAugmentation-1.0.3/src/
+drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-13 14:30:10.934603 BahnarTextAugmentation-1.0.3/src/BahnarTextAugmentation/
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     5743 2023-07-12 06:59:53.000000 BahnarTextAugmentation-1.0.3/src/BahnarTextAugmentation/EDA.py
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     1779 2023-07-12 07:56:32.000000 BahnarTextAugmentation-1.0.3/src/BahnarTextAugmentation/MTLCombination.py
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      929 2023-07-12 07:00:13.000000 BahnarTextAugmentation-1.0.3/src/BahnarTextAugmentation/SentenceBoundary.py
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     4885 2023-07-12 07:56:17.000000 BahnarTextAugmentation-1.0.3/src/BahnarTextAugmentation/Single.py
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     2117 2023-07-12 07:00:05.000000 BahnarTextAugmentation-1.0.3/src/BahnarTextAugmentation/Word2Vec.py
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)       45 2023-07-12 08:02:09.000000 BahnarTextAugmentation-1.0.3/src/BahnarTextAugmentation/__init__.py
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)       41 2023-07-13 14:29:48.000000 BahnarTextAugmentation-1.0.3/src/BahnarTextAugmentation/_version.py
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)     1611 2023-07-12 08:08:31.000000 BahnarTextAugmentation-1.0.3/src/BahnarTextAugmentation/utils.py
+drwxrwxr-x   0 ledong0110  (1000) ledong0110  (1000)        0 2023-07-13 14:30:10.934603 BahnarTextAugmentation-1.0.3/src/BahnarTextAugmentation.egg-info/
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      140 2023-07-13 14:30:10.000000 BahnarTextAugmentation-1.0.3/src/BahnarTextAugmentation.egg-info/PKG-INFO
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      583 2023-07-13 14:30:10.000000 BahnarTextAugmentation-1.0.3/src/BahnarTextAugmentation.egg-info/SOURCES.txt
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)        1 2023-07-13 14:30:10.000000 BahnarTextAugmentation-1.0.3/src/BahnarTextAugmentation.egg-info/dependency_links.txt
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)      101 2023-07-13 14:30:10.000000 BahnarTextAugmentation-1.0.3/src/BahnarTextAugmentation.egg-info/requires.txt
+-rw-rw-r--   0 ledong0110  (1000) ledong0110  (1000)       23 2023-07-13 14:30:10.000000 BahnarTextAugmentation-1.0.3/src/BahnarTextAugmentation.egg-info/top_level.txt
```

### Comparing `BahnarTextAugmentation-1.0.2a0/src/BahnarTextAugmentation/EDA.py` & `BahnarTextAugmentation-1.0.3/src/BahnarTextAugmentation/EDA.py`

 * *Files identical despite different names*

### Comparing `BahnarTextAugmentation-1.0.2a0/src/BahnarTextAugmentation/MTLCombination.py` & `BahnarTextAugmentation-1.0.3/src/BahnarTextAugmentation/MTLCombination.py`

 * *Files identical despite different names*

### Comparing `BahnarTextAugmentation-1.0.2a0/src/BahnarTextAugmentation/SentenceBoundary.py` & `BahnarTextAugmentation-1.0.3/src/BahnarTextAugmentation/SentenceBoundary.py`

 * *Files identical despite different names*

### Comparing `BahnarTextAugmentation-1.0.2a0/src/BahnarTextAugmentation/Single.py` & `BahnarTextAugmentation-1.0.3/src/BahnarTextAugmentation/Single.py`

 * *Files identical despite different names*

### Comparing `BahnarTextAugmentation-1.0.2a0/src/BahnarTextAugmentation/Word2Vec.py` & `BahnarTextAugmentation-1.0.3/src/BahnarTextAugmentation/Word2Vec.py`

 * *Files identical despite different names*

### Comparing `BahnarTextAugmentation-1.0.2a0/src/BahnarTextAugmentation/utils.py` & `BahnarTextAugmentation-1.0.3/src/BahnarTextAugmentation/utils.py`

 * *Files identical despite different names*

### Comparing `BahnarTextAugmentation-1.0.2a0/src/BahnarTextAugmentation.egg-info/SOURCES.txt` & `BahnarTextAugmentation-1.0.3/src/BahnarTextAugmentation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

