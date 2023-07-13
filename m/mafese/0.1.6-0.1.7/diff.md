# Comparing `tmp/mafese-0.1.6.tar.gz` & `tmp/mafese-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mafese-0.1.6.tar", last modified: Sat Jul  1 09:51:10 2023, max compression
+gzip compressed data, was "mafese-0.1.7.tar", last modified: Thu Jul 13 10:58:39 2023, max compression
```

## Comparing `mafese-0.1.6.tar` & `mafese-0.1.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:51:10.820963 mafese-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-01 09:50:03.000000 mafese-0.1.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-01 09:50:03.000000 mafese-0.1.6/ChangeLog.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 09:50:03.000000 mafese-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-01 09:50:03.000000 mafese-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13007 2023-07-01 09:51:10.820963 mafese-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10036 2023-07-01 09:50:03.000000 mafese-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:51:10.816963 mafese-0.1.6/mafese/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:51:10.816963 mafese-0.1.6/mafese/embedded/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/embedded/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/embedded/lasso.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/embedded/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/unsupervised.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:51:10.820963 mafese-0.1.6/mafese/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/utils/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/utils/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/utils/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/utils/estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/utils/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/utils/mealpy_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/utils/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:51:10.820963 mafese-0.1.6/mafese/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34491 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/wrapper/mha.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/wrapper/recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-07-01 09:50:03.000000 mafese-0.1.6/mafese/wrapper/sequential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:51:10.816963 mafese-0.1.6/mafese.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13007 2023-07-01 09:51:10.000000 mafese-0.1.6/mafese.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-01 09:51:10.000000 mafese-0.1.6/mafese.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 09:51:10.000000 mafese-0.1.6/mafese.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-01 09:51:10.000000 mafese-0.1.6/mafese.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-01 09:51:10.000000 mafese-0.1.6/mafese.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 09:51:10.820963 mafese-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-01 09:50:03.000000 mafese-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 09:51:10.820963 mafese-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-01 09:50:03.000000 mafese-0.1.6/tests/test_embedded.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-01 09:50:03.000000 mafese-0.1.6/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-01 09:50:03.000000 mafese-0.1.6/tests/test_unsupervised.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-01 09:50:03.000000 mafese-0.1.6/tests/test_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:58:39.781923 mafese-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-13 10:57:18.000000 mafese-0.1.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-13 10:57:18.000000 mafese-0.1.7/ChangeLog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-13 10:57:18.000000 mafese-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-13 10:57:18.000000 mafese-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14689 2023-07-13 10:58:39.781923 mafese-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11709 2023-07-13 10:57:18.000000 mafese-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:58:39.777923 mafese-0.1.7/mafese/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:58:39.777923 mafese-0.1.7/mafese/embedded/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/embedded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/embedded/lasso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/embedded/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/unsupervised.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:58:39.781923 mafese-0.1.7/mafese/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/utils/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/utils/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/utils/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/utils/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/utils/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/utils/mealpy_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/utils/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:58:39.781923 mafese-0.1.7/mafese/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32353 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/wrapper/mha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/wrapper/recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-07-13 10:57:18.000000 mafese-0.1.7/mafese/wrapper/sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:58:39.777923 mafese-0.1.7/mafese.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14689 2023-07-13 10:58:39.000000 mafese-0.1.7/mafese.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-13 10:58:39.000000 mafese-0.1.7/mafese.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 10:58:39.000000 mafese-0.1.7/mafese.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-13 10:58:39.000000 mafese-0.1.7/mafese.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-13 10:58:39.000000 mafese-0.1.7/mafese.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 10:58:39.781923 mafese-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-13 10:57:18.000000 mafese-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:58:39.781923 mafese-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-13 10:57:18.000000 mafese-0.1.7/tests/test_embedded.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-13 10:57:18.000000 mafese-0.1.7/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-13 10:57:18.000000 mafese-0.1.7/tests/test_unsupervised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-13 10:57:18.000000 mafese-0.1.7/tests/test_wrapper.py
```

### Comparing `mafese-0.1.6/CODE_OF_CONDUCT.md` & `mafese-0.1.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `mafese-0.1.6/ChangeLog.md` & `mafese-0.1.7/ChangeLog.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Version 0.1.7
+
++ Remove some unknown datasets
++ Fix bug name in Kendall and Spearman functions of FilterSelector 
++ Add Relief-based family to FilterSelector 
+  + Relief Original 
+  + Relief-F 
+  + VLS-Relief-F: Very Large Scale ReliefF 
++ Remove rtf transfer function in MhaSelector
++ Update save results file of MultiMhaSelector's evaluate() function.
++ Update examples for some Selector class
+
+---------------------------------------------------------------------
+
 # Version 0.1.6
 
 + Rename some public functions to private functions
 + Add MultiMhaSelector class
 + Add Matplotlib library and support visualization for MultiMhaSelector class
 + Add dependency plotly>=5.10.0 and kaleido >=0.2.1
 + Update examples for some Selector class
```

