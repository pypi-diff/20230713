# Comparing `tmp/data_understand-0.0.2.tar.gz` & `tmp/data_understand-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_understand-0.0.2.tar", last modified: Wed Jul  5 23:40:25 2023, max compression
+gzip compressed data, was "data_understand-0.0.3.tar", last modified: Thu Jul 13 18:20:22 2023, max compression
```

## Comparing `data_understand-0.0.2.tar` & `data_understand-0.0.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:40:25.699728 data_understand-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-05 23:39:29.000000 data_understand-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-05 23:40:25.699728 data_understand-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-07-05 23:39:29.000000 data_understand-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:40:25.695728 data_understand-0.0.2/data_understand/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:40:25.695728 data_understand-0.0.2/data_understand/class_imbalance/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/class_imbalance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/class_imbalance/imbalance.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:40:25.695728 data_understand-0.0.2/data_understand/dataset_characteristics/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/dataset_characteristics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/dataset_characteristics/characteristics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:40:25.699728 data_understand-0.0.2/data_understand/dataset_statistics/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/dataset_statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/dataset_statistics/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:40:25.699728 data_understand-0.0.2/data_understand/feature_correlation/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/feature_correlation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/feature_correlation/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/input_validations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/jupyter_notebook_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:40:25.699728 data_understand-0.0.2/data_understand/load_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/load_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/load_dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)    14712 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/pdf_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:40:25.699728 data_understand-0.0.2/data_understand/target_characteristics/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/target_characteristics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/target_characteristics/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:40:25.699728 data_understand-0.0.2/data_understand/value_distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/value_distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/value_distributions/box_plot_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/value_distributions/cat_frequency_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/value_distributions/distribution_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/value_distributions/histogram_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-05 23:39:29.000000 data_understand-0.0.2/data_understand/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:40:25.695728 data_understand-0.0.2/data_understand.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-05 23:40:25.000000 data_understand-0.0.2/data_understand.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-05 23:40:25.000000 data_understand-0.0.2/data_understand.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 23:40:25.000000 data_understand-0.0.2/data_understand.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-05 23:40:25.000000 data_understand-0.0.2/data_understand.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-05 23:40:25.000000 data_understand-0.0.2/data_understand.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-05 23:40:25.000000 data_understand-0.0.2/data_understand.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-05 23:39:29.000000 data_understand-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 23:40:25.699728 data_understand-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-05 23:39:29.000000 data_understand-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:20:22.908021 data_understand-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-13 18:19:28.000000 data_understand-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-13 18:20:22.908021 data_understand-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-07-13 18:19:28.000000 data_understand-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:20:22.904021 data_understand-0.0.3/data_understand/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-13 18:19:28.000000 data_understand-0.0.3/data_understand/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:20:22.904021 data_understand-0.0.3/data_understand/class_imbalance/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-13 18:19:28.000000 data_understand-0.0.3/data_understand/class_imbalance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-13 18:19:28.000000 data_understand-0.0.3/data_understand/class_imbalance/imbalance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-13 18:19:28.000000 data_understand-0.0.3/data_understand/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:20:22.904021 data_understand-0.0.3/data_understand/dataset_characteristics/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-13 18:19:28.000000 data_understand-0.0.3/data_understand/dataset_characteristics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-13 18:19:28.000000 data_understand-0.0.3/data_understand/dataset_characteristics/characteristics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:20:22.904021 data_understand-0.0.3/data_understand/dataset_statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-13 18:19:28.000000 data_understand-0.0.3/data_understand/dataset_statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-13 18:19:28.000000 data_understand-0.0.3/data_understand/dataset_statistics/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:20:22.904021 data_understand-0.0.3/data_understand/feature_correlation/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-13 18:19:28.000000 data_understand-0.0.3/data_understand/feature_correlation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-07-13 18:19:28.000000 data_understand-0.0.3/data_understand/feature_correlation/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-13 18:19:28.000000 data_understand-0.0.3/data_understand/input_validations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-07-13 18:19:28.000000 data_understand-0.0.3/data_understand/jupyter_notebook_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:20:22.904021 data_understand-0.0.3/data_understand/load_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-13 18:19:28.000000 data_understand-0.0.3/data_understand/load_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-13 18:19:28.000000 data_understand-0.0.3/data_understand/load_dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-13 18:19:28.000000 data_understand-0.0.3/data_understand/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-07-13 18:19:28.000000 data_understand-0.0.3/data_understand/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14712 2023-07-13 18:19:28.000000 data_understand-0.0.3/data_understand/pdf_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:20:22.904021 data_understand-0.0.3/data_understand/target_characteristics/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-13 18:19:28.000000 data_understand-0.0.3/data_understand/target_characteristics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-13 18:19:28.000000 data_understand-0.0.3/data_understand/target_characteristics/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-13 18:19:28.000000 data_understand-0.0.3/data_understand/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:20:22.908021 data_understand-0.0.3/data_understand/value_distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-13 18:19:28.000000 data_understand-0.0.3/data_understand/value_distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-13 18:19:28.000000 data_understand-0.0.3/data_understand/value_distributions/box_plot_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-13 18:19:28.000000 data_understand-0.0.3/data_understand/value_distributions/cat_frequency_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-13 18:19:28.000000 data_understand-0.0.3/data_understand/value_distributions/distribution_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-07-13 18:19:28.000000 data_understand-0.0.3/data_understand/value_distributions/histogram_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-13 18:19:28.000000 data_understand-0.0.3/data_understand/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:20:22.904021 data_understand-0.0.3/data_understand.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-13 18:20:22.000000 data_understand-0.0.3/data_understand.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-13 18:20:22.000000 data_understand-0.0.3/data_understand.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 18:20:22.000000 data_understand-0.0.3/data_understand.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-13 18:20:22.000000 data_understand-0.0.3/data_understand.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-13 18:20:22.000000 data_understand-0.0.3/data_understand.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-13 18:20:22.000000 data_understand-0.0.3/data_understand.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-13 18:19:28.000000 data_understand-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 18:20:22.908021 data_understand-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-13 18:19:28.000000 data_understand-0.0.3/setup.py
```

### Comparing `data_understand-0.0.2/LICENSE` & `data_understand-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.2/PKG-INFO` & `data_understand-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_understand
-Version: 0.0.2
+Version: 0.0.3
 Summary: Utility package for generating insights for datasets
 Home-page: https://github.com/ggupta2005/data.understand
 Author: Gaurav Gupta
 Author-email: ggupta2005@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `data_understand-0.0.2/README.md` & `data_understand-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.2/data_understand/class_imbalance/imbalance.py` & `data_understand-0.0.3/data_understand/class_imbalance/imbalance.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.2/data_understand/dataset_characteristics/__init__.py` & `data_understand-0.0.3/data_understand/dataset_characteristics/__init__.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.2/data_understand/dataset_characteristics/characteristics.py` & `data_understand-0.0.3/data_understand/dataset_characteristics/characteristics.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.2/data_understand/dataset_statistics/statistics.py` & `data_understand-0.0.3/data_understand/dataset_statistics/statistics.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.2/data_understand/feature_correlation/__init__.py` & `data_understand-0.0.3/data_understand/feature_correlation/__init__.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.2/data_understand/feature_correlation/correlation.py` & `data_understand-0.0.3/data_understand/feature_correlation/correlation.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.2/data_understand/input_validations.py` & `data_understand-0.0.3/data_understand/input_validations.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.2/data_understand/jupyter_notebook_generator.py` & `data_understand-0.0.3/data_understand/jupyter_notebook_generator.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.2/data_understand/load_dataset/dataset.py` & `data_understand-0.0.3/data_understand/load_dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.2/data_understand/main.py` & `data_understand-0.0.3/data_understand/main.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.2/data_understand/messages.py` & `data_understand-0.0.3/data_understand/messages.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.2/data_understand/pdf_generator.py` & `data_understand-0.0.3/data_understand/pdf_generator.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.2/data_understand/target_characteristics/target.py` & `data_understand-0.0.3/data_understand/target_characteristics/target.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.2/data_understand/utils.py` & `data_understand-0.0.3/data_understand/utils.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.2/data_understand/value_distributions/__init__.py` & `data_understand-0.0.3/data_understand/value_distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.2/data_understand/value_distributions/box_plot_distribution.py` & `data_understand-0.0.3/data_understand/value_distributions/box_plot_distribution.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.2/data_understand/value_distributions/cat_frequency_distribution.py` & `data_understand-0.0.3/data_understand/value_distributions/cat_frequency_distribution.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.2/data_understand/value_distributions/distribution_utils.py` & `data_understand-0.0.3/data_understand/value_distributions/distribution_utils.py`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.2/data_understand/value_distributions/histogram_distribution.py` & `data_understand-0.0.3/data_understand/value_distributions/histogram_distribution.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 
 from data_understand.utils import construct_image_name
 
