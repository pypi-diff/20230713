# Comparing `tmp/pheno-utils-0.3.4.tar.gz` & `tmp/pheno-utils-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheno-utils-0.3.4.tar", last modified: Thu Jul 13 06:13:59 2023, max compression
+gzip compressed data, was "pheno-utils-0.3.5.tar", last modified: Thu Jul 13 10:33:06 2023, max compression
```

## Comparing `pheno-utils-0.3.4.tar` & `pheno-utils-0.3.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 06:13:59.716379 pheno-utils-0.3.4/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-21 16:13:16.000000 pheno-utils-0.3.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      111 2023-06-21 16:13:16.000000 pheno-utils-0.3.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1418 2023-07-13 06:13:59.715463 pheno-utils-0.3.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      634 2023-07-11 10:26:59.000000 pheno-utils-0.3.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 06:13:59.677920 pheno-utils-0.3.4/pheno_utils/
--rw-r--r--   0 root         (0) root         (0)      342 2023-07-13 06:05:32.000000 pheno-utils-0.3.4/pheno_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17797 2023-07-13 06:05:32.000000 pheno-utils-0.3.4/pheno_utils/_modidx.py
--rw-r--r--   0 root         (0) root         (0)    16963 2023-07-13 06:05:32.000000 pheno-utils-0.3.4/pheno_utils/age_reference_plots.py
--rw-r--r--   0 root         (0) root         (0)     5322 2023-07-13 06:05:32.000000 pheno-utils-0.3.4/pheno_utils/basic_analysis.py
--rw-r--r--   0 root         (0) root         (0)     2870 2023-07-13 06:05:32.000000 pheno-utils-0.3.4/pheno_utils/basic_plots.py
--rw-r--r--   0 root         (0) root         (0)     2517 2023-07-13 06:05:32.000000 pheno-utils-0.3.4/pheno_utils/blandaltman_plots.py
--rw-r--r--   0 root         (0) root         (0)     7865 2023-07-13 06:05:32.000000 pheno-utils-0.3.4/pheno_utils/cgm_plots.py
--rw-r--r--   0 root         (0) root         (0)     3036 2023-07-13 06:05:32.000000 pheno-utils-0.3.4/pheno_utils/cohort_selector.py
--rw-r--r--   0 root         (0) root         (0)     3594 2023-07-13 06:05:32.000000 pheno-utils-0.3.4/pheno_utils/config.py
--rw-r--r--   0 root         (0) root         (0)     2825 2023-07-13 06:05:32.000000 pheno-utils-0.3.4/pheno_utils/dates_plots.py
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-13 06:05:32.000000 pheno-utils-0.3.4/pheno_utils/ecg_analysis.py
--rw-r--r--   0 root         (0) root         (0)     7781 2023-07-13 06:05:32.000000 pheno-utils-0.3.4/pheno_utils/meta_loader.py
--rw-r--r--   0 root         (0) root         (0)    19901 2023-07-13 06:05:32.000000 pheno-utils-0.3.4/pheno_utils/pheno_loader.py
--rw-r--r--   0 root         (0) root         (0)    13210 2023-07-13 06:05:32.000000 pheno-utils-0.3.4/pheno_utils/sleep_plots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 06:13:59.711885 pheno-utils-0.3.4/pheno_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1418 2023-07-13 06:13:59.000000 pheno-utils-0.3.4/pheno_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      684 2023-07-13 06:13:59.000000 pheno-utils-0.3.4/pheno_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 06:13:59.000000 pheno-utils-0.3.4/pheno_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-13 06:13:59.000000 pheno-utils-0.3.4/pheno_utils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 16:16:15.000000 pheno-utils-0.3.4/pheno_utils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      143 2023-07-13 06:13:59.000000 pheno-utils-0.3.4/pheno_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-13 06:13:59.000000 pheno-utils-0.3.4/pheno_utils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1085 2023-07-13 06:05:06.000000 pheno-utils-0.3.4/settings.ini
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 06:13:59.716859 pheno-utils-0.3.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2560 2023-06-21 16:13:16.000000 pheno-utils-0.3.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 10:33:05.999109 pheno-utils-0.3.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-21 16:13:16.000000 pheno-utils-0.3.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-21 16:13:16.000000 pheno-utils-0.3.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1417 2023-07-13 10:33:05.997610 pheno-utils-0.3.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      633 2023-07-13 10:31:33.000000 pheno-utils-0.3.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 10:33:05.952057 pheno-utils-0.3.5/pheno_utils/
+-rw-r--r--   0 root         (0) root         (0)      342 2023-07-13 10:32:42.000000 pheno-utils-0.3.5/pheno_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17797 2023-07-13 10:32:42.000000 pheno-utils-0.3.5/pheno_utils/_modidx.py
+-rw-r--r--   0 root         (0) root         (0)    16963 2023-07-13 10:32:42.000000 pheno-utils-0.3.5/pheno_utils/age_reference_plots.py
+-rw-r--r--   0 root         (0) root         (0)     5322 2023-07-13 10:32:42.000000 pheno-utils-0.3.5/pheno_utils/basic_analysis.py
+-rw-r--r--   0 root         (0) root         (0)     2870 2023-07-13 10:32:42.000000 pheno-utils-0.3.5/pheno_utils/basic_plots.py
+-rw-r--r--   0 root         (0) root         (0)     2672 2023-07-13 10:32:42.000000 pheno-utils-0.3.5/pheno_utils/blandaltman_plots.py
+-rw-r--r--   0 root         (0) root         (0)     7865 2023-07-13 10:32:42.000000 pheno-utils-0.3.5/pheno_utils/cgm_plots.py
+-rw-r--r--   0 root         (0) root         (0)     3036 2023-07-13 10:32:42.000000 pheno-utils-0.3.5/pheno_utils/cohort_selector.py
+-rw-r--r--   0 root         (0) root         (0)     3594 2023-07-13 10:32:42.000000 pheno-utils-0.3.5/pheno_utils/config.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-07-13 10:32:42.000000 pheno-utils-0.3.5/pheno_utils/dates_plots.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-13 10:32:42.000000 pheno-utils-0.3.5/pheno_utils/ecg_analysis.py
+-rw-r--r--   0 root         (0) root         (0)     7781 2023-07-13 10:32:42.000000 pheno-utils-0.3.5/pheno_utils/meta_loader.py
+-rw-r--r--   0 root         (0) root         (0)    19901 2023-07-13 10:32:42.000000 pheno-utils-0.3.5/pheno_utils/pheno_loader.py
+-rw-r--r--   0 root         (0) root         (0)    13210 2023-07-13 10:32:42.000000 pheno-utils-0.3.5/pheno_utils/sleep_plots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 10:33:05.990569 pheno-utils-0.3.5/pheno_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1417 2023-07-13 10:33:05.000000 pheno-utils-0.3.5/pheno_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      684 2023-07-13 10:33:05.000000 pheno-utils-0.3.5/pheno_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 10:33:05.000000 pheno-utils-0.3.5/pheno_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-13 10:33:05.000000 pheno-utils-0.3.5/pheno_utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 16:16:15.000000 pheno-utils-0.3.5/pheno_utils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      143 2023-07-13 10:33:05.000000 pheno-utils-0.3.5/pheno_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-13 10:33:05.000000 pheno-utils-0.3.5/pheno_utils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      961 2023-07-13 10:28:37.000000 pheno-utils-0.3.5/settings.ini
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 10:33:05.999719 pheno-utils-0.3.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2560 2023-06-21 16:13:16.000000 pheno-utils-0.3.5/setup.py
```

### Comparing `pheno-utils-0.3.4/LICENSE` & `pheno-utils-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.4/PKG-INFO` & `pheno-utils-0.3.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.3.4
+Version: 0.3.5
 Summary: Pheno data utils - viz, loaders, mergers
