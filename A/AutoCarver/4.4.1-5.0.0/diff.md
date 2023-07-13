# Comparing `tmp/AutoCarver-4.4.1.tar.gz` & `tmp/AutoCarver-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoCarver-4.4.1.tar", last modified: Mon Jun 12 12:14:28 2023, max compression
+gzip compressed data, was "AutoCarver-5.0.0.tar", last modified: Thu Jul 13 12:07:18 2023, max compression
```

## Comparing `AutoCarver-4.4.1.tar` & `AutoCarver-5.0.0.tar`

### file list

```diff
@@ -1,17 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:14:28.942246 AutoCarver-4.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:14:28.942246 AutoCarver-4.4.1/AutoCarver/
--rw-r--r--   0 runner    (1001) docker     (123)    24410 2023-06-12 12:14:19.000000 AutoCarver-4.4.1/AutoCarver/AutoCarver.py
--rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-06-12 12:14:19.000000 AutoCarver-4.4.1/AutoCarver/Converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    52397 2023-06-12 12:14:19.000000 AutoCarver-4.4.1/AutoCarver/Discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27508 2023-06-12 12:14:19.000000 AutoCarver-4.4.1/AutoCarver/FeatureSelector.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 12:14:19.000000 AutoCarver-4.4.1/AutoCarver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:14:28.942246 AutoCarver-4.4.1/AutoCarver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-06-12 12:14:28.000000 AutoCarver-4.4.1/AutoCarver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-12 12:14:28.000000 AutoCarver-4.4.1/AutoCarver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 12:14:28.000000 AutoCarver-4.4.1/AutoCarver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 12:14:28.000000 AutoCarver-4.4.1/AutoCarver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-12 12:14:19.000000 AutoCarver-4.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-06-12 12:14:28.942246 AutoCarver-4.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17418 2023-06-12 12:14:19.000000 AutoCarver-4.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 12:14:28.942246 AutoCarver-4.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-12 12:14:19.000000 AutoCarver-4.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:07:18.914507 AutoCarver-5.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:07:18.910507 AutoCarver-5.0.0/AutoCarver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/AutoCarver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31613 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/AutoCarver/auto_carver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/AutoCarver/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:07:18.910507 AutoCarver-5.0.0/AutoCarver/discretizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/AutoCarver/discretizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24378 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/AutoCarver/discretizers/discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:07:18.914507 AutoCarver-5.0.0/AutoCarver/discretizers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/AutoCarver/discretizers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34585 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/AutoCarver/discretizers/utils/base_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27174 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/AutoCarver/discretizers/utils/qualitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/AutoCarver/discretizers/utils/quantitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/AutoCarver/discretizers/utils/type_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28712 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/AutoCarver/feature_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:07:18.910507 AutoCarver-5.0.0/AutoCarver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18831 2023-07-13 12:07:18.000000 AutoCarver-5.0.0/AutoCarver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-13 12:07:18.000000 AutoCarver-5.0.0/AutoCarver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 12:07:18.000000 AutoCarver-5.0.0/AutoCarver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 12:07:18.000000 AutoCarver-5.0.0/AutoCarver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18831 2023-07-13 12:07:18.914507 AutoCarver-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18087 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-13 12:07:18.914507 AutoCarver-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 12:07:18.914507 AutoCarver-5.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/tests/test_auto_carver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/tests/test_base_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/tests/test_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/tests/test_feature_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/tests/test_qualitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/tests/test_quantitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-13 12:07:06.000000 AutoCarver-5.0.0/tests/test_type_discretizers.py
```

### Comparing `AutoCarver-4.4.1/AutoCarver/AutoCarver.py` & `AutoCarver-5.0.0/AutoCarver/auto_carver.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,37 @@
-from .Discretizers import GroupedList, GroupedListDiscretizer, is_equal
-from IPython.display import display_html
+"""Tool to build optimized buckets out of Quantitative and Qualitative features
+for a binary classification model.
+"""
+
+from typing import Any, Dict, List, Tuple
+
+import numpy as np
+from IPython.display import display_html  # TODO: remove this
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 from matplotlib.pyplot import subplots
 from matplotlib.ticker import PercentFormatter
-from numpy import sqrt
-from pandas import DataFrame, Series, notna, unique, crosstab
-from pandas.api.types import is_string_dtype
+from pandas import DataFrame, Series, crosstab, unique
 from scipy.stats import chi2_contingency
 from seaborn import color_palette, despine
-from tqdm.notebook import tqdm
-from typing import Any, Dict, List, Tuple
+from tqdm import tqdm
+
+from .discretizers.discretizers import Discretizer
+from .discretizers.utils.base_discretizers import (
+    GroupedList,
+    GroupedListDiscretizer,
+    convert_to_labels,
+    convert_to_values,
+    is_equal,
+)
 
 
+# TODO: display tables
 class AutoCarver(GroupedListDiscretizer):
-    """ Automatic carving of continuous, categorical and categorical ordinal
+    """Automatic carving of continuous, categorical and categorical ordinal
     features that maximizes association with a binary target.
 
     Modalities/values of features are carved/regrouped according to a computed
     specific order defined based on their types:
      - [Qualitative features] grouped based on modality target rate.
      - [Qualitative ordinal features] grouped based on specified modality order
      - [Quantitative features] grouped based on the order of their values.
@@ -99,589 +112,781 @@
     pipe += [('AutoCarver', auto_carver)]
     pipe = Pipeline(pipe)
 
     # applying pipe to a validation set or in production
     X_val = pipe.transform(X_val)
 
     """
-   
+
     def __init__(
-            self,
-            values_orders: Dict[str, Any],
-            *,
-            max_n_mod: int=5,
-            sort_by: str='tschuprowt',
-            str_nan: str='__NAN__',
-            dropna: bool=True,
-            copy: bool=False,
-            verbose: bool=True
-        ) -> None:
-        
-        self.features = list(values_orders.keys())
+        self,
+        quantitative_features: List[str],
+        qualitative_features: List[str],
+        min_freq: float,
+        *,
+        ordinal_features: List[str] = None,
+        values_orders: Dict[str, GroupedList] = None,
+        max_n_mod: int = 5,
+        min_carved_freq: float = 0,  # TODO: update this parameter so that it is set according to frequency rather than number of groups
+        sort_by: str = "tschuprowt",
+        str_nan: str = "__NAN__",
+        str_default: str = "__OTHER__",
+        output_dtype: str = 'float',
+        dropna: bool = True,
+        copy: bool = False,
+        verbose: bool = True,
+    ) -> None:
+        """_summary_
+
+        Parameters
+        ----------
+        quantitative_features : List[str]
+            _description_
+        qualitative_features : List[str]
+            _description_
+        min_freq : float
+            _description_
+        ordinal_features : List[str], optional
+            _description_, by default None
+        values_orders : Dict[str, GroupedList], optional
+            _description_, by default None
+        max_n_mod : int, optional
+            _description_, by default 5
+        min_carved_freq : float, optional
+            _description_, by default 0
+        str_nan : str, optional
+            _description_, by default "__NAN__"
+        str_default : str, optional
+            _description_, by default "__OTHER__"
+        output_dtype : str, optional
+            _description_, by default 'float'
+        dropna : bool, optional
+            _description_, by default True
+        copy : bool, optional
+            _description_, by default False
+        verbose : bool, optional
+            _description_, by default True
+        """        
+        # copying quantitative features and checking for duplicates
+        self.quantitative_features = quantitative_features[:]
+        assert len(list(set(quantitative_features))) == len(
+            quantitative_features
+        ), "Column duplicates in quantitative_features"
+
+        # copying qualitative features and checking for duplicates
+        self.qualitative_features = qualitative_features[:]
+        assert len(list(set(qualitative_features))) == len(
+            qualitative_features
+        ), "Column duplicates in qualitative_features"
+
+        # copying ordinal features and checking for duplicates
+        if ordinal_features is None:
+            ordinal_features = []
+        self.ordinal_features = ordinal_features[:]
+        assert len(list(set(ordinal_features))) == len(
+            ordinal_features
+        ), "Column duplicates in ordinal_features"
+
+        # initiating values_orders
+        if values_orders is None:
+            values_orders = {}
         self.values_orders = {k: GroupedList(v) for k, v in values_orders.items()}
-        self.non_viable_features: List[str] = []  # list of features non viable features
-        self.max_n_mod = max_n_mod  # maximum number of modality per feature
-        self.dropna = dropna  # whether or not to group NaNs with other modalities
-        
+
+        # list of all features
+        self.features = list(set(quantitative_features + qualitative_features + ordinal_features))
+
+        # minimum frequency per base bucket
+        self.min_freq = min_freq
+        # maximum number of modality per feature
+        self.max_n_mod = max_n_mod
+        # whether or not to group NaNs with other modalities
+        self.dropna = dropna
+
         # association measure used to find the best groups
-        measures = ['tschuprowt', 'cramerv']
-        assert sort_by in measures, f"""{sort_by} not yet implemented. Choose
+        measures = ["tschuprowt", "cramerv"]
+        assert (
+            sort_by in measures
+        ), f"""{sort_by} not yet implemented. Choose
                                         from: {', '.join(measures)}."""
         self.sort_by = sort_by
 
         self.copy = copy
         self.verbose = verbose
         self.str_nan = str_nan
-    
+        self.str_default = str_default
+
+        self.min_carved_freq = min_carved_freq
+        self.min_group_size = 1
+        self.input_dtypes = {}
+        self.output_dtype = output_dtype
+
     def prepare_data(
-            self,
-            X: DataFrame,
-            y: Series,
-            X_test: DataFrame=None,
-            y_test: Series=None
-        ) -> Tuple[DataFrame, Series, DataFrame, Series]:
-        """ Checks validity of provided data"""
-        
+        self,
+        X: DataFrame,
+        y: Series,
+        X_test: DataFrame = None,
+        y_test: Series = None,
+    ) -> Tuple[DataFrame, DataFrame]:
+        """Checks validity of provided data"""
+
         # preparing train sample
         # checking for binary target
         y_values = unique(y)
-        assert (0 in y_values) & (1 in y_values), "y must be a binary Series (int or float, not object)"
+        assert (0 in y_values) & (
+            1 in y_values
+        ), "y must be a binary Series (int or float, not object)"
         assert len(y_values) == 2, "y must be a binary Series (int or float, not object)"
-        
-        # checking for quantitative columns
-        is_object = X[self.features].dtypes.apply(is_string_dtype)
-        assert all(is_object), f"Non-string features in X: {', '.join(is_object[~is_object].index)}, consider using Discretizer."
-        
+
         # Copying DataFrame if requested
-        Xc = X
+        x_copy = X
         if self.copy:
-            Xc = X.copy()
-        
+            x_copy = X.copy()
+
         # preparing test sample
         # checking for binary target
         if y_test is not None:
             assert X_test is not None, "y_test was provided but X_test is missing"
             y_values = unique(y_test)
-            assert (0 in y_values) & (1 in y_values), "y_test must be a binary Series (int or float, not object)"
+            assert (0 in y_values) & (
+                1 in y_values
+            ), "y_test must be a binary Series (int or float, not object)"
             assert len(y_values) == 2, "y_test must be a binary Series (int or float, not object)"
-        
+
         # Copying DataFrame if requested
-        Xtestc = X_test
+        x_test_copy = X_test
         if X_test is not None:
             assert y_test is not None, "X_test was provided but y_test is missing"
             if self.copy:
-                Xtestc = X_test.copy()
-        
-            # checking for quantitative columns
-            is_object = X_test[self.features].dtypes.apply(is_string_dtype)
-            assert all(is_object), f"Non-string features in X_test: {', '.join(is_object[~is_object].index)}, consider using Discretizer."
-            
-        return Xc, y, Xtestc, y_test
-    
+                x_test_copy = X_test.copy()
+
+        return x_copy, x_test_copy
+
     def fit(
-            self,
-            X: DataFrame,
-            y: Series,
-            X_test: DataFrame=None,
-            y_test: Series=None
-        ) -> None:
+        self,
+        X: DataFrame,
+        y: Series,
+        X_test: DataFrame = None,
+        y_test: Series = None,
+    ) -> None:
+        """_summary_
 
+        Parameters
+        ----------
+        X : DataFrame
+            _description_
+        y : Series
+            _description_
+        X_test : DataFrame, optional
+            _description_, by default None
+        y_test : Series, optional
+            _description_, by default None
+        """
         # preparing datasets and checking for wrong values
-        Xc, y, Xtestc, y_test = self.prepare_data(X, y, X_test, y_test)
-        
-        # automatic carving of each feature
-        for n, feature in tqdm(enumerate(self.features), total=len(self.features), disable=self.verbose):
+        x_copy, x_test_copy = self.prepare_data(X, y, X_test, y_test)
 
-            # printing the group statistics and determining default ordering
-            if self.verbose:
+        # discretizing all features
+        discretizer = Discretizer(
+            quantitative_features=self.quantitative_features,
+            qualitative_features=self.qualitative_features,
+            min_freq=self.min_freq,
+            ordinal_features=self.ordinal_features,
+            values_orders=self.values_orders,
+            str_nan=self.str_nan,
+            str_default=self.str_default,
+            copy=False,
+            verbose=self.verbose,
+        )
+        x_copy = discretizer.fit_transform(x_copy, y)
+        if x_test_copy is not None:
+            x_test_copy = discretizer.transform(x_test_copy, y_test)
+        self.input_dtypes.update(discretizer.input_dtypes)  # saving data types
+
+        # updating values_orders according to base bucketization
+        self.values_orders.update(discretizer.values_orders)
+
+        # removing dropped features
+        for feature in self.features:
+            if feature not in discretizer.values_orders:
+                self.remove_feature(feature)
+
+
+        # converting potential quantiles into there respective labels
+        labels_orders = convert_to_labels(
+            features=self.features,
+            quantitative_features=self.quantitative_features,
+            values_orders=self.values_orders,
+            str_nan=self.str_nan,
+            dropna=False,
+        )
+
+        # computing crosstabs for each feature on train/test
+        xtabs = get_xtabs(self.features, x_copy, y, labels_orders)
+        xtabs_test = get_xtabs(self.features, x_test_copy, y_test, labels_orders)
+
+        # optimal butcketization/carving of each feature
+        for n, feature in enumerate(self.features):
+            if self.verbose:  # verbose if requested
                 print(f"\n---\n[AutoCarver] Fit {feature} ({n+1}/{len(self.features)})")
 
-            # getting best combination
-            best_groups = self.get_best_combination(feature, Xc, y, Xtestc, y_test)
-
-            # feature can not be carved robustly
-            if not bool(best_groups):
-                self.non_viable_features += [feature]  # adding it to list of non viable features
-
-        # discretizing features based on each feature's values_order
-        super().__init__(self.values_orders, str_nan=self.str_nan, copy=self.copy, output=float)
-        super().fit(X, y)
-
-        return self
-
-
-    def get_best_combination(
-            self,
-            feature: str,
-            X: DataFrame,
-            y: Series,
-            X_test: DataFrame=None,
-            y_test: Series=None
-        ) -> Dict[str, Any]:
-        """ Carves a feature"""
-
-        # computing crosstabs
-        # crosstab on TRAIN
-        xtab = nan_crosstab(X[feature], y, self.str_nan)
-
-        # crosstab on TEST
-        xtab_test = None
-        if X_test is not None:
-            xtab_test = nan_crosstab(X_test[feature], y_test, self.str_nan)
-
-        # printing the group statistics
-        if self.verbose:
-            self.display_xtabs(feature, 'Raw', xtab, xtab_test)
-
-        # measuring association with target for each combination and testing for stability on TEST
-        best_groups = best_combination(self.values_orders.get(feature), self.max_n_mod, self.sort_by, xtab, xtab_test, dropna=True, str_nan=self.str_nan)
-
-        # update of the values_orders grouped modalities in values_orders
-        if best_groups:
-            xtab, xtab_test = self.update_order(feature, best_groups['combination'], xtab, xtab_test)
-
-        # testing adding NaNs to built groups
-        if (self.str_nan in xtab.index) & self.dropna & (self.str_nan not in self.values_orders.get(feature)):
-
-            # measuring association with target for each combination and testing for stability on TEST
-            best_groups = best_combination(self.values_orders.get(feature), self.max_n_mod, self.sort_by, xtab, xtab_test, dropna=False, str_nan=self.str_nan)
-
-            # adding NaN to the order
-            self.insert_nan(feature, xtab)
+            # getting xtabs on train/test
+            xtab = xtabs[feature]
+            xtab_test = xtabs_test[feature]
+            if self.verbose:  # verbose if requested
+                print(xtab)
 
