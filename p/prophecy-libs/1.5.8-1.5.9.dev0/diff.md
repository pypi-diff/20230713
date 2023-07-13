# Comparing `tmp/prophecy-libs-1.5.8.tar.gz` & `tmp/prophecy-libs-1.5.9.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prophecy-libs-1.5.8.tar", last modified: Wed Jul 12 14:13:54 2023, max compression
+gzip compressed data, was "prophecy-libs-1.5.9.dev0.tar", last modified: Thu Jul 13 12:52:58 2023, max compression
```

## Comparing `prophecy-libs-1.5.8.tar` & `prophecy-libs-1.5.9.dev0.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-12 14:13:54.367941 prophecy-libs-1.5.8/
--rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2023-07-12 14:13:54.367941 prophecy-libs-1.5.8/PKG-INFO
--rw-r--r--   0 jenkins    (109) jenkins    (114)       22 2023-03-12 14:51:36.000000 prophecy-libs-1.5.8/README.md
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-12 14:13:54.359941 prophecy-libs-1.5.8/prophecy/
--rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.5.8/prophecy/__init__.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-12 14:13:54.359941 prophecy-libs-1.5.8/prophecy/config/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.5.8/prophecy/config/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     2221 2023-03-12 14:51:36.000000 prophecy-libs-1.5.8/prophecy/config/config_base.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     4442 2023-06-09 08:12:50.000000 prophecy-libs-1.5.8/prophecy/config/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-12 14:13:54.359941 prophecy-libs-1.5.8/prophecy/libs/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       20 2023-03-12 14:51:36.000000 prophecy-libs-1.5.8/prophecy/libs/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     1500 2023-06-28 17:51:30.000000 prophecy-libs-1.5.8/prophecy/libs/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-12 14:13:54.359941 prophecy-libs-1.5.8/prophecy/lookups/
--rw-r--r--   0 jenkins    (109) jenkins    (114)     3191 2023-03-12 14:51:36.000000 prophecy-libs-1.5.8/prophecy/lookups/LookupsBase.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.5.8/prophecy/lookups/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     3118 2023-03-12 14:51:36.000000 prophecy-libs-1.5.8/prophecy/random_data_creator.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-12 14:13:54.359941 prophecy-libs-1.5.8/prophecy/streaming/
--rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.5.8/prophecy/streaming/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     5283 2023-03-12 14:51:36.000000 prophecy-libs-1.5.8/prophecy/streaming/delta_lake_utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-12 14:13:54.363941 prophecy-libs-1.5.8/prophecy/test/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       30 2023-03-12 14:51:36.000000 prophecy-libs-1.5.8/prophecy/test/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     1165 2023-05-15 15:31:20.000000 prophecy-libs-1.5.8/prophecy/test/base_test_case.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     9189 2023-04-19 07:54:52.000000 prophecy-libs-1.5.8/prophecy/test/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-12 14:13:54.363941 prophecy-libs-1.5.8/prophecy/udfs/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       87 2023-03-12 14:51:36.000000 prophecy-libs-1.5.8/prophecy/udfs/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     2154 2023-03-12 14:51:36.000000 prophecy-libs-1.5.8/prophecy/udfs/rest_api_udf.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      172 2023-03-12 14:51:36.000000 prophecy-libs-1.5.8/prophecy/udfs/sample_udf.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      988 2023-05-26 15:20:32.000000 prophecy-libs-1.5.8/prophecy/udfs/scala_udf_wrapper.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-12 14:13:54.363941 prophecy-libs-1.5.8/prophecy/utils/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       46 2023-06-28 17:51:30.000000 prophecy-libs-1.5.8/prophecy/utils/__init__.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-12 14:13:54.367941 prophecy-libs-1.5.8/prophecy/utils/transpiler/
--rw-r--r--   0 jenkins    (109) jenkins    (114)      117 2023-06-28 17:51:30.000000 prophecy-libs-1.5.8/prophecy/utils/transpiler/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      789 2023-06-28 17:51:30.000000 prophecy-libs-1.5.8/prophecy/utils/transpiler/abi_base.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)    22828 2023-06-28 17:51:30.000000 prophecy-libs-1.5.8/prophecy/utils/transpiler/abi_core_fcns.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     1591 2023-06-28 17:51:30.000000 prophecy-libs-1.5.8/prophecy/utils/transpiler/abi_fcn_wrapper.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     6521 2023-06-28 17:51:30.000000 prophecy-libs-1.5.8/prophecy/utils/transpiler/dataframe_fcns.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     6399 2023-06-28 17:51:30.000000 prophecy-libs-1.5.8/prophecy/utils/transpiler/fixed_file_schema.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)    18113 2023-07-12 14:13:52.000000 prophecy-libs-1.5.8/prophecy/utils/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-12 14:13:54.367941 prophecy-libs-1.5.8/prophecy_libs.egg-info/
--rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2023-07-12 14:13:54.000000 prophecy-libs-1.5.8/prophecy_libs.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (109) jenkins    (114)     1061 2023-07-12 14:13:54.000000 prophecy-libs-1.5.8/prophecy_libs.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-07-12 14:13:54.000000 prophecy-libs-1.5.8/prophecy_libs.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-03-12 14:51:37.000000 prophecy-libs-1.5.8/prophecy_libs.egg-info/not-zip-safe
--rw-r--r--   0 jenkins    (109) jenkins    (114)       33 2023-07-12 14:13:54.000000 prophecy-libs-1.5.8/prophecy_libs.egg-info/requires.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        9 2023-07-12 14:13:54.000000 prophecy-libs-1.5.8/prophecy_libs.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)       38 2023-07-12 14:13:54.367941 prophecy-libs-1.5.8/setup.cfg
--rw-r--r--   0 jenkins    (109) jenkins    (114)      474 2023-07-12 14:13:52.000000 prophecy-libs-1.5.8/setup.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-13 12:52:58.799620 prophecy-libs-1.5.9.dev0/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      318 2023-07-13 12:52:58.799620 prophecy-libs-1.5.9.dev0/PKG-INFO
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       22 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev0/README.md
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-13 12:52:58.791620 prophecy-libs-1.5.9.dev0/prophecy/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev0/prophecy/__init__.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-13 12:52:58.791620 prophecy-libs-1.5.9.dev0/prophecy/config/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev0/prophecy/config/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     2221 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev0/prophecy/config/config_base.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     4442 2023-06-09 08:12:50.000000 prophecy-libs-1.5.9.dev0/prophecy/config/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-13 12:52:58.791620 prophecy-libs-1.5.9.dev0/prophecy/libs/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       20 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev0/prophecy/libs/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     1500 2023-06-28 17:51:30.000000 prophecy-libs-1.5.9.dev0/prophecy/libs/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-13 12:52:58.791620 prophecy-libs-1.5.9.dev0/prophecy/lookups/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     3191 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev0/prophecy/lookups/LookupsBase.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev0/prophecy/lookups/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     3118 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev0/prophecy/random_data_creator.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-13 12:52:58.795620 prophecy-libs-1.5.9.dev0/prophecy/streaming/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev0/prophecy/streaming/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     5283 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev0/prophecy/streaming/delta_lake_utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-13 12:52:58.795620 prophecy-libs-1.5.9.dev0/prophecy/test/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       30 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev0/prophecy/test/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     1165 2023-05-15 15:31:20.000000 prophecy-libs-1.5.9.dev0/prophecy/test/base_test_case.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     9189 2023-04-19 07:54:52.000000 prophecy-libs-1.5.9.dev0/prophecy/test/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-13 12:52:58.795620 prophecy-libs-1.5.9.dev0/prophecy/udfs/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       87 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev0/prophecy/udfs/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     2154 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev0/prophecy/udfs/rest_api_udf.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      172 2023-03-12 14:51:36.000000 prophecy-libs-1.5.9.dev0/prophecy/udfs/sample_udf.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      988 2023-05-26 15:20:32.000000 prophecy-libs-1.5.9.dev0/prophecy/udfs/scala_udf_wrapper.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-13 12:52:58.795620 prophecy-libs-1.5.9.dev0/prophecy/utils/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       46 2023-06-28 17:51:30.000000 prophecy-libs-1.5.9.dev0/prophecy/utils/__init__.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-13 12:52:58.799620 prophecy-libs-1.5.9.dev0/prophecy/utils/transpiler/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      117 2023-06-28 17:51:30.000000 prophecy-libs-1.5.9.dev0/prophecy/utils/transpiler/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      789 2023-06-28 17:51:30.000000 prophecy-libs-1.5.9.dev0/prophecy/utils/transpiler/abi_base.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)    22828 2023-06-28 17:51:30.000000 prophecy-libs-1.5.9.dev0/prophecy/utils/transpiler/abi_core_fcns.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     1591 2023-06-28 17:51:30.000000 prophecy-libs-1.5.9.dev0/prophecy/utils/transpiler/abi_fcn_wrapper.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     6521 2023-06-28 17:51:30.000000 prophecy-libs-1.5.9.dev0/prophecy/utils/transpiler/dataframe_fcns.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      399 2023-07-13 12:52:57.000000 prophecy-libs-1.5.9.dev0/prophecy/utils/transpiler/dml_schema.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     6399 2023-06-28 17:51:30.000000 prophecy-libs-1.5.9.dev0/prophecy/utils/transpiler/fixed_file_schema.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)    18113 2023-07-12 14:13:52.000000 prophecy-libs-1.5.9.dev0/prophecy/utils/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-07-13 12:52:58.799620 prophecy-libs-1.5.9.dev0/prophecy_libs.egg-info/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      318 2023-07-13 12:52:58.000000 prophecy-libs-1.5.9.dev0/prophecy_libs.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     1101 2023-07-13 12:52:58.000000 prophecy-libs-1.5.9.dev0/prophecy_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-07-13 12:52:58.000000 prophecy-libs-1.5.9.dev0/prophecy_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-03-12 14:51:37.000000 prophecy-libs-1.5.9.dev0/prophecy_libs.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       33 2023-07-13 12:52:58.000000 prophecy-libs-1.5.9.dev0/prophecy_libs.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        9 2023-07-13 12:52:58.000000 prophecy-libs-1.5.9.dev0/prophecy_libs.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       38 2023-07-13 12:52:58.799620 prophecy-libs-1.5.9.dev0/setup.cfg
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      479 2023-07-13 12:52:57.000000 prophecy-libs-1.5.9.dev0/setup.py
```

### Comparing `prophecy-libs-1.5.8/prophecy/config/config_base.py` & `prophecy-libs-1.5.9.dev0/prophecy/config/config_base.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.8/prophecy/config/utils.py` & `prophecy-libs-1.5.9.dev0/prophecy/config/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.8/prophecy/libs/utils.py` & `prophecy-libs-1.5.9.dev0/prophecy/libs/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.8/prophecy/lookups/LookupsBase.py` & `prophecy-libs-1.5.9.dev0/prophecy/lookups/LookupsBase.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.8/prophecy/random_data_creator.py` & `prophecy-libs-1.5.9.dev0/prophecy/random_data_creator.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.8/prophecy/streaming/delta_lake_utils.py` & `prophecy-libs-1.5.9.dev0/prophecy/streaming/delta_lake_utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.8/prophecy/test/base_test_case.py` & `prophecy-libs-1.5.9.dev0/prophecy/test/base_test_case.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.8/prophecy/test/utils.py` & `prophecy-libs-1.5.9.dev0/prophecy/test/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.8/prophecy/udfs/rest_api_udf.py` & `prophecy-libs-1.5.9.dev0/prophecy/udfs/rest_api_udf.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.8/prophecy/udfs/scala_udf_wrapper.py` & `prophecy-libs-1.5.9.dev0/prophecy/udfs/scala_udf_wrapper.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.8/prophecy/utils/transpiler/abi_base.py` & `prophecy-libs-1.5.9.dev0/prophecy/utils/transpiler/abi_base.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.8/prophecy/utils/transpiler/abi_core_fcns.py` & `prophecy-libs-1.5.9.dev0/prophecy/utils/transpiler/abi_core_fcns.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.8/prophecy/utils/transpiler/abi_fcn_wrapper.py` & `prophecy-libs-1.5.9.dev0/prophecy/utils/transpiler/abi_fcn_wrapper.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.8/prophecy/utils/transpiler/dataframe_fcns.py` & `prophecy-libs-1.5.9.dev0/prophecy/utils/transpiler/dataframe_fcns.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.8/prophecy/utils/transpiler/fixed_file_schema.py` & `prophecy-libs-1.5.9.dev0/prophecy/utils/transpiler/fixed_file_schema.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.8/prophecy/utils/utils.py` & `prophecy-libs-1.5.9.dev0/prophecy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.8/prophecy_libs.egg-info/SOURCES.txt` & `prophecy-libs-1.5.9.dev0/prophecy_libs.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 prophecy/utils/__init__.py
 prophecy/utils/utils.py
 prophecy/utils/transpiler/__init__.py
 prophecy/utils/transpiler/abi_base.py
 prophecy/utils/transpiler/abi_core_fcns.py
 prophecy/utils/transpiler/abi_fcn_wrapper.py
 prophecy/utils/transpiler/dataframe_fcns.py
+prophecy/utils/transpiler/dml_schema.py
 prophecy/utils/transpiler/fixed_file_schema.py
 prophecy_libs.egg-info/PKG-INFO
 prophecy_libs.egg-info/SOURCES.txt
 prophecy_libs.egg-info/dependency_links.txt
 prophecy_libs.egg-info/not-zip-safe
 prophecy_libs.egg-info/requires.txt
 prophecy_libs.egg-info/top_level.txt
```

