# Comparing `tmp/ProcessPLS-1.8.tar.gz` & `tmp/ProcessPLS-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProcessPLS-1.8.tar", last modified: Thu Feb  9 13:14:37 2023, max compression
+gzip compressed data, was "ProcessPLS-1.9.tar", last modified: Thu Jul 13 12:16:41 2023, max compression
```

## Comparing `ProcessPLS-1.8.tar` & `ProcessPLS-1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-02-09 13:14:37.878797 ProcessPLS-1.8/
--rw-rw-rw-   0        0        0     1348 2023-02-09 13:06:53.000000 ProcessPLS-1.8/LICENSE
--rw-rw-rw-   0        0        0     5192 2023-02-09 13:14:37.878797 ProcessPLS-1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-02-09 13:14:37.852794 ProcessPLS-1.8/ProcessPLS.egg-info/
--rw-rw-rw-   0        0        0     5192 2023-02-09 13:14:37.000000 ProcessPLS-1.8/ProcessPLS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2023-02-09 13:14:37.000000 ProcessPLS-1.8/ProcessPLS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-09 13:14:37.000000 ProcessPLS-1.8/ProcessPLS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-02-09 13:14:37.000000 ProcessPLS-1.8/ProcessPLS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-02-09 13:14:37.000000 ProcessPLS-1.8/ProcessPLS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4413 2023-02-09 13:06:53.000000 ProcessPLS-1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-02-09 13:14:37.862808 ProcessPLS-1.8/processPLS/
--rw-rw-rw-   0        0        0        0 2023-02-09 13:06:53.000000 ProcessPLS-1.8/processPLS/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-09 13:14:37.877795 ProcessPLS-1.8/processPLS/data/
--rw-rw-rw-   0        0        0  5768466 2023-02-09 13:06:53.000000 ProcessPLS-1.8/processPLS/data/OilDistillationData.csv
--rw-rw-rw-   0        0        0     3919 2023-02-09 13:06:53.000000 ProcessPLS-1.8/processPLS/data/ValdeLoirData.csv
--rw-rw-rw-   0        0        0        0 2023-02-09 13:06:53.000000 ProcessPLS-1.8/processPLS/data/__init__.py
--rw-rw-rw-   0        0        0     2454 2023-02-09 13:06:53.000000 ProcessPLS-1.8/processPLS/datasets.py
--rw-rw-rw-   0        0        0    27625 2023-02-09 13:10:21.000000 ProcessPLS-1.8/processPLS/model.py
--rw-rw-rw-   0        0        0       86 2023-02-09 13:14:37.880795 ProcessPLS-1.8/setup.cfg
--rw-rw-rw-   0        0        0     1509 2023-02-09 13:13:44.000000 ProcessPLS-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:16:41.502702 ProcessPLS-1.9/
+-rw-rw-rw-   0        0        0     1348 2023-02-09 13:06:53.000000 ProcessPLS-1.9/LICENSE
+-rw-rw-rw-   0        0        0     5194 2023-07-13 12:16:41.502702 ProcessPLS-1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-13 12:16:41.471704 ProcessPLS-1.9/ProcessPLS.egg-info/
+-rw-rw-rw-   0        0        0     5194 2023-07-13 12:16:41.000000 ProcessPLS-1.9/ProcessPLS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2023-07-13 12:16:41.000000 ProcessPLS-1.9/ProcessPLS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 12:16:41.000000 ProcessPLS-1.9/ProcessPLS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-07-13 12:16:41.000000 ProcessPLS-1.9/ProcessPLS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-13 12:16:41.000000 ProcessPLS-1.9/ProcessPLS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4415 2023-07-13 12:07:25.000000 ProcessPLS-1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 12:16:41.482702 ProcessPLS-1.9/processPLS/
+-rw-rw-rw-   0        0        0        0 2023-02-09 13:06:53.000000 ProcessPLS-1.9/processPLS/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 12:16:41.501703 ProcessPLS-1.9/processPLS/data/
+-rw-rw-rw-   0        0        0  5768466 2023-02-09 13:06:53.000000 ProcessPLS-1.9/processPLS/data/OilDistillationData.csv
+-rw-rw-rw-   0        0        0     3919 2023-02-09 13:06:53.000000 ProcessPLS-1.9/processPLS/data/ValdeLoirData.csv
+-rw-rw-rw-   0        0        0        0 2023-02-09 13:06:53.000000 ProcessPLS-1.9/processPLS/data/__init__.py
+-rw-rw-rw-   0        0        0     2454 2023-02-09 13:06:53.000000 ProcessPLS-1.9/processPLS/datasets.py
+-rw-rw-rw-   0        0        0    27621 2023-07-13 12:00:33.000000 ProcessPLS-1.9/processPLS/model.py
+-rw-rw-rw-   0        0        0       86 2023-07-13 12:16:41.504703 ProcessPLS-1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1509 2023-07-13 12:16:18.000000 ProcessPLS-1.9/setup.py
```

### Comparing `ProcessPLS-1.8/LICENSE` & `ProcessPLS-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ProcessPLS-1.8/PKG-INFO` & `ProcessPLS-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProcessPLS
-Version: 1.8
+Version: 1.9
 Summary: Implementation of ProcessPLS in Python
 Home-page: UNKNOWN
 Author: Sin Yong Teng
 Author-email: tsyet12@gmail.com
 License: BSD 2-Clause
 Keywords: Path Modelling,Chemometrics,Process Analytical Technology,Machine Learning
 Platform: UNKNOWN
