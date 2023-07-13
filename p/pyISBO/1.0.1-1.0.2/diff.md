# Comparing `tmp/pyISBO-1.0.1.tar.gz` & `tmp/pyISBO-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyISBO-1.0.1.tar", last modified: Thu Jul 13 01:32:34 2023, max compression
+gzip compressed data, was "dist\pyISBO-1.0.2.tar", last modified: Thu Jul 13 07:04:33 2023, max compression
```

## Comparing `pyISBO-1.0.1.tar` & `pyISBO-1.0.2.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 01:32:34.000000 pyISBO-1.0.1/
--rw-rw-rw-   0        0        0      304 2023-07-13 01:32:34.000000 pyISBO-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-13 01:32:34.000000 pyISBO-1.0.1/pyISBO/
-drwxrwxrwx   0        0        0        0 2023-07-13 01:32:34.000000 pyISBO-1.0.1/pyISBO/SBO_grb/
--rw-rw-rw-   0        0        0     4455 2023-07-13 01:19:56.000000 pyISBO-1.0.1/pyISBO/SBO_grb/AutoRegression.py
--rw-rw-rw-   0        0        0     7041 2023-07-12 11:17:06.000000 pyISBO-1.0.1/pyISBO/SBO_grb/DecisionTree.py
--rw-rw-rw-   0        0        0     4071 2023-07-12 09:58:51.000000 pyISBO-1.0.1/pyISBO/SBO_grb/LinearRegression.py
--rw-rw-rw-   0        0        0     5305 2023-07-12 09:58:51.000000 pyISBO-1.0.1/pyISBO/SBO_grb/LogisticRegression.py
--rw-rw-rw-   0        0        0     6989 2023-07-12 09:58:51.000000 pyISBO-1.0.1/pyISBO/SBO_grb/NeuralNetwork.py
--rw-rw-rw-   0        0        0     4438 2023-07-12 09:58:51.000000 pyISBO-1.0.1/pyISBO/SBO_grb/QuadraticRegression.py
--rw-rw-rw-   0        0        0     6850 2023-07-12 11:17:06.000000 pyISBO-1.0.1/pyISBO/SBO_grb/RandomForest.py
--rw-rw-rw-   0        0        0     6530 2023-07-12 09:58:51.000000 pyISBO-1.0.1/pyISBO/SBO_grb/RegressionSplines.py
--rw-rw-rw-   0        0        0        0 2023-04-03 12:01:13.000000 pyISBO-1.0.1/pyISBO/SBO_grb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 01:32:34.000000 pyISBO-1.0.1/pyISBO/SBO_pulp/
--rw-rw-rw-   0        0        0     4191 2023-07-13 01:19:56.000000 pyISBO-1.0.1/pyISBO/SBO_pulp/AutoRegression.py
--rw-rw-rw-   0        0        0     6902 2023-07-12 11:17:06.000000 pyISBO-1.0.1/pyISBO/SBO_pulp/DecisionTree.py
--rw-rw-rw-   0        0        0     3889 2023-07-12 09:58:51.000000 pyISBO-1.0.1/pyISBO/SBO_pulp/LinearRegression.py
--rw-rw-rw-   0        0        0     5224 2023-07-12 09:58:51.000000 pyISBO-1.0.1/pyISBO/SBO_pulp/LogisticRegression.py
--rw-rw-rw-   0        0        0     6882 2023-07-12 09:58:51.000000 pyISBO-1.0.1/pyISBO/SBO_pulp/NeuralNetwork.py
--rw-rw-rw-   0        0        0     7632 2023-07-12 11:17:06.000000 pyISBO-1.0.1/pyISBO/SBO_pulp/RandomForest.py
--rw-rw-rw-   0        0        0     6322 2023-07-12 09:58:51.000000 pyISBO-1.0.1/pyISBO/SBO_pulp/RegressionSplines.py
--rw-rw-rw-   0        0        0        0 2023-04-03 12:01:13.000000 pyISBO-1.0.1/pyISBO/SBO_pulp/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-03 12:01:13.000000 pyISBO-1.0.1/pyISBO/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 01:32:34.000000 pyISBO-1.0.1/pyISBO.egg-info/
--rw-rw-rw-   0        0        0      304 2023-07-13 01:32:34.000000 pyISBO-1.0.1/pyISBO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      717 2023-07-13 01:32:34.000000 pyISBO-1.0.1/pyISBO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 01:32:34.000000 pyISBO-1.0.1/pyISBO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-13 01:32:34.000000 pyISBO-1.0.1/pyISBO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 01:32:34.000000 pyISBO-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      736 2023-07-13 01:31:59.000000 pyISBO-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:04:33.000000 pyISBO-1.0.2/
+-rw-rw-rw-   0        0        0      304 2023-07-13 07:04:33.000000 pyISBO-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-13 07:04:33.000000 pyISBO-1.0.2/pyISBO/
+drwxrwxrwx   0        0        0        0 2023-07-13 07:04:33.000000 pyISBO-1.0.2/pyISBO/SBO_grb/
+-rw-rw-rw-   0        0        0     4602 2023-07-13 01:37:48.000000 pyISBO-1.0.2/pyISBO/SBO_grb/AutoRegression.py
+-rw-rw-rw-   0        0        0     7086 2023-07-13 01:54:16.000000 pyISBO-1.0.2/pyISBO/SBO_grb/DecisionTree.py
+-rw-rw-rw-   0        0        0     4126 2023-07-13 01:54:17.000000 pyISBO-1.0.2/pyISBO/SBO_grb/LinearRegression.py
+-rw-rw-rw-   0        0        0     5362 2023-07-13 01:54:17.000000 pyISBO-1.0.2/pyISBO/SBO_grb/LogisticRegression.py
+-rw-rw-rw-   0        0        0     7019 2023-07-13 02:10:21.000000 pyISBO-1.0.2/pyISBO/SBO_grb/NeuralNetwork.py
+-rw-rw-rw-   0        0        0     4496 2023-07-13 01:54:17.000000 pyISBO-1.0.2/pyISBO/SBO_grb/QuadraticRegression.py
+-rw-rw-rw-   0        0        0     6895 2023-07-13 01:54:17.000000 pyISBO-1.0.2/pyISBO/SBO_grb/RandomForest.py
+-rw-rw-rw-   0        0        0     6548 2023-07-13 01:57:32.000000 pyISBO-1.0.2/pyISBO/SBO_grb/RegressionSplines.py
+-rw-rw-rw-   0        0        0        0 2023-04-03 12:01:13.000000 pyISBO-1.0.2/pyISBO/SBO_grb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:04:33.000000 pyISBO-1.0.2/pyISBO/SBO_pulp/
+-rw-rw-rw-   0        0        0     4318 2023-07-13 01:38:27.000000 pyISBO-1.0.2/pyISBO/SBO_pulp/AutoRegression.py
+-rw-rw-rw-   0        0        0     6947 2023-07-13 01:54:17.000000 pyISBO-1.0.2/pyISBO/SBO_pulp/DecisionTree.py
+-rw-rw-rw-   0        0        0     3944 2023-07-13 01:54:17.000000 pyISBO-1.0.2/pyISBO/SBO_pulp/LinearRegression.py
+-rw-rw-rw-   0        0        0     5281 2023-07-13 01:54:17.000000 pyISBO-1.0.2/pyISBO/SBO_pulp/LogisticRegression.py
+-rw-rw-rw-   0        0        0     6912 2023-07-13 07:02:35.000000 pyISBO-1.0.2/pyISBO/SBO_pulp/NeuralNetwork.py
+-rw-rw-rw-   0        0        0     7677 2023-07-13 01:54:17.000000 pyISBO-1.0.2/pyISBO/SBO_pulp/RandomForest.py
+-rw-rw-rw-   0        0        0     6340 2023-07-13 01:57:32.000000 pyISBO-1.0.2/pyISBO/SBO_pulp/RegressionSplines.py
+-rw-rw-rw-   0        0        0        0 2023-04-03 12:01:13.000000 pyISBO-1.0.2/pyISBO/SBO_pulp/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-03 12:01:13.000000 pyISBO-1.0.2/pyISBO/__init__.py
+-rw-rw-rw-   0        0        0      323 2023-07-13 01:39:46.000000 pyISBO-1.0.2/pyISBO/main.py
+drwxrwxrwx   0        0        0        0 2023-07-13 07:04:33.000000 pyISBO-1.0.2/pyISBO.egg-info/
+-rw-rw-rw-   0        0        0      304 2023-07-13 07:04:33.000000 pyISBO-1.0.2/pyISBO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      732 2023-07-13 07:04:33.000000 pyISBO-1.0.2/pyISBO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 07:04:33.000000 pyISBO-1.0.2/pyISBO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-13 07:04:33.000000 pyISBO-1.0.2/pyISBO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 07:04:33.000000 pyISBO-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      736 2023-07-13 07:02:35.000000 pyISBO-1.0.2/setup.py
```

### Comparing `pyISBO-1.0.1/pyISBO/SBO_grb/AutoRegression.py` & `pyISBO-1.0.2/pyISBO/SBO_grb/AutoRegression.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from copy import deepcopy
 from .DecisionTree import DT
 from .LinearRegression import LR
 from .LogisticRegression import LogR
 from .NeuralNetwork import NN
 from .QuadraticRegression import QR
 from .RandomForest import RF
 from .RegressionSplines import MARS
