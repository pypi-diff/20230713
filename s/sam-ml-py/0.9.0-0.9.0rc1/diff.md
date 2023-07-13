# Comparing `tmp/sam_ml-py-0.9.0.tar.gz` & `tmp/sam_ml-py-0.9.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sam_ml-py-0.9.0.tar", last modified: Fri Jul  7 11:13:35 2023, max compression
+gzip compressed data, was "sam_ml-py-0.9.0rc1.tar", last modified: Thu Jul  6 12:01:15 2023, max compression
```

## Comparing `sam_ml-py-0.9.0.tar` & `sam_ml-py-0.9.0rc1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:13:35.539350 sam_ml-py-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-07 11:13:35.539350 sam_ml-py-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:13:35.535350 sam_ml-py-0.9.0/sam_ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:13:35.535350 sam_ml-py-0.9.0/sam_ml/config/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/config/global_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/config/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:13:35.535350 sam_ml-py-0.9.0/sam_ml/data/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/data/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/data/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/data/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/data/scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/data/synthetic_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:13:35.539350 sam_ml-py-0.9.0/sam_ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/models/AdaBoostClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/models/BaggingClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/models/BernoulliNB.py
--rw-r--r--   0 runner    (1001) docker     (123)    22309 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/models/ClassifierTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/models/DecisionTreeClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/models/ExtraTreesClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/models/GaussianNB.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/models/GaussianProcessClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/models/GradientBoostingMachine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/models/KNeighborsClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/models/LinearDiscriminantAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/models/LinearSupportVectorClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/models/LogisticRegression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/models/MLPClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/models/QuadraticDiscriminantAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/models/RandomForestClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/models/SupportVectorClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/models/XGBoostClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22835 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/models/main_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/models/main_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/models/main_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/sam_ml/models/scorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:13:35.539350 sam_ml-py-0.9.0/sam_ml_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-07 11:13:35.000000 sam_ml-py-0.9.0/sam_ml_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-07 11:13:35.000000 sam_ml-py-0.9.0/sam_ml_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 11:13:35.000000 sam_ml-py-0.9.0/sam_ml_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-07 11:13:35.000000 sam_ml-py-0.9.0/sam_ml_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-07 11:13:35.000000 sam_ml-py-0.9.0/sam_ml_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-07 11:13:35.539350 sam_ml-py-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:13:35.539350 sam_ml-py-0.9.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/test/test_CTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/test/test_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-07-07 11:13:25.000000 sam_ml-py-0.9.0/test/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:15.551675 sam_ml-py-0.9.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-06 12:01:15.551675 sam_ml-py-0.9.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:15.539675 sam_ml-py-0.9.0rc1/sam_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:15.539675 sam_ml-py-0.9.0rc1/sam_ml/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/config/global_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/config/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:15.543675 sam_ml-py-0.9.0rc1/sam_ml/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/data/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/data/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/data/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/data/scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/data/synthetic_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:15.547675 sam_ml-py-0.9.0rc1/sam_ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/AdaBoostClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/BaggingClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/BernoulliNB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21838 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/ClassifierTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/DecisionTreeClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/ExtraTreesClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/GaussianNB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/GaussianProcessClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/GradientBoostingMachine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/KNeighborsClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/LinearDiscriminantAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/LinearSupportVectorClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/LogisticRegression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/MLPClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/QuadraticDiscriminantAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/RandomForestClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/SupportVectorClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/XGBoostClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22835 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/main_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/main_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7700 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/main_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/sam_ml/models/scorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:15.551675 sam_ml-py-0.9.0rc1/sam_ml_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-06 12:01:15.000000 sam_ml-py-0.9.0rc1/sam_ml_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-06 12:01:15.000000 sam_ml-py-0.9.0rc1/sam_ml_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 12:01:15.000000 sam_ml-py-0.9.0rc1/sam_ml_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-06 12:01:15.000000 sam_ml-py-0.9.0rc1/sam_ml_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 12:01:15.000000 sam_ml-py-0.9.0rc1/sam_ml_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-06 12:01:15.551675 sam_ml-py-0.9.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:15.551675 sam_ml-py-0.9.0rc1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/test/test_CTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/test/test_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-07-06 12:01:03.000000 sam_ml-py-0.9.0rc1/test/test_pipeline.py
```

### Comparing `sam_ml-py-0.9.0/LICENSE` & `sam_ml-py-0.9.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.9.0/PKG-INFO` & `sam_ml-py-0.9.0rc1/sam_ml_py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sam_ml-py
-Version: 0.9.0
+Name: sam-ml-py
+Version: 0.9.0rc1
 Summary: a library for ML programing created by Samuel Brinkmann
 Author: Samuel Brinkmann
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: with_swig
```

### Comparing `sam_ml-py-0.9.0/README.md` & `sam_ml-py-0.9.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.9.0/sam_ml/config/global_variables.py` & `sam_ml-py-0.9.0rc1/sam_ml/config/global_variables.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.9.0/sam_ml/config/logging.py` & `sam_ml-py-0.9.0rc1/sam_ml/config/logging.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.9.0/sam_ml/data/embeddings.py` & `sam_ml-py-0.9.0rc1/sam_ml/data/embeddings.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,20 +25,23 @@
             **kwargs:
                 additional parameters for CountVectorizer or TfidfVectorizer
         """
         self.vec_type = vec
         self._grid: dict[str, list] = {} # for pipeline structure
 
         if vec == "bert":
+            logger.debug("using quora-distilbert-multilingual model as vectorizer")
             self.vectorizer = SentenceTransformer("quora-distilbert-multilingual")
 
         elif vec == "count":
+            logger.debug("using CountVectorizer as vectorizer")
             self.vectorizer = CountVectorizer(**kwargs)
 
         elif vec == "tfidf":
+            logger.debug("using TfidfVectorizer as vectorizer")
             self.vectorizer = TfidfVectorizer(**kwargs)
 
         else:
             logger.error(f"the entered vectorizer '{vec}' cannot be used --> using CountVectorizer as vectorizer")
             self.vectorizer = CountVectorizer()
             self.vec_type = "count"
```

### Comparing `sam_ml-py-0.9.0/sam_ml/data/feature_selection.py` & `sam_ml-py-0.9.0rc1/sam_ml/data/feature_selection.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.9.0/sam_ml/data/sampling.py` & `sam_ml-py-0.9.0rc1/sam_ml/data/sampling.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.9.0/sam_ml/data/scaler.py` & `sam_ml-py-0.9.0rc1/sam_ml/data/scaler.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,35 +33,43 @@
             **kwargs:
                 additional parameters for scaler
         """
         self.scaler_type = scaler
         self._grid: dict[str, list] = {} # for pipeline structure
 
         if scaler == "standard":