-            # update of the values_orders grouped modalities in values_orders
-            if best_groups:
-                xtab, xtab_test = self.update_order(feature, best_groups['combination'], xtab, xtab_test)
+            # ordering
+            order = labels_orders[feature]
 
-        # printing the new group statistics
-        if self.verbose and best_groups:
-            self.display_xtabs(feature, 'Fitted', xtab, xtab_test)
+            # getting best combination
+            best_combination = self.get_best_combination(order, xtab, xtab_test=xtab_test)
 
-        return best_groups
+            # checking that a suitable combination has been found
+            if best_combination is not None:
+                order, xtab, xtab_test = best_combination
+                if self.verbose:  # verbose if requested
+                    print(xtab)
 
-    def insert_nan(
-            self,
-            feature: str,
-            xtab: DataFrame
-        ) -> GroupedList:
-        """ Inserts NaNs in the order"""
+                # updating label_orders
+                labels_orders.update({feature: order})
+            
+            # no suitable combination has been found -> removing feature
+            else:
+                print(f"No robust combination for feature '{feature}' could be found. It will be ignored. You might have to increase the size of your test sample (test sample not representative of test sample for this feature) or you should consider dropping this features.")
+                self.remove_feature(feature)
+                if feature in labels_orders:
+                    labels_orders.pop(feature)
+
+
+        # converting potential labels into there respective values (quantiles)
+        self.values_orders.update(
+            convert_to_values(
+                features=self.features,
+                quantitative_features=self.quantitative_features,
+                values_orders=self.values_orders,
+                label_orders=labels_orders,
+                str_nan=self.str_nan,
+            )
+        )
 
-        # accessing order for specified feature
-        order = self.values_orders.get(feature)
+        # TODO convert to float
+        # TODO pretty displaying
 
-        # adding nans at the end of the order
-        if self.str_nan not in order:
-            order = order.append(self.str_nan)
+        # discretizing features based on each feature's values_order
+        super().__init__(
+            features=self.features,
+            values_orders=self.values_orders,
+            copy=self.copy,
+            input_dtypes=self.input_dtypes,
+            str_nan=self.str_nan,
+            verbose=self.verbose,
+            output_dtype=self.output_dtype,
+        )
+        super().fit(X, y)
 
-            # updating values_orders
-            self.values_orders.update({feature: order})
+        return self
 
-    def update_order(
-            self,
-            feature: str,
-            best_groups: GroupedList,
-            xtab: DataFrame,
-            xtab_test: DataFrame=None
-        ) -> Tuple[DataFrame, DataFrame]:
-        """ Updates the values_orders and xtabs according to the best_groups"""
+    def remove_feature(self, feature: str) -> None:
+        """Removes a feature from all instances 
 
-        # updating values_orders with best_combination 
-        self.values_orders.update({feature: best_groups})
+        Parameters
+        ----------
+        feature : str
+            Column name
+        """        
+        
+        self.features.remove(feature)
+        if feature in self.values_orders:
+            self.values_orders.pop(feature)
+        if feature in self.input_dtypes:
+            self.input_dtypes.pop(feature)
+        if feature in self.qualitative_features:
+            self.qualitative_features.remove(feature)
+        if feature in self.ordinal_features:
+            self.ordinal_features.remove(feature)
+        if feature in self.quantitative_features:
+            self.quantitative_features.remove(feature)
 
-        # update of the TRAIN crosstab
-        best_combi = list(map(best_groups.get_group, xtab.index))
-        xtab = xtab.groupby(best_combi, dropna=False).sum()
+    def get_best_combination(
+        self,
+        order: GroupedList,
+        xtab: DataFrame,
+        *,
+        xtab_test: DataFrame = None,
+    ) -> Tuple[GroupedList, DataFrame, DataFrame]:
+        # raw ordering
+        raw_order = GroupedList(order)
+        if self.str_nan in raw_order:
+            raw_order.remove(self.str_nan)
+
+        # filtering out nans if requested from train/test crosstabs
+        raw_xtab = filter_nan_xtab(xtab, self.str_nan)
+        raw_xtab_test = filter_nan_xtab(xtab_test, self.str_nan)
+
+        # checking for non-nan values
+        best_association = None
+        if raw_xtab.shape[0] > 1:
+            # all possible consecutive combinations
+            combinations = consecutive_combinations(
+                raw_order, self.max_n_mod, min_group_size=self.min_group_size
+            )
+
+            # getting most associated combination
+            best_association = get_best_association(
+                raw_xtab,
+                combinations,
+                sort_by=self.sort_by,
+                xtab_test=raw_xtab_test,
+                verbose=self.verbose,
+            )
+            # TODO test missing values in test
+
+            # applying best_combination to order and xtabs
+            if best_association is not None:
+                order = order_apply_combination(order, best_association["combination"])
+                xtab = xtab_apply_order(xtab, order)
+                xtab_test = xtab_apply_order(xtab_test, order)
+
+            # grouping NaNs if requested to drop them (dropna=True)
+            if self.dropna and self.str_nan in order and best_association is not None:
+                # raw ordering without nans
+                raw_order = GroupedList(order)
+                raw_order.remove(self.str_nan)
+
+                # all possible consecutive combinations
+                combinations = consecutive_combinations(
+                    raw_order, self.max_n_mod, min_group_size=self.min_group_size
+                )
+
+                # adding combinations with NaNs
+                nan_combinations = add_nan_in_combinations(
+                    combinations, self.str_nan, self.max_n_mod
+                )
+
+                # getting most associated combination
+                best_association = get_best_association(
+                    xtab,
+                    nan_combinations,
+                    sort_by=self.sort_by,
+                    xtab_test=xtab_test,
+                    verbose=self.verbose,
+                )
+
+                # applying best_combination to order and xtab
+                if best_association is not None:
+                    order = order_apply_combination(order, best_association["combination"])
+                    xtab = xtab_apply_order(xtab, order)
+                    xtab_test = xtab_apply_order(xtab_test, order)
+
+        # checking that a suitable combination has been found
+        if best_association is not None:
+            return order, xtab, xtab_test
 
-        # update of the TEST crosstab
-        if xtab_test is not None:
-            best_combi = list(map(best_groups.get_group, xtab_test.index))
-            xtab_test = xtab_test.groupby(best_combi, dropna=False).sum()
-        
-        return xtab, xtab_test
-    
     def display_xtabs(
-            self,
-            feature: str,
-            caption: str,
-            xtab: DataFrame,
-            xtab_test: DataFrame=None
-        ) -> None:
-        """ Pretty display of frequency and target rate per modality on the same line. """
-        
+        self,
+        feature: str,
+        caption: str,
+        xtab: DataFrame,
+        xtab_test: DataFrame = None,
+    ) -> None:
+        """Pretty display of frequency and target rate per modality on the same line."""
+
         # known_order per feature
-        known_order = self.values_orders.get(feature)
-        
+        known_order = self.values_orders[feature]
+
         # target rate and frequency on TRAIN
         train_stats = stats_xtab(xtab, known_order)
-    
+
         # target rate and frequency on TEST
         if xtab_test is not None:
             test_stats = stats_xtab(xtab_test, train_stats.index, train_stats.labels)
-            test_stats = test_stats.set_index('labels')  # setting labels as indices
-        
+            test_stats = test_stats.set_index("labels")  # setting labels as indices
+
         # setting TRAIN labels as indices
-        train_stats = train_stats.set_index('labels')
+        train_stats = train_stats.set_index("labels")
 
         # Displaying TRAIN modality level stats
-        train_style = train_stats.style.background_gradient(cmap='coolwarm')  # color scaling
-        train_style = train_style.set_table_attributes("style='display:inline'")  # printing in notebook
-        train_style = train_style.set_caption(f'{caption} distribution on X:')  # title
+        train_style = train_stats.style.background_gradient(cmap="coolwarm")  # color scaling
+        train_style = train_style.set_table_attributes(
+            "style='display:inline'"
+        )  # printing in notebook
+        train_style = train_style.set_caption(f"{caption} distribution on X:")  # title
         html = train_style._repr_html_()
-        
+
         # adding TEST modality level stats
         if xtab_test is not None:
-            test_style = test_stats.style.background_gradient(cmap='coolwarm')  # color scaling
-            test_style = test_style.set_table_attributes("style='display:inline'")  # printing in notebook
-            test_style = test_style.set_caption(f'{caption} distribution on X_test:')  # title
-            html += ' ' + test_style._repr_html_()
+            test_style = test_stats.style.background_gradient(cmap="coolwarm")  # color scaling
+            test_style = test_style.set_table_attributes(
+                "style='display:inline'"
+            )  # printing in notebook
+            test_style = test_style.set_caption(f"{caption} distribution on X_test:")  # title
+            html += " " + test_style._repr_html_()
 
         # displaying html of colored DataFrame
         display_html(html, raw=True)
 
-def groupedlist_combination(
-        combination: List[List[Any]],
-        order: GroupedList
-    ) -> GroupedList:
-    """ Converts a list of combination to a GroupedList"""
-    
-    order_copy = GroupedList(order)
-    for combi in combination:
-        order_copy.group_list(combi, combi[0])
-    
-    return order_copy
 
 def stats_xtab(
-        xtab: DataFrame,
-        known_order: List[Any]=None,
-        known_labels: List[Any]=None
-    ) -> DataFrame:
-    """ Computes column (target) rate per row (modality) and row frequency"""
-    
+    xtab: DataFrame,
+    known_order: List[Any] = None,
+    known_labels: List[Any] = None,
+) -> DataFrame:
+    """Computes column (target) rate per row (modality) and row frequency"""
+
     # target rate and frequency statistics per modality
-    stats = DataFrame({
-        # target rate per modality
-        'target_rate': xtab[1].divide(xtab.sum(axis=1)),
-        # frequency per modality
-        'frequency': xtab.sum(axis=1) / xtab.sum().sum()
-    })
-    
+    stats = DataFrame(
+        {
+            # target rate per modality
+            "target_rate": xtab[1].divide(xtab.sum(axis=1)),
+            # frequency per modality
+            "frequency": xtab.sum(axis=1) / xtab.sum().sum(),
+        }
+    )
+
     # sorting statistics
     # case 0: default ordering based on observed target rate
     if known_order is None:
-        order = list(stats.sort_values('target_rate', ascending=True).index)
-    
+        order = list(stats.sort_values("target_rate", ascending=True).index)
+
     # case 1: a known_order was provided
     else:
         order = known_order[:]
-      
+
     # modalities' labels
     # case 0: default labels
     if known_labels is None:
-        
         # accessing string representation of the GroupedList
         if isinstance(known_order, GroupedList):
             labels = known_order.get_repr()
 
         # labels are the default order
         else:
             labels = order[:]
-            
+
     # case 1: known_labels were provided
     else:
         labels = known_labels[:]
-            
-            
+
     # keeping values missing from the order at the end
     unknown_modality = [mod for mod in xtab.index if mod not in order]
     for mod in unknown_modality:
         order = [c for c in order if not is_equal(c, mod)] + [mod]
         labels = [c for c in labels if not is_equal(c, mod)] + [mod]
-    
+
     # sorting statistics
     stats = stats.reindex(order, fill_value=0)
-    stats['labels'] = labels
-    
+    stats["labels"] = labels
+
     return stats
 
-def apply_combination(
-        xtab: DataFrame,
-        combination: GroupedList
-    ) -> Dict[str, Any]:
-    """ applies a modality combination to a crosstab """
 
-    # initiating association dict
-    association = {'combination': combination}
+def filter_nan_xtab(xtab: DataFrame, str_nan: str) -> DataFrame:
+    """Filters out nans from the crosstab"""
 
-    # grouping modalities in the initial crosstab
-    groups = list(map(combination.get_group, xtab.index))
-    combi_xtab = xtab.groupby(groups, dropna=False).sum()
-    association.update({'combi_xtab': combi_xtab})
+    # cehcking for values in crosstab
+    filtered_xtab = None
+    if xtab is not None:
+        # filtering out nans if requested from train crosstab
+        filtered_xtab = xtab.copy()
+        if str_nan in xtab.index:
+            filtered_xtab = xtab.drop(str_nan, axis=0)
 
-    # measuring association with the target
-    association.update(association_xtab(combi_xtab))
+    return filtered_xtab
 
-    return association
 
-def best_combination(
-        order: GroupedList,
-        max_n_mod: int,
-        sort_by: str,
-        xtab_train: DataFrame,
-        xtab_dev: DataFrame=None,
-        dropna: bool=True,
-        str_nan: str=None
-    ) -> Dict[str, Any]:
-    """ Finds the best combination of groups of feature's values:
-     - Most associated combination on train sample 
-     - Stable target rate of combination on test sample.
-    """
-    
-    # copying crosstabs
-    xtab = xtab_train
-    xtab_test = xtab_dev
-    
-    # removing nans if requested
-    if dropna:
-        
-        # crosstab on TRAIN
-        xtab = xtab_train[xtab_train.index != str_nan]  # filtering out nans
+def get_xtabs(
+    features: List[str], X: DataFrame, y: Series, labels_orders: Dict[str, GroupedList]
+) -> Dict[str, DataFrame]:
+    """Computes crosstabs for specified features and ensures that the crosstab is ordered according to the known labels"""
 
-        # crosstab on TEST
-        if xtab_test is not None:
-            xtab_test = xtab_dev[xtab_dev.index != str_nan]  # filtering out nans
-    
-        # getting all possible combinations for the feature without NaNS
-        combinations = get_all_combinations(order, max_n_mod, raw=False)
-    
-    # keeping nans as a modality
-    else:
-    
-        # getting all possible combinations for the feature with NaNS
-        combinations = get_all_nan_combinations(order, str_nan, max_n_mod)
-
-    # computing association measure per combination 
-    associations = [apply_combination(xtab, combi) for combi in combinations]
-
-    # sort according to association measure
-    if len(combinations) > 0:
-        associations = DataFrame(associations)
-        associations.sort_values(sort_by, inplace=True, ascending=False)
-        associations = associations.to_dict(orient='records')
-
-    # testing associations
-    # case 0: no test set was provided
-    if xtab_test is None and len(associations) > 0:
-        return associations[0]
-    
-    # case 1: testing viability on provided TEST sample
-    else:
-        for association in associations:
-            
-            # needed parameters
-            combination, combi_xtab = association['combination'], association['combi_xtab']
+    # checking for empty datasets
+    xtabs = {feature: None for feature in features}
+    if X is not None:
+        # crosstab for each feature
+        for feature in features:
+            # computing crosstab with str_nan
+            xtab = crosstab(X[feature], y)
 
