# Comparing `tmp/dsmlibrary_viz-0.0.2.tar.gz` & `tmp/dsmlibrary_viz-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsmlibrary_viz-0.0.2.tar", last modified: Wed Jul 12 14:26:32 2023, max compression
+gzip compressed data, was "dsmlibrary_viz-0.0.3.tar", last modified: Thu Jul 13 09:15:23 2023, max compression
```

## Comparing `dsmlibrary_viz-0.0.2.tar` & `dsmlibrary_viz-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-12 14:26:32.471256 dsmlibrary_viz-0.0.2/
--rw-r--r--   0 naii       (501) staff       (20)     1066 2023-07-12 12:08:08.000000 dsmlibrary_viz-0.0.2/LICENSE
--rw-r--r--   0 naii       (501) staff       (20)     1054 2023-07-12 14:26:32.469952 dsmlibrary_viz-0.0.2/PKG-INFO
--rw-r--r--   0 naii       (501) staff       (20)      355 2023-07-12 14:26:15.000000 dsmlibrary_viz-0.0.2/README.md
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-12 14:26:32.452189 dsmlibrary_viz-0.0.2/dsmlibrary_viz/
--rw-r--r--   0 naii       (501) staff       (20)      160 2023-07-12 14:26:28.000000 dsmlibrary_viz-0.0.2/dsmlibrary_viz/__init__.py
--rw-r--r--   0 naii       (501) staff       (20)     2255 2023-07-12 14:14:40.000000 dsmlibrary_viz-0.0.2/dsmlibrary_viz/base.py
--rw-r--r--   0 naii       (501) staff       (20)     1335 2023-07-12 14:19:49.000000 dsmlibrary_viz-0.0.2/dsmlibrary_viz/data_viz.py
--rw-r--r--   0 naii       (501) staff       (20)      232 2023-07-12 14:07:14.000000 dsmlibrary_viz-0.0.2/dsmlibrary_viz/utils.py
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-12 14:26:32.468687 dsmlibrary_viz-0.0.2/dsmlibrary_viz.egg-info/
--rw-r--r--   0 naii       (501) staff       (20)     1054 2023-07-12 14:26:32.000000 dsmlibrary_viz-0.0.2/dsmlibrary_viz.egg-info/PKG-INFO
--rw-r--r--   0 naii       (501) staff       (20)      316 2023-07-12 14:26:32.000000 dsmlibrary_viz-0.0.2/dsmlibrary_viz.egg-info/SOURCES.txt
--rw-r--r--   0 naii       (501) staff       (20)        1 2023-07-12 14:26:32.000000 dsmlibrary_viz-0.0.2/dsmlibrary_viz.egg-info/dependency_links.txt
--rw-r--r--   0 naii       (501) staff       (20)       28 2023-07-12 14:26:32.000000 dsmlibrary_viz-0.0.2/dsmlibrary_viz.egg-info/requires.txt
--rw-r--r--   0 naii       (501) staff       (20)       15 2023-07-12 14:26:32.000000 dsmlibrary_viz-0.0.2/dsmlibrary_viz.egg-info/top_level.txt
--rw-r--r--   0 naii       (501) staff       (20)       38 2023-07-12 14:26:32.471797 dsmlibrary_viz-0.0.2/setup.cfg
--rw-r--r--   0 naii       (501) staff       (20)     1410 2023-07-12 14:24:27.000000 dsmlibrary_viz-0.0.2/setup.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-13 09:15:23.989722 dsmlibrary_viz-0.0.3/
+-rw-r--r--   0 naii       (501) staff       (20)     1066 2023-07-12 12:08:08.000000 dsmlibrary_viz-0.0.3/LICENSE
+-rw-r--r--   0 naii       (501) staff       (20)     1054 2023-07-13 09:15:23.989324 dsmlibrary_viz-0.0.3/PKG-INFO
+-rw-r--r--   0 naii       (501) staff       (20)      355 2023-07-12 14:26:15.000000 dsmlibrary_viz-0.0.3/README.md
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-13 09:15:23.986050 dsmlibrary_viz-0.0.3/dsmlibrary_viz/
+-rw-r--r--   0 naii       (501) staff       (20)      160 2023-07-13 09:15:09.000000 dsmlibrary_viz-0.0.3/dsmlibrary_viz/__init__.py
+-rw-r--r--   0 naii       (501) staff       (20)     2255 2023-07-12 14:14:40.000000 dsmlibrary_viz-0.0.3/dsmlibrary_viz/base.py
+-rw-r--r--   0 naii       (501) staff       (20)     2222 2023-07-13 09:14:39.000000 dsmlibrary_viz-0.0.3/dsmlibrary_viz/data_viz.py
+-rw-r--r--   0 naii       (501) staff       (20)      619 2023-07-12 15:26:02.000000 dsmlibrary_viz-0.0.3/dsmlibrary_viz/utils.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-13 09:15:23.988485 dsmlibrary_viz-0.0.3/dsmlibrary_viz.egg-info/
+-rw-r--r--   0 naii       (501) staff       (20)     1054 2023-07-13 09:15:23.000000 dsmlibrary_viz-0.0.3/dsmlibrary_viz.egg-info/PKG-INFO
+-rw-r--r--   0 naii       (501) staff       (20)      316 2023-07-13 09:15:23.000000 dsmlibrary_viz-0.0.3/dsmlibrary_viz.egg-info/SOURCES.txt
+-rw-r--r--   0 naii       (501) staff       (20)        1 2023-07-13 09:15:23.000000 dsmlibrary_viz-0.0.3/dsmlibrary_viz.egg-info/dependency_links.txt
+-rw-r--r--   0 naii       (501) staff       (20)       28 2023-07-13 09:15:23.000000 dsmlibrary_viz-0.0.3/dsmlibrary_viz.egg-info/requires.txt
+-rw-r--r--   0 naii       (501) staff       (20)       15 2023-07-13 09:15:23.000000 dsmlibrary_viz-0.0.3/dsmlibrary_viz.egg-info/top_level.txt
+-rw-r--r--   0 naii       (501) staff       (20)       38 2023-07-13 09:15:23.989860 dsmlibrary_viz-0.0.3/setup.cfg
+-rw-r--r--   0 naii       (501) staff       (20)     1410 2023-07-12 14:24:27.000000 dsmlibrary_viz-0.0.3/setup.py
```

### Comparing `dsmlibrary_viz-0.0.2/LICENSE` & `dsmlibrary_viz-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dsmlibrary_viz-0.0.2/PKG-INFO` & `dsmlibrary_viz-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsmlibrary_viz
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple way to use Dataset. for dsm
 Home-page: https://github.com/storemesh/dsmlibrary-viz
 Author: DigitalStoreMesh Co.,Ltd
 Author-email: contact@storemesh.com
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dsmlibrary_viz-0.0.2/dsmlibrary_viz/base.py` & `dsmlibrary_viz-0.0.3/dsmlibrary_viz/base.py`

 * *Files identical despite different names*

### Comparing `dsmlibrary_viz-0.0.2/dsmlibrary_viz/data_viz.py` & `dsmlibrary_viz-0.0.3/dsmlibrary_viz/data_viz.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,63 @@
 import re
 import duckdb
 from . import base