@@ -44,20 +45,20 @@
         :return: A float number.
             The cross-validation score of the fitted model based on the scoring metric you choose.
         """
         if Classification:
             self.model = LogR(self.parameterInfo, self.scoring)
             self.model.fit(X, y)
         else:
-            LRmodel = LR(self.parameterInfo, self.scoring)
-            QRmodel = QR(self.parameterInfo, self.scoring)
-            NNmodel = NN(self.parameterInfo, self.scoring)
-            DTmodel = DT(self.parameterInfo, self.scoring)
-            RFmodel = RF(self.parameterInfo, self.scoring)
-            RSmodel = MARS(self.parameterInfo, self.scoring)
+            LRmodel = LR(deepcopy(self.parameterInfo), deepcopy(self.scoring))
+            QRmodel = QR(deepcopy(self.parameterInfo), deepcopy(self.scoring))
+            NNmodel = NN(deepcopy(self.parameterInfo), deepcopy(self.scoring))
+            DTmodel = DT(deepcopy(self.parameterInfo), deepcopy(self.scoring))
+            RFmodel = RF(deepcopy(self.parameterInfo), deepcopy(self.scoring))
+            RSmodel = MARS(deepcopy(self.parameterInfo), deepcopy(self.scoring))
             score = [LRmodel.fit(X,y), QRmodel.fit(X,y), NNmodel.fit(X,y), DTmodel.fit(X,y), RFmodel.fit(X,y),
                      RSmodel.fit(X,y)]
             index = score.index(max(score))
             if index == 0:
                 self.model = LRmodel
             elif index == 1:
                 self.model = QRmodel
```

### Comparing `pyISBO-1.0.1/pyISBO/SBO_grb/DecisionTree.py` & `pyISBO-1.0.2/pyISBO/SBO_grb/DecisionTree.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         :param X:{array-like, sparse matrix} of shape (n_samples, n_features)T
             Training data.
         :param y:array-like of shape (n_samples,) or (n_samples, n_targets)
             Target values. Will be cast to X's dtype if necessary.
         :return: A float number.
             The cross-validation score of the fitted model based on the scoring metric you choose.
         """