### Comparing `mafese-0.1.6/LICENSE` & `mafese-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mafese-0.1.6/PKG-INFO` & `mafese-0.1.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: mafese
-Version: 0.1.6
+Version: 0.1.7
 Summary: MAFESE: Metaheuristic Algorithm for Feature Selection - An Open Source Python Library
 Home-page: https://github.com/thieu1995/mafese
 Author: Thieu
 Author-email: nguyenthieu2102@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://mafese.readthedocs.io/
 Project-URL: Source Code, https://github.com/thieu1995/mafese
 Project-URL: Bug Tracker, https://github.com/thieu1995/mafese/issues
 Project-URL: Change Log, https://github.com/thieu1995/mafese/blob/master/ChangeLog.md
 Project-URL: Forum, https://t.me/+fRVCJGuGJg1mNDg1
-Keywords: engineering optimization problems,mathematical optimization,feature selection,classification problem,feature selector,dimensionality reduction,subset selection,wrapper methods,embedded methods,mutual information,correlation-based feature selection,recursive feature selection,principal component analysis,PCA,lasso regularization,ridge regularization,Genetic algorithm (GA),Particle swarm optimization (PSO),Ant colony optimization (ACO),Differential evolution (DE),Simulated annealing,Grey wolf optimizer (GWO),Whale Optimization Algorithm (WOA),confusion matrix,recall,precision,accuracy,K-Nearest Neighbors,random forest,support vector machine,pearson correlation coefficient (PCC),spearman correlation coefficient (SCC),relief,multi-objectives optimization problems,Stochastic optimization,Global optimization,Convergence analysis,Search space exploration,Local search,Computational intelligence,Robust optimization,Performance analysis,Intelligent optimization,Simulations
+Keywords: engineering optimization problems,mathematical optimization,feature selection,classification problem,feature selector,dimensionality reduction,subset selection,wrapper methods,embedded methods,mutual information,correlation-based feature selection,recursive feature selection,principal component analysis,PCA,lasso regularization,ridge regularization,Genetic algorithm (GA),Particle swarm optimization (PSO),Ant colony optimization (ACO),Differential evolution (DE),Simulated annealing,Grey wolf optimizer (GWO),Whale Optimization Algorithm (WOA),confusion matrix,recall,precision,accuracy,K-Nearest Neighbors,random forest,support vector machine,pearson correlation coefficient (PCC),spearman correlation coefficient (SCC),relief,relief-f,multi-objectives optimization problems,Stochastic optimization,Global optimization,Convergence analysis,Search space exploration,Local search,Computational intelligence,Robust optimization,Performance analysis,Intelligent optimization,Simulations
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
@@ -43,15 +43,15 @@
 
 
 <p align="center"><img style="height:300px;" src=".github/img/logo.png" alt="MAFESE" title="MAFESE"/></p>
 
 ---
 
 