-            # grouping modalities in the initial crosstab
-            combi_xtab_test = xtab_test.groupby(list(map(combination.get_group, xtab_test.index)), dropna=False).sum()
+            # reordering according to known_order
+            xtab = xtab.reindex(labels_orders[feature])  # TODO: fill nans for x_test?
 
-            # checking that all non-nan groups are in TRAIN and TEST
-            unq_x =  [v for v in unique(combi_xtab.index) if v != notna(v)]
-            unq_xtest = [v for v in unique(combi_xtab_test.index) if v != notna(v)]
-            viability = all([e in unq_x for e in unq_xtest])
-            viability = viability and all([e in unq_xtest for e in unq_x])
+            # storing results
+            xtabs.update({feature: xtab})
 
-            # same target rate order in TRAIN and TEST
-            train_target_rate = combi_xtab[1].divide(combi_xtab[0]).sort_values()
-            test_target_rate = combi_xtab_test[1].divide(combi_xtab_test[0]).sort_values()
-            viability = viability and all(train_target_rate.index == test_target_rate.index)
+    return xtabs
 
-            # checking that some combinations were provided
-            if viability:
 
-                association.update({'combi_xtab_test': combi_xtab_test})
+def association_xtab(xtab: DataFrame, n_obs, n_mod_y) -> Dict[str, float]:
+    """Computes measures of association between feature x and feature2."""
 
-                return association
+    # number of values taken by the features
+    n_mod_x = xtab.shape[0]
 
+    # Chi2 statistic
+    chi2 = chi2_contingency(xtab)[0]
 
-def get_all_combinations(
-        values: GroupedList,
-        max_n_mod: int=None,
-        raw: bool=False
-    ) -> List[GroupedList]:
-    """ Returns all possible triangular combinations"""
+    # Cramer's V
+    cramerv = np.sqrt(chi2 / n_obs / (n_mod_y - 1))
 
-    # maximum number of classes
-    q = len(values)
+    # Tschuprow's T
+    tschuprowt = np.sqrt(chi2 / n_obs / np.sqrt((n_mod_x - 1) * (n_mod_y - 1)))
 
-    # desired max number of classes
-    if max_n_mod is None:
-        max_n_mod = q
+    return {"cramerv": cramerv, "tschuprowt": tschuprowt}
 
-    # all possible combinations
-    combinations = list()
-    for n_class in range(2, max_n_mod + 1):
-        combinations += get_combinations(n_class, q)
 
-    # getting real feature values
-    combinations = [[values[int(c[0]): int(c[1]) + 1] for c in combi] for combi in combinations]
-    
-    # converting back to GroupedList
-    if not raw:
-        combinations = [groupedlist_combination(combination, values) for combination in combinations]
+def vectorized_groupby_sum(xtab: DataFrame, groupby: List[str]):
+    """Groups a crosstab by groupby and sums column values by groups"""
 
-    return combinations
+    # all indices that may be duplicated
+    index_values = np.array(groupby)
 
-def get_all_nan_combinations(
-        order: GroupedList,
-        str_nan: str,
-        max_n_mod: int
-    ) -> List[GroupedList]:
-    """ all possible combinations of modalities with numpy.nan"""
-    
-    # computing all non-NaN combinations
-    # case 0: several modalities -> several combinations
-    if len(order) > 1:
-        combinations = get_all_combinations(order, max_n_mod-1, raw=True)
-    # case 1: unique or no modality -> two combinations
-    else:
-        combinations = []
+    # all unique indices deduplicated
+    unique_indices = np.unique(index_values)
 
-    # iterating over each combinations of non-NaNs
-    new_combinations = []
-    for combi in combinations:
+    # initiating summed up array with zeros
+    summed_values = np.zeros((len(unique_indices), len(xtab.columns)))
 
-         # NaNs not attributed to a group (own modality)
-        new_combinations += [combi + [[str_nan]]] 
+    # for each unique_index found in index_values sums xtab.Values at corresponding position in summed_values
+    np.add.at(summed_values, np.searchsorted(unique_indices, index_values), xtab.values)
 
-        # NaNs attributed to a group of non NaNs
-        for n in range(len(combi)):
+    # converting back to dataframe
+    grouped_xtab = DataFrame(summed_values, index=unique_indices, columns=xtab.columns)
 
-            # grouping NaNs with an existing group
-            new_combination = [combi[n] + [str_nan]]
+    return grouped_xtab
 
-            # adding other groups unchanged
-            pre = [o for o in combi[:n]]
-            nex = [o for o in combi[n+1:]]
-            new_combinations += [pre + new_combination + nex]
-            
-    # adding NaN to order
-    if str_nan not in order:
-        order = order.append(str_nan)
-    
-    # converting back to GroupedList
-    new_combinations = [groupedlist_combination(combination, order) for combination in new_combinations] 
 
-    return new_combinations
+def combinations_at_index(start_idx, order, nb_remaining_groups, min_group_size=1):
+    """Gets all possible combinations of sizes up to the last element of a list"""
 
+    # iterating over each possible length of groups
+    for size in range(min_group_size, len(order) + 1):
+        next_idx = start_idx + size  # index from which to start the next group
 
-def consecutive_combinations(
-        n_remaining: int,
-        start: int,
-        end: int,
-        grp_for_this_step: list=None
-    ) -> None:
-    """HELPER finds all consecutive combinations between start and end.    """
+        # checking that next index is not off the order list
+        if next_idx < len(order) + 1:
+            # checking that there are remaining groups or that it is the last group
+            if (nb_remaining_groups > 1) | (next_idx == len(order)):
+                combination = list(order[start_idx:next_idx])
+                yield (combination, next_idx, nb_remaining_groups - 1)
 
-    # Import de la liste globale
-    global __li_of_res__
 
-    # initiating group
-    if not grp_for_this_step:
-        grp_for_this_step = []
-    
-    # stopping when there are non more remaining classes
-    if n_remaining == 0:
-        
-        ### On ajoute le dernier quantile restant au découpage ###
-        grp_for_this_step += [(start, end)]
+def consecutive_combinations(
+    raw_order,
+    max_group_size,
+    min_group_size=1,
+    nb_remaining_group=None,
+    current_combination=None,
+    next_index=None,
+    all_combinations=None,
+):
+    """Computes all possible combinations of values of order up to max_group_size."""
+
+    # initiating recursive attributes
+    if current_combination is None:
+        current_combination = []
+    if next_index is None:
+        next_index = 0
+    if nb_remaining_group is None:
+        nb_remaining_group = max_group_size
+    if all_combinations is None:
+        all_combinations = []
+
+    # getting combinations for next index
+    next_combinations = [
+        elt
+        for elt in combinations_at_index(next_index, raw_order, nb_remaining_group, min_group_size)
+    ]
+
+    # stop case: no next_combinations possible -> adding to all_combinations
+    if len(next_combinations) == 0 and min_group_size < len(current_combination) <= max_group_size:
+        # saving up combination
+        all_combinations += [current_combination]
+
+        # resetting remaining number of groups
+        nb_remaining_group = max_group_size
+
+    # otherwise: adding all next_combinations to the current_combination
+    for combination, next_index, current_nb_remaining_group in next_combinations:
+        # going a rank further in the raw_xtab
+        consecutive_combinations(
+            raw_order,
+            max_group_size,
+            min_group_size=min_group_size,
+            nb_remaining_group=current_nb_remaining_group,
+            current_combination=current_combination + [combination],
+            next_index=next_index,
+            all_combinations=all_combinations,
+        )
+
+    return all_combinations
+
+
+def xtab_target_rate(xtab: DataFrame) -> DataFrame:
+    """Computes target rate per row for a binary target (column) in a crosstab"""
+
+    return xtab[1].divide(xtab[0]).sort_values()
+
+
+def get_best_association(
+    xtab: DataFrame,
+    combinations: List[List[str]],
+    sort_by: str,
+    xtab_test: DataFrame = None,
+    verbose: bool = False,
+) -> Dict[str, Any]:
+    """Computes associations of the xtab for each combination"""
+
+    # values to groupby indices with
+    indices_to_groupby = [
+        [value for values in ([group[0]] * len(group) for group in combination) for value in values]
+        for combination in combinations
+    ]
+
+    # grouping xtab by its indices
+    grouped_xtabs = [
+        vectorized_groupby_sum(xtab, index_to_groupby)
+        for index_to_groupby in tqdm(
+            indices_to_groupby, disable=not verbose, desc="Grouping modalities   "
+        )
+    ]
+
+    # computing associations for each xtabs
+    n_obs = xtab.sum().sum()  # number of observation
+    n_mod_y = len(xtab.columns)  # number of modalities and minimum number of modalities
+    associations_xtab = [
+        association_xtab(grouped_xtab, n_obs, n_mod_y)
+        for grouped_xtab in tqdm(grouped_xtabs, disable=not verbose, desc="Computing associations")
+    ]
+
+    # adding corresponding combination to the association
+    for combination, index_to_groupby, association, grouped_xtab in zip(
+        combinations, indices_to_groupby, associations_xtab, grouped_xtabs
+    ):
+        association.update(
+            {"combination": combination, "index_to_groupby": index_to_groupby, "xtab": grouped_xtab}
+        )
+
+    # sorting associations according to specified metric
+    associations_xtab = (
+        DataFrame(associations_xtab).sort_values(sort_by, ascending=False).to_dict(orient="records")
+    )
 
-        ### Ajout du découpage réalisé au groupe des solutions ###
-        __li_of_res__ += [grp_for_this_step]
+    # case 0: no test sample provided -> not testing for robustness
+    if xtab_test is None:
+        return associations_xtab[0]
+
+    # case 1: testing viability on provided test sample
+    for association in tqdm(associations_xtab, disable=not verbose, desc="Testing robustness    "):
+        # needed parameters
+        index_to_groupby, xtab = (
+            association["index_to_groupby"],
+            association["xtab"],
+        )
+
+        # grouping rows of the test crosstab
+        grouped_xtab_test = vectorized_groupby_sum(xtab_test, index_to_groupby)
+
+        # computing target rate ranks per value
+        train_ranks = xtab_target_rate(xtab).index
+        test_ranks = xtab_target_rate(grouped_xtab_test).index
+
+        # viable on test sample: grouped values have the same ranks in train/test
+        if all(train_ranks == test_ranks):
+            return association
+
+
+def add_nan_in_combinations(
+    combinations: List[List[str]], str_nan: str, max_n_mod: int
+) -> List[List[str]]:
+    """Adds nan to each possible group and a last group only with nan if the max_n_mod is not reached by the combination"""
+
+    # iterating over each combination
+    nan_combinations = []
+    for combination in combinations:
+        # adding nan to each group of the combination
+        nan_combination = []
+        for n in range(len(combination)):
+            # copying input combination
+            new_combination = combination[:]
+            # adding nan to the nth group
+            new_combination[n] = new_combination[n] + [str_nan]
+            # storing updated combination with attributed group to nan
+            nan_combination += [new_combination]
+
+        # if max_n_mod is not reached adding a combination with nans alone
+        if len(combination) < max_n_mod:
+            # copying input combination
+            new_combination = combination[:]
+            # adding a group for nans only
+            nan_combination += [new_combination + [[str_nan]]]
 
-    
-    # adding all possible combinations of each possible range
-    else:
-        
-        ### Parcours de toutes les valeurs possibles de fin pour le i-ème groupe du groupement à x quantiles ###
-        for i in range(start, end):
+        nan_combinations += nan_combination
 
-            consecutive_combinations(n_remaining-1, i+1, end, grp_for_this_step + [(start, i)])
-            
-def get_combinations(n_class: int, q: int) -> List[List[str]]:
-    """HELPER recupération des combinaisons possibles de q quantiles pour n_class."""
-    
-    globals()['__li_of_res__'] = []
-
-    consecutive_combinations(n_class-1, 0, q-1)
-    
-    combinations = [list(map(lambda u: (str(u[0]).zfill(len(str(q-1))), str(u[1]).zfill(len(str(q-1)))), l)) for l in __li_of_res__]
-    
-    return combinations
+    return nan_combinations
 
-def association_xtab(xtab: DataFrame) -> Dict[str, float]:
-    """ Computes measures of association between feature x and feature2. """
 
-    # numnber of observations
-    n_obs = xtab.sum().sum()
+def order_apply_combination(order: GroupedList, combination: List[List[Any]]) -> GroupedList:
+    """Converts a list of combination to a GroupedList"""
 
-    # number of values taken by the features
-    n_mod_x, n_mod_y = len(xtab.index), len(xtab.columns)
-    min_n_mod = min(n_mod_x, n_mod_y)
+    order_copy = GroupedList(order)
+    for combi in combination:
+        order_copy.group_list(combi, combi[0])
 
-    # Chi2 statistic
-    chi2 = chi2_contingency(xtab)[0]
+    return order_copy
 
-    # Cramer's V
-    cramerv = 0
-    if min_n_mod > 1:
-        cramerv = sqrt(chi2 / n_obs / (min_n_mod - 1))
 
-    # Tschuprow's T
-    dof_mods = sqrt((n_mod_x - 1) * (n_mod_y - 1))
-    tschuprowt = 0
-    if dof_mods > 0:
-        tschuprowt = sqrt(chi2 / n_obs / dof_mods)
-
-    results = {'cramerv': cramerv, 'tschuprowt': tschuprowt}
-    
-    return results
+def xtab_apply_order(xtab: DataFrame, order: GroupedList) -> DataFrame:
+    """Applies an order (combination) to a crosstab
 
-def nan_crosstab(
-        x: Series,
-        y: Series,
-        str_nan: str='__NAN__'
-    ):
-    """ Crosstab that keeps nans as a specific value"""
-    
-    # keeping NaNs as a specific modality
-    x_filled = x.fillna(str_nan)  # filling NaNs
-
-    # computing initial crosstabs
-    xtab = crosstab(x_filled, y)
-    
-    return xtab
+    Parameters
+    ----------
+    xtab : DataFrame
+        Crosstab
+    order : GroupedList
+        Combination of index to apply to the crosstab
+
+    Returns
+    -------
+    Dict[str, Any]
+        _description_
+    """
+    # checking for input values
+    combi_xtab = None
+    if xtab is not None:
+        # grouping modalities in the crosstab
+        groups = list(map(order.get_group, xtab.index))
+        combi_xtab = xtab.groupby(groups, dropna=False, sort=False).sum()
+
+    return combi_xtab
 
 
 def plot_stats(stats: DataFrame) -> Tuple[Figure, Axes]:
-    """ Barplot of the volume and target rate"""
-    
-    x = [0] + [elt for e in stats['frequency'].cumsum()[:-1] for elt in [e] * 2] + [1]
-    y2 = [elt for e in list(stats['target_rate']) for elt in [e]*2]
+    """Barplot of the volume and target rate"""
+
+    x = [0] + [elt for e in stats["frequency"].cumsum()[:-1] for elt in [e] * 2] + [1]
+    y2 = [elt for e in list(stats["target_rate"]) for elt in [e] * 2]
     s = list(stats.index)
-    scaled_y2 = [(y-min(y2)) / (max(y2) - min(y2)) for y in y2]
+    scaled_y2 = [(y - min(y2)) / (max(y2) - min(y2)) for y in y2]
     c = color_palette("coolwarm", as_cmap=True)(scaled_y2)
 
     fig, ax = subplots()
 
     for i in range(len(stats)):