+        print("Now fitting Decision Tree.")
         M_score = []
         M_model = []
         for i in range(4, 9):
             model = DecisionTreeRegressor(max_depth=i, min_samples_leaf=5)  # 实例化
             model.fit(X, y)
             score = np.mean(cross_val_score(model, X, y, cv=5, scoring=self.scoring))
             M_score.append(score)
```

### Comparing `pyISBO-1.0.1/pyISBO/SBO_grb/LinearRegression.py` & `pyISBO-1.0.2/pyISBO/SBO_grb/LinearRegression.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         :param X:{array-like, sparse matrix} of shape (n_samples, n_features)T
             Training data.
         :param y:array-like of shape (n_samples,) or (n_samples, n_targets)
             Target values. Will be cast to X's dtype if necessary.
         :return: A float number.
             The cross-validation score of the fitted model based on the scoring metric you choose.
         """
+        print("Now fitting Linear Regression model.")
         self.model = LinearRegression()
         self.model.fit(X, y)
         score = cross_val_score(self.model, X, y, cv=5, scoring=self.scoring)
         return np.mean(score)
 
     def predict(self, X):
         """
```

### Comparing `pyISBO-1.0.1/pyISBO/SBO_grb/LogisticRegression.py` & `pyISBO-1.0.2/pyISBO/SBO_grb/LogisticRegression.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         :param X:{array-like, sparse matrix} of shape (n_samples, n_features)T
             Training data.
         :param y:array-like of shape (n_samples,) or (n_samples, n_targets)
             Target values. Will be cast to X's dtype if necessary.
         :return: A float number.
             The cross-validation score of the fitted model based on the scoring metric you choose.
         """
+        print("Now fitting Logistic Regression model.")
         self.model = LogisticRegression(max_iter=1e5)
         self.model.fit(X, y)
         try:
             for i in range(len(self.model.classes_)):
                 float(self.model.classes_[i])
         except ValueError:
             print("pyISO can only recognize digital classification.")
```

### Comparing `pyISBO-1.0.1/pyISBO/SBO_grb/NeuralNetwork.py` & `pyISBO-1.0.2/pyISBO/SBO_grb/NeuralNetwork.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,30 +56,30 @@
         :param X:{array-like, sparse matrix} of shape (n_samples, n_features)T
             Training data.
         :param y:array-like of shape (n_samples,) or (n_samples, n_targets)
             Target values. Will be cast to X's dtype if necessary.
         :return: A float number.
             The cross-validation score of the fitted model based on the scoring metric you choose.
         """