+import pandas as pd
 
 class DataViz(base.Base):
     
     def __init__(self, token=None, verbose=True, dataplatform_api_uri=None, object_storage_uri=None, apikey=None):
         try:
             duckdb.sql("install 'httpfs';")
         except Exception as e:
             pass
         super().__init__(token, verbose, dataplatform_api_uri, object_storage_uri, apikey)
 
     def _find_fileID(self, match):
         match = match.group()
         _file_id = match.split(':')[-1]
         meta = self.get_meta_file(file_id=_file_id)
-        return f"s3://dataplatform/{meta.get('s3_key')}/*.parquet"
+        osd_key = meta.get('s3_key')
+        return f"s3://dataplatform/{osd_key}/*.parquet"
+    
+    def _find_fileID2(self, match):
+        match = match.group()
+        _file_id = match.split(':')[-1]
+        meta = self.get_meta_file(file_id=_file_id)
+        osd_key = meta.get('s3_key')
+        return f"s3://dataplatform/{osd_key}/*/*.parquet"
+    
+    def _find_fileID3(self, match):
+        match = match.group()
+        _file_id = match.split(':')[-1]
+        meta = self.get_meta_file(file_id=_file_id)
+        osd_key = meta.get('s3_key')
+        return f"s3://dataplatform/{osd_key}/*/*/*.parquet",
+
 
     def _query(self, query_str):
         _storage_options = self._storage_options
         query = f"""
         load 'httpfs';
         SET s3_endpoint='{_storage_options.get('client_kwargs',{}).get('endpoint_url', "").replace("http://","")}';
         SET s3_access_key_id='{_storage_options.get('key', "PLEASE INPUT ACCESS KEY")}';
         SET s3_secret_access_key='{_storage_options.get('secret', "PLEASE INPUT SECRET KEY")}';
         SET s3_url_style = 'path';
         SET s3_use_ssl=false;
         {query_str}
         """
-        query = re.sub("DISCOVERY:\d*", self._find_fileID, query)
-        return query
+        return [
+            re.sub("DISCOVERY:\d*", self._find_fileID, query),
+            re.sub("DISCOVERY:\d*", self._find_fileID2, query),
+            re.sub("DISCOVERY:\d*", self._find_fileID3, query)
+        ]
 
     def query(self, query_str):
-        query = self._query(query_str)
-        return duckdb.sql(query).to_df()
+        querys = self._query(query_str)
+        for query in querys:
+            try:
+                output = duckdb.sql(query).to_df()
+            except Exception as e:
+                pass
+            else:
+                return output
+        return pd.DataFrame()
```

### Comparing `dsmlibrary_viz-0.0.2/dsmlibrary_viz.egg-info/PKG-INFO` & `dsmlibrary_viz-0.0.3/dsmlibrary_viz.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsmlibrary-viz
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple way to use Dataset. for dsm
 Home-page: https://github.com/storemesh/dsmlibrary-viz
 Author: DigitalStoreMesh Co.,Ltd
 Author-email: contact@storemesh.com
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dsmlibrary_viz-0.0.2/setup.py` & `dsmlibrary_viz-0.0.3/setup.py`

 * *Files identical despite different names*