@@ -78,15 +78,15 @@
 ```
 
 ## Call and Fit the Process PLS model
 ```python
 import matplotlib.pyplot as plt
 model = ProcessPLS()
 model.fit(X,Y,matrix)
-model.plot
+model.plot()
 plt.show()
 ```
 
 ## Main Function Arguments
 ```python
 Process_PLS(cv=RepeatedKFold(n_splits=5,n_repeats=2,random_state=999),scoring='neg_mean_squared_error',max_lv=30,overwrite_lv=False,inner_forced_lv=None,outer_forced_lv=None,name=None)
```

### Comparing `ProcessPLS-1.8/ProcessPLS.egg-info/PKG-INFO` & `ProcessPLS-1.9/ProcessPLS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProcessPLS
-Version: 1.8
+Version: 1.9
 Summary: Implementation of ProcessPLS in Python
 Home-page: UNKNOWN
 Author: Sin Yong Teng
 Author-email: tsyet12@gmail.com
 License: BSD 2-Clause
 Keywords: Path Modelling,Chemometrics,Process Analytical Technology,Machine Learning
 Platform: UNKNOWN
@@ -78,15 +78,15 @@
 ```
 
 ## Call and Fit the Process PLS model
 ```python
 import matplotlib.pyplot as plt
 model = ProcessPLS()
 model.fit(X,Y,matrix)
-model.plot
+model.plot()
 plt.show()
 ```
 
 ## Main Function Arguments
 ```python
 Process_PLS(cv=RepeatedKFold(n_splits=5,n_repeats=2,random_state=999),scoring='neg_mean_squared_error',max_lv=30,overwrite_lv=False,inner_forced_lv=None,outer_forced_lv=None,name=None)
```

### Comparing `ProcessPLS-1.8/README.md` & `ProcessPLS-1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 ```
 
 ## Call and Fit the Process PLS model
 ```python
 import matplotlib.pyplot as plt
 model = ProcessPLS()
 model.fit(X,Y,matrix)
-model.plot
+model.plot()
 plt.show()
 ```
 
 ## Main Function Arguments
 ```python
 Process_PLS(cv=RepeatedKFold(n_splits=5,n_repeats=2,random_state=999),scoring='neg_mean_squared_error',max_lv=30,overwrite_lv=False,inner_forced_lv=None,outer_forced_lv=None,name=None)
```

### Comparing `ProcessPLS-1.8/processPLS/data/OilDistillationData.csv` & `ProcessPLS-1.9/processPLS/data/OilDistillationData.csv`

 * *Files identical despite different names*

### Comparing `ProcessPLS-1.8/processPLS/data/ValdeLoirData.csv` & `ProcessPLS-1.9/processPLS/data/ValdeLoirData.csv`

 * *Files identical despite different names*

### Comparing `ProcessPLS-1.8/processPLS/datasets.py` & `ProcessPLS-1.9/processPLS/datasets.py`

 * *Files identical despite different names*

### Comparing `ProcessPLS-1.8/processPLS/model.py` & `ProcessPLS-1.9/processPLS/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -389,17 +389,17 @@
           outer_x_weights=inner_scaler_x.transform(simpls.x_weights_)
           ##scale scores and weights for y
           inner_scaler_y=InnerScaler()
           outer_y_scores=inner_scaler_y.fit_transform(simpls.y_scores_,simpls.yfrac_var_)
           outer_y_weights=inner_scaler_y.transform(simpls.y_weights_) #y weights are scaled
           G.add_node(node,outer_model=simpls,inner_scaler_x=inner_scaler_x,inner_scaler_y=inner_scaler_y,outer_x_scores=outer_x_scores,outer_x_weights=outer_x_weights,outer_y_scores=outer_y_scores,outer_y_weights=outer_y_weights) #put models in graph
           if node not in list(Y.keys()):     #only choose nodes which are not the 'end node'
-              G.add_node(node,exp_var=simpls.xfrac_var_,R2m=np.trace(simpls.x_loadings_.T*simpls.x_loadings_.T)/(simpls.x_scores_.shape[0]-1))
+              G.add_node(node,exp_var=simpls.xfrac_var_,R2m=np.trace(simpls.x_loadings_.T@simpls.x_loadings_)/(simpls.x_scores_.shape[0]-1))
           else:
-              G.add_node(node,exp_var=simpls.yfrac_var_,R2m=np.trace(simpls.y_loadings_.T*simpls.y_loadings_.T)/(simpls.y_scores_.shape[0]-1))
+              G.add_node(node,exp_var=simpls.yfrac_var_,R2m=np.trace(simpls.y_loadings_.T@simpls.y_loadings_)/(simpls.y_scores_.shape[0]-1))
           
       ######## INNER MODEL###########
       ##Make the inner models on target nodes##
       for node in G: #loop through chosen nodes
           inner_x=np.array([]) #define array to store inner x
           inner_x_size=[] #define list to store inner x size accumulatively
           pred_list=list(G.predecessors(node)) #set the pred list for predecessor nodes
```

### Comparing `ProcessPLS-1.8/setup.py` & `ProcessPLS-1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 install_requires = [] 
 if os.path.isfile(requirementPath):
     with open(requirementPath) as f:
         install_requires = f.read().splitlines()
 
 
 setup(name='ProcessPLS', 
-version='1.08', 
+version='1.09', 
 license='BSD 2-Clause',
 description="Implementation of ProcessPLS in Python",
 author='Sin Yong Teng',
 long_description=long_description,
 long_description_content_type="text/markdown",
 author_email='tsyet12@gmail.com',
 keywords = ['Path Modelling', 'Chemometrics', 'Process Analytical Technology', 'Machine Learning'],
```