-        k = i*2
-        ax.fill_between(x[k: k+2], [0, 0], y2[k: k+2], color=c[k])
-        ax.text(sum(x[k: k+2]) / 2, y2[k], s[i], rotation=90, ha='center', va='bottom')
-
-    ax.xaxis.set_major_formatter(PercentFormatter(xmax=1))    
-    ax.yaxis.set_major_formatter(PercentFormatter(xmax=1))    
-    ax.set_xlabel('Volume')
-    ax.set_ylabel('Target rate')
+        k = i * 2
+        ax.fill_between(x[k : k + 2], [0, 0], y2[k : k + 2], color=c[k])
+        ax.text(
+            sum(x[k : k + 2]) / 2,
+            y2[k],
+            s[i],
+            rotation=90,
+            ha="center",
+            va="bottom",
+        )
+
+    ax.xaxis.set_major_formatter(PercentFormatter(xmax=1))
+    ax.yaxis.set_major_formatter(PercentFormatter(xmax=1))
+    ax.set_xlabel("Volume")
+    ax.set_ylabel("Target rate")
     ax.set_xlim(0, 1)
     ax.set_ylim(0)
     despine()
-    
+
     return fig, ax
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `AutoCarver-4.4.1/AutoCarver/Converters.py` & `AutoCarver-5.0.0/AutoCarver/converters.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,286 +1,378 @@
-from numpy import select, nan, tanh
-from pandas import isna, notna, DataFrame, Series, to_datetime
-from sklearn.base import BaseEstimator, TransformerMixin
-from typing import List, Tuple, Any, Dict
-
+"""Tools for FeatureEngineering."""
 
-class StringConverter(BaseEstimator, TransformerMixin):
-    """ Converts specified columns a DataFrame into str
-    
-     - Keeps NaN inplace
-     - Converts floats of int to int
+from typing import Any, Dict, List
 
-    Parameters
-    ----------
-    features: list, default []
-        List of columns to be converted to string.
-    """
-    
-    def __init__(self, features: List[str]=[], copy: bool=False) -> None:
-    
-        self.features = features[:]
-        self.copy = copy
-        
-    def fit(self, X: DataFrame, y: Series=None):
-        
-        return self
-        
-    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
-        
-        # copying DataFrame if requested
-        Xc = X
-        if self.copy:
-            Xc = X.copy()
-
-        # storing nans
-        nans = isna(Xc[self.features])
-
-        # storing ints
-        ints = Xc[self.features].applymap(lambda u: isinstance(u, float) and float.is_integer(u))
-        
-        # converting to string
-        Xc[self.features] = Xc[self.features].astype(str)
-        
-        # converting to int-strings
-        converted_ints = Xc[ints][self.features].applymap(lambda u: str(int(float(u))) if isinstance(u, str) else u)
-        Xc[self.features] = select([ints], [converted_ints], default=Xc[self.features])
-        
-        # converting back to nan
-        Xc[nans] = nan
-        
-        return Xc
+from numpy import nan, tanh
+from pandas import DataFrame, Series, notna, to_datetime
+from sklearn.base import BaseEstimator, TransformerMixin
 
 
 class TimeDeltaConverter(BaseEstimator, TransformerMixin):
-    """ Converts specified DateTime columns into TimeDeltas between themselves
+    """Converts specified DateTime columns into TimeDeltas between themselves
 
      - Str Columns are converted to pandas datetime columns
      - New TimeDelta column names are stored in TimeDeltaConverter.delta_features
 
     Parameters
     ----------
     features: List[str]
         List of DateTime columns to be converted to string.
     nans: Any, default numpy.nan
         Date value to be considered as missing data.
     drop: bool, default True
         Whether or not to drop initial DateTime columns (specified in features).
     """
-    
-    def __init__(self, features: List[str], nans: Any=nan, copy: bool=False, drop: bool=True) -> None:
-        
+
+    def __init__(
+        self,
+        features: List[str],
+        nans: Any = nan,
+        copy: bool = False,
+        drop: bool = True,
+    ) -> None:
+        """_summary_
+
+        Parameters
+        ----------
+        features : List[str]
+            _description_
+        nans : Any, optional
+            _description_, by default nan
+        copy : bool, optional
+            _description_, by default False
+        drop : bool, optional
+            _description_, by default True
+        """
+        print("Warning: not tested for package version greater than 4.")
         self.features = features[:]
         self.copy = copy
         self.new_features: List[str] = []
         self.nans = nans
         self.drop = drop
-        
+
     def fit(self, X: DataFrame, y=None) -> None:
-        
+        """_summary_
+
+        Parameters
+        ----------
+        X : DataFrame
+            _description_
+        y : _type_, optional
+            _description_, by default None
+        """
         # creating list of names of delta featuers
         for i, date1 in enumerate(self.features):
-            for date2 in self.features[i+1:]:
-                self.new_features += [f'delta_{date1}_{date2}']
-        
+            for date2 in self.features[i + 1 :]:
+                self.new_features += [f"delta_{date1}_{date2}"]
+
         return self
-    
-    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
-        
+
+    def transform(self, X: DataFrame, y: Series = None) -> DataFrame:
+        """_summary_
+
+        Parameters
+        ----------
+        X : DataFrame
+            _description_
+        y : Series, optional
+            _description_, by default None
+
+        Returns
+        -------
+        DataFrame
+            _description_
+        """
         # copying dataset
         Xc = X
         if self.copy:
             Xc = X.copy()
-            
+
         # converting back nans
         if notna(self.nans):
-            Xc[self.features] = Xc[self.features].where(Xc[self.features]!=self.nans, nan)
-        
+            Xc[self.features] = Xc[self.features].where(Xc[self.features] != self.nans, nan)
+
         # converting to datetime
         Xc[self.features] = to_datetime(Xc[self.features].stack()).unstack()
-        
+
         # iterating over each combination of dates
         for i, date1 in enumerate(self.features):
-            for date2 in self.features[i+1:]:
-                
+            for date2 in self.features[i + 1 :]:
                 # computing timedelta of days
-                Xc[f'delta_{date1}_{date2}'] = (Xc[date1] - Xc[date2]).dt.days
-        
+                Xc[f"delta_{date1}_{date2}"] = (Xc[date1] - Xc[date2]).dt.days
+
         # dropping date columns
         Xc = Xc.drop(self.features, axis=1)
-        
+
         return Xc
 
+
 class GroupNormalizer(BaseEstimator, TransformerMixin):
-    """ Normalizes a feature's values based on specified means and stds per groups' values
+    """Normalizes a feature's values based on specified means and stds per groups' values
 
     Parameters
     ----------
     groups: List[str]
         List of qualitative features used to compute feature's mean/std per there modalities.
     features: List[str]
         List of quantitative features to be normalized.
     """
 
-    def __init__(self, groups: List[str], features: List[str], copy: bool=True) -> None:
-        
+    def __init__(self, groups: List[str], features: List[str], copy: bool = True) -> None:
+        """_summary_
+
+        Parameters
+        ----------
+        groups : List[str]
+            _description_
+        features : List[str]
+            _description_
+        copy : bool, optional
+            _description_, by default True
+        """
+        print("Warning: not tested for package version greater than 4.")
         self.features = features[:]
         self.groups = groups[:]
-        
+
         self.copy = copy
-        
-        self.group_means = dict()
-        self.group_stds = dict()
-        
-        self.new_features = list()
 
-    def fit(self, X: DataFrame, y: Series=None) -> None:
-        
+        self.group_means = {}
+        self.group_stds = {}
+
+        self.new_features = []
+
+    def fit(self, X: DataFrame, y: Series = None) -> None:
+        """_summary_
+
+        Parameters
+        ----------
+        X : DataFrame
+            _description_
+        y : Series, optional
+            _description_, by default None
+        """
         # iterating over each grouping column
         for group in self.groups:
-            
             # computing group mean
             self.group_means.update({group: X.groupby(group)[self.features].mean().to_dict()})
-            
+
             # computing group std
             self.group_stds.update({group: X.groupby(group)[self.features].std().to_dict()})
-            
+
             # adding built features
             self.new_features += [f"{f}_norm_{group}" for f in self.features]
 
         return self
 
-    
+    def transform(self, X: DataFrame, y: Series = None) -> DataFrame:
+        """_summary_
 
-    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
-        
+        Parameters
+        ----------
+        X : DataFrame
+            _description_
+        y : Series, optional
+            _description_, by default None
+
+        Returns
+        -------
+        DataFrame
+            _description_
+        """
         # coppying dataframe
         Xc = X
         if self.copy:
             Xc = X.copy()
-        
+
         # iterating over each group
         for group in self.groups:
-            
             # computing observation level mean
-            means = Xc[self.features].apply(lambda u: Xc[group].apply(self.group_means[group][u.name].get))
+            means = Xc[self.features].apply(
+                lambda u: Xc[group].apply(self.group_means[group][u.name].get)
+            )
 
             # computing observation level std
-            stds = Xc[self.features].apply(lambda u: Xc[group].apply(self.group_stds[group][u.name].get))
-            
+            stds = Xc[self.features].apply(
+                lambda u: Xc[group].apply(self.group_stds[group][u.name].get)
+            )
+
             # applying normalization to the feature
             Xc = Xc.join(
-                Xc[self.features].sub(means)\
-                                 .replace(0, nan)\
-                                 .divide(stds)\
-                                 .rename({f: f"{f}_norm_{group}" for f in self.features}, axis=1)
+                Xc[self.features]
+                .sub(means)
+                .replace(0, nan)
+                .divide(stds)
+                .rename({f: f"{f}_norm_{group}" for f in self.features}, axis=1)
             )
 
         del means
         del stds
-        
+
         return Xc
 
+
 class TanhNormalizer(BaseEstimator, TransformerMixin):
-    """ Tanh Normalization that keeps data distribution and borns between 0 and 1
+    """Tanh Normalization that keeps data distribution and borns between 0 and 1
 
     Parameters
     ----------
     features: List[str]
         List of quantitative features to be normalized.
     """
-    
-    def __init__(self, features: List[str], copy: bool=False) -> None:
-        
+
+    def __init__(self, features: List[str], copy: bool = False) -> None:
+        """_summary_
+
+        Parameters
+        ----------
+        features : List[str]
+            _description_
+        copy : bool, optional
+            _description_, by default False
+        """
+        print("Warning: not tested for package versions greater than 4.")
         self.features = features[:]
         self.copy = copy
-        
+
+        self.distribs = None
+
     def fit(self, X: DataFrame, y=None) -> None:
-        
-        self.distribs = X[self.features].agg(['mean', 'std']).to_dict(orient='index')
-        
+        """_summary_
+
+        Parameters
+        ----------
+        X : DataFrame
+            _description_
+        y : _type_, optional
+            _description_, by default None
+        """
+        self.distribs = X[self.features].agg(["mean", "std"]).to_dict(orient="index")
+
         return self
-    
-    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
-        
+
+    def transform(self, X: DataFrame, y: Series = None) -> DataFrame:
+        """_summary_
+
+        Parameters
+        ----------
+        X : DataFrame
+            _description_
+        y : Series, optional
+            _description_, by default None
+
+        Returns
+        -------
+        DataFrame
+            _description_
+        """
         # copying dataset
         Xc = X
         if self.copy:
             Xc = X.copy()
-        
+
         # applying tanh normalization
-        Xc[self.features] = (tanh(Xc[self.features].sub(self.distribs['mean']).divide(self.distribs['std']) * 0.01) + 1 ) / 2
-        
+        Xc[self.features] = (
+            tanh(Xc[self.features].sub(self.distribs["mean"]).divide(self.distribs["std"]) * 0.01)
+            + 1
+        ) / 2
+
         return Xc
 
+
 class CrossConverter(BaseEstimator, TransformerMixin):
-    """ Normalizes a feature's values based on specified means and stds per groups' values
+    """Normalizes a feature's values based on specified means and stds per groups' values
 
     Parameters
     ----------
     features: List[str]
         List of qualitative features to be crossed should be passed through AutoCarver early on.
     """
 
-    def __init__(self, features: List[str], copy: bool=True) -> None:
-        
+    def __init__(self, features: List[str], copy: bool = True) -> None:
+        """_summary_
+
+        Parameters
+        ----------
+        features : List[str]
+            _description_
+        copy : bool, optional
+            _description_, by default True
+        """
+        print("Warning: not tested for package version greater than 4.")
         self.features = features[:]
         self.copy = copy
-        self.new_features: List[str] = list()
-        self.values: Dict[str, List[Any]] = dict()
+        self.new_features: List[str] = []
+        self.values: Dict[str, List[Any]] = {}
 
-    def fit(self, X: DataFrame, y: Series=None) -> None:
-        
+    def fit(self, X: DataFrame, y: Series = None) -> None:
+        """_summary_
+
+        Parameters
+        ----------
+        X : DataFrame
+            _description_
+        y : Series, optional
+            _description_, by default None
+        """
         # iterating over each feature
         for i, feature1 in enumerate(self.features):
-            
             # unique values of feature1
             unq1 = X[feature1].astype(str).unique()
-            
-            for feature2 in self.features[i+1:]:
-            
+
+            for feature2 in self.features[i + 1 :]:
                 # adding features names to the list of built features
-                self.new_features += [f'{feature2}_x_{feature1}']
-            
+                self.new_features += [f"{feature2}_x_{feature1}"]
+
                 # unique values of feature2
                 unq2 = X[feature2].astype(str).unique()
-                
-                self.values.update({
-                    f'{feature2}_x_{feature1}': [u2 + '_x_' + u1 for u2 in unq2 for u1 in unq1]
-                })
+
+                self.values.update(
+                    {f"{feature2}_x_{feature1}": [u2 + "_x_" + u1 for u2 in unq2 for u1 in unq1]}
+                )
 
         return self
 
-    
+    def transform(self, X: DataFrame, y: Series = None) -> DataFrame:
+        """_summary_
 
-    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
-        
+        Parameters
+        ----------
+        X : DataFrame
+            _description_
+        y : Series, optional
+            _description_, by default None
+
+        Returns
+        -------
+        DataFrame
+            _description_
+        """
         # coppying dataframe
         Xc = X
         if self.copy:
             Xc = X.copy()
-            
+
         # converting features to strings
         Xc_features = Xc[self.features].astype(str)
-        
+
         # iterating over each group
         for i, feature in enumerate(self.features):
-            
             # features to cross with
-            Xc_tocross = Xc_features[self.features[i+1:]]
-            
+            Xc_tocross = Xc_features[self.features[i + 1 :]]
+
             # feature to be crossed
             Xc_crosser = Xc_features[feature]
 
             # crossing features
-            Xc_crossed = Xc_tocross.apply(lambda u: u + '_x_' + Xc_crosser)\
-                                   .rename({f: f"{f}_x_{feature}" for f in self.features[i+1:]}, axis=1)
-            
+            Xc_crossed = Xc_tocross.apply(lambda u: u + "_x_" + Xc_crosser).rename(
+                {f: f"{f}_x_{feature}" for f in self.features[i + 1 :]}, axis=1
+            )
+
             # applying normalization to the feature
             Xc = Xc.join(Xc_crossed)
-        
+
         del Xc_features
         del Xc_crossed
         del Xc_tocross
         del Xc_crosser
-        
-        return Xc
+
+        return Xc
```

### Comparing `AutoCarver-4.4.1/AutoCarver/FeatureSelector.py` & `AutoCarver-5.0.0/AutoCarver/feature_selector.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,59 @@
-from IPython.display import display_html
+"""Tools to select the best Quantitative and Qualitative features."""
+
 from math import sqrt
-from numpy import triu, ones, nan, inf
-from pandas import DataFrame, Series, notna, crosstab
 from random import shuffle