+        print("Now fitting neural network.")
         n = len(self.types)
         stats = X.describe().transpose()
         self.mean = stats['mean']
         self.std = stats['std']
         normed_X = self.norm(X)
         scorer = get_scorer(self.scoring)
         Scores = []
         for K in range(2, 10):
             score = 0
-            print("K=%d" % K)
-            kfold = KFold(5,shuffle=True)
+            kfold = KFold(5, shuffle=True)
             for train_index, test_index in kfold.split(X):
                 X_train, X_test = X.iloc[train_index], X.iloc[test_index]
                 y_train, y_test = y.iloc[train_index], y.iloc[test_index]
                 model = self.__create_model(K, n)
-                model.fit(X_train, y_train, epochs=100)
+                model.fit(X_train, y_train, epochs=100, verbose=None)
                 score += scorer(model, X_test, y_test)
             Scores.append(score/5)
 
         k = Scores.index(max(Scores)) + 2
         self.model = self.__create_model(k, n)
         self.model.fit(normed_X, y)
         return max(Scores)
```

### Comparing `pyISBO-1.0.1/pyISBO/SBO_grb/QuadraticRegression.py` & `pyISBO-1.0.2/pyISBO/SBO_grb/QuadraticRegression.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         :param X:{array-like, sparse matrix} of shape (n_samples, n_features)T
             Training data.
         :param y:array-like of shape (n_samples,) or (n_samples, n_targets)
             Target values. Will be cast to X's dtype if necessary.
         :return: A float number.
             The cross-validation score of the fitted model based on the scoring metric you choose.
         """
+        print("Now fitting Quadratic Regression model.")
         self.model = make_pipeline(PolynomialFeatures(degree=2),LinearRegression())
         self.model.fit(X, y)
         score = cross_val_score(self.model, X, y, cv=5, scoring=self.scoring)
         return np.mean(score)
 
     def predict(self, X):
         """