+            logger.debug("using StandardScaler as scaler")
             self.scaler = StandardScaler(**kwargs)
 
         elif scaler == "minmax":
+            logger.debug("using MinMaxScaler as scaler")
             self.scaler = MinMaxScaler(**kwargs)
 
         elif scaler == "maxabs":
+            logger.debug("using MaxAbsScaler as scaler")
             self.scaler = MaxAbsScaler(**kwargs)
 
         elif scaler == "robust":
+            logger.debug("using RobustScaler as scaler")
             self.scaler = RobustScaler(**kwargs)
             
         elif scaler == "normalizer":
+            logger.debug("using Normalizer as scaler")
             self.scaler = Normalizer(**kwargs)
 
         elif scaler == "power":
+            logger.debug("using PowerTransformer as scaler")
             self.scaler = PowerTransformer(**kwargs)
 
         elif scaler == "quantile":
+            logger.debug("using QuantileTransformer as scaler")
             self.scaler = QuantileTransformer(**kwargs)
 
         elif scaler == "quantile_normal":
+            logger.debug("using QuantileTransformer with output_distribution='normal' as scaler")
             self.scaler = QuantileTransformer(output_distribution="normal", **kwargs)
 
         else:
             logger.error(f"scaler='{scaler}' is no valid input -> using StandardScaler")
             self.scaler = StandardScaler()
             self.scaler_type = "standard"
