# Comparing `tmp/treeordination-1.3.2.tar.gz` & `tmp/treeordination-1.3.3.tar.gz`

## Comparing `treeordination-1.3.2.tar` & `treeordination-1.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 treeordination-1.3.2/environment.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 treeordination-1.3.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 treeordination-1.3.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 treeordination-1.3.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 treeordination-1.3.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     8766 2020-02-02 00:00:00.000000 treeordination-1.3.2/TreeOrdination/TreeOrdination.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 treeordination-1.3.2/TreeOrdination/__init__.py
--rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 treeordination-1.3.2/TreeOrdination/feature_importance_treeord.py
--rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 treeordination-1.3.2/TreeOrdination/transformers_treeord.py
--rw-r--r--   0        0        0     9119 2020-02-02 00:00:00.000000 treeordination-1.3.2/docs/API.md
--rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 treeordination-1.3.2/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 treeordination-1.3.2/notebooks/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 treeordination-1.3.2/tests/__init__.py
--rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 treeordination-1.3.2/tests/test_treeord.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 treeordination-1.3.2/.gitignore
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 treeordination-1.3.2/LICENSE
--rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 treeordination-1.3.2/README.md
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 treeordination-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     5821 2020-02-02 00:00:00.000000 treeordination-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 treeordination-1.3.3/environment.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 treeordination-1.3.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 treeordination-1.3.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 treeordination-1.3.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 treeordination-1.3.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     9137 2020-02-02 00:00:00.000000 treeordination-1.3.3/TreeOrdination/TreeOrdination.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 treeordination-1.3.3/TreeOrdination/__init__.py
+-rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 treeordination-1.3.3/TreeOrdination/feature_importance_treeord.py
+-rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 treeordination-1.3.3/TreeOrdination/transformers_treeord.py
+-rw-r--r--   0        0        0     9119 2020-02-02 00:00:00.000000 treeordination-1.3.3/docs/API.md
+-rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 treeordination-1.3.3/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 treeordination-1.3.3/notebooks/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 treeordination-1.3.3/tests/__init__.py
+-rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 treeordination-1.3.3/tests/test_treeord.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 treeordination-1.3.3/.gitignore
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 treeordination-1.3.3/LICENSE
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 treeordination-1.3.3/README.md
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 treeordination-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     5646 2020-02-02 00:00:00.000000 treeordination-1.3.3/PKG-INFO
```

### Comparing `treeordination-1.3.2/.github/ISSUE_TEMPLATE/bug_report.md` & `treeordination-1.3.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `treeordination-1.3.2/.github/ISSUE_TEMPLATE/feature_request.md` & `treeordination-1.3.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `treeordination-1.3.2/.github/workflows/ci.yml` & `treeordination-1.3.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `treeordination-1.3.2/.github/workflows/python-publish.yml` & `treeordination-1.3.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `treeordination-1.3.2/TreeOrdination/TreeOrdination.py` & `treeordination-1.3.3/TreeOrdination/TreeOrdination.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import numpy as np
  
 from sklearn.ensemble import ExtraTreesClassifier, ExtraTreesRegressor
 from sklearn.preprocessing import LabelEncoder
 from sklearn.base import ClassifierMixin, BaseEstimator, clone
 from sklearn.decomposition import PCA
 
+from scipy.sparse import csr_array
+from scipy.sparse import hstack as sp_hstack
+
 from umap import UMAP
 
 from LANDMark import LANDMarkClassifier
 
 from matplotlib import pyplot as plt
 
 import seaborn as sns
@@ -57,14 +60,15 @@
 # Tree Ordination class
 class TreeOrdination(ClassifierMixin, BaseEstimator):
     def __init__(
         self,
         feature_names,
         resampler=None,
         metric="hamming",
+        prox_method = "terminal",
         supervised_clf=ExtraTreesClassifier(1024),
         proxy_model = ExtraTreesRegressor(1024),
         landmark_model = LANDMarkClassifier(160, use_nnet=False, n_jobs = 8),
         n_iter_unsup=5,
         transformer=None,
         exclude_col=[False, 0],
         n_neighbors=8,
@@ -72,14 +76,15 @@
         min_dist=0.001,
     ):
         self.feature_names = feature_names
 
         self.resampler = resampler
 
         self.metric = metric
