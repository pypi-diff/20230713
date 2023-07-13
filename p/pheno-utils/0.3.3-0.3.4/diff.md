# Comparing `tmp/pheno-utils-0.3.3.tar.gz` & `tmp/pheno-utils-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheno-utils-0.3.3.tar", last modified: Wed Jul 12 06:53:15 2023, max compression
+gzip compressed data, was "pheno-utils-0.3.4.tar", last modified: Thu Jul 13 06:13:59 2023, max compression
```

## Comparing `pheno-utils-0.3.3.tar` & `pheno-utils-0.3.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:53:15.390483 pheno-utils-0.3.3/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-21 16:13:16.000000 pheno-utils-0.3.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      111 2023-06-21 16:13:16.000000 pheno-utils-0.3.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1418 2023-07-12 06:53:15.388326 pheno-utils-0.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      634 2023-07-11 10:26:59.000000 pheno-utils-0.3.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:53:15.339529 pheno-utils-0.3.3/pheno_utils/
--rw-r--r--   0 root         (0) root         (0)      342 2023-07-12 06:51:10.000000 pheno-utils-0.3.3/pheno_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17797 2023-07-12 06:51:10.000000 pheno-utils-0.3.3/pheno_utils/_modidx.py
--rw-r--r--   0 root         (0) root         (0)    16963 2023-07-12 06:51:10.000000 pheno-utils-0.3.3/pheno_utils/age_reference_plots.py
--rw-r--r--   0 root         (0) root         (0)     5322 2023-07-12 06:51:10.000000 pheno-utils-0.3.3/pheno_utils/basic_analysis.py
--rw-r--r--   0 root         (0) root         (0)     2870 2023-07-12 06:51:10.000000 pheno-utils-0.3.3/pheno_utils/basic_plots.py
--rw-r--r--   0 root         (0) root         (0)     2517 2023-07-12 06:51:10.000000 pheno-utils-0.3.3/pheno_utils/blandaltman_plots.py
--rw-r--r--   0 root         (0) root         (0)     7865 2023-07-12 06:51:10.000000 pheno-utils-0.3.3/pheno_utils/cgm_plots.py
--rw-r--r--   0 root         (0) root         (0)     3036 2023-07-12 06:51:10.000000 pheno-utils-0.3.3/pheno_utils/cohort_selector.py
--rw-r--r--   0 root         (0) root         (0)     3594 2023-07-12 06:51:10.000000 pheno-utils-0.3.3/pheno_utils/config.py
--rw-r--r--   0 root         (0) root         (0)     2825 2023-07-12 06:51:10.000000 pheno-utils-0.3.3/pheno_utils/dates_plots.py
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-12 06:51:10.000000 pheno-utils-0.3.3/pheno_utils/ecg_analysis.py
--rw-r--r--   0 root         (0) root         (0)     7781 2023-07-12 06:51:10.000000 pheno-utils-0.3.3/pheno_utils/meta_loader.py
--rw-r--r--   0 root         (0) root         (0)    19887 2023-07-12 06:51:10.000000 pheno-utils-0.3.3/pheno_utils/pheno_loader.py
--rw-r--r--   0 root         (0) root         (0)    13210 2023-07-12 06:51:10.000000 pheno-utils-0.3.3/pheno_utils/sleep_plots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 06:53:15.381653 pheno-utils-0.3.3/pheno_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1418 2023-07-12 06:53:15.000000 pheno-utils-0.3.3/pheno_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      684 2023-07-12 06:53:15.000000 pheno-utils-0.3.3/pheno_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 06:53:15.000000 pheno-utils-0.3.3/pheno_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-12 06:53:15.000000 pheno-utils-0.3.3/pheno_utils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 16:16:15.000000 pheno-utils-0.3.3/pheno_utils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      143 2023-07-12 06:53:15.000000 pheno-utils-0.3.3/pheno_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-12 06:53:15.000000 pheno-utils-0.3.3/pheno_utils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1085 2023-07-12 06:51:06.000000 pheno-utils-0.3.3/settings.ini
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 06:53:15.392259 pheno-utils-0.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2560 2023-06-21 16:13:16.000000 pheno-utils-0.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 06:13:59.716379 pheno-utils-0.3.4/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-21 16:13:16.000000 pheno-utils-0.3.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-21 16:13:16.000000 pheno-utils-0.3.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1418 2023-07-13 06:13:59.715463 pheno-utils-0.3.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      634 2023-07-11 10:26:59.000000 pheno-utils-0.3.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 06:13:59.677920 pheno-utils-0.3.4/pheno_utils/
+-rw-r--r--   0 root         (0) root         (0)      342 2023-07-13 06:05:32.000000 pheno-utils-0.3.4/pheno_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17797 2023-07-13 06:05:32.000000 pheno-utils-0.3.4/pheno_utils/_modidx.py
+-rw-r--r--   0 root         (0) root         (0)    16963 2023-07-13 06:05:32.000000 pheno-utils-0.3.4/pheno_utils/age_reference_plots.py
+-rw-r--r--   0 root         (0) root         (0)     5322 2023-07-13 06:05:32.000000 pheno-utils-0.3.4/pheno_utils/basic_analysis.py
+-rw-r--r--   0 root         (0) root         (0)     2870 2023-07-13 06:05:32.000000 pheno-utils-0.3.4/pheno_utils/basic_plots.py
+-rw-r--r--   0 root         (0) root         (0)     2517 2023-07-13 06:05:32.000000 pheno-utils-0.3.4/pheno_utils/blandaltman_plots.py
+-rw-r--r--   0 root         (0) root         (0)     7865 2023-07-13 06:05:32.000000 pheno-utils-0.3.4/pheno_utils/cgm_plots.py
+-rw-r--r--   0 root         (0) root         (0)     3036 2023-07-13 06:05:32.000000 pheno-utils-0.3.4/pheno_utils/cohort_selector.py
+-rw-r--r--   0 root         (0) root         (0)     3594 2023-07-13 06:05:32.000000 pheno-utils-0.3.4/pheno_utils/config.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-07-13 06:05:32.000000 pheno-utils-0.3.4/pheno_utils/dates_plots.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-13 06:05:32.000000 pheno-utils-0.3.4/pheno_utils/ecg_analysis.py
+-rw-r--r--   0 root         (0) root         (0)     7781 2023-07-13 06:05:32.000000 pheno-utils-0.3.4/pheno_utils/meta_loader.py
+-rw-r--r--   0 root         (0) root         (0)    19901 2023-07-13 06:05:32.000000 pheno-utils-0.3.4/pheno_utils/pheno_loader.py
+-rw-r--r--   0 root         (0) root         (0)    13210 2023-07-13 06:05:32.000000 pheno-utils-0.3.4/pheno_utils/sleep_plots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 06:13:59.711885 pheno-utils-0.3.4/pheno_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1418 2023-07-13 06:13:59.000000 pheno-utils-0.3.4/pheno_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      684 2023-07-13 06:13:59.000000 pheno-utils-0.3.4/pheno_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 06:13:59.000000 pheno-utils-0.3.4/pheno_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-13 06:13:59.000000 pheno-utils-0.3.4/pheno_utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 16:16:15.000000 pheno-utils-0.3.4/pheno_utils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      143 2023-07-13 06:13:59.000000 pheno-utils-0.3.4/pheno_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-13 06:13:59.000000 pheno-utils-0.3.4/pheno_utils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-07-13 06:05:06.000000 pheno-utils-0.3.4/settings.ini
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 06:13:59.716859 pheno-utils-0.3.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2560 2023-06-21 16:13:16.000000 pheno-utils-0.3.4/setup.py
```

### Comparing `pheno-utils-0.3.3/LICENSE` & `pheno-utils-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.3/PKG-INFO` & `pheno-utils-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.3.3
+Version: 0.3.4
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pheno-utils-0.3.3/README.md` & `pheno-utils-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.3/pheno_utils/_modidx.py` & `pheno-utils-0.3.4/pheno_utils/_modidx.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.3/pheno_utils/age_reference_plots.py` & `pheno-utils-0.3.4/pheno_utils/age_reference_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.3/pheno_utils/basic_analysis.py` & `pheno-utils-0.3.4/pheno_utils/basic_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.3/pheno_utils/basic_plots.py` & `pheno-utils-0.3.4/pheno_utils/basic_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.3/pheno_utils/blandaltman_plots.py` & `pheno-utils-0.3.4/pheno_utils/blandaltman_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.3/pheno_utils/cgm_plots.py` & `pheno-utils-0.3.4/pheno_utils/cgm_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.3/pheno_utils/cohort_selector.py` & `pheno-utils-0.3.4/pheno_utils/cohort_selector.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.3/pheno_utils/config.py` & `pheno-utils-0.3.4/pheno_utils/config.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.3/pheno_utils/dates_plots.py` & `pheno-utils-0.3.4/pheno_utils/dates_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.3/pheno_utils/ecg_analysis.py` & `pheno-utils-0.3.4/pheno_utils/ecg_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.3/pheno_utils/meta_loader.py` & `pheno-utils-0.3.4/pheno_utils/meta_loader.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.3/pheno_utils/pheno_loader.py` & `pheno-utils-0.3.4/pheno_utils/pheno_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,15 +264,15 @@
         cols = [col for col in bulk_fields.index.to_list() if col in data.columns] 
         dataset_bulk_data_path = {k:v.format(dataset=self.dataset) for k, v in BULK_DATA_PATH.items()}
         category_cols = self.dict.loc[self.dict.index.isin(fields)].query('pandas_dtype == "category"').index
     
         for col in category_cols: 
             data[col] = data[col].astype(str)
 
-        data[cols] = data[cols].replace(dataset_bulk_data_path, regex=True)
+        data[cols] = data[cols].fillna('nan').replace(dataset_bulk_data_path, regex=True)
         for col in category_cols: 
             data[col] = data[col].astype('category')
             
         return data
```

### Comparing `pheno-utils-0.3.3/pheno_utils/sleep_plots.py` & `pheno-utils-0.3.4/pheno_utils/sleep_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.3/pheno_utils.egg-info/PKG-INFO` & `pheno-utils-0.3.4/pheno_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.3.3
+Version: 0.3.4
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pheno-utils-0.3.3/pheno_utils.egg-info/SOURCES.txt` & `pheno-utils-0.3.4/pheno_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.3/settings.ini` & `pheno-utils-0.3.4/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = pheno-utils
 lib_name = %(repo)s
-version = 0.3.3
+version = 0.3.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = pheno_utils
```

### Comparing `pheno-utils-0.3.3/setup.py` & `pheno-utils-0.3.4/setup.py`

 * *Files identical despite different names*