```

### Comparing `sam_ml-py-0.9.0/sam_ml/data/synthetic_data.py` & `sam_ml-py-0.9.0rc1/sam_ml/data/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.9.0/sam_ml/models/AdaBoostClassifier.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/AdaBoostClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.9.0/sam_ml/models/BaggingClassifier.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/BaggingClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.9.0/sam_ml/models/BernoulliNB.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/BernoulliNB.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.9.0/sam_ml/models/ClassifierTest.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/ClassifierTest.py`

 * *Files 3% similar despite different names*

```diff
@@ -429,61 +429,54 @@
             except:
                 logger.warning(f"modeltype in '{key}' is not supported for this search -> will be skipped")
 
         total_model_num = len(model_dict)
         logger.info(f"total number of models: {total_model_num}")
         split_num = int(np.log2(total_model_num))+1
         split_size =int(1/split_num*len(x_train))
-        logger.info(f"split number: {split_num-1}, split_size (x_train): {split_size}")
         if split_size < 300:
             raise RuntimeError(f"not enough data for the amout of models. Data per split should be over 300, but {split_size} < 300")
+        logger.info(f"split number: {split_num}, split_size (x_train): {split_size}")
 
         # shuffle x_train/y_train
         x_train = x_train.sample(frac=1, random_state=42)
         y_train = y_train.sample(frac=1, random_state=42)
 
         for split_idx in tqdm(range(split_num-1), desc="splits"):
             x_train_train = x_train[split_idx*split_size:(split_idx+1)*split_size]
             x_train_test = x_train[(split_idx+1)*split_size:]
             y_train_train = y_train[split_idx*split_size:(split_idx+1)*split_size]
             y_train_test = y_train[(split_idx+1)*split_size:]
-            logger.info(f"split {split_idx+1}: length x_train/y_train {len(x_train_train)}/{len(y_train_train)}, length x_test/y_test {len(x_train_test)}/{len(y_train_test)}")
+            logger.info(f"length x_train/y_train {len(x_train_train)}/{len(y_train_train)}, length x_test/y_test {len(x_train_test)}/{len(y_train_test)}")
             split_scores: dict = {}
-            best_score: float = -1
             # train models in model_dict
             for key in tqdm(model_dict.keys(), desc=f"split {split_idx+1}", leave=leave_loadbar):
                 # train data classes in first split on all train data
                 if split_idx == 0:
-                    pre_x, _ = model_dict[key]._Pipeline__data_prepare(x_train, y_train)
-                    logger.debug(f"total length of train data after pipeline pre-processing: {len(pre_x)} ({key})")
+                    model_dict[key]._Pipeline__data_prepare(x_train, y_train)
 
                 # XGBoostClassifier has different warm_start implementation
                 if model_dict[key].model_type != "XGBC" or split_idx==0:
                     tscore, ttime = model_dict[key].train_warm_start(x_train_train, y_train_train, console_out=False)
                 else:
                     start = time.time()
                     model_dict[key].fit_warm_start(x_train_train, y_train_train, xgb_model=model_dict[key].model)
                     end = time.time()
                     tscore, ttime = model_dict[key].get_train_score(x_train_train, y_train_train), str(timedelta(seconds=int(end-start)))
                 
                 score = model_dict[key].evaluate(x_train_test, y_train_test, avg=avg, pos_label=pos_label, console_out=False, secondary_scoring=secondary_scoring, strength=strength)
                 score["train_score"] = tscore
                 score["train_time"] = ttime
                 split_scores[key] = score