-from scipy.stats import kruskal, chi2_contingency
+from typing import Any, Callable, Dict, Tuple
+
+from IPython.display import display_html
+from numpy import inf, nan, ones, triu
+from pandas import DataFrame, Series, crosstab, notna
+from scipy.stats import chi2_contingency, kruskal
 from sklearn.base import BaseEstimator, TransformerMixin
 from statsmodels.formula.api import ols
 from statsmodels.stats.outliers_influence import variance_inflation_factor
-from typing import List, Dict, Any, Callable, Tuple
 
+from .discretizers.utils.base_discretizers import GroupedList, GroupedListDiscretizer
 
+# TODO: convert to groupedlistdiscretizer
+# TODO: add parameter to shut down displayed info
 class FeatureSelector(BaseEstimator, TransformerMixin):
-    """ A pipeline of measures to perform EDA and feature pre-selection
-     
+    """A pipeline of measures to perform EDA and feature pre-selection
+
      - best features are the n_best of each measure
      - selected features are stored in FeatureSelector.best_features
-        
+
     Parameters
     ----------
-    features: List[str]
+    features: list[str]
         Features on which to compute association.
     n_best, int:
         Number of features to be selected
     sample_size: float, default 1.
         Should be set between ]0, 1]
-        Size of sampled list of features speeds up computation. 
+        Size of sampled list of features speeds up computation.
         By default, all features are used. For sample_size=0.5,