```

### Comparing `pyISBO-1.0.1/pyISBO/SBO_grb/RandomForest.py` & `pyISBO-1.0.2/pyISBO/SBO_grb/RandomForest.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         :param X:{array-like, sparse matrix} of shape (n_samples, n_features)T
             Training data.
         :param y:array-like of shape (n_samples,) or (n_samples, n_targets)
             Target values. Will be cast to X's dtype if necessary.
         :return: A float number.
             The cross-validation score of the fitted model based on the scoring metric you choose.
         """
+        print("Now fitting Random Forest.")
         M_score = []
         M_model = []
         for i in range(4, 9):
             model = RandomForestRegressor(max_depth=i, min_samples_leaf=5)  # 实例化
             model.fit(X, y)
             score = np.mean(cross_val_score(model, X, y, cv=5, scoring=self.scoring))
             M_score.append(score)
```

### Comparing `pyISBO-1.0.1/pyISBO/SBO_grb/RegressionSplines.py` & `pyISBO-1.0.2/pyISBO/SBO_grb/RegressionSplines.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         :param X:{array-like, sparse matrix} of shape (n_samples, n_features)T
             Training data.
         :param y:array-like of shape (n_samples,) or (n_samples, n_targets)
             Target values. Will be cast to X's dtype if necessary.
         :return: A float number.
             The cross-validation score of the fitted model based on the scoring metric you choose.
         """
+        print("Now fitting MARS model.")
         self.model = Earth()
         self.model.fit(X, y)
         score = cross_val_score(self.model, X, y, cv=5, scoring=self.scoring)
         return np.mean(score)
 
     def predict(self, X):
         """
@@ -78,15 +79,14 @@
             while "" in summary[i]:
                 summary[i].remove("")
         for i in range(len(summary)):
             if summary[i][1] == "Yes":
                 summary[i] = ""
         while "" in summary:
             summary.remove("")
-        print(summary)
         branch_index = [i for i in range(len(summary))]
         intercept = self.model.coef_[0][0]
 
         self.MIP = Model("MARS")
         inputInfo = {}
         for i in range(len(self.types)):
             inputInfo[(i)] = [self.bounds[i][0], self.bounds[i][1], self.types[i]]
```

### Comparing `pyISBO-1.0.1/pyISBO/SBO_pulp/AutoRegression.py` & `pyISBO-1.0.2/pyISBO/SBO_pulp/AutoRegression.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from copy import deepcopy
 from .DecisionTree import DT
 from .LinearRegression import LR
 from .LogisticRegression import LogR
 from .NeuralNetwork import NN
 from .RandomForest import RF
 from .RegressionSplines import MARS
 
@@ -43,19 +44,19 @@
         :return: A float number.
             The cross-validation score of the fitted model based on the scoring metric you choose.
         """
         if Classification:
             self.model = LogR(self.parameterInfo, self.scoring)
             self.model.fit(X, y)
         else:
-            LRmodel = LR(self.parameterInfo, self.scoring)
-            NNmodel = NN(self.parameterInfo, self.scoring)
-            DTmodel = DT(self.parameterInfo, self.scoring)
-            RFmodel = RF(self.parameterInfo, self.scoring)
-            RSmodel = MARS(self.parameterInfo, self.scoring)
+            LRmodel = LR(deepcopy(self.parameterInfo), deepcopy(self.scoring))
+            NNmodel = NN(deepcopy(self.parameterInfo), deepcopy(self.scoring))
+            DTmodel = DT(deepcopy(self.parameterInfo), deepcopy(self.scoring))
+            RFmodel = RF(deepcopy(self.parameterInfo), deepcopy(self.scoring))
+            RSmodel = MARS(deepcopy(self.parameterInfo), deepcopy(self.scoring))
             score = [LRmodel.fit(X,y), NNmodel.fit(X,y), DTmodel.fit(X,y), RFmodel.fit(X,y),
                      RSmodel.fit(X,y)]
             index = score.index(max(score))
             if index == 0:
                 self.model = LRmodel
             elif index == 1:
                 self.model = NNmodel
