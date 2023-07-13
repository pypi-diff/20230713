# Comparing `tmp/lusidtools-1.0.8.tar.gz` & `tmp/lusidtools-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusidtools-1.0.8.tar", last modified: Fri Dec 23 14:19:39 2022, max compression
+gzip compressed data, was "lusidtools-1.0.9.tar", last modified: Thu Jan 12 14:48:05 2023, max compression
```

## Comparing `lusidtools-1.0.8.tar` & `lusidtools-1.0.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 14:19:39.780973 lusidtools-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2022-12-23 14:19:30.000000 lusidtools-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      121 2022-12-23 14:19:30.000000 lusidtools-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      315 2022-12-23 14:19:39.780973 lusidtools-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2022-12-23 14:19:30.000000 lusidtools-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 14:19:39.772973 lusidtools-1.0.8/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 14:19:30.000000 lusidtools-1.0.8/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2022-12-23 14:19:30.000000 lusidtools-1.0.8/features/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 14:19:39.772973 lusidtools-1.0.8/lusidtools/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 14:19:39.776973 lusidtools-1.0.8/lusidtools/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12001 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/apps/flush_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/apps/upsert_holdings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/apps/upsert_instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/apps/upsert_portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/apps/upsert_quotes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/apps/upsert_transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 14:19:39.780973 lusidtools-1.0.8/lusidtools/cocoon/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/cocoon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/cocoon/async_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    63159 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/cocoon/cocoon.py
--rw-r--r--   0 runner    (1001) docker     (123)    11581 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/cocoon/cocoon_printer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 14:19:39.780973 lusidtools-1.0.8/lusidtools/cocoon/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/cocoon/config/domain_settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/cocoon/config/seed_sample_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     5793 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/cocoon/dateorcutlabel.py
--rw-r--r--   0 runner    (1001) docker     (123)    17194 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/cocoon/instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)    14180 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/cocoon/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/cocoon/seed_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/cocoon/systemConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/cocoon/transaction_type_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)    59648 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/cocoon/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7381 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/cocoon/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 14:19:39.780973 lusidtools-1.0.8/lusidtools/extract/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14775 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/extract/group_holdings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 14:19:39.780973 lusidtools-1.0.8/lusidtools/iam/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/iam/roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 14:19:39.780973 lusidtools-1.0.8/lusidtools/jupyter_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/jupyter_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/jupyter_tools/hide_code_button.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/jupyter_tools/stop_execution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 14:19:39.780973 lusidtools-1.0.8/lusidtools/logger/
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/logger/LusidLogger.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/logger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 14:19:39.780973 lusidtools-1.0.8/lusidtools/pandas_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/pandas_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2022-12-23 14:19:30.000000 lusidtools-1.0.8/lusidtools/pandas_utils/lusid_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 14:19:39.776973 lusidtools-1.0.8/lusidtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2022-12-23 14:19:39.000000 lusidtools-1.0.8/lusidtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2022-12-23 14:19:39.000000 lusidtools-1.0.8/lusidtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-23 14:19:39.000000 lusidtools-1.0.8/lusidtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      415 2022-12-23 14:19:39.000000 lusidtools-1.0.8/lusidtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2022-12-23 14:19:39.000000 lusidtools-1.0.8/lusidtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2022-12-23 14:19:39.000000 lusidtools-1.0.8/lusidtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-23 14:19:39.780973 lusidtools-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2022-12-23 14:19:30.000000 lusidtools-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 14:48:05.158167 lusidtools-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-01-12 14:47:45.000000 lusidtools-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-01-12 14:47:45.000000 lusidtools-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-01-12 14:48:05.158167 lusidtools-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-01-12 14:47:45.000000 lusidtools-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 14:48:05.150167 lusidtools-1.0.9/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 14:47:45.000000 lusidtools-1.0.9/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-01-12 14:47:45.000000 lusidtools-1.0.9/features/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 14:48:05.150167 lusidtools-1.0.9/lusidtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 14:48:05.154167 lusidtools-1.0.9/lusidtools/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/apps/flush_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/apps/upsert_holdings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/apps/upsert_instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/apps/upsert_portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/apps/upsert_quotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/apps/upsert_transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 14:48:05.158167 lusidtools-1.0.9/lusidtools/cocoon/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/cocoon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/cocoon/async_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63159 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/cocoon/cocoon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14007 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/cocoon/cocoon_printer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 14:48:05.158167 lusidtools-1.0.9/lusidtools/cocoon/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/cocoon/config/domain_settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/cocoon/config/seed_sample_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/cocoon/dateorcutlabel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17194 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/cocoon/instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14180 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/cocoon/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/cocoon/seed_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/cocoon/systemConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/cocoon/transaction_type_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59648 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/cocoon/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/cocoon/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 14:48:05.158167 lusidtools-1.0.9/lusidtools/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14775 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/extract/group_holdings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 14:48:05.158167 lusidtools-1.0.9/lusidtools/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/iam/roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 14:48:05.158167 lusidtools-1.0.9/lusidtools/jupyter_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/jupyter_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/jupyter_tools/hide_code_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/jupyter_tools/stop_execution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 14:48:05.158167 lusidtools-1.0.9/lusidtools/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/logger/LusidLogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/logger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 14:48:05.158167 lusidtools-1.0.9/lusidtools/pandas_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/pandas_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-01-12 14:47:45.000000 lusidtools-1.0.9/lusidtools/pandas_utils/lusid_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 14:48:05.154167 lusidtools-1.0.9/lusidtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-01-12 14:48:04.000000 lusidtools-1.0.9/lusidtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-01-12 14:48:05.000000 lusidtools-1.0.9/lusidtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 14:48:04.000000 lusidtools-1.0.9/lusidtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-01-12 14:48:04.000000 lusidtools-1.0.9/lusidtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-01-12 14:48:04.000000 lusidtools-1.0.9/lusidtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-12 14:48:04.000000 lusidtools-1.0.9/lusidtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 14:48:05.158167 lusidtools-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-01-12 14:47:45.000000 lusidtools-1.0.9/setup.py
```

### Comparing `lusidtools-1.0.8/LICENSE` & `lusidtools-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lusidtools-1.0.8/README.md` & `lusidtools-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `lusidtools-1.0.8/lusidtools/apps/flush_transactions.py` & `lusidtools-1.0.9/lusidtools/apps/flush_transactions.py`

 * *Files identical despite different names*