+        self.prox_method = prox_method
 
         self.supervised_clf = supervised_clf
         self.proxy_model = proxy_model
         self.landmark_model = landmark_model
 
         self.n_iter_unsup = n_iter_unsup
 
@@ -113,28 +118,30 @@
             model = clone(self.landmark_model)
 
             model.fit(X_rand, y_rand)
             self.Rs.append(model)
 
             # Get proximity
             X_trf = resampler.transform(X)
-            self.LM_emb.append(model.proximity(X_trf))
+
+            # Update Overall Proximity
+            if i > 0:
+                self.LM_emb = sp_hstack((self.LM_emb, model.proximity(X_trf, self.prox_method)))
+            else:
+                self.LM_emb = model.proximity(X_trf, self.prox_method)
 
             # Save the resampler
             self.transformers.append(resampler)
 
-        # Get Overall Proximity
-        self.LM_emb = np.hstack(self.LM_emb)
-
         # Get Embeddings
         self.UMAP_trf = UMAP(
             n_neighbors=self.n_neighbors,
             n_components=15,
             min_dist=self.min_dist,
-            metric=self.metric,
+            metric="hamming",
             densmap=False,
         ).fit(self.LM_emb)
 
         self.UMAP_emb = self.UMAP_trf.transform(self.LM_emb)
 
         self.PCA_trf = PCA(self.n_components, whiten = True).fit(self.UMAP_emb)
 
@@ -244,15 +251,15 @@
 
         ax.legend(loc="center left", bbox_to_anchor=(1, 0.5))
 
         return fig, ax
 
     def predict_proba(self, X):
 
-        tree_emb = self.emb_transform(X, "LM")
+        tree_emb = self.emb_transform(X, "UMAP")
 
         P = self.p_model.predict_proba(tree_emb)
 
         return P
 
     def predict(self, X):
 
@@ -277,19 +284,18 @@
             for i in range(self.n_iter_unsup):
 
                 # Get trained model
                 model = self.Rs[i]
                 transformer = self.transformers[i]
 
                 # Get proximity
-                proximity = model.proximity(transformer.transform(X))
-
-                tree_emb.append(proximity)
-
-            tree_emb = np.hstack(tree_emb)
+                if i != 0:
+                    tree_emb = sp_hstack((tree_emb, model.proximity(transformer.transform(X), self.prox_method)))
+                else:
+                    tree_emb = model.proximity(transformer.transform(X), self.prox_method)
 
             if trf_type == "LM":
                 return tree_emb
 
             umap_emb = self.UMAP_trf.transform(tree_emb)
             if trf_type == "UMAP":
                 return umap_emb
```

### Comparing `treeordination-1.3.2/TreeOrdination/feature_importance_treeord.py` & `treeordination-1.3.3/TreeOrdination/feature_importance_treeord.py`

 * *Files identical despite different names*

### Comparing `treeordination-1.3.2/TreeOrdination/transformers_treeord.py` & `treeordination-1.3.3/TreeOrdination/transformers_treeord.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 
         self.do_clr = do_clr
         self.delta = delta
 
     def fit_transform(self, X, y=None, **kwargs):
 
         if self.do_clr:
-            return clr(multiplicative_replacement(closure(X), delta=self.delta))
+            return clr(multiplicative_replacement(closure(X), delta=self.delta)).astype(np.float32)
 
         else:
-            return closure(X)
+            return closure(X).astype(np.float32)
 
     def transform(self, X, y=None, **kwargs):
 
         if self.do_clr:
-            return clr(multiplicative_replacement(closure(X), delta=self.delta))
+            return clr(multiplicative_replacement(closure(X), delta=self.delta)).astype(np.float32)
 
         else:
-            return closure(X)
+            return closure(X).astype(np.float32)
 
 
 class ResampleRandomizeTransform(BaseEstimator, TransformerMixin):
     def __init__(self, resampler, transformer, exclude_cols):
 
         self.resampler = resampler
         self.transformer = transformer