```

### Comparing `pyISBO-1.0.1/pyISBO/SBO_pulp/DecisionTree.py` & `pyISBO-1.0.2/pyISBO/SBO_pulp/DecisionTree.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         :param X:{array-like, sparse matrix} of shape (n_samples, n_features)T
             Training data.
         :param y:array-like of shape (n_samples,) or (n_samples, n_targets)
             Target values. Will be cast to X's dtype if necessary.
         :return: A float number.
             The cross-validation score of the fitted model based on the scoring metric you choose.
         """
+        print("Now fitting Decision Tree.")
         M_score = []
         M_model = []
         for i in range(4, 9):
             model = DecisionTreeRegressor(max_depth=i, min_samples_leaf=5)  # 实例化
             model.fit(X, y)
             score = np.mean(cross_val_score(model, X, y, cv=5, scoring=self.scoring))
             M_score.append(score)
```

### Comparing `pyISBO-1.0.1/pyISBO/SBO_pulp/LinearRegression.py` & `pyISBO-1.0.2/pyISBO/SBO_pulp/LinearRegression.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         :param X:{array-like, sparse matrix} of shape (n_samples, n_features)T
             Training data.
         :param y:array-like of shape (n_samples,) or (n_samples, n_targets)
             Target values. Will be cast to X's dtype if necessary.
         :return: A float number.
             The cross-validation score of the fitted model based on the scoring metric you choose.
         """
+        print("Now fitting Linear Regression model.")
         self.model = LinearRegression()
         self.model.fit(X, y)
         score = cross_val_score(self.model, X, y, cv=5, scoring=self.scoring)
         return np.mean(score)
 
     def predict(self, X):
         """
```

### Comparing `pyISBO-1.0.1/pyISBO/SBO_pulp/LogisticRegression.py` & `pyISBO-1.0.2/pyISBO/SBO_pulp/LogisticRegression.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         :param X:{array-like, sparse matrix} of shape (n_samples, n_features)T
             Training data.
         :param y:array-like of shape (n_samples,) or (n_samples, n_targets)
             Target values. Will be cast to X's dtype if necessary.
         :return: A float number.
             The cross-validation score of the fitted model based on the scoring metric you choose.
         """
+        print("Now fitting Logistic Regression model.")
         self.model = LogisticRegression(max_iter=1e5)
         self.model.fit(X, y)
         try:
             for i in range(len(self.model.classes_)):
                 float(self.model.classes_[i])
         except ValueError:
             print("pyISO can only recognize digital classification.")
```

### Comparing `pyISBO-1.0.1/pyISBO/SBO_pulp/NeuralNetwork.py` & `pyISBO-1.0.2/pyISBO/SBO_pulp/NeuralNetwork.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,30 +57,30 @@
         :param X:{array-like, sparse matrix} of shape (n_samples, n_features)T
             Training data.
         :param y:array-like of shape (n_samples,) or (n_samples, n_targets)
             Target values. Will be cast to X's dtype if necessary.
         :return: A float number.
             The cross-validation score of the fitted model based on the scoring metric you choose.
         """
+        print("Now fitting neural network.")
         n = len(self.types)
         stats = X.describe().transpose()
         self.mean = stats['mean']
         self.std = stats['std']
         normed_X = self.norm(X)
         scorer = get_scorer(self.scoring)
         Scores = []
         for K in range(2, 10):
             score = 0
-            print("K=%d" % K)
-            kfold = KFold(5,shuffle=True)
+            kfold = KFold(5, shuffle=True)
             for train_index, test_index in kfold.split(X):
                 X_train, X_test = X.iloc[train_index], X.iloc[test_index]
                 y_train, y_test = y.iloc[train_index], y.iloc[test_index]
                 model = self.__create_model(K, n)
-                model.fit(X_train, y_train, epochs=100)
+                model.fit(X_train, y_train, epochs=100, verbose=None)
                 score += scorer(model, X_test, y_test)
             Scores.append(score/5)
 
         k = Scores.index(max(Scores)) + 2
         self.model = self.__create_model(k, n)
         self.model.fit(normed_X, y)
         return max(Scores)
```

### Comparing `pyISBO-1.0.1/pyISBO/SBO_pulp/RandomForest.py` & `pyISBO-1.0.2/pyISBO/SBO_pulp/RandomForest.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         :param X:{array-like, sparse matrix} of shape (n_samples, n_features)T
             Training data.
         :param y:array-like of shape (n_samples,) or (n_samples, n_targets)
             Target values. Will be cast to X's dtype if necessary.
         :return: A float number.
             The cross-validation score of the fitted model based on the scoring metric you choose.
         """