+Y_LABEL_DESCRIPTION = "Probability Density Distribution"
+
 
 def _get_histogram_distribution(data: np.ndarray) -> Tuple[Any, Any]:
     """
     Generate a histogram distribution for the given data.
 
     param data: The data to generate the histogram distribution for.
     type data: np.ndarray
@@ -54,15 +56,15 @@
     numeric_features = df.select_dtypes(include="number").columns.tolist()
     for feature in numeric_features:
         x, plot = _get_histogram_distribution(df[feature].values)
         plt.plot(x, plot, color="red", linewidth=2, label="Gaussian PDF")
 
         # Add labels and a legend
         plt.xlabel(feature)
-        plt.ylabel("Y axis label")
+        plt.ylabel(Y_LABEL_DESCRIPTION)
         plt.legend()
 
         # Set the title
         plt.title("Distribution Plot")
 
         # Show the plot
         plt.show()
@@ -87,15 +89,15 @@
 
     for feature in numeric_features:
         x, plot = _get_histogram_distribution(df[feature].values)
         plt.plot(x, plot, color="red", linewidth=2, label="Gaussian PDF")
 
         # Add labels and a legend
         plt.xlabel(feature)
-        plt.ylabel("Y axis label")
+        plt.ylabel(Y_LABEL_DESCRIPTION)
         plt.legend()
 
         # Set the title
         plt.title("Distribution Plot")
         saved_image_name = construct_image_name(
             "value_distribution", current_execution_uuid, index
         )
```

### Comparing `data_understand-0.0.2/data_understand.egg-info/PKG-INFO` & `data_understand-0.0.3/data_understand.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-understand
-Version: 0.0.2
+Version: 0.0.3
 Summary: Utility package for generating insights for datasets
 Home-page: https://github.com/ggupta2005/data.understand
 Author: Gaurav Gupta
 Author-email: ggupta2005@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `data_understand-0.0.2/data_understand.egg-info/SOURCES.txt` & `data_understand-0.0.3/data_understand.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data_understand-0.0.2/setup.py` & `data_understand-0.0.3/setup.py`

 * *Files identical despite different names*

