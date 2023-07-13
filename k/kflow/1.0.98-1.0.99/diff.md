# Comparing `tmp/kflow-1.0.98.tar.gz` & `tmp/kflow-1.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kflow-1.0.98.tar", last modified: Tue Dec  6 13:41:54 2022, max compression
+gzip compressed data, was "kflow-1.0.99.tar", last modified: Mon Dec 12 15:03:50 2022, max compression
```

## Comparing `kflow-1.0.98.tar` & `kflow-1.0.99.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:41:54.189089 kflow-1.0.98/
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2022-12-06 13:41:41.000000 kflow-1.0.98/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      575 2022-12-06 13:41:54.189089 kflow-1.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      216 2022-12-06 13:41:41.000000 kflow-1.0.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:41:54.189089 kflow-1.0.98/kflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 13:41:41.000000 kflow-1.0.98/kflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7074 2022-12-06 13:41:41.000000 kflow-1.0.98/kflow/authn.py
--rw-r--r--   0 runner    (1001) docker     (123)    24368 2022-12-06 13:41:41.000000 kflow-1.0.98/kflow/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)    25900 2022-12-06 13:41:41.000000 kflow-1.0.98/kflow/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2022-12-06 13:41:41.000000 kflow-1.0.98/kflow/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7948 2022-12-06 13:41:41.000000 kflow-1.0.98/kflow/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 13:41:54.189089 kflow-1.0.98/kflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2022-12-06 13:41:54.000000 kflow-1.0.98/kflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      238 2022-12-06 13:41:54.000000 kflow-1.0.98/kflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 13:41:54.000000 kflow-1.0.98/kflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-06 13:41:54.000000 kflow-1.0.98/kflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-06 13:41:54.189089 kflow-1.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      960 2022-12-06 13:41:41.000000 kflow-1.0.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 15:03:50.338219 kflow-1.0.99/
+-rw-r--r--   0 runner    (1001) docker     (123)     9145 2022-12-12 15:03:33.000000 kflow-1.0.99/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2022-12-12 15:03:50.338219 kflow-1.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2022-12-12 15:03:33.000000 kflow-1.0.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 15:03:50.338219 kflow-1.0.99/kflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 15:03:33.000000 kflow-1.0.99/kflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7074 2022-12-12 15:03:33.000000 kflow-1.0.99/kflow/authn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24368 2022-12-12 15:03:33.000000 kflow-1.0.99/kflow/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25882 2022-12-12 15:03:33.000000 kflow-1.0.99/kflow/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2022-12-12 15:03:33.000000 kflow-1.0.99/kflow/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7948 2022-12-12 15:03:33.000000 kflow-1.0.99/kflow/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 15:03:50.338219 kflow-1.0.99/kflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2022-12-12 15:03:50.000000 kflow-1.0.99/kflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2022-12-12 15:03:50.000000 kflow-1.0.99/kflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 15:03:50.000000 kflow-1.0.99/kflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-12 15:03:50.000000 kflow-1.0.99/kflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-12 15:03:50.338219 kflow-1.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2022-12-12 15:03:33.000000 kflow-1.0.99/setup.py
```

### Comparing `kflow-1.0.98/LICENSE.txt` & `kflow-1.0.99/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kflow-1.0.98/PKG-INFO` & `kflow-1.0.99/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kflow
-Version: 1.0.98
+Version: 1.0.99
 Summary: KLog.co package for ETLs
 Home-page: https://github.com/teu-ai/etl
 Author: KLog.co Data & BI
 Author-email: data@klog.co
 License: Apache
 Keywords: etl data science airflow
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `kflow-1.0.98/kflow/authn.py` & `kflow-1.0.99/kflow/authn.py`

 * *Files identical despite different names*

### Comparing `kflow-1.0.98/kflow/extract.py` & `kflow-1.0.99/kflow/extract.py`

 * *Files identical despite different names*

### Comparing `kflow-1.0.98/kflow/load.py` & `kflow-1.0.99/kflow/load.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
     base_env:str='WarehouseProd'
         "WarehouseProd" - Productive enviroment on Redshift 
     """
 
     warehouse_engine = authn.getConnectionDB(base_env)
 
     if to_lake_args:
-        DataFrameToLake(*to_lake_args, format="parquet")
+        DataFrameToLake(*to_lake_args)
 
     if delete_table:
         schema = to_sql_kwargs["schema"] if "schema" in to_sql_kwargs.keys() else "public"
         WarehouseDeleteTable(table, schema=schema, warehouse_engine=warehouse_engine)
     try:
         df.to_sql(table, warehouse_engine, dtype=dtype, **to_sql_kwargs)
     except Exception as e:
```

### Comparing `kflow-1.0.98/kflow/log.py` & `kflow-1.0.99/kflow/log.py`

 * *Files identical despite different names*

### Comparing `kflow-1.0.98/kflow/tools.py` & `kflow-1.0.99/kflow/tools.py`

 * *Files identical despite different names*

### Comparing `kflow-1.0.98/kflow.egg-info/PKG-INFO` & `kflow-1.0.99/kflow.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kflow
-Version: 1.0.98
+Version: 1.0.99
 Summary: KLog.co package for ETLs
 Home-page: https://github.com/teu-ai/etl
 Author: KLog.co Data & BI
 Author-email: data@klog.co
 License: Apache
 Keywords: etl data science airflow
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `kflow-1.0.98/setup.py` & `kflow-1.0.99/setup.py`

 * *Files identical despite different names*