```

### Comparing `treeordination-1.3.2/docs/API.md` & `treeordination-1.3.3/docs/API.md`

 * *Files identical despite different names*

### Comparing `treeordination-1.3.2/docs/CONTRIBUTING.md` & `treeordination-1.3.3/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `treeordination-1.3.2/tests/test_treeord.py` & `treeordination-1.3.3/tests/test_treeord.py`

 * *Files identical despite different names*

### Comparing `treeordination-1.3.2/.gitignore` & `treeordination-1.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `treeordination-1.3.2/LICENSE` & `treeordination-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `treeordination-1.3.2/README.md` & `treeordination-1.3.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -67,10 +67,7 @@
    
 Geurts P, Ernst D, Wehenkel L. Extremely Randomized Trees. Machine Learning. 2006;63(1):3–42.
     
 Rudar, J., Golding, G.B., Kremer, S.C., Hajibabaei, M. (2023). Decision Tree Ensembles Utilizing 
 Multivariate Splits Are Effective at Investigating Beta Diversity in Medically Relevant 16S Amplicon 
 Sequencing Data. Microbiology Spectrum e02065-22.
 
-Klaise J., Van Looveren A., Vacanti G., and Coca A. Alibi Explain: Algorithms for Explaining Machine
-Learning Models. Journal of Machine Learning Research. 2021;22(181):1-7.
-
```

### Comparing `treeordination-1.3.2/pyproject.toml` & `treeordination-1.3.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "TreeOrdination"
-version = "1.3.2"
+version = "1.3.3"
 authors = [
     {name = "Josip Rudar", email = "rudarj@uoguelph.ca"},
     {name = "G. Brian Golding"},
     {name = "Stefan C. Kremer"},
     {name = "Mehrdad Hajibabaei", email = "mhajibab@uoguelph.ca"}
 ]
 description = "Projection of High-Dimensional Data Using Multivariate Decision Trees and UMAP"
@@ -36,15 +36,15 @@
 dependencies = [
     "numpy == 1.23.5",
     "scikit-learn >= 1.1.2",
     "scikit-bio >= 0.5.8",
     "umap-learn >= 0.5.3",
     "seaborn",
     "shap >= 0.40.0",
-    "LANDMarkClassifier >= 2.0.4"
+    "LANDMarkClassifier >= 2.1.0"
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project.urls]
 "Homepage" = "https://github.com/jrudar/TreeOrdination"
```

### Comparing `treeordination-1.3.2/PKG-INFO` & `treeordination-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TreeOrdination
-Version: 1.3.2
+Version: 1.3.3
 Summary: Projection of High-Dimensional Data Using Multivariate Decision Trees and UMAP
 Project-URL: Homepage, https://github.com/jrudar/TreeOrdination
 Project-URL: Repository, https://github.com/jrudar/TreeOrdination.git
 Project-URL: Bug Tracker, https://github.com/jrudar/TreeOrdination/issues
 Author: G. Brian Golding, Stefan C. Kremer
 Author-email: Josip Rudar <rudarj@uoguelph.ca>, Mehrdad Hajibabaei <mhajibab@uoguelph.ca>
 License: MIT License
@@ -38,15 +38,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
-Requires-Dist: landmarkclassifier>=2.0.4
+Requires-Dist: landmarkclassifier>=2.1.0
 Requires-Dist: numpy==1.23.5
 Requires-Dist: scikit-bio>=0.5.8
 Requires-Dist: scikit-learn>=1.1.2
 Requires-Dist: seaborn
 Requires-Dist: shap>=0.40.0
 Requires-Dist: umap-learn>=0.5.3
 Provides-Extra: dev
@@ -128,10 +128,7 @@
    
 Geurts P, Ernst D, Wehenkel L. Extremely Randomized Trees. Machine Learning. 2006;63(1):3–42.
     
 Rudar, J., Golding, G.B., Kremer, S.C., Hajibabaei, M. (2023). Decision Tree Ensembles Utilizing 
 Multivariate Splits Are Effective at Investigating Beta Diversity in Medically Relevant 16S Amplicon 
 Sequencing Data. Microbiology Spectrum e02065-22.
 
-Klaise J., Van Looveren A., Vacanti G., and Coca A. Alibi Explain: Algorithms for Explaining Machine
-Learning Models. Journal of Machine Learning Research. 2021;22(181):1-7.
-
```