-                sorted_split_scores = dict(sorted(split_scores.items(), key=lambda item: (item[1][scoring], item[1]["s_score"], item[1]["train_time"]), reverse=True))
-                if score[scoring] > best_score:
-                    best_model_name = list(sorted_split_scores.keys())[0]
-                    logger.info(f"new best {scoring}: {best_score} -> {score[scoring]} ({best_model_name})")
-                    best_score = score[scoring]
-
+            sorted_split_scores = dict(sorted(split_scores.items(), key=lambda item: (item[1][scoring], item[1]["s_score"], item[1]["train_time"]), reverse=True))
             sorted_split_scores_pd = pd.DataFrame(sorted_split_scores).transpose()
 
             # save model scores
             if save_results_path is not None:
-                sorted_split_scores_pd.to_csv(save_results_path.split(".")[0]+f"_split{split_idx+1}."+save_results_path.split(".")[1])
+                sorted_split_scores_pd.to_csv(save_results_path.split(".")[0]+f"_split{split_idx}."+save_results_path.split(".")[1])
 
             logger.info(f"Split scores (top 5): \n{sorted_split_scores_pd.head(5)}")
 
             # only keep better half of the models
             for key in list(sorted_split_scores.keys())[int(len(sorted_split_scores)/2):]:
                 del model_dict[key]
```

### Comparing `sam_ml-py-0.9.0/sam_ml/models/DecisionTreeClassifier.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/DecisionTreeClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.9.0/sam_ml/models/ExtraTreesClassifier.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/ExtraTreesClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.9.0/sam_ml/models/GaussianNB.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/GaussianNB.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.9.0/sam_ml/models/GaussianProcessClassifier.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/GaussianProcessClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.9.0/sam_ml/models/GradientBoostingMachine.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/GradientBoostingMachine.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.9.0/sam_ml/models/KNeighborsClassifier.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/KNeighborsClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.9.0/sam_ml/models/LinearDiscriminantAnalysis.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/LinearDiscriminantAnalysis.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.9.0/sam_ml/models/LinearSupportVectorClassifier.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/LinearSupportVectorClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.9.0/sam_ml/models/LogisticRegression.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.9.0/sam_ml/models/MLPClassifier.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/MLPClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.9.0/sam_ml/models/QuadraticDiscriminantAnalysis.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/QuadraticDiscriminantAnalysis.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.9.0/sam_ml/models/RandomForestClassifier.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/RandomForestClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.9.0/sam_ml/models/SupportVectorClassifier.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/SupportVectorClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.9.0/sam_ml/models/XGBoostClassifier.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/XGBoostClassifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.9.0/sam_ml/models/__init__.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.9.0/sam_ml/models/main_classifier.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/main_classifier.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.9.0/sam_ml/models/main_model.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/main_model.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.9.0/sam_ml/models/main_pipeline.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/main_pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,15 +78,15 @@
             elif self.sampler.algorithm in ("nm", "tl") and self.model_type in sampling_problems:
                 logger.warning(self.model_type+f" does not work with sampling='{self.sampler.algorithm}' --> going on with sampling='rus'")
                 self.sampler = Sampler(algorithm="rus")
 
         self.vectorizer_dict: dict[str, Embeddings_builder] = {}
 
         # keep track if model was trained for warm_start
-        self._data_classes_trained: bool = False
+        self.data_classes_trained: bool = False
 
     def __repr__(self) -> str:
         params: str = ""
         data_steps = ("vectorizer", self.vectorizer), ("scaler", self.scaler), ("selector", self.selector), ("sampler", self.sampler)
         for step in data_steps:
             params += step[0]+"="+step[1].__str__()+", "
 