### Comparing `lusidtools-1.0.8/lusidtools/apps/upsert_holdings.py` & `lusidtools-1.0.9/lusidtools/apps/upsert_holdings.py`

 * *Files identical despite different names*

### Comparing `lusidtools-1.0.8/lusidtools/apps/upsert_instruments.py` & `lusidtools-1.0.9/lusidtools/apps/upsert_instruments.py`

 * *Files identical despite different names*

### Comparing `lusidtools-1.0.8/lusidtools/apps/upsert_portfolios.py` & `lusidtools-1.0.9/lusidtools/apps/upsert_portfolios.py`

 * *Files identical despite different names*

### Comparing `lusidtools-1.0.8/lusidtools/apps/upsert_quotes.py` & `lusidtools-1.0.9/lusidtools/apps/upsert_quotes.py`

 * *Files identical despite different names*

### Comparing `lusidtools-1.0.8/lusidtools/apps/upsert_transactions.py` & `lusidtools-1.0.9/lusidtools/apps/upsert_transactions.py`

 * *Files identical despite different names*

### Comparing `lusidtools-1.0.8/lusidtools/cocoon/__init__.py` & `lusidtools-1.0.9/lusidtools/cocoon/__init__.py`

 * *Files identical despite different names*

### Comparing `lusidtools-1.0.8/lusidtools/cocoon/async_tools.py` & `lusidtools-1.0.9/lusidtools/cocoon/async_tools.py`

 * *Files identical despite different names*

### Comparing `lusidtools-1.0.8/lusidtools/cocoon/cocoon.py` & `lusidtools-1.0.9/lusidtools/cocoon/cocoon.py`

 * *Files identical despite different names*

### Comparing `lusidtools-1.0.8/lusidtools/cocoon/cocoon_printer.py` & `lusidtools-1.0.9/lusidtools/cocoon/cocoon_printer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,87 @@
 import pandas as pd
 import numpy as np
 from lusidtools.cocoon import checkargs
 from lusid.exceptions import ApiException
 from flatten_json import flatten
 
 