-Home-page: https://github.com/hrossman/pheno-utils
+Home-page: https://github.com/pheno-ai/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -20,16 +20,17 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # pheno-utils
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
-pheno-utils is a dynamic Python package developed by Pheno.AI, for handling our medical datasets. 
-It simplifies data loading, enables effective merging, and offers intuitive visualization tools.
+pheno-utils is a dynamic Python package developed by Pheno.AI, for
+handling our medical datasets. It simplifies data loading, enables
+effective merging, and offers intuitive visualization tools.
 
 ## Install
 
 ``` sh
 pip install pheno_utils
 ```
```

### Comparing `pheno-utils-0.3.4/README.md` & `pheno-utils-0.3.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # pheno-utils
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
-pheno-utils is a dynamic Python package developed by Pheno.AI, for handling our medical datasets. 
-It simplifies data loading, enables effective merging, and offers intuitive visualization tools.
+pheno-utils is a dynamic Python package developed by Pheno.AI, for
+handling our medical datasets. It simplifies data loading, enables
+effective merging, and offers intuitive visualization tools.
 
 ## Install
 
 ``` sh
 pip install pheno_utils
 ```
```

### Comparing `pheno-utils-0.3.4/pheno_utils/_modidx.py` & `pheno-utils-0.3.5/pheno_utils/_modidx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Autogenerated by nbdev
 
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/pheno-utils',
-                'doc_host': 'https://hrossman.github.io',
-                'git_url': 'https://github.com/hrossman/pheno-utils',
+                'doc_host': 'https://pheno-ai.github.io',
+                'git_url': 'https://github.com/pheno-ai/pheno-utils',
                 'lib_path': 'pheno_utils'},
   'syms': { 'pheno_utils.age_reference_plots': { 'pheno_utils.age_reference_plots.AgeRefPlot': ( 'age_reference_plots.html#agerefplot',
                                                                                                  'pheno_utils/age_reference_plots.py'),
                                                  'pheno_utils.age_reference_plots.AgeRefPlot.__init__': ( 'age_reference_plots.html#agerefplot.__init__',
                                                                                                           'pheno_utils/age_reference_plots.py'),
                                                  'pheno_utils.age_reference_plots.AgeRefPlot.calc_linear_fit': ( 'age_reference_plots.html#agerefplot.calc_linear_fit',
                                                                                                                  'pheno_utils/age_reference_plots.py'),
```

### Comparing `pheno-utils-0.3.4/pheno_utils/age_reference_plots.py` & `pheno-utils-0.3.5/pheno_utils/age_reference_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.4/pheno_utils/basic_analysis.py` & `pheno-utils-0.3.5/pheno_utils/basic_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.4/pheno_utils/basic_plots.py` & `pheno-utils-0.3.5/pheno_utils/basic_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.4/pheno_utils/blandaltman_plots.py` & `pheno-utils-0.3.5/pheno_utils/blandaltman_plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,24 +20,26 @@
 except ImportError:
     raise ImportError("The 'pyCompare' library is not installed. Please install it using 'pip install pyCompare' before running this script.")
 
 from pyCompare import blandAltman
 
 # %% ../nbs/02_blandaltman_plots.ipynb 5
 def bland_altman_triple_plot(
-    data: pd.DataFrame, m1_col: str, m2_col: str, feature_str: str = ""
+    data: pd.DataFrame, m1_col: str, m2_col: str, feature_str: str = "",
+    scale: str = "linear",
 ) -> None:
     """
     Generates a triple plot consisting of a scatter correlation plot, Bland-Altman plot, and a percentage Bland-Altman plot.
 
     Args:
         data (pd.DataFrame): A pandas DataFrame containing the data.
         m1_col (str): The name of the first measurement column in the DataFrame.
         m2_col (str): The name of the second measurement column in the DataFrame.
         feature_str (str, optional): A string to include in the title of the plots. Defaults to "".
+        scale (str, optional): The scale of the axes. Defaults to "linear".
 
     Returns:
         None
     """
 
     m1 = data.dropna(subset=[m1_col, m2_col])[m1_col] 
     m2 = data.dropna(subset=[m1_col, m2_col])[m2_col]
@@ -62,12 +64,15 @@
     r = np.round(pearsonr(data.dropna(subset=[m1_col,m2_col])[m1_col], data.dropna(subset=[m1_col,m2_col])[m2_col])[0], 3)
     ax.set_title(f"r={r}")
 
     ax = axes[1]
     blandAltman(m1, m2, ax=ax)
     ax.set_xlabel(f"Mean of {m1.name} and {m2.name}")
     ax.set_ylabel(f"{m1.name} - {m2.name}")
+    ax.set_xscale(scale)
 
     ax = axes[2]
     blandAltman(m1, m2, ax=ax, percentage=True)
     ax.set_xlabel(f"Mean of {m1.name} and {m2.name}")
     ax.set_ylabel(f"Percentage ({m1.name} - {m2.name})")
+    ax.set_xscale(scale)
+
```

### Comparing `pheno-utils-0.3.4/pheno_utils/cgm_plots.py` & `pheno-utils-0.3.5/pheno_utils/cgm_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.4/pheno_utils/cohort_selector.py` & `pheno-utils-0.3.5/pheno_utils/cohort_selector.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.4/pheno_utils/config.py` & `pheno-utils-0.3.5/pheno_utils/config.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.4/pheno_utils/dates_plots.py` & `pheno-utils-0.3.5/pheno_utils/dates_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.4/pheno_utils/ecg_analysis.py` & `pheno-utils-0.3.5/pheno_utils/ecg_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.4/pheno_utils/meta_loader.py` & `pheno-utils-0.3.5/pheno_utils/meta_loader.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.4/pheno_utils/pheno_loader.py` & `pheno-utils-0.3.5/pheno_utils/pheno_loader.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.4/pheno_utils/sleep_plots.py` & `pheno-utils-0.3.5/pheno_utils/sleep_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.4/pheno_utils.egg-info/PKG-INFO` & `pheno-utils-0.3.5/pheno_utils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.3.4
+Version: 0.3.5
 Summary: Pheno data utils - viz, loaders, mergers
-Home-page: https://github.com/hrossman/pheno-utils
+Home-page: https://github.com/pheno-ai/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -20,16 +20,17 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # pheno-utils
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
-pheno-utils is a dynamic Python package developed by Pheno.AI, for handling our medical datasets. 
-It simplifies data loading, enables effective merging, and offers intuitive visualization tools.
+pheno-utils is a dynamic Python package developed by Pheno.AI, for
+handling our medical datasets. It simplifies data loading, enables
+effective merging, and offers intuitive visualization tools.
 
 ## Install
 
 ``` sh
 pip install pheno_utils
 ```
```

### Comparing `pheno-utils-0.3.4/pheno_utils.egg-info/SOURCES.txt` & `pheno-utils-0.3.5/pheno_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.4/setup.py` & `pheno-utils-0.3.5/setup.py`

 * *Files identical despite different names*