@@ -119,35 +119,35 @@
             X = self.__auto_vectorizing(X, train_on=train_on)
         if self.scaler is not None:
             X = self.scaler.scale(X, train_on=train_on)
         if self.selector is not None:
             X = self.selector.select(X, y, train_on=train_on)
         if self.sampler is not None and train_on:
             X, y = self.sampler.sample(X, y)
-        self._data_classes_trained = True
+        self.data_classes_trained = True
         return X, y
 
     def train(self, x_train: pd.DataFrame, y_train: pd.Series, console_out: bool = True) -> tuple[float, str]:
         x_train_pre, y_train_pre = self.__data_prepare(x_train, y_train, train_on=True)
         return super().train(x_train_pre, y_train_pre, console_out)
     
     def train_warm_start(self, x_train: pd.DataFrame, y_train: pd.Series, console_out: bool = True) -> tuple[float, str]:
-        x_train_pre, y_train_pre = self.__data_prepare(x_train, y_train, train_on = not self._data_classes_trained)
+        x_train_pre, y_train_pre = self.__data_prepare(x_train, y_train, train_on = not self.data_classes_trained)
         return super().train(x_train_pre, y_train_pre, console_out)
 
     def fit(self, x_train: pd.DataFrame, y_train: pd.Series, **kwargs):
         x_train_pre, y_train_pre = self.__data_prepare(x_train, y_train, train_on=True)
         return super().fit(x_train_pre, y_train_pre, **kwargs)
     
     def fit_warm_start(self, x_train: pd.DataFrame, y_train: pd.Series, **kwargs):
-        x_train_pre, y_train_pre = self.__data_prepare(x_train, y_train, train_on = not self._data_classes_trained)
+        x_train_pre, y_train_pre = self.__data_prepare(x_train, y_train, train_on = not self.data_classes_trained)
         return super().fit(x_train_pre, y_train_pre, **kwargs)
     
     def get_train_score(self, x_train: pd.DataFrame, y_train: pd.Series) -> float:
-        x_train_pre, y_train_pre = self.__data_prepare(x_train, y_train, train_on = not self._data_classes_trained)
+        x_train_pre, y_train_pre = self.__data_prepare(x_train, y_train, train_on = not self.data_classes_trained)
         return super().get_train_score(x_train_pre, y_train_pre)
 
     def predict(self, x_test: pd.DataFrame) -> list:
         x_test_pre, _ = self.__data_prepare(x_test, None, train_on=False)
         return super().predict(x_test_pre)
 
     def get_params(self, deep: bool = True) -> dict[str, any]:
```

### Comparing `sam_ml-py-0.9.0/sam_ml/models/scorer.py` & `sam_ml-py-0.9.0rc1/sam_ml/models/scorer.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.9.0/sam_ml_py.egg-info/PKG-INFO` & `sam_ml-py-0.9.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sam-ml-py
-Version: 0.9.0
+Name: sam_ml-py
+Version: 0.9.0rc1
 Summary: a library for ML programing created by Samuel Brinkmann
 Author: Samuel Brinkmann
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: with_swig
```

### Comparing `sam_ml-py-0.9.0/sam_ml_py.egg-info/SOURCES.txt` & `sam_ml-py-0.9.0rc1/sam_ml_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.9.0/setup.py` & `sam_ml-py-0.9.0rc1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="sam_ml-py",
-    version="0.9.0",
+    version="0.9.0rc1",
     description="a library for ML programing created by Samuel Brinkmann",
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires=">=3.10",
     packages=find_packages(),
     package_data={},
     scripts=[],
```

### Comparing `sam_ml-py-0.9.0/test/test_classifier.py` & `sam_ml-py-0.9.0rc1/test/test_classifier.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import pandas as pd
 import pytest
 from sklearn.datasets import make_classification
-from sklearn.exceptions import NotFittedError
 
 from sam_ml.models import (
     ABC,
     BC,
     BNB,
     DTC,
     ETC,
@@ -20,84 +19,71 @@
     QDA,
     RFC,
     SVC,
     XGBC,
 )
 from sam_ml.models.main_classifier import SMAC_INSTALLED
 