+class CocoonPrinter:
+    VALID_KEYS = [
+        "portfolios",
+        "instruments",
+        "transactions",
+        "quotes",
+        "holdings",
+        "reference_portfolios",
+    ]
+
+    def __init__(
+        self, response, extended_error_details=False, data_entity_details=False
+    ):
+        self.validate(response)
+
+        self.response = response
+        self.file_type = list(response.keys())[0]
+        self.extended_error_details = extended_error_details
+        self.data_entity_details = data_entity_details
+
+    def validate(self, response):
+        if len(response.keys()) == 0:
+            message = (
+                f"Response doesn't contain any keys. Valid keys are {self.VALID_KEYS}"
+            )
+            raise ValueError(message)
+
+        if len(response.keys()) > 1:
+            message = f"Response contains too many keys - only one is allowed, but received {list(response.keys())}"
+            raise ValueError(message)
+
+        key = list(response.keys())[0]
+
+        if key not in self.VALID_KEYS:
+            message = f"Response contains invalid key. Valid keys are {self.VALID_KEYS}, but received {key}"
+            raise ValueError(message)
+
+    def format_instruments_response(self):
+        return format_instruments_response(
+            self.response,
+            extended_error_details=self.extended_error_details,
+            data_entity_details=self.data_entity_details,
+        )
+
+    def format_portfolios_response(self):
+        return format_portfolios_response(
+            self.response, extended_error_details=self.extended_error_details
+        )
+
+    def format_transactions_response(self):
+        return format_transactions_response(
+            self.response, extended_error_details=self.extended_error_details
+        )
+
+    def format_quotes_response(self):
+        return format_quotes_response(
+            self.response, extended_error_details=self.extended_error_details,
+        )
+
+    def format_holdings_response(self):
+        return format_holdings_response(
+            self.response, extended_error_details=self.extended_error_details,
+        )
+
+    def format_reference_portfolios_response(self):
+        return format_reference_portfolios_response(
+            self.response, extended_error_details=self.extended_error_details,
+        )
+
+    def format_response(self):
+        return getattr(CocoonPrinter, f"format_{self.file_type}_response")(self)
+
+
 @checkargs
 def check_dict_for_required_keys(
     target_dict: dict, target_name: str, required_keys: list
 ):
     """
     This function checks that a named dictionary contains a list of required key
```

### Comparing `lusidtools-1.0.8/lusidtools/cocoon/config/domain_settings.json` & `lusidtools-1.0.9/lusidtools/cocoon/config/domain_settings.json`

 * *Files identical despite different names*

### Comparing `lusidtools-1.0.8/lusidtools/cocoon/config/seed_sample_data.json` & `lusidtools-1.0.9/lusidtools/cocoon/config/seed_sample_data.json`

 * *Files identical despite different names*

### Comparing `lusidtools-1.0.8/lusidtools/cocoon/dateorcutlabel.py` & `lusidtools-1.0.9/lusidtools/cocoon/dateorcutlabel.py`

 * *Files identical despite different names*

### Comparing `lusidtools-1.0.8/lusidtools/cocoon/instruments.py` & `lusidtools-1.0.9/lusidtools/cocoon/instruments.py`

 * *Files identical despite different names*

### Comparing `lusidtools-1.0.8/lusidtools/cocoon/properties.py` & `lusidtools-1.0.9/lusidtools/cocoon/properties.py`

 * *Files identical despite different names*

### Comparing `lusidtools-1.0.8/lusidtools/cocoon/seed_sample_data.py` & `lusidtools-1.0.9/lusidtools/cocoon/seed_sample_data.py`

 * *Files identical despite different names*

### Comparing `lusidtools-1.0.8/lusidtools/cocoon/systemConfiguration.py` & `lusidtools-1.0.9/lusidtools/cocoon/systemConfiguration.py`

 * *Files identical despite different names*

### Comparing `lusidtools-1.0.8/lusidtools/cocoon/transaction_type_upload.py` & `lusidtools-1.0.9/lusidtools/cocoon/transaction_type_upload.py`

 * *Files identical despite different names*

### Comparing `lusidtools-1.0.8/lusidtools/cocoon/utilities.py` & `lusidtools-1.0.9/lusidtools/cocoon/utilities.py`

 * *Files identical despite different names*

### Comparing `lusidtools-1.0.8/lusidtools/cocoon/validator.py` & `lusidtools-1.0.9/lusidtools/cocoon/validator.py`

 * *Files identical despite different names*

### Comparing `lusidtools-1.0.8/lusidtools/extract/group_holdings.py` & `lusidtools-1.0.9/lusidtools/extract/group_holdings.py`

 * *Files identical despite different names*

### Comparing `lusidtools-1.0.8/lusidtools/iam/roles.py` & `lusidtools-1.0.9/lusidtools/iam/roles.py`

 * *Files identical despite different names*

### Comparing `lusidtools-1.0.8/lusidtools/jupyter_tools/hide_code_button.py` & `lusidtools-1.0.9/lusidtools/jupyter_tools/hide_code_button.py`

 * *Files identical despite different names*

### Comparing `lusidtools-1.0.8/lusidtools/logger/LusidLogger.py` & `lusidtools-1.0.9/lusidtools/logger/LusidLogger.py`

 * *Files identical despite different names*

### Comparing `lusidtools-1.0.8/lusidtools/pandas_utils/lusid_pandas.py` & `lusidtools-1.0.9/lusidtools/pandas_utils/lusid_pandas.py`

 * *Files identical despite different names*

### Comparing `lusidtools-1.0.8/lusidtools.egg-info/SOURCES.txt` & `lusidtools-1.0.9/lusidtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lusidtools-1.0.8/setup.py` & `lusidtools-1.0.9/setup.py`

 * *Files identical despite different names*