-[![GitHub release](https://img.shields.io/badge/release-0.1.6-yellow.svg)](https://github.com/thieu1995/mafese/releases)
+[![GitHub release](https://img.shields.io/badge/release-0.1.7-yellow.svg)](https://github.com/thieu1995/mafese/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/mafese) 
 [![PyPI version](https://badge.fury.io/py/mafese.svg)](https://badge.fury.io/py/mafese)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mafese.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/mafese.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mafese.svg)
 [![Downloads](https://pepy.tech/badge/mafese)](https://pepy.tech/project/mafese)
 [![Tests & Publishes to PyPI](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml)
@@ -65,15 +65,15 @@
 
 
 MAFESE (Metaheuristic Algorithms for FEature SElection) is the largest python library for feature selection problem 
 using meta-heuristic algorithms. 
 
 * **Free software:** GNU General Public License (GPL) V3 license
 * **Total Wrapper-based (Metaheuristic Algorithms)**: > 180 methods
-* **Total Filter-based (Statistical-based)**: > 12 methods
+* **Total Filter-based (Statistical-based)**: > 15 methods
 * **Total Embedded-based (Tree and Lasso)**: > 10 methods
 * **Total Unsupervised-based**: >= 4 methods
 * **Total classification dataset**: >= 30 datasets
 * **Total regression dataset**: >= 7 datasets
 * **Total performance metrics (as fitness)**: > 30 metrics
 * **Documentation:** https://mafese.readthedocs.io/en/latest/
 * **Python versions:** 3.7.x, 3.8.x, 3.9.x, 3.10.x, 3.11.x
@@ -82,15 +82,15 @@
 
 # Installation
 
 ### Install with pip
 
 Install the [current PyPI release](https://pypi.python.org/pypi/mafese):
 ```sh 
-$ pip install mafese==0.1.6
+$ pip install mafese==0.1.7
 ```
 
 ### Install directly from source code
 ```sh 
 $ git clone https://github.com/thieu1995/mafese.git
 $ cd mafese
 $ python setup.py install
@@ -100,17 +100,22 @@
 ### Lib's structure
 
 ```code 
 docs
 examples
 mafese
     data/
-        Arrhythmia.csv
-        BreastCancer.csv
-        ...
+        cls/
+            aggregation.csv
+            Arrhythmia.csv
+            ...
+        reg/
+            boston-housing.csv
+            diabetes.csv
+            ...
     wrapper/
         mha.py
         recursive.py
         sequential.py
     embedded/
         lasso.py
         tree.py
@@ -275,14 +280,53 @@
 
 2) How do I know my Selector support which estimator? which methods?
 ```python 
 print(feat_selector.SUPPORT) 
 ```
 Or you better read the document from: https://mafese.readthedocs.io/en/latest/
 
+3) I got this type of error
+```python 
+raise ValueError("Existed at least one new label in y_pred.")
+ValueError: Existed at least one new label in y_pred.
+``` 
+How to solve this?
+
++ This occurs only when you are working on a classification problem with a small dataset that has many classes. For 
+  instance, the "Zoo" dataset contains only 101 samples, but it has 7 classes. If you split the dataset into a 
+  training and testing set with a ratio of around 80% - 20%, there is a chance that one or more classes may appear 
+  in the testing set but not in the training set. As a result, when you calculate the performance metrics, you may 
+  encounter this error. You cannot predict or assign new data to a new label because you have no knowledge about the 
+  new label. There are several solutions to this problem.
+
++ 1st: Use the SMOTE method to address imbalanced data and ensure that all classes have the same number of samples.
+
+```python 
+from imblearn.over_sampling import SMOTE
+import pandas as pd
+from mafese import Data
+
+dataset = pd.read_csv('examples/dataset.csv', index_col=0).values
+X, y = dataset[:, 0:-1], dataset[:, -1]
+
+X_new, y_new = SMOTE().fit_resample(X, y)
+data = Data(X_new, y_new)
+```
+
++ 2nd: Use different random_state numbers in split_train_test() function.
+```python
+import pandas as pd 
+from mafese import Data 
+
+dataset = pd.read_csv('examples/dataset.csv', index_col=0).values
+X, y = dataset[:, 0:-1], dataset[:, -1]
+data = Data(X, y)
+data.split_train_test(test_size=0.2, random_state=10)   # Try different random_state value 
+```
+
 
 For more usage examples please look at [examples](/examples) folder.
 
 
 # Get helps (questions, problems)
 
 * Official source code repo: https://github.com/thieu1995/mafese
```

### Comparing `mafese-0.1.6/README.md` & `mafese-0.1.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 <p align="center"><img style="height:300px;" src=".github/img/logo.png" alt="MAFESE" title="MAFESE"/></p>
 
 ---
 
 
-[![GitHub release](https://img.shields.io/badge/release-0.1.6-yellow.svg)](https://github.com/thieu1995/mafese/releases)
+[![GitHub release](https://img.shields.io/badge/release-0.1.7-yellow.svg)](https://github.com/thieu1995/mafese/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/mafese) 
 [![PyPI version](https://badge.fury.io/py/mafese.svg)](https://badge.fury.io/py/mafese)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mafese.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/mafese.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mafese.svg)
 [![Downloads](https://pepy.tech/badge/mafese)](https://pepy.tech/project/mafese)
 [![Tests & Publishes to PyPI](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml)
@@ -22,15 +22,15 @@
 
 
 MAFESE (Metaheuristic Algorithms for FEature SElection) is the largest python library for feature selection problem 
 using meta-heuristic algorithms. 
 
 * **Free software:** GNU General Public License (GPL) V3 license
 * **Total Wrapper-based (Metaheuristic Algorithms)**: > 180 methods
-* **Total Filter-based (Statistical-based)**: > 12 methods
+* **Total Filter-based (Statistical-based)**: > 15 methods
 * **Total Embedded-based (Tree and Lasso)**: > 10 methods
 * **Total Unsupervised-based**: >= 4 methods
 * **Total classification dataset**: >= 30 datasets
 * **Total regression dataset**: >= 7 datasets
 * **Total performance metrics (as fitness)**: > 30 metrics
 * **Documentation:** https://mafese.readthedocs.io/en/latest/
 * **Python versions:** 3.7.x, 3.8.x, 3.9.x, 3.10.x, 3.11.x
@@ -39,15 +39,15 @@
 
 # Installation
 
 ### Install with pip
 
 Install the [current PyPI release](https://pypi.python.org/pypi/mafese):
 ```sh 
-$ pip install mafese==0.1.6
+$ pip install mafese==0.1.7
 ```
 
 ### Install directly from source code
 ```sh 
 $ git clone https://github.com/thieu1995/mafese.git
 $ cd mafese
 $ python setup.py install
@@ -57,17 +57,22 @@
 ### Lib's structure
 
 ```code 
 docs
 examples
 mafese
     data/
-        Arrhythmia.csv
-        BreastCancer.csv
-        ...
+        cls/
+            aggregation.csv
+            Arrhythmia.csv
+            ...
+        reg/
+            boston-housing.csv
+            diabetes.csv
+            ...
     wrapper/
         mha.py
         recursive.py
         sequential.py
     embedded/
         lasso.py
         tree.py
@@ -232,14 +237,53 @@
 
 2) How do I know my Selector support which estimator? which methods?
 ```python 
 print(feat_selector.SUPPORT) 
 ```
 Or you better read the document from: https://mafese.readthedocs.io/en/latest/
 
+3) I got this type of error
+```python 
+raise ValueError("Existed at least one new label in y_pred.")
+ValueError: Existed at least one new label in y_pred.
+``` 
+How to solve this?
+
++ This occurs only when you are working on a classification problem with a small dataset that has many classes. For 
+  instance, the "Zoo" dataset contains only 101 samples, but it has 7 classes. If you split the dataset into a 
+  training and testing set with a ratio of around 80% - 20%, there is a chance that one or more classes may appear 
+  in the testing set but not in the training set. As a result, when you calculate the performance metrics, you may 
+  encounter this error. You cannot predict or assign new data to a new label because you have no knowledge about the 
+  new label. There are several solutions to this problem.
+
++ 1st: Use the SMOTE method to address imbalanced data and ensure that all classes have the same number of samples.
+
+```python 
+from imblearn.over_sampling import SMOTE
+import pandas as pd
+from mafese import Data
+
+dataset = pd.read_csv('examples/dataset.csv', index_col=0).values
+X, y = dataset[:, 0:-1], dataset[:, -1]
+
+X_new, y_new = SMOTE().fit_resample(X, y)
+data = Data(X_new, y_new)
+```
+
++ 2nd: Use different random_state numbers in split_train_test() function.
+```python
+import pandas as pd 
+from mafese import Data 
+
+dataset = pd.read_csv('examples/dataset.csv', index_col=0).values
+X, y = dataset[:, 0:-1], dataset[:, -1]
+data = Data(X, y)
+data.split_train_test(test_size=0.2, random_state=10)   # Try different random_state value 
+```
+
 
 For more usage examples please look at [examples](/examples) folder.
 
 
 # Get helps (questions, problems)
 
 * Official source code repo: https://github.com/thieu1995/mafese
```

### Comparing `mafese-0.1.6/mafese/__init__.py` & `mafese-0.1.7/mafese/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 15:23, 06/03/2022 ----------%                                                                               
 #       Email: nguyenthieu2102@gmail.com            %                                                    
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
-__version__ = "0.1.6"
+__version__ = "0.1.7"
 
 from mafese.utils.data_loader import Data, get_dataset
 from mafese.filter import FilterSelector
 from mafese.wrapper.recursive import RecursiveSelector
 from mafese.wrapper.sequential import SequentialSelector
 from mafese.wrapper.mha import MhaSelector, MultiMhaSelector
 from mafese.embedded.lasso import LassoSelector
```

### Comparing `mafese-0.1.6/mafese/embedded/lasso.py` & `mafese-0.1.7/mafese/embedded/lasso.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.6/mafese/embedded/tree.py` & `mafese-0.1.7/mafese/embedded/tree.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.6/mafese/selector.py` & `mafese-0.1.7/mafese/selector.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.6/mafese/unsupervised.py` & `mafese-0.1.7/mafese/unsupervised.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.6/mafese/utils/data_loader.py` & `mafese-0.1.7/mafese/utils/data_loader.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.6/mafese/utils/encoder.py` & `mafese-0.1.7/mafese/utils/encoder.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.6/mafese/utils/estimator.py` & `mafese-0.1.7/mafese/utils/estimator.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.6/mafese/utils/evaluator.py` & `mafese-0.1.7/mafese/utils/evaluator.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.6/mafese/utils/mealpy_util.py` & `mafese-0.1.7/mafese/utils/mealpy_util.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.6/mafese/utils/transfer.py` & `mafese-0.1.7/mafese/utils/transfer.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.6/mafese/utils/validator.py` & `mafese-0.1.7/mafese/utils/validator.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.6/mafese/wrapper/mha.py` & `mafese-0.1.7/mafese/wrapper/mha.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     array([ 0, 1, 2, 5, 9])
     >>> # call transform() on X to filter it down to selected features
     >>> X_filtered = feat_selector.transform(X)
     """
 
     SUPPORT = {
         "estimator": ["knn", "svm", "rf", "adaboost", "xgb", "tree", "ann"],
-        "transfer_func": ["vstf_01", "vstf_02", "vstf_03", "vstf_04", "sstf_01", "sstf_02", "sstf_03", "sstf_04", "rtf"],
+        "transfer_func": ["vstf_01", "vstf_02", "vstf_03", "vstf_04", "sstf_01", "sstf_02", "sstf_03", "sstf_04"],
         "regression_objective": {"MAE": "min", "MSE": "min", "RMSE": "min", "MRE": "min", "MAPE": "min", "MASE": "min",
                              "NSE": "max", "NNSE": "max", "WI": "max", "PCC": "max", "R2s": "max", "R2": "max", "AR2": "max",
                              "CI": "max", "KGE": "max", "VAF": "max", "A10": "max", "A20": "max"},
         "classification_objective": {"AS": "max", "PS": "max", "NPV": "max", "RS": "max", "F1S": "max", "F2S": "max",
                              "FBS": "max", "SS": "max", "MCC": "max", "JSI": "max", "CKS": "max", "ROC-AUC": "max"},
         "optimizer": list(get_all_optimizers().keys())
     }
@@ -236,26 +236,17 @@
             "obj": self.optimizer.solution[1][1][1],
             "fit": self.optimizer.solution[1][1][0]
         }
 
 
 class MultiMhaSelector(Selector):
 
-    # SUPPORTED_ESTIMATORS = ["knn", "svm", "rf", "adaboost", "xgb", "tree", "ann"]
-    # SUPPORTED_TRANSFER_FUNCS = ["vstf_01", "vstf_02", "vstf_03", "vstf_04", "sstf_01", "sstf_02", "sstf_03", "sstf_04", "rtf"]
-    # SUPPORTED_REG_METRICS = {"MAE": "min", "MSE": "min", "RMSE": "min", "MRE": "min", "MAPE": "min", "MASE": "min",
-    #                          "NSE": "max", "NNSE": "max", "WI": "max", "PCC": "max", "R2s": "max", "R2": "max", "AR2": "max",
-    #                          "CI": "max", "KGE": "max", "VAF": "max", "A10": "max", "A20": "max"}
-    # SUPPORTED_CLS_METRICS = {"AS": "max", "PS": "max", "NPV": "max", "RS": "max", "F1S": "max", "F2S": "max",
-    #                          "FBS": "max", "SS": "max", "MCC": "max", "JSI": "max", "CKS": "max", "ROC-AUC": "max"}
-    # SUPPORTED_OPTIMIZERS = list(get_all_optimizers().keys())
-
     SUPPORT = {
         "estimator": ["knn", "svm", "rf", "adaboost", "xgb", "tree", "ann"],
-        "transfer_func": ["vstf_01", "vstf_02", "vstf_03", "vstf_04", "sstf_01", "sstf_02", "sstf_03", "sstf_04", "rtf"],
+        "transfer_func": ["vstf_01", "vstf_02", "vstf_03", "vstf_04", "sstf_01", "sstf_02", "sstf_03", "sstf_04"],
         "regression_objective": {"MAE": "min", "MSE": "min", "RMSE": "min", "MRE": "min", "MAPE": "min", "MASE": "min",
                              "NSE": "max", "NNSE": "max", "WI": "max", "PCC": "max", "R2s": "max", "R2": "max", "AR2": "max",
                              "CI": "max", "KGE": "max", "VAF": "max", "A10": "max", "A20": "max"},
         "classification_objective": {"AS": "max", "PS": "max", "NPV": "max", "RS": "max", "F1S": "max", "F2S": "max",
                              "FBS": "max", "SS": "max", "MCC": "max", "JSI": "max", "CKS": "max", "ROC-AUC": "max"},
         "optimizer": list(get_all_optimizers().keys())
     }
@@ -523,16 +514,15 @@
                 raise ValueError("trial index should be >= 1 and <= n_trials.")
 
     def fit_transform(self, X, y=None, n_trials=2, n_jobs=2, save_path="history", save_results=True,
                       verbose=True, fit_weights=(0.9, 0.1), mode='single', n_workers=None, termination=None):
         self.fit(X, y, n_trials, n_jobs, save_path, save_results, verbose, fit_weights, mode, n_workers, termination)
         return self.transform(X, trial=1, model="BaseGa", all_models=False)
 
-    def evaluate(self, estimator=None, estimator_paras=None, data=None, metrics=None,
-                 trial=1, model="BaseGA", all_models=False):
+    def evaluate(self, estimator=None, estimator_paras=None, data=None, metrics=None, save_path="history", verbose=False):
         """
         Evaluate the new dataset. We will re-train the estimator with training set
         and return the metrics of both training and testing set
 
         Parameters
         ----------
         estimator : str or Estimator instance (from scikit-learn or custom)
@@ -553,23 +543,19 @@
 
         data : Data, an instance of Data class. It must have training and testing set
 
         metrics : tuple, list, default = None
             Depend on the regression or classification you are trying to tackle. The supported metrics can be found at:
             https://github.com/thieu1995/permetrics
 
-        trial : int.
-            The index of i-th trial
-
-        model : str.
-            The name of the tested optimizer
+        save_path : str, default="history"
+            The path to save the file
 
-        all_models : bool, default = False
-            If True, it will ignore `trial` and `model` parameters. It will calculate metrics for all of models in all trials
-            If False, it will calculate the metrics for `model` in i-th `trial`
+        verbose : bool, default=False
+            Print the results to console or not.
 
         Returns
         -------
         metrics_results: dict.
             The metrics for both training and testing set.
         """
 
@@ -583,39 +569,24 @@
         elif (hasattr(estimator, 'fit') and hasattr(estimator, 'predict')) and (callable(estimator.fit) and callable(estimator.predict)):
             est_ = estimator
         else:
             raise NotImplementedError(f"Your estimator needs to implement at least 'fit' and 'predict' functions.")
         if (metrics is None) or (type(metrics) not in (tuple, list)):
             raise ValueError("You need to pass a tuple/list of performance metrics. See the supported metrics at https://github.com/thieu1995/permetrics")
         if isinstance(data, Data):
-            if all_models:
-                dict_results = {}
-                dict_X_train = self.transform(data.X_train, all_models=True)
-                dict_X_test = self.transform(data.X_test, all_models=True)
-                for trial_, model_ in dict_X_train.items():
-                    dict_results[trial_] = {}
-                    for name_, X_train_selected in model_.items():
-                        est_.fit(X_train_selected, data.y_train)
-                        y_train_pred = est_.predict(X_train_selected)
-                        y_test_pred = est_.predict(dict_X_test[trial_][name_])
-                        train_result = get_metrics(self.problem, data.y_train, y_train_pred, metrics=metrics, testcase="train")
-                        test_result = get_metrics(self.problem, data.y_test, y_test_pred, metrics=metrics, testcase="test")
-                        dict_results[trial_][name_] = {**train_result, **test_result}
-                return dict_results
-            else:
-                if type(trial) is int and 1 <= trial <= self.n_trials:
-                    list_models = [model.get_name() for model in self.list_optimizers]
-                    if type(model) is str and model in list_models:
-                        X_train = self.transform(data.X_train, trial, model)
-                        X_test = self.transform(data.X_test, trial, model)
-                        est_.fit(X_train, data.y_train)
-                        y_train_pred = est_.predict(X_train)
-                        y_test_pred = est_.predict(X_test)
-                        train_result = get_metrics(self.problem, data.y_train, y_train_pred, metrics=metrics, testcase="train")
-                        test_result = get_metrics(self.problem, data.y_test, y_test_pred, metrics=metrics, testcase="test")
-                        return {**train_result, **test_result}
-                    else:
-                        raise ValueError(f"model: {model} is not trained yet.")
-                else:
-                    raise ValueError("trial index should be >= 1 and <= n_trials.")
+            list_results = []
+            dict_X_train = self.transform(data.X_train, all_models=True)
+            dict_X_test = self.transform(data.X_test, all_models=True)
+            for trial_, model_ in dict_X_train.items():
+                for name_, X_train_selected in model_.items():
+                    est_.fit(X_train_selected, data.y_train)
+                    y_train_pred = est_.predict(X_train_selected)
+                    y_test_pred = est_.predict(dict_X_test[trial_][name_])
+                    train_result = get_metrics(self.problem, data.y_train, y_train_pred, metrics=metrics, testcase="train")
+                    test_result = get_metrics(self.problem, data.y_test, y_test_pred, metrics=metrics, testcase="test")
+                    list_results.append({"model": name_, "trial": trial_, **train_result, **test_result})
+            if verbose:
+                print(list_results)
+            df = pd.DataFrame(list_results)
+            df.to_csv(f"{save_path}/evaluation_results.csv", index_label="Index")
         else:
             raise ValueError("'data' should be an instance of Data class.")
```

### Comparing `mafese-0.1.6/mafese/wrapper/recursive.py` & `mafese-0.1.7/mafese/wrapper/recursive.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.6/mafese/wrapper/sequential.py` & `mafese-0.1.7/mafese/wrapper/sequential.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.6/mafese.egg-info/PKG-INFO` & `mafese-0.1.7/mafese.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: mafese
-Version: 0.1.6
+Version: 0.1.7
 Summary: MAFESE: Metaheuristic Algorithm for Feature Selection - An Open Source Python Library
 Home-page: https://github.com/thieu1995/mafese
 Author: Thieu
 Author-email: nguyenthieu2102@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://mafese.readthedocs.io/
 Project-URL: Source Code, https://github.com/thieu1995/mafese
 Project-URL: Bug Tracker, https://github.com/thieu1995/mafese/issues
 Project-URL: Change Log, https://github.com/thieu1995/mafese/blob/master/ChangeLog.md
 Project-URL: Forum, https://t.me/+fRVCJGuGJg1mNDg1
-Keywords: engineering optimization problems,mathematical optimization,feature selection,classification problem,feature selector,dimensionality reduction,subset selection,wrapper methods,embedded methods,mutual information,correlation-based feature selection,recursive feature selection,principal component analysis,PCA,lasso regularization,ridge regularization,Genetic algorithm (GA),Particle swarm optimization (PSO),Ant colony optimization (ACO),Differential evolution (DE),Simulated annealing,Grey wolf optimizer (GWO),Whale Optimization Algorithm (WOA),confusion matrix,recall,precision,accuracy,K-Nearest Neighbors,random forest,support vector machine,pearson correlation coefficient (PCC),spearman correlation coefficient (SCC),relief,multi-objectives optimization problems,Stochastic optimization,Global optimization,Convergence analysis,Search space exploration,Local search,Computational intelligence,Robust optimization,Performance analysis,Intelligent optimization,Simulations
+Keywords: engineering optimization problems,mathematical optimization,feature selection,classification problem,feature selector,dimensionality reduction,subset selection,wrapper methods,embedded methods,mutual information,correlation-based feature selection,recursive feature selection,principal component analysis,PCA,lasso regularization,ridge regularization,Genetic algorithm (GA),Particle swarm optimization (PSO),Ant colony optimization (ACO),Differential evolution (DE),Simulated annealing,Grey wolf optimizer (GWO),Whale Optimization Algorithm (WOA),confusion matrix,recall,precision,accuracy,K-Nearest Neighbors,random forest,support vector machine,pearson correlation coefficient (PCC),spearman correlation coefficient (SCC),relief,relief-f,multi-objectives optimization problems,Stochastic optimization,Global optimization,Convergence analysis,Search space exploration,Local search,Computational intelligence,Robust optimization,Performance analysis,Intelligent optimization,Simulations
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
@@ -43,15 +43,15 @@
 
 
 <p align="center"><img style="height:300px;" src=".github/img/logo.png" alt="MAFESE" title="MAFESE"/></p>
 
 ---
 
 
-[![GitHub release](https://img.shields.io/badge/release-0.1.6-yellow.svg)](https://github.com/thieu1995/mafese/releases)
+[![GitHub release](https://img.shields.io/badge/release-0.1.7-yellow.svg)](https://github.com/thieu1995/mafese/releases)
 [![Wheel](https://img.shields.io/pypi/wheel/gensim.svg)](https://pypi.python.org/pypi/mafese) 
 [![PyPI version](https://badge.fury.io/py/mafese.svg)](https://badge.fury.io/py/mafese)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mafese.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/mafese.svg)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mafese.svg)
 [![Downloads](https://pepy.tech/badge/mafese)](https://pepy.tech/project/mafese)
 [![Tests & Publishes to PyPI](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml/badge.svg)](https://github.com/thieu1995/mafese/actions/workflows/publish-package.yaml)
@@ -65,15 +65,15 @@
 
 
 MAFESE (Metaheuristic Algorithms for FEature SElection) is the largest python library for feature selection problem 
 using meta-heuristic algorithms. 
 
 * **Free software:** GNU General Public License (GPL) V3 license
 * **Total Wrapper-based (Metaheuristic Algorithms)**: > 180 methods
-* **Total Filter-based (Statistical-based)**: > 12 methods
+* **Total Filter-based (Statistical-based)**: > 15 methods
 * **Total Embedded-based (Tree and Lasso)**: > 10 methods
 * **Total Unsupervised-based**: >= 4 methods
 * **Total classification dataset**: >= 30 datasets
 * **Total regression dataset**: >= 7 datasets
 * **Total performance metrics (as fitness)**: > 30 metrics
 * **Documentation:** https://mafese.readthedocs.io/en/latest/
 * **Python versions:** 3.7.x, 3.8.x, 3.9.x, 3.10.x, 3.11.x
@@ -82,15 +82,15 @@
 
 # Installation
 
 ### Install with pip
 
 Install the [current PyPI release](https://pypi.python.org/pypi/mafese):
 ```sh 
-$ pip install mafese==0.1.6
+$ pip install mafese==0.1.7
 ```
 
 ### Install directly from source code
 ```sh 
 $ git clone https://github.com/thieu1995/mafese.git
 $ cd mafese
 $ python setup.py install
@@ -100,17 +100,22 @@
 ### Lib's structure
 
 ```code 
 docs
 examples
 mafese
     data/
-        Arrhythmia.csv
-        BreastCancer.csv
-        ...
+        cls/
+            aggregation.csv
+            Arrhythmia.csv
+            ...
+        reg/
+            boston-housing.csv
+            diabetes.csv
+            ...
     wrapper/
         mha.py
         recursive.py
         sequential.py
     embedded/
         lasso.py
         tree.py
@@ -275,14 +280,53 @@
 
 2) How do I know my Selector support which estimator? which methods?
 ```python 
 print(feat_selector.SUPPORT) 
 ```
 Or you better read the document from: https://mafese.readthedocs.io/en/latest/
 
+3) I got this type of error
+```python 
+raise ValueError("Existed at least one new label in y_pred.")
+ValueError: Existed at least one new label in y_pred.
+``` 
+How to solve this?
+
++ This occurs only when you are working on a classification problem with a small dataset that has many classes. For 
+  instance, the "Zoo" dataset contains only 101 samples, but it has 7 classes. If you split the dataset into a 
+  training and testing set with a ratio of around 80% - 20%, there is a chance that one or more classes may appear 
+  in the testing set but not in the training set. As a result, when you calculate the performance metrics, you may 
+  encounter this error. You cannot predict or assign new data to a new label because you have no knowledge about the 
+  new label. There are several solutions to this problem.
+
++ 1st: Use the SMOTE method to address imbalanced data and ensure that all classes have the same number of samples.
+
+```python 
+from imblearn.over_sampling import SMOTE
+import pandas as pd
+from mafese import Data
+
+dataset = pd.read_csv('examples/dataset.csv', index_col=0).values
+X, y = dataset[:, 0:-1], dataset[:, -1]
+
+X_new, y_new = SMOTE().fit_resample(X, y)
+data = Data(X_new, y_new)
+```
+
++ 2nd: Use different random_state numbers in split_train_test() function.
+```python
+import pandas as pd 
+from mafese import Data 
+
+dataset = pd.read_csv('examples/dataset.csv', index_col=0).values
+X, y = dataset[:, 0:-1], dataset[:, -1]
+data = Data(X, y)
+data.split_train_test(test_size=0.2, random_state=10)   # Try different random_state value 
+```
+
 
 For more usage examples please look at [examples](/examples) folder.
 
 
 # Get helps (questions, problems)
 
 * Official source code repo: https://github.com/thieu1995/mafese
```

### Comparing `mafese-0.1.6/mafese.egg-info/SOURCES.txt` & `mafese-0.1.7/mafese.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mafese-0.1.6/setup.py` & `mafese-0.1.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,30 +11,30 @@
     with open('README.md', encoding='utf-8') as f:
         README = f.read()
     return README
 
 
 setup(
     name="mafese",
-    version="0.1.6",
+    version="0.1.7",
     author="Thieu",
     author_email="nguyenthieu2102@gmail.com",
     description="MAFESE: Metaheuristic Algorithm for Feature Selection - An Open Source Python Library",
     long_description=readme(),
     long_description_content_type="text/markdown",
     keywords=["engineering optimization problems", "mathematical optimization",
               "feature selection", "classification problem",
               "feature selector", "dimensionality reduction",
               "subset selection", "wrapper methods", "embedded methods", "mutual information", "correlation-based feature selection",
               "recursive feature selection", "principal component analysis", "PCA", "lasso regularization", "ridge regularization",
               "Genetic algorithm (GA)", "Particle swarm optimization (PSO)", "Ant colony optimization (ACO)",
               "Differential evolution (DE)", "Simulated annealing", "Grey wolf optimizer (GWO)", "Whale Optimization Algorithm (WOA)",
               "confusion matrix", "recall", "precision", "accuracy", "K-Nearest Neighbors", "random forest",
               "support vector machine", "pearson correlation coefficient (PCC)", "spearman correlation coefficient (SCC)",
-              "relief", "multi-objectives optimization problems", "Stochastic optimization", "Global optimization",
+              "relief", "relief-f", "multi-objectives optimization problems", "Stochastic optimization", "Global optimization",
               "Convergence analysis", "Search space exploration", "Local search", "Computational intelligence", "Robust optimization",
               "Performance analysis", "Intelligent optimization", "Simulations"],
     url="https://github.com/thieu1995/mafese",
     project_urls={
         'Documentation': 'https://mafese.readthedocs.io/',
         'Source Code': 'https://github.com/thieu1995/mafese',
         'Bug Tracker': 'https://github.com/thieu1995/mafese/issues',
```

### Comparing `mafese-0.1.6/tests/test_embedded.py` & `mafese-0.1.7/tests/test_embedded.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.6/tests/test_filter.py` & `mafese-0.1.7/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.6/tests/test_unsupervised.py` & `mafese-0.1.7/tests/test_unsupervised.py`

 * *Files identical despite different names*

### Comparing `mafese-0.1.6/tests/test_wrapper.py` & `mafese-0.1.7/tests/test_wrapper.py`

 * *Files identical despite different names*