+        print("Now fitting Random Forest.")
         M_score = []
         M_model = []
         for i in range(4, 9):
             model = RandomForestRegressor(max_depth=i, min_samples_leaf=5)  # 实例化
             model.fit(X, y)
             score = np.mean(cross_val_score(model, X, y, cv=5, scoring=self.scoring))
             M_score.append(score)
```

### Comparing `pyISBO-1.0.1/pyISBO/SBO_pulp/RegressionSplines.py` & `pyISBO-1.0.2/pyISBO/SBO_pulp/RegressionSplines.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         :param X:{array-like, sparse matrix} of shape (n_samples, n_features)T
             Training data.
         :param y:array-like of shape (n_samples,) or (n_samples, n_targets)
             Target values. Will be cast to X's dtype if necessary.
         :return: A float number.
             The cross-validation score of the fitted model based on the scoring metric you choose.
         """
+        print("Now fitting MARS model.")
         self.model = Earth()
         self.model.fit(X, y)
         score = cross_val_score(self.model, X, y, cv=5, scoring=self.scoring)
         return np.mean(score)
 
     def predict(self, X):
         """
@@ -77,15 +78,14 @@
             while "" in summary[i]:
                 summary[i].remove("")
         for i in range(len(summary)):
             if summary[i][1] == "Yes":
                 summary[i] = ""
         while "" in summary:
             summary.remove("")
-        print(summary)
         branch_index = [i for i in range(len(summary))]
         intercept = self.model.coef_[0][0]
 
         self.MIP = LpProblem("MARS", LpMinimize)
         x = {}
         for i in range(len(self.types)):
             x[i] = LpVariable("x_%d" % i, self.bounds[i][0], self.bounds[i][1], cat=self.types[i])
```

### Comparing `pyISBO-1.0.1/pyISBO.egg-info/SOURCES.txt` & `pyISBO-1.0.2/pyISBO.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 setup.py
 pyISBO/__init__.py
+pyISBO/main.py
 pyISBO.egg-info/PKG-INFO
 pyISBO.egg-info/SOURCES.txt
 pyISBO.egg-info/dependency_links.txt
 pyISBO.egg-info/top_level.txt
 pyISBO/SBO_grb/AutoRegression.py
 pyISBO/SBO_grb/DecisionTree.py
 pyISBO/SBO_grb/LinearRegression.py
```

### Comparing `pyISBO-1.0.1/setup.py` & `pyISBO-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name="pyISBO",
-      version="1.0.1",
+      version="1.0.2",
       author="Liu Xiangting and Zhu Zesheng",
       author_email="liu-xt22@mails.tsinghua.edu.cn",
       packages = find_packages(),
       description="An integrated Surrogate-Base Optimization Toolbox",
       package_dir={"pyISBO":"pyISBO"},
       package_data={"pyISBO":['pyISBO/OperationData.xlsx']},
       url="https://github.com/Shawn1eo/pyISBO",
```