-        FeatureSelector will search for the best features in 
+        FeatureSelector will search for the best features in
         features[:len(features)//2] and then in features[len(features)//2:]
-    measures, List[Callable]: default list().
+    measures, list[Callable]: default list().
         List of association measures to be used.
         Implemented measures are:
-            [Quantitative Features] 
+            [Quantitative Features]
              - For association evaluation: `kruskal_measure`, `R_measure`
              - For outlier detection: `zscore_measure`, `iqr_measure`
-            [Qualitative Features] 
+            [Qualitative Features]
              - For correlation: `chi2_measure`, `cramerv_measure`, `tschuprowt_measure`
         Ranks features based on last measure of the list.
-    filters, List[Callable]: default list().
+    filters, list[Callable]: default list().
         List of filters to be used.
         Implemented filters are:
-            [Quantitative Features] 
+            [Quantitative Features]
              - For linear correlation: `spearman_filter`, `pearson_filter`
              - For multicoloinearity: `vif_filter`
-            [Qualitative Features] 
+            [Qualitative Features]
              - For correlation: `cramerv_filter`, `tschuprowt_filter`
 
     Thresholds (to be passed as kwargs)
     ----------
     thresh_measure, float: default 0.
         Minimum association between target and features
         To be used with: `measure_filter`
@@ -70,692 +76,786 @@
         Maximum VIF between features
         To be used with: `vif_filter`
     ascending, bool default False
         According to this measure:
          - True: Lower values of the measure are to be considered as more associated to the target
          - False: Higher values of the measure are to be considered as more associated to the target
     """
-    
+
     def __init__(
-            self,
-            features: List[str],
-            n_best: int,
-            measures: List[Callable]=list(),
-            filters: List[Callable]=list(),
-            sample_size: float=1.,
-            copy: bool=True,
-            verbose: bool=True,
-            **params
-        ) -> None:
-        
-        self.features = features[:]
+        self,
+        features: list[str],
+        n_best: int,
+        measures: list[Callable],
+        *,
+        filters: list[Callable] = None,
+        sample_size: float = 1.0,
+        values_orders: dict[str, GroupedList] = None,
+        copy: bool = True,
+        drop: bool = False,  # TODO
+        verbose: bool = True,
+        **params,
+    ) -> None:
+        """_summary_
+
+        Parameters
+        ----------
+        features : list[str]
+            _description_
+        n_best : int
+            _description_
+        measures : list[Callable], optional
+            _description_, by default list()
+        filters : list[Callable], optional
+            _description_, by default list()
+        sample_size : float, optional
+            _description_, by default 1.0
+        copy : bool, optional
+            _description_, by default True
+        verbose : bool, optional
+            _description_, by default True
+        """
+        print("Warning: not fully optimized for package versions greater than 4.")
+
+        self.features = list(set(features))
         self.n_best = n_best
         assert n_best <= len(features), "Must set n_best <= len(features)"
         self.best_features = features[:]
         self.sample_size = sample_size
-        
+
         self.measures = [dtype_measure, nans_measure, mode_measure] + measures[:]
+        if filters is None:
+            filters = []
         self.filters = [thresh_filter] + filters[:]
         self.sort_measures = [measure.__name__ for measure in measures[::-1]]
 
+        # Values_orders from GroupedListDiscretizer
+        if values_orders is None:
+            values_orders = {}
+        self.values_orders = {feature: GroupedList(value) for feature, value in values_orders.items()}
+
+        self.drop = drop
         self.copy = copy
         self.verbose = verbose
         self.params = params
-    
+
+        self.associations = None
+        self.filtered_associations = None
+
     def measure(self, x: Series, y: Series) -> Dict[str, Any]:
-        """ Measures association between x and y """
-        
+        """Measures association between x and y"""
+
         passed = True  # measures keep going only if previous basic tests are passed
         association = {}
 
         # iterating over each measure
         for measure in self.measures:
             passed, association = measure(passed, association, x, y, **self.params)
-            
+
         return association
-    
-    def measure_apply(self, X: DataFrame, y: Series, features: List[str]) -> None:
-        """ Measures association between columns of X and y
 
-    Parameters
-    ----------
-    ascending, bool default False
-        According to this measure:
-         - True: Lower values of the measure are to be considered as more associated to the target
-         - False: Higher values of the measure are to be considered as more associated to the target
-    """
-        
+    def measure_apply(self, X: DataFrame, y: Series, features: list[str]) -> None:
+        """Measures association between columns of X and y
+
+        Parameters
+        ----------
+        ascending, bool default False
+            According to this measure:
+             - True: Lower values of the measure are to be considered as more associated to the target
+             - False: Higher values of the measure are to be considered as more associated to the target
+        """
+
         # applying association measure to each column
-        self.associations = X[features].apply(self.measure, y=y, result_type='expand', axis=0).T
-        
+        self.associations = X[features].apply(self.measure, y=y, result_type="expand", axis=0).T
+
         # filtering non association measure (pct_zscore, pct_iqr...)
-        asso_measures = [c for c in self.associations if '_measure' in c]
+        asso_measures = [c for c in self.associations if "_measure" in c]
         self.sort_measures = [c for c in self.sort_measures if c in asso_measures]
-        
+
         # sorting statistics if an association measure was provided
         self.associations = self.associations.sort_values(
-            self.sort_measures, ascending=self.params.get('ascending', False)
+            self.sort_measures, ascending=self.params.get("ascending", False)
         )
-    
+
     def filter_apply(self, X: DataFrame, sort_measure: str) -> DataFrame:
-        """ Filters out too correlated features (least relevant first)
+        """Filters out too correlated features (least relevant first)
+
+        Parameters
+        ----------
+        ascending, bool default False
+            According to this measure:
+             - True: Lower values of the measure are to be considered as more associated to the target
+             - False: Higher values of the measure are to be considered as more associated to the target
+        """
 
-    Parameters
-    ----------
-    ascending, bool default False
-        According to this measure:
-         - True: Lower values of the measure are to be considered as more associated to the target
-         - False: Higher values of the measure are to be considered as more associated to the target
-    """
-        
         # ordering features by sort_by
-        self.filtered_associations = self.associations.sort_values(sort_measure, ascending=self.params.get('ascending', False))
+        self.filtered_associations = self.associations.sort_values(
+            sort_measure, ascending=self.params.get("ascending", False)
+        )
 
         # applying successive filters
         for filtering in self.filters:
-
             # ordered filtering
             self.filtered_associations = filtering(X, self.filtered_associations, **self.params)
-    
+
     def display_stats(self, association: DataFrame, caption: str) -> None:
-        """ EDA of fitted associations"""
-        
-        # appllying style 
-        subset = [c for c in association if 'pct_' in c or '_measure' in c or '_filter' in c]
-        style = association.style.background_gradient(cmap='coolwarm', subset=subset)
+        """EDA of fitted associations"""
+
+        # appllying style
+        subset = [c for c in association if "pct_" in c or "_measure" in c or "_filter" in c]
+        style = association.style.background_gradient(cmap="coolwarm", subset=subset)
         style = style.set_table_attributes("style='display:inline'")
         style = style.set_caption(caption)
         display_html(style._repr_html_(), raw=True)
-        
-    def fit_features(self, X: DataFrame, y: Series, features: List[str], n_best: int) -> List[str]:
-        """ Selects the n_best features amongst the specified ones"""
-        
+
+    def fit_features(self, X: DataFrame, y: Series, features: list[str], n_best: int) -> list[str]:
+        """Selects the n_best features amongst the specified ones"""
+
         # initial computation of all association measures
         self.measure_apply(X, y, features)
 
         # displaying association measure
         if self.verbose:
-            self.display_stats(self.associations, 'Raw association')
-        
-        # iterating over each sort_measures 
+            self.display_stats(self.associations, "Raw association")
+
+        # iterating over each sort_measures
         # useful when measures hints to specific associations
         ranks = []
         for n, sort_measure in enumerate(self.sort_measures):
-            
             # filtering by sort_measure
             self.filter_apply(X, sort_measure)
             ranks += [list(self.filtered_associations.index)]
 
             # displaying filtered out association measure
             if n == 0 and self.verbose and len(self.filters) > 1:
-                self.display_stats(self.filtered_associations, 'Filtered association')
+                self.display_stats(self.filtered_associations, "Filtered association")
 
         # retrieving the n_best features per each ranking
         best_features = []
         if len(self.sort_measures) > 0:
             best_features = [feature for rank in ranks for feature in rank[:n_best]]
             best_features = list(set(best_features))  # deduplicating
-        
+
         return best_features
-    
+
     def fit(self, X: DataFrame, y: Series) -> None:
-        """ Selects the n_best features"""
-        
+        """Selects the n_best features"""
+
         # splitting features in chunks
         if self.sample_size < 1:
-            
             # shuffling features to get random samples of features
             shuffle(self.features)
 
             # number of features per sample
             chunks = int(len(self.features) // (1 / self.sample_size))
 
             # splitting feature list in samples
-            feature_samples = [self.features[chunks * i: chunks * (i + 1)] for i in range(int(1 / self.sample_size)-1)]
+            feature_samples = [
+                self.features[chunks * i : chunks * (i + 1)]
+                for i in range(int(1 / self.sample_size) - 1)
+            ]
 
             # adding last sample with all remaining features
-            feature_samples += [self.features[chunks * (int(1 / self.sample_size) - 1):]]
+            feature_samples += [self.features[chunks * (int(1 / self.sample_size) - 1) :]]
 
             # iterating over each feature samples
             best_features = []
             for features in feature_samples:
-
                 # fitting association on features
                 best_features += self.fit_features(X, y, features, int(self.n_best // 2))
-        
+
         # splitting in chunks not requested
         else:
             best_features = self.features[:]
-        
+
         # final selection with all best_features selected
         self.best_features = self.fit_features(X, y, best_features, self.n_best)
-            
-        # dropped features
-        self.dropped_features = [c for c in self.features if c not in self.best_features]
 
-        return self
+        # ordering best_features according to their rank
+        self.best_features = [
+            f for f in self.filtered_associations.index if f in self.best_features
+        ]
+
+        # removing feature from values_orders
+        dropped_features = [f for f in self.associations.index if f not in self.best_features]
+        for feature in dropped_features:
+            if feature in self.values_orders:
+                self.values_orders.pop(feature)
 
-    def transform(self, X: DataFrame, y: Series=None) -> DataFrame:
+        return self
 
-        # copying dataset
-        Xc = X
-        if self.copy:
-            Xc.copy()
+    def transform(self, X: DataFrame, y: Series = None) -> DataFrame:
+        """Drops the non-selected columns from `features`.
 
-        # filtering out unwanted features
-        Xc = Xc.drop(self.dropped_features, axis=1)
+        Parameters
+        ----------
+        X : DataFrame
+            Contains columns named in `features`
+        y : Series, optional
+            Model target, by default None
+
+        Returns
+        -------
+        DataFrame
+            `X` without non-selected columns from `features`.
+        """
 
-        return Xc
+        return X
 
 
 # MEASURES
-def nans_measure(active: bool, association: Dict[str, Any], x: Series, y: Series=None, **params) -> Tuple[bool, Dict[str, Any]]:
-    """ Measure of the percentage of NaNs
+def nans_measure(
+    active: bool,
+    association: Dict[str, Any],
+    x: Series,
+    y: Series = None,
+    **params,
+) -> Tuple[bool, Dict[str, Any]]:
+    """Measure of the percentage of NaNs
 
     Parameters
     ----------
     thresh_nan, float: default 1.
       Maximum percentage of NaNs in a feature
     """
-    
+
     # whether or not tests where passed
     if active:
-    
         nans = x.isnull()  # ckecking for nans
-        pct_nan = nans.mean()   # Computing percentage of nans
-    
+        pct_nan = nans.mean()  # Computing percentage of nans
+
         # updating association
-        association.update({'pct_nan': pct_nan})
-    
+        association.update({"pct_nan": pct_nan})
+
         # Excluding feature that have to many NaNs
-        active = pct_nan < params.get('thresh_nan', 1.)
-    
+        active = pct_nan < params.get("thresh_nan", 1.0)
+
     return active, association
 
-def dtype_measure(active: bool, association: Dict[str, Any], x: Series, y: Series=None, **params) -> Tuple[bool, Dict[str, Any]]:
-    """ Gets dtype"""
-    
+
+def dtype_measure(
+    active: bool,
+    association: Dict[str, Any],
+    x: Series,
+    y: Series = None,
+    **params,
+) -> Tuple[bool, Dict[str, Any]]:
+    """Gets dtype"""
+
     # updating association
-    association.update({'dtype': x.dtype})
-        
+    association.update({"dtype": x.dtype})
+
     return active, association
 
-def mode_measure(active: bool, association: Dict[str, Any], x: Series, y: Series=None, **params) -> Tuple[bool, Dict[str, Any]]:
-    """ Measure of the percentage of the Mode
+
+def mode_measure(
+    active: bool,
+    association: Dict[str, Any],
+    x: Series,
+    y: Series = None,
+    **params,
+) -> Tuple[bool, Dict[str, Any]]:
+    """Measure of the percentage of the Mode
 
     Parameters
     ----------
     thresh_mode, float: default 1.
       Maximum percentage of the mode of a feature
     """
-    
+
     # whether or not tests where passed
     if active:
-    
         mode = x.mode(dropna=True).values[0]  # computing mode
         pct_mode = (x == mode).mean()  # Computing percentage of the mode
-    
+
         # updating association
-        association.update({'pct_mode': pct_mode, 'mode': mode})
-    
+        association.update({"pct_mode": pct_mode, "mode": mode})
+
         # Excluding feature with too frequent modes
-        active = pct_mode < params.get('thresh_mode', 1.)
-    
+        active = pct_mode < params.get("thresh_mode", 1.0)
+
     return active, association
 
-def kruskal_measure(active: bool, association: Dict[str, Any], x: Series, y: Series, **params) -> Tuple[bool, Dict[str, Any]]:
-    """ Kruskal-Wallis statistic between x (quantitative) and y (binary)"""
-    
+
+def kruskal_measure(
+    active: bool, association: Dict[str, Any], x: Series, y: Series, **params
+) -> Tuple[bool, Dict[str, Any]]:
+    """Kruskal-Wallis statistic between x (quantitative) and y (binary)"""
+
     # check that previous steps where passed
     if active:
-    
         nans = x.isnull()  # ckecking for nans
-        
+
         # computation of Kruskal-Wallis statistic
         kw = kruskal(x[(~nans) & (y == 0)], x[(~nans) & (y == 1)])
-        
+
         # updating association
         if kw:
-            association.update({'kruskal_measure': kw[0]})
-        
+            association.update({"kruskal_measure": kw[0]})
+
     return active, association
 
-def R_measure(active: bool, association: Dict[str, Any], x: Series, y: Series, **params) -> Tuple[bool, Dict[str, Any]]:
-    """ R of the linear regression of x (quantitative) by y (binary)"""
-    
+
+def R_measure(
+    active: bool, association: Dict[str, Any], x: Series, y: Series, **params
+) -> Tuple[bool, Dict[str, Any]]:
+    """R of the linear regression of x (quantitative) by y (binary)"""
+
     # check that previous steps where passed
     if active:
-    
         nans = x.isnull()  # ckecking for nans
 
         # grouping feature and target
-        ols_df = DataFrame({'feature': x[~nans], 'target': y[~nans]})
-        
+        ols_df = DataFrame({"feature": x[~nans], "target": y[~nans]})
+
         # fitting regression of feature by target
-        regression = ols('feature~C(target)', ols_df).fit()
-        
+        regression = ols("feature~C(target)", ols_df).fit()
+
         # updating association
         if regression.rsquared:
             if regression.rsquared >= 0:
-                association.update({'R_measure': sqrt(regression.rsquared)})
+                association.update({"R_measure": sqrt(regression.rsquared)})
             else:
-                association.update({'R_measure': nan})
-        
+                association.update({"R_measure": nan})
+
     return active, association
 
 
-def zscore_measure(active: bool, association: Dict[str, Any], x: Series, y: Series=None, **params) -> Tuple[bool, Dict[str, Any]]:
-    """ Computes outliers based on the z-score
+def zscore_measure(
+    active: bool,
+    association: Dict[str, Any],
+    x: Series,
+    y: Series = None,
+    **params,
+) -> Tuple[bool, Dict[str, Any]]:
+    """Computes outliers based on the z-score
 
     Parameters
     ----------
     thresh_outlier, float: default 1.
       Maximum percentage of Outliers in a feature
     """
-    
+
     # check that previous steps where passed for computational optimization
     if active:
-        
         mean = x.mean()  # mean of the feature
         std = x.std()  # standard deviation of the feature
-        zscore = (x-mean) / std  # zscore per observation
-        
+        zscore = (x - mean) / std  # zscore per observation
+
         # checking for outliers
         outliers = abs(zscore) > 3
         pct_zscore = outliers.mean()
-        
+
         # updating association
-        association.update({
-            'pct_zscore': pct_zscore,
-            'min': x.min(),
-            'max': x.max(),
-            'mean': mean,
-            'std': std
-        })
+        association.update(
+            {
+                "pct_zscore": pct_zscore,
+                "min": x.min(),
+                "max": x.max(),
+                "mean": mean,
+                "std": std,
+            }
+        )
 
         # Excluding feature with too frequent modes
-        active = pct_zscore < params.get('thresh_outlier', 1.)
-        
+        active = pct_zscore < params.get("thresh_outlier", 1.0)
+
     return active, association
 
-def iqr_measure(active: bool, association: Dict[str, Any], x: Series, y: Series=None, **params) -> Tuple[bool, Dict[str, Any]]:
-    """ Computes outliers based on the inter-quartile range
+
+def iqr_measure(
+    active: bool,
+    association: Dict[str, Any],
+    x: Series,
+    y: Series = None,
+    **params,
+) -> Tuple[bool, Dict[str, Any]]:
+    """Computes outliers based on the inter-quartile range
 
     Parameters
     ----------
     thresh_outlier, float: default 1.
       Maximum percentage of Outliers in a feature
     """
-    
+
     # check that previous steps where passed for computational optimization
     if active:
-        
         q3 = x.quantile(0.75)  # 3rd quartile
         q1 = x.quantile(0.25)  # 1st quartile
         iqr = q3 - q1  # inter quartile range
         iqr_bounds = q1 - 1.5 * iqr, q3 + 1.5 * iqr  # bounds of the iqr range
-        
+
         # checking for outliers
         outliers = ~x.between(*iqr_bounds)
         pct_iqr = outliers.mean()
-        
+
         # updating association
-        association.update({
-            'pct_iqr': pct_iqr,
-            'q1': q1,
-            'median': x.median(),
-            'q3': q3
-        })
+        association.update({"pct_iqr": pct_iqr, "q1": q1, "median": x.median(), "q3": q3})
 
         # Excluding feature with too frequent modes
-        active = pct_iqr < params.get('thresh_outlier', 1.)
-        
+        active = pct_iqr < params.get("thresh_outlier", 1.0)
+
     return active, association
 
-def chi2_measure(active: bool, association: Dict[str, Any], x: Series,
-                 y: Series, **params) -> Tuple[bool, Dict[str, Any]]:
-    """ Chi2 Measure between two Series of qualitative features"""
-        
+
+def chi2_measure(
+    active: bool, association: Dict[str, Any], x: Series, y: Series, **params
+) -> Tuple[bool, Dict[str, Any]]:
+    """Chi2 Measure between two Series of qualitative features"""
+
     # check that previous steps where passed
     if active:
-    
         # computing crosstab between x and y
         xtab = crosstab(x, y)
 
-        # numnber of observations
-        n_obs = xtab.sum(axis=None)
-
-        # number of values taken by the features
-        n_mod_x, n_mod_y = len(xtab.index), len(xtab.columns)
-
         # Chi2 statistic
         chi2 = chi2_contingency(xtab)[0]
 
         # updating association
-        association.update({'chi2_measure': chi2})
-    
+        association.update({"chi2_measure": chi2})
+
     return active, association
 
-def cramerv_measure(active: bool, association: Dict[str, Any], x: Series,
-                    y: Series, **params) -> Tuple[bool, Dict[str, Any]]:
-    """ Carmer's V between two Series of qualitative features"""
+
+def cramerv_measure(
+    active: bool, association: Dict[str, Any], x: Series, y: Series, **params
+) -> Tuple[bool, Dict[str, Any]]:
+    """Carmer's V between two Series of qualitative features"""
 
     # check that previous steps where passed
     if active:
-    
         # computing chi2
-        if 'chi2_measure' not in association:
+        if "chi2_measure" not in association:
             active, association = chi2_measure(active, association, x, y, **params)
 
         # numnber of observations
         n_obs = (notna(x) & notna(y)).sum()
 
         # number of values taken by the features
         n_mod_x, n_mod_y = x.nunique(), y.nunique()
         min_n_mod = min(n_mod_x, n_mod_y)
-        
+
         # Chi2 statistic
-        chi2 = association.get('chi2_measure')
+        chi2 = association.get("chi2_measure")
 
         # Cramer's V
         cramerv = sqrt(chi2 / n_obs / (min_n_mod - 1))
 
         # updating association
-        association.update({'cramerv_measure': cramerv})
-    
+        association.update({"cramerv_measure": cramerv})
+
     return active, association
 
-def tschuprowt_measure(active: bool, association: Dict[str, Any],x: Series,
-                       y: Series, **params) -> Tuple[bool, Dict[str, Any]]:
-    """ Tschuprow's T between two Series of qualitative features"""
-        
+
+def tschuprowt_measure(
+    active: bool, association: Dict[str, Any], x: Series, y: Series, **params
+) -> Tuple[bool, Dict[str, Any]]:
+    """Tschuprow's T between two Series of qualitative features"""
+
     # check that previous steps where passed
     if active:
-    
         # computing chi2
-        if 'chi2_measure' not in association:
+        if "chi2_measure" not in association:
             active, association = chi2_measure(active, association, x, y, **params)
 
         # numnber of observations
         n_obs = (notna(x) & notna(y)).sum()
 
         # number of values taken by the features
         n_mod_x, n_mod_y = x.nunique(), y.nunique()
-        
+
         # Chi2 statistic
-        chi2 = association.get('chi2_measure')
+        chi2 = association.get("chi2_measure")
 
         # Tschuprow's T
         dof_mods = sqrt((n_mod_x - 1) * (n_mod_y - 1))
         tschuprowt = 0
         if dof_mods > 0:
             tschuprowt = sqrt(chi2 / n_obs / dof_mods)
 
         # updating association
-        association.update({'tschuprowt_measure': tschuprowt})
-    
+        association.update({"tschuprowt_measure": tschuprowt})
+
     return active, association
 
-    
-# FILTERS 
+
+# FILTERS
 def thresh_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
-    """ Filters out missing association measure (did not pass a threshold)"""
-    
+    """Filters out missing association measure (did not pass a threshold)"""
+
     # drops rows with nans
     associations = ranks.dropna(axis=0)
-    
+
     return associations
 
+
 def measure_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
-    """ Filters out specified measure's lower ranks than threshold
+    """Filters out specified measure's lower ranks than threshold
 
     Parameters
     ----------
     thresh_measure, float: default 0.
         Minimum association between target and features
         To be used with: `association_filter`
     name_measure, str
         Measure to be used for minimum association filtering
         To be used with: `association_filter`
     """
-    
+
     associations = ranks.copy()
 
     # drops rows with nans
-    if 'name_measure' in params:
-        associations = ranks[ranks[params.get('name_measure')] > params.get('thresh_measure', 0.)]
-    
+    if "name_measure" in params:
+        associations = ranks[ranks[params.get("name_measure")] > params.get("thresh_measure", 0.0)]
+
     return associations
 
-def quantitative_filter(X: DataFrame, ranks: DataFrame, corr_measure: str, **params) -> Dict[str, Any]:
-    """ Computes max association between X and X (quantitative) excluding features 
-    that are correlated to a feature more associated with the target 
+
+def quantitative_filter(
+    X: DataFrame, ranks: DataFrame, corr_measure: str, **params
+) -> Dict[str, Any]:
+    """Computes max association between X and X (quantitative) excluding features
+    that are correlated to a feature more associated with the target
     (defined by the ranks).
 
     Parameters
     ----------
     thresh_corr, float: default 1.
         Maximum association between features
     """
-    
+
     # accessing the prefered order
     prefered_order = ranks.index
 
     # computing correlation between features
     X_corr = X[prefered_order].corr(corr_measure).abs()
     X_corr = X_corr.where(triu(ones(X_corr.shape), k=1).astype(bool))
-    
+
     # initiating list of maximum association per feature
     associations = []
-    
+
     # iterating over each feature by target association order
     for feature in prefered_order:
-            
         # correlation with features more associated to the target
         corr_with_better_features = X_corr.loc[:feature, feature]
-        
+
         # maximum correlation with a better feature
-        corr_with, worst_corr = corr_with_better_features.agg(['idxmax', 'max'])
-        
+        corr_with, worst_corr = corr_with_better_features.agg(["idxmax", "max"])
+
         # dropping the feature if it was too correlated to a better feature
-        if worst_corr > params.get('thresh_corr', 1):
+        if worst_corr > params.get("thresh_corr", 1):
             X_corr = X_corr.drop(feature, axis=0).drop(feature, axis=1)
-            
+
         # kept feature: updating associations with this feature
         else:
-            associations += [{
-                'feature': feature, 
-                f'{corr_measure}_filter': worst_corr,
-                f'{corr_measure}_with': corr_with
-            }]
-            
+            associations += [
+                {
+                    "feature": feature,
+                    f"{corr_measure}_filter": worst_corr,
+                    f"{corr_measure}_with": corr_with,
+                }
+            ]
+
     # formatting ouput to DataFrame
-    associations = DataFrame(associations).set_index('feature')
-            
+    associations = DataFrame(associations).set_index("feature")
+
     # applying filter on association
-    associations = ranks.join(associations, how='right')
-    
-    return associations 
+    associations = ranks.join(associations, how="right")
+
+    return associations
 
 
 def spearman_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
-    """ Computes max Spearman between X and X (quantitative) excluding features 
-    that are correlated to a feature more associated with the target 
+    """Computes max Spearman between X and X (quantitative) excluding features
+    that are correlated to a feature more associated with the target
     (defined by the ranks).
 
     Parameters
     ----------
     thresh_corr, float: default 1.
       Maximum association between features
     """
-            
+
     # applying quantitative filter with spearman correlation
-    return quantitative_filter(X, ranks, 'spearman', **params)
+    return quantitative_filter(X, ranks, "spearman", **params)
+
 
 def pearson_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
-    """ Computes max Pearson between X and X (quantitative) excluding features 
-    that are correlated to a feature more associated with the target 
+    """Computes max Pearson between X and X (quantitative) excluding features
+    that are correlated to a feature more associated with the target
     (defined by the ranks).
 
     Parameters
     ----------
     thresh_corr, float: default 1.
       Maximum association between features
     """
-            
+
     # applying quantitative filter with spearman correlation
-    return quantitative_filter(X, ranks, 'pearson', **params)
+    return quantitative_filter(X, ranks, "pearson", **params)
+
 
 def vif_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
-    """ Computes Variance Inflation Factor (multicolinearity)
+    """Computes Variance Inflation Factor (multicolinearity)
 
     Parameters
     ----------
     thresh_vif, float: default inf
       Maximum VIF between features
     """
-    
+
     # accessing the prefered order
     prefered_order = ranks.index
-    
+
     # initiating list association per feature
     associations = []
-    
+
     # list of dropped features
     dropped = []
-    
+
     # iterating over each column
     for i, feature in enumerate(prefered_order):
-        
         # identifying remaining more associated features
-        better_features = [f for f in prefered_order[:i+1] if f not in dropped]
-        
+        better_features = [f for f in prefered_order[: i + 1] if f not in dropped]
+
         X_vif = X[better_features]  # keeping only better features
         X_vif = X_vif.dropna(axis=0)  # dropping NaNs for OLS
-        
+
         # computation of VIF
         vif = nan
         if len(better_features) > 1 and len(X_vif) > 0:
-            vif = variance_inflation_factor(X_vif.values, len(better_features)-1)
-        
+            vif = variance_inflation_factor(X_vif.values, len(better_features) - 1)
+
         # dropping the feature if it was too correlated to a better feature
-        if vif > params.get('thresh_vif', inf) and notna(vif):
+        if vif > params.get("thresh_vif", inf) and notna(vif):
             dropped += [feature]
-            
+
         # kept feature: updating associations with this feature
         else:
-            associations += [{'feature': feature, 'vif_filter': vif}]
-    
+            associations += [{"feature": feature, "vif_filter": vif}]
+
     # formatting ouput to DataFrame
-    associations = DataFrame(associations).set_index('feature')
-            
+    associations = DataFrame(associations).set_index("feature")
+
     # applying filter on association
-    associations = ranks.join(associations, how='right')
-    
+    associations = ranks.join(associations, how="right")
+
     return associations
 
-def qualitative_worst_corr(X: DataFrame, feature: str, ranks: DataFrame, corr_measure: Callable, **params):
-    """ Computes maximum association between a feature and features 
+
+def qualitative_worst_corr(
+    X: DataFrame,
+    feature: str,
+    ranks: DataFrame,
+    corr_measure: Callable,
+    **params,
+):
+    """Computes maximum association between a feature and features
     more associated to the target (according to ranks)
     """
-    
+
     # measure name
     measure_name = corr_measure.__name__
-    measure = measure_name.replace('_measure', '')
-        
+    measure = measure_name.replace("_measure", "")
+
     # initiating worst correlation
-    worst_corr = {'feature': feature}
-    
+    worst_corr = {"feature": feature}
+
     # features more associated with target
     better_features = list(ranks.loc[:feature].index)[:-1]
 
     # iterating over each better feature
     for better_feature in better_features:
-
         # computing association with better feature
-        _, association = corr_measure(True, {f'{measure}_with': better_feature}, 
-                                      X[feature], X[better_feature], **params)
-
+        _, association = corr_measure(
+            True,
+            {f"{measure}_with": better_feature},
+            X[feature],
+            X[better_feature],
+            **params,
+        )
 
         # updating association if it's greater than previous better features
         if association.get(measure_name) > worst_corr.get(measure_name, 0):
-
             # renaming association measure as filter
-            association[f'{measure}_filter'] = association.pop(measure_name)
-            
+            association[f"{measure}_filter"] = association.pop(measure_name)
+
             # removing temporary measures
-            association = {k: v for k, v in association.items() if '_measure' not in k}
+            association = {k: v for k, v in association.items() if "_measure" not in k}
 
             # updating worst known association
             worst_corr.update(association)
 
         # stopping measurements if association is greater than threshold
-        if association.get(f'{measure}_filter') > params.get('thresh_corr', 1):
+        if association.get(f"{measure}_filter") > params.get("thresh_corr", 1):
             ranks = ranks.drop(feature, axis=0)  # removing feature from ranks
-            
+
             return ranks, None
-    
+
     return ranks, worst_corr
 
-def qualitative_filter(X: DataFrame, ranks: DataFrame, corr_measure: Callable, **params) -> Dict[str, Any]:
-    """ Computes max association between X and X (qualitative) excluding features 
-    that are correlated to a feature more associated with the target 
+
+def qualitative_filter(
+    X: DataFrame, ranks: DataFrame, corr_measure: Callable, **params
+) -> Dict[str, Any]:
+    """Computes max association between X and X (qualitative) excluding features
+    that are correlated to a feature more associated with the target
     (defined by the ranks).
 
     Parameters
     ----------
     thresh_corr, float: default 1.
         Maximum association between features
     """
-    
+
     # accessing the prefered order
     prefered_order = ranks.index
 
     # initiating list of maximum association per feature
     associations = []
-    
+
     # iterating over each feature by target association order
     for feature in prefered_order:
-        
-        
         # computing correlation with better features anf filtering out ranks
         ranks, worst_corr = qualitative_worst_corr(X, feature, ranks, corr_measure, **params)
-        
+
         # updating associations
         if worst_corr:
             associations += [worst_corr]
 
     # formatting ouput to DataFrame
-    associations = DataFrame(associations).set_index('feature')
-            
+    associations = DataFrame(associations).set_index("feature")
+
     # applying filter on association
-    associations = ranks.join(associations, how='right')
-    
-    return associations 
+    associations = ranks.join(associations, how="right")
+
+    return associations
+
 
 def cramerv_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
-    """ Computes max Cramer's V between X and X (qualitative) excluding features 
-    that are correlated to a feature more associated with the target 
+    """Computes max Cramer's V between X and X (qualitative) excluding features
+    that are correlated to a feature more associated with the target
     (defined by the ranks).
 
     Parameters
     ----------
     thresh_corr, float: default 1.
         Maximum association between features
     """
-            
-    # applying quantitative filter with Cramer's V correlation    
+
+    # applying quantitative filter with Cramer's V correlation
     return qualitative_filter(X, ranks, cramerv_measure, **params)
 
+
 def tschuprowt_filter(X: DataFrame, ranks: DataFrame, **params) -> Dict[str, Any]:
-    """ Computes max Tschuprow's T between X and X (qualitative) excluding features 
-    that are correlated to a feature more associated with the target 
+    """Computes max Tschuprow's T between X and X (qualitative) excluding
+     features that are correlated to a feature more associated with the target
     (defined by the ranks).
 
     Parameters
     ----------
     thresh_corr, float: default 1.
         Maximum association between features
     """
-            
+
     # applying quantitative filter with Tschuprow's T correlation
     return qualitative_filter(X, ranks, tschuprowt_measure, **params)
```

### Comparing `AutoCarver-4.4.1/AutoCarver.egg-info/PKG-INFO` & `AutoCarver-5.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,8 @@
-Metadata-Version: 2.1
-Name: AutoCarver
-Version: 4.4.1
-Summary: Automatic Bucketizing of Features with Optimal Association
-Home-page: https://github.com/mdefrance/AutoCarver
-Author: Mario DEFRANCE
-Author-email: defrancemario@gmail.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: Unix
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-\n</p>
+</p>
 <p align="center">
     <img alt="PyPI" src="https://img.shields.io/pypi/v/autocarver?style=flat-square">
     <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/autocarver?style=flat-square">
     <img alt="GitHub" src="https://img.shields.io/github/license/mdefrance/autocarver?style=flat-square">
 </p>
 
 This is a work in progress.
@@ -43,46 +21,40 @@
 <pre>
 pip install autocarver
 </pre>
 
 
 ## Quick-Start Examples
 
-### Setting up Samples
+### Setting up Samples, initiating Pipeline
 
 `AutoCarver` is able to test the robustness of buckets on a dev sample `X_dev`.
 
+One of the great advantages of the `AutoCarver` package is its seamless integration with scikit-learn pipelines, making it incredibly convenient for production-level implementations. By leveraging scikit-learn's pipeline functionality, `AutoCarver` can be effortlessly incorporated into the end-to-end machine learning workflow.
+
 ```python
 # defining training and testing sets
 X_train, y_train = ...  # used to fit the AutoCarver and the model
 X_dev, y_dev = ...  # used to validate the AutoCarver's buckets and optimize the model's parameters/hyperparameters
 X_test, y_test = ...  # used to evaluate the final model's performances
-```
-
-### Initiating Pipeline
 
-One of the great advantages of the `AutoCarver` package is its seamless integration with scikit-learn pipelines, making it incredibly convenient for production-level implementations. By leveraging scikit-learn's pipeline functionality, `AutoCarver` can be effortlessly incorporated into the end-to-end machine learning workflow.
-
-```python
-from sklearn.pipeline import Pipeline
-
-pipe = Pipeline()
+pipe = []  # initiating as an empty list that will be filled along the feature engineering
 ```
 
 ### Quickly build basic buckets with Discretizer
 
 The `AutoCarver.Discretizers` is a user-friendly tool that enables the discretization of various types of data into basic buckets. With this package, users can easily transform qualitative, qualitative ordinal, and quantitative data into discrete categories for further analysis and modeling.
 
 **TODO: add info from `QuantitativeDiscretizer` and `QuantitativeDiscretizer`**
 **TODO: add stringconverter**
 `Discretizer` is the combination of `QuantitativeDiscretizer` and `QuantitativeDiscretizer`.
 
 Following parameters must be set for `Discretizer`:
-- `quantitative_features`, list of column names of quantitative data to discretize
-- `quantitative_features`, list of column names of qualitative and qualitative ordinal data to discretize
+- `quanti_features`, list of column names of quantitative data to discretize
+- `quanli_features`, list of column names of qualitative and qualitative ordinal data to discretize
 - `min_freq`, should be set from 0.01 (preciser, decreased stability) to 0.05 (faster, increased stability).
   - *For qualitative data:*  Minimal frequency of a modality, less frequent modalities are grouped in the `default_value='__OTHER__'` modality. Values are ordered based on `y_train` bucket mean.
   - *For qualitative ordinal data:* Less frequent modalities are grouped to the closest modality  (smallest frequency or closest target rate), between the superior and inferior values (specified in the `values_orders` dictionnary).
   - *For quantitative data:* Equivalent to the inverse of `QuantitativeDiscretizer`'s `q` parameter. Number of quantiles to initialy cut the feature in. Values more frequent than `min_freq` will be set as their own group and remaining frequency will be cut into proportionaly less quantiles (`1/min_freq:=max(round(non_frequent * 1/min_freq), 1)`). 
 - `values_orders`, dict of qualitative ordinal features matched to the order of their modalities
   - *For qualitative ordinal data:* `dict` of features values and `GroupedList` of their values. Modalities less frequent than `min_freq` are automaticaly grouped to the closest modality (smallest frequency or closest target rate), between the superior and inferior values.
 
@@ -95,23 +67,23 @@
 # specifying orders of qualitative ordinal features
 values_orders = {
     'age': ['0-18', '18-30', '30-50', '50+'],
     'grade': ['A', 'B', 'C', 'D', 'J', 'K', 'NN']
 }
 
 # pre-processing of features into categorical ordinal features
-discretizer = Discretizer(quantitative_features=quanti_features, qualitative_features=quali_features, min_freq=0.02, values_orders=values_orders)
+discretizer = Discretizer(quanti_features=quanti_features, quali_features=quali_features, min_freq=0.02, values_orders=values_orders)
 discretizer.fit_transform(X_train, y_train)
 discretizer.transform(X_dev)
 
 # storing built buckets
 values_orders.update(discretizer.values_orders)
 
 # append the discretizer to the feature engineering pipeline
-pipe.steps.append(['Discretizer', discretizer])
+pipe += [('Discretizer', discretizer)]
 ```
 
 
 Overall, the Discretizers package provides a straightforward and efficient solution for discretizing qualitative, qualitative ordinal, and quantitative data into simple buckets. By transforming data into discrete categories, it enables researchers, analysts, and data scientists to gain insights, perform statistical analyses, and build models on discretized data.
 
 For more details and further functionnalities look into AutoCarver.Discretizers README.
 
@@ -136,19 +108,19 @@
 ```python
 from AutoCarver.AutoCarver import AutoCarver
 
 # intiating AutoCarver
 auto_carver = AutoCarver(values_orders=values_orders, sort_by='cramerv', max_n_mod=5, verbose=True)
 
 # fitting on training sample, a test sample can be specified to evaluate carving robustness
-auto_carver.fit_transform(X_train, y_train, X_dev, y_dev)
+auto_carver.fit_transform(X_train, y_train, X_test=X_dev, y_test=y_dev)
 auto_carver.transform(X_dev)
 
 # append the auto_carver to the feature engineering pipeline
-pipe.steps.append(['AutoCarver', auto_carver])
+pipe += [('AutoCarver', auto_carver)]
 ```
 <p align="left">
   <img width="500" src="/docs/auto_carver_fit.PNG" />
 </p>
 
 
 ### Cherry picking the most target-associated features with FeatureSelector
@@ -190,32 +162,28 @@
     name_measure='cramerv_measure', thresh_measure=0.06,  # filters out features with cramerv_measure lower than 0.06
     verbose=True  # displays statistics
 )
 X_train = quali_selector.fit_transform(X_train, y_train)
 X_dev = quali_selector.transform(X_dev)
 
 # append the selector to the feature engineering pipeline
-pipe.steps.append(['QualiFeatureSelector', quali_selector])
+pipe += [('QualiFeatureSelector', quali_selector)]
 ```
 
 
 
 ### Storing, reusing the AutoCarver
 
 The `Discretizer` and `AutoCarver` steps can be stored in a `Pipeline` and can than be stored as a `pickle` file.
 
 ```python
 from pickle import dump
 from sklearn.pipeline import Pipeline
 
-# storing Discretizer
-pipe = [('Discretizer', discretizer)]
-
-# storing fitted AutoCarver in a Pipeline
-pipe += [('AutoCarver', auto_carver)]
+# storing fitted Discretizer, AutoCarver and FeatureSelector in a Pipeline
 pipe = Pipeline(pipe)
 
 # storing as pickle file
 dump(pipe, open('my_pipe.pkl', 'wb'))
 ```
 
 The stored `Pipeline`, can then be used to transform new datasets.
@@ -362,11 +330,34 @@
     verbose=True  # displays statistics
 )
 X_train = quanti_selector.fit_transform(X_train, y_train)
 X_dev = quanti_selector.transform(X_dev)
 
 # append the selector to the feature engineering pipeline
 pipe.steps.append(['QuantiFeatureSelector', quanti_selector])
+pipe += [('QuantiFeatureSelector', quanti_selector)]
 ```
 
 
 **FeatureSelector TODO: add how to build on measures and filters**
+
+
+### Converters Examples
+#### CrossConverter
+
+             
+```python
+from AutoCarver.Converters import CrossConverter
+
+# qualitative and quantitative features should be discretized (and bucketized with AutoCarver)
+to_cross = quali_features + quanti_features
+
+cross_converter = CrossConverter(to_cross)
+X_train = cross_converter.fit_transform(X_train, y_train)
+X_dev = cross_converter.transform(X_dev)
+
+# append the crosser to the feature engineering pipeline
+pipe += [('CrossConverter', cross_converter)]
+
+quali_features_built = crosser.new_features  # adding to qualitative_features_built for no further feature engineering
+print(f"Qualitative features built: total {len(quali_features_built)}")
+```
```

### Comparing `AutoCarver-4.4.1/LICENSE` & `AutoCarver-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoCarver-4.4.1/PKG-INFO` & `AutoCarver-5.0.0/AutoCarver.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 4.4.1
+Version: 5.0.0
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -43,46 +41,40 @@
 <pre>
 pip install autocarver
 </pre>
 
 
 ## Quick-Start Examples
 
-### Setting up Samples
+### Setting up Samples, initiating Pipeline
 
 `AutoCarver` is able to test the robustness of buckets on a dev sample `X_dev`.
 
+One of the great advantages of the `AutoCarver` package is its seamless integration with scikit-learn pipelines, making it incredibly convenient for production-level implementations. By leveraging scikit-learn's pipeline functionality, `AutoCarver` can be effortlessly incorporated into the end-to-end machine learning workflow.
+
 ```python
 # defining training and testing sets
 X_train, y_train = ...  # used to fit the AutoCarver and the model
 X_dev, y_dev = ...  # used to validate the AutoCarver's buckets and optimize the model's parameters/hyperparameters
 X_test, y_test = ...  # used to evaluate the final model's performances
-```
-
-### Initiating Pipeline
-
-One of the great advantages of the `AutoCarver` package is its seamless integration with scikit-learn pipelines, making it incredibly convenient for production-level implementations. By leveraging scikit-learn's pipeline functionality, `AutoCarver` can be effortlessly incorporated into the end-to-end machine learning workflow.
 
-```python
-from sklearn.pipeline import Pipeline
-
-pipe = Pipeline()
+pipe = []  # initiating as an empty list that will be filled along the feature engineering
 ```
 
 ### Quickly build basic buckets with Discretizer
 
 The `AutoCarver.Discretizers` is a user-friendly tool that enables the discretization of various types of data into basic buckets. With this package, users can easily transform qualitative, qualitative ordinal, and quantitative data into discrete categories for further analysis and modeling.
 
 **TODO: add info from `QuantitativeDiscretizer` and `QuantitativeDiscretizer`**
 **TODO: add stringconverter**
 `Discretizer` is the combination of `QuantitativeDiscretizer` and `QuantitativeDiscretizer`.
 
 Following parameters must be set for `Discretizer`:
-- `quantitative_features`, list of column names of quantitative data to discretize
-- `quantitative_features`, list of column names of qualitative and qualitative ordinal data to discretize
+- `quanti_features`, list of column names of quantitative data to discretize
+- `quanli_features`, list of column names of qualitative and qualitative ordinal data to discretize
 - `min_freq`, should be set from 0.01 (preciser, decreased stability) to 0.05 (faster, increased stability).
   - *For qualitative data:*  Minimal frequency of a modality, less frequent modalities are grouped in the `default_value='__OTHER__'` modality. Values are ordered based on `y_train` bucket mean.
   - *For qualitative ordinal data:* Less frequent modalities are grouped to the closest modality  (smallest frequency or closest target rate), between the superior and inferior values (specified in the `values_orders` dictionnary).
   - *For quantitative data:* Equivalent to the inverse of `QuantitativeDiscretizer`'s `q` parameter. Number of quantiles to initialy cut the feature in. Values more frequent than `min_freq` will be set as their own group and remaining frequency will be cut into proportionaly less quantiles (`1/min_freq:=max(round(non_frequent * 1/min_freq), 1)`). 
 - `values_orders`, dict of qualitative ordinal features matched to the order of their modalities
   - *For qualitative ordinal data:* `dict` of features values and `GroupedList` of their values. Modalities less frequent than `min_freq` are automaticaly grouped to the closest modality (smallest frequency or closest target rate), between the superior and inferior values.
 
@@ -95,23 +87,23 @@
 # specifying orders of qualitative ordinal features
 values_orders = {
     'age': ['0-18', '18-30', '30-50', '50+'],
     'grade': ['A', 'B', 'C', 'D', 'J', 'K', 'NN']
 }
 
 # pre-processing of features into categorical ordinal features
-discretizer = Discretizer(quantitative_features=quanti_features, qualitative_features=quali_features, min_freq=0.02, values_orders=values_orders)
+discretizer = Discretizer(quanti_features=quanti_features, quali_features=quali_features, min_freq=0.02, values_orders=values_orders)
 discretizer.fit_transform(X_train, y_train)
 discretizer.transform(X_dev)
 
 # storing built buckets
 values_orders.update(discretizer.values_orders)
 
 # append the discretizer to the feature engineering pipeline
-pipe.steps.append(['Discretizer', discretizer])
+pipe += [('Discretizer', discretizer)]
 ```
 
 
 Overall, the Discretizers package provides a straightforward and efficient solution for discretizing qualitative, qualitative ordinal, and quantitative data into simple buckets. By transforming data into discrete categories, it enables researchers, analysts, and data scientists to gain insights, perform statistical analyses, and build models on discretized data.
 
 For more details and further functionnalities look into AutoCarver.Discretizers README.
 
@@ -136,19 +128,19 @@
 ```python
 from AutoCarver.AutoCarver import AutoCarver
 
 # intiating AutoCarver
 auto_carver = AutoCarver(values_orders=values_orders, sort_by='cramerv', max_n_mod=5, verbose=True)
 
 # fitting on training sample, a test sample can be specified to evaluate carving robustness
-auto_carver.fit_transform(X_train, y_train, X_dev, y_dev)
+auto_carver.fit_transform(X_train, y_train, X_test=X_dev, y_test=y_dev)
 auto_carver.transform(X_dev)
 
 # append the auto_carver to the feature engineering pipeline
-pipe.steps.append(['AutoCarver', auto_carver])
+pipe += [('AutoCarver', auto_carver)]
 ```
 <p align="left">
   <img width="500" src="/docs/auto_carver_fit.PNG" />
 </p>
 
 
 ### Cherry picking the most target-associated features with FeatureSelector
@@ -190,32 +182,28 @@
     name_measure='cramerv_measure', thresh_measure=0.06,  # filters out features with cramerv_measure lower than 0.06
     verbose=True  # displays statistics
 )
 X_train = quali_selector.fit_transform(X_train, y_train)
 X_dev = quali_selector.transform(X_dev)
 
 # append the selector to the feature engineering pipeline
-pipe.steps.append(['QualiFeatureSelector', quali_selector])
+pipe += [('QualiFeatureSelector', quali_selector)]
 ```
 
 
 
 ### Storing, reusing the AutoCarver
 
 The `Discretizer` and `AutoCarver` steps can be stored in a `Pipeline` and can than be stored as a `pickle` file.
 
 ```python
 from pickle import dump
 from sklearn.pipeline import Pipeline
 
-# storing Discretizer
-pipe = [('Discretizer', discretizer)]
-
-# storing fitted AutoCarver in a Pipeline
-pipe += [('AutoCarver', auto_carver)]
+# storing fitted Discretizer, AutoCarver and FeatureSelector in a Pipeline
 pipe = Pipeline(pipe)
 
 # storing as pickle file
 dump(pipe, open('my_pipe.pkl', 'wb'))
 ```
 
 The stored `Pipeline`, can then be used to transform new datasets.
@@ -362,11 +350,34 @@
     verbose=True  # displays statistics
 )
 X_train = quanti_selector.fit_transform(X_train, y_train)
 X_dev = quanti_selector.transform(X_dev)
 
 # append the selector to the feature engineering pipeline
 pipe.steps.append(['QuantiFeatureSelector', quanti_selector])
+pipe += [('QuantiFeatureSelector', quanti_selector)]
 ```
 
 
 **FeatureSelector TODO: add how to build on measures and filters**
+
+
+### Converters Examples
+#### CrossConverter
+
+             
+```python
+from AutoCarver.Converters import CrossConverter
+
+# qualitative and quantitative features should be discretized (and bucketized with AutoCarver)
+to_cross = quali_features + quanti_features
+
+cross_converter = CrossConverter(to_cross)
+X_train = cross_converter.fit_transform(X_train, y_train)
+X_dev = cross_converter.transform(X_dev)
+
+# append the crosser to the feature engineering pipeline
+pipe += [('CrossConverter', cross_converter)]
+
+quali_features_built = crosser.new_features  # adding to qualitative_features_built for no further feature engineering
+print(f"Qualitative features built: total {len(quali_features_built)}")
+```
```

### Comparing `AutoCarver-4.4.1/README.md` & `AutoCarver-5.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,28 @@
-</p>
+Metadata-Version: 2.1
+Name: AutoCarver
+Version: 5.0.0
+Summary: Automatic Bucketizing of Features with Optimal Association
+Home-page: https://github.com/mdefrance/AutoCarver
+Author: Mario DEFRANCE
+Author-email: defrancemario@gmail.com
+License: MIT
+Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: Unix
+Classifier: Operating System :: Microsoft :: Windows
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+\n</p>
 <p align="center">
     <img alt="PyPI" src="https://img.shields.io/pypi/v/autocarver?style=flat-square">
     <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/autocarver?style=flat-square">
     <img alt="GitHub" src="https://img.shields.io/github/license/mdefrance/autocarver?style=flat-square">
 </p>
 
 This is a work in progress.
@@ -21,46 +41,40 @@
 <pre>
 pip install autocarver
 </pre>
 
 
 ## Quick-Start Examples
 
-### Setting up Samples
+### Setting up Samples, initiating Pipeline
 
 `AutoCarver` is able to test the robustness of buckets on a dev sample `X_dev`.
 
+One of the great advantages of the `AutoCarver` package is its seamless integration with scikit-learn pipelines, making it incredibly convenient for production-level implementations. By leveraging scikit-learn's pipeline functionality, `AutoCarver` can be effortlessly incorporated into the end-to-end machine learning workflow.
+
 ```python
 # defining training and testing sets
 X_train, y_train = ...  # used to fit the AutoCarver and the model
 X_dev, y_dev = ...  # used to validate the AutoCarver's buckets and optimize the model's parameters/hyperparameters
 X_test, y_test = ...  # used to evaluate the final model's performances
-```
-
-### Initiating Pipeline
 
-One of the great advantages of the `AutoCarver` package is its seamless integration with scikit-learn pipelines, making it incredibly convenient for production-level implementations. By leveraging scikit-learn's pipeline functionality, `AutoCarver` can be effortlessly incorporated into the end-to-end machine learning workflow.
-
-```python
-from sklearn.pipeline import Pipeline
-
-pipe = Pipeline()
+pipe = []  # initiating as an empty list that will be filled along the feature engineering
 ```
 
 ### Quickly build basic buckets with Discretizer
 
 The `AutoCarver.Discretizers` is a user-friendly tool that enables the discretization of various types of data into basic buckets. With this package, users can easily transform qualitative, qualitative ordinal, and quantitative data into discrete categories for further analysis and modeling.
 
 **TODO: add info from `QuantitativeDiscretizer` and `QuantitativeDiscretizer`**
 **TODO: add stringconverter**
 `Discretizer` is the combination of `QuantitativeDiscretizer` and `QuantitativeDiscretizer`.
 
 Following parameters must be set for `Discretizer`:
-- `quantitative_features`, list of column names of quantitative data to discretize
-- `quantitative_features`, list of column names of qualitative and qualitative ordinal data to discretize
+- `quanti_features`, list of column names of quantitative data to discretize
+- `quanli_features`, list of column names of qualitative and qualitative ordinal data to discretize
 - `min_freq`, should be set from 0.01 (preciser, decreased stability) to 0.05 (faster, increased stability).
   - *For qualitative data:*  Minimal frequency of a modality, less frequent modalities are grouped in the `default_value='__OTHER__'` modality. Values are ordered based on `y_train` bucket mean.
   - *For qualitative ordinal data:* Less frequent modalities are grouped to the closest modality  (smallest frequency or closest target rate), between the superior and inferior values (specified in the `values_orders` dictionnary).
   - *For quantitative data:* Equivalent to the inverse of `QuantitativeDiscretizer`'s `q` parameter. Number of quantiles to initialy cut the feature in. Values more frequent than `min_freq` will be set as their own group and remaining frequency will be cut into proportionaly less quantiles (`1/min_freq:=max(round(non_frequent * 1/min_freq), 1)`). 
 - `values_orders`, dict of qualitative ordinal features matched to the order of their modalities
   - *For qualitative ordinal data:* `dict` of features values and `GroupedList` of their values. Modalities less frequent than `min_freq` are automaticaly grouped to the closest modality (smallest frequency or closest target rate), between the superior and inferior values.
 
@@ -73,23 +87,23 @@
 # specifying orders of qualitative ordinal features
 values_orders = {
     'age': ['0-18', '18-30', '30-50', '50+'],
     'grade': ['A', 'B', 'C', 'D', 'J', 'K', 'NN']
 }
 
 # pre-processing of features into categorical ordinal features
-discretizer = Discretizer(quantitative_features=quanti_features, qualitative_features=quali_features, min_freq=0.02, values_orders=values_orders)
+discretizer = Discretizer(quanti_features=quanti_features, quali_features=quali_features, min_freq=0.02, values_orders=values_orders)
 discretizer.fit_transform(X_train, y_train)
 discretizer.transform(X_dev)
 
 # storing built buckets
 values_orders.update(discretizer.values_orders)
 
 # append the discretizer to the feature engineering pipeline
-pipe.steps.append(['Discretizer', discretizer])
+pipe += [('Discretizer', discretizer)]
 ```
 
 
 Overall, the Discretizers package provides a straightforward and efficient solution for discretizing qualitative, qualitative ordinal, and quantitative data into simple buckets. By transforming data into discrete categories, it enables researchers, analysts, and data scientists to gain insights, perform statistical analyses, and build models on discretized data.
 
 For more details and further functionnalities look into AutoCarver.Discretizers README.
 
@@ -114,19 +128,19 @@
 ```python
 from AutoCarver.AutoCarver import AutoCarver
 
 # intiating AutoCarver
 auto_carver = AutoCarver(values_orders=values_orders, sort_by='cramerv', max_n_mod=5, verbose=True)
 
 # fitting on training sample, a test sample can be specified to evaluate carving robustness
-auto_carver.fit_transform(X_train, y_train, X_dev, y_dev)
+auto_carver.fit_transform(X_train, y_train, X_test=X_dev, y_test=y_dev)
 auto_carver.transform(X_dev)
 
 # append the auto_carver to the feature engineering pipeline
-pipe.steps.append(['AutoCarver', auto_carver])
+pipe += [('AutoCarver', auto_carver)]
 ```
 <p align="left">
   <img width="500" src="/docs/auto_carver_fit.PNG" />
 </p>
 
 
 ### Cherry picking the most target-associated features with FeatureSelector
@@ -168,32 +182,28 @@
     name_measure='cramerv_measure', thresh_measure=0.06,  # filters out features with cramerv_measure lower than 0.06
     verbose=True  # displays statistics
 )
 X_train = quali_selector.fit_transform(X_train, y_train)
 X_dev = quali_selector.transform(X_dev)
 
 # append the selector to the feature engineering pipeline
-pipe.steps.append(['QualiFeatureSelector', quali_selector])
+pipe += [('QualiFeatureSelector', quali_selector)]
 ```
 
 
 
 ### Storing, reusing the AutoCarver
 
 The `Discretizer` and `AutoCarver` steps can be stored in a `Pipeline` and can than be stored as a `pickle` file.
 
 ```python
 from pickle import dump
 from sklearn.pipeline import Pipeline
 
-# storing Discretizer
-pipe = [('Discretizer', discretizer)]
-
-# storing fitted AutoCarver in a Pipeline
-pipe += [('AutoCarver', auto_carver)]
+# storing fitted Discretizer, AutoCarver and FeatureSelector in a Pipeline
 pipe = Pipeline(pipe)
 
 # storing as pickle file
 dump(pipe, open('my_pipe.pkl', 'wb'))
 ```
 
 The stored `Pipeline`, can then be used to transform new datasets.
@@ -340,11 +350,34 @@
     verbose=True  # displays statistics
 )
 X_train = quanti_selector.fit_transform(X_train, y_train)
 X_dev = quanti_selector.transform(X_dev)
 
 # append the selector to the feature engineering pipeline
 pipe.steps.append(['QuantiFeatureSelector', quanti_selector])
+pipe += [('QuantiFeatureSelector', quanti_selector)]
 ```
 
 
 **FeatureSelector TODO: add how to build on measures and filters**
+
+
+### Converters Examples
+#### CrossConverter
+
+             
+```python
+from AutoCarver.Converters import CrossConverter
+
+# qualitative and quantitative features should be discretized (and bucketized with AutoCarver)
+to_cross = quali_features + quanti_features
+
+cross_converter = CrossConverter(to_cross)
+X_train = cross_converter.fit_transform(X_train, y_train)
+X_dev = cross_converter.transform(X_dev)
+
+# append the crosser to the feature engineering pipeline
+pipe += [('CrossConverter', cross_converter)]
+
+quali_features_built = crosser.new_features  # adding to qualitative_features_built for no further feature engineering
+print(f"Qualitative features built: total {len(quali_features_built)}")
+```
```

### Comparing `AutoCarver-4.4.1/setup.py` & `AutoCarver-5.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from codecs import open
 from os import path
-from setuptools import setup
+
+from setuptools import setup,find_packages
 
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
-    name='AutoCarver',
-    version='4.4.1',
-    author='Mario DEFRANCE',
-    author_email='defrancemario@gmail.com',
-    description='Automatic Bucketizing of Features with Optimal Association',
+    name="AutoCarver",
+    version="5.0.0",
+    author="Mario DEFRANCE",
+    author_email="defrancemario@gmail.com",
+    description="Automatic Bucketizing of Features with Optimal Association",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url='https://github.com/mdefrance/AutoCarver',
+    url="https://github.com/mdefrance/AutoCarver",
     project_urls={
         "Bug Tracker": "https://github.com/mdefrance/AutoCarver/issues"
     },
-    license='MIT',
-    packages=['AutoCarver'],
+    license="MIT",
+    # install_requires= # TODO,
+    packages=find_packages(),
     classifiers=[
         # ou 4 - Beta ou 5 - Production/Stable
-        'Development Status :: 4 - Beta',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
+        "Development Status :: 4 - Beta",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Operating System :: Unix",
         # "Operating System :: MacOS :: MacOS X",
-        "Operating System :: Microsoft :: Windows"
+        "Operating System :: Microsoft :: Windows",
     ],
-    python_requires='>=3.7'
+    python_requires=">=3.7",
 )
```