-
-def get_models() -> list:
-    return [ABC(), BC(), BNB(), DTC(), ETC(), GNB(), GPC(), GBM(), KNC(), LDA(), LSVC(), LR(), MLPC(), QDA(), RFC(), SVC(), XGBC()]
-
+MODELS = [ABC(), BC(), BNB(), DTC(), ETC(), GNB(), GPC(), GBM(), KNC(), LDA(), LSVC(), LR(), MLPC(), QDA(), RFC(), SVC(), XGBC()]
 X, Y = make_classification(n_samples = 50,
                             n_features = 5,
                             n_informative = 5,
                             n_redundant = 0,
                             n_classes = 3,
                             weights = [.2, .3, .8])
 X = pd.DataFrame(X, columns=["col1", "col2", "col3", "col4", "col5"])
 Y = pd.Series(Y)
 
 
 def test_classifier_fit_evaluate():
-    for classifier in get_models():
+    for classifier in MODELS:
         classifier.fit(X, Y)
         classifier.evaluate(X, Y, console_out=False)
         classifier.evaluate_score(X, Y)
 
-def test_get_train_score_error():
-    with pytest.raises(NotFittedError):
-        for classifier in get_models():
-            classifier.get_train_score(X,Y)
-
-def test_get_train_score():
-    for classifier in get_models():
-        classifier.train(X, Y)
-        classifier.get_train_score(X,Y)
-
 def test_classifier_train_evaluate():
-    for classifier in get_models():
+    for classifier in MODELS:
         classifier.train(X, Y, console_out=False)
         classifier.evaluate(X, Y, console_out=False)
         classifier.evaluate_score(X, Y)
 
 def test_classifier_crossvalidation():
-    for classifier in get_models():
+    for classifier in MODELS:
         classifier.cross_validation(X, Y, cv_num=2)
 
 def test_classifier_crossvalidation_small_data():
-    for classifier in get_models():
+    for classifier in MODELS:
         classifier.cross_validation_small_data(X, Y)
 
 def test_classifier_randomCVsearch():
-    for classifier in get_models():
+    for classifier in MODELS:
         best_param, _ = classifier.randomCVsearch(X, Y, n_trails=5, cv_num=2)
         assert best_param != {}, "should always find a parameter combination"
 
 def test_classifier_randomCVsearch_small_data():
-    for classifier in get_models():
+    for classifier in MODELS:
         best_param, _ = classifier.randomCVsearch(X, Y, n_trails=5, cv_num=2, small_data_eval=True)
         assert best_param != {}, "should always find a parameter combination"
 
 @pytest.mark.with_swig
 def test_classifier_smac_search():
     if SMAC_INSTALLED:
-        for classifier in get_models():
+        for classifier in MODELS:
             best_param = classifier.smac_search(X, Y, n_trails=5, cv_num=2)
             assert best_param != {}, "should always find a parameter combination"
     else:
         with pytest.raises(ImportError):
-            for classifier in get_models():
+            for classifier in MODELS:
                 best_param = classifier.smac_search(X, Y, n_trails=5, cv_num=2)
                 assert best_param != {}, "should always find a parameter combination"
 
 @pytest.mark.with_swig
 def test_classifier_smac_search_small_data():
     if SMAC_INSTALLED:
-        for classifier in get_models():
+        for classifier in MODELS:
             best_param = classifier.smac_search(X, Y, n_trails=5, cv_num=2, small_data_eval=True)
             assert best_param != {}, "should always find a parameter combination"
     else:
         with pytest.raises(ImportError):
-            for classifier in get_models():
+            for classifier in MODELS:
                 best_param = classifier.smac_search(X, Y, n_trails=5, cv_num=2, small_data_eval=True)
                 assert best_param != {}, "should always find a parameter combination"
```

