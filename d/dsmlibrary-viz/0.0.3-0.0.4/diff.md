# Comparing `tmp/dsmlibrary_viz-0.0.3.tar.gz` & `tmp/dsmlibrary_viz-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsmlibrary_viz-0.0.3.tar", last modified: Thu Jul 13 09:15:23 2023, max compression
+gzip compressed data, was "dsmlibrary_viz-0.0.4.tar", last modified: Thu Jul 13 09:19:24 2023, max compression
```

## Comparing `dsmlibrary_viz-0.0.3.tar` & `dsmlibrary_viz-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-13 09:15:23.989722 dsmlibrary_viz-0.0.3/
--rw-r--r--   0 naii       (501) staff       (20)     1066 2023-07-12 12:08:08.000000 dsmlibrary_viz-0.0.3/LICENSE
--rw-r--r--   0 naii       (501) staff       (20)     1054 2023-07-13 09:15:23.989324 dsmlibrary_viz-0.0.3/PKG-INFO
--rw-r--r--   0 naii       (501) staff       (20)      355 2023-07-12 14:26:15.000000 dsmlibrary_viz-0.0.3/README.md
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-13 09:15:23.986050 dsmlibrary_viz-0.0.3/dsmlibrary_viz/
--rw-r--r--   0 naii       (501) staff       (20)      160 2023-07-13 09:15:09.000000 dsmlibrary_viz-0.0.3/dsmlibrary_viz/__init__.py
--rw-r--r--   0 naii       (501) staff       (20)     2255 2023-07-12 14:14:40.000000 dsmlibrary_viz-0.0.3/dsmlibrary_viz/base.py
--rw-r--r--   0 naii       (501) staff       (20)     2222 2023-07-13 09:14:39.000000 dsmlibrary_viz-0.0.3/dsmlibrary_viz/data_viz.py
--rw-r--r--   0 naii       (501) staff       (20)      619 2023-07-12 15:26:02.000000 dsmlibrary_viz-0.0.3/dsmlibrary_viz/utils.py
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-13 09:15:23.988485 dsmlibrary_viz-0.0.3/dsmlibrary_viz.egg-info/
--rw-r--r--   0 naii       (501) staff       (20)     1054 2023-07-13 09:15:23.000000 dsmlibrary_viz-0.0.3/dsmlibrary_viz.egg-info/PKG-INFO
--rw-r--r--   0 naii       (501) staff       (20)      316 2023-07-13 09:15:23.000000 dsmlibrary_viz-0.0.3/dsmlibrary_viz.egg-info/SOURCES.txt
--rw-r--r--   0 naii       (501) staff       (20)        1 2023-07-13 09:15:23.000000 dsmlibrary_viz-0.0.3/dsmlibrary_viz.egg-info/dependency_links.txt
--rw-r--r--   0 naii       (501) staff       (20)       28 2023-07-13 09:15:23.000000 dsmlibrary_viz-0.0.3/dsmlibrary_viz.egg-info/requires.txt
--rw-r--r--   0 naii       (501) staff       (20)       15 2023-07-13 09:15:23.000000 dsmlibrary_viz-0.0.3/dsmlibrary_viz.egg-info/top_level.txt
--rw-r--r--   0 naii       (501) staff       (20)       38 2023-07-13 09:15:23.989860 dsmlibrary_viz-0.0.3/setup.cfg
--rw-r--r--   0 naii       (501) staff       (20)     1410 2023-07-12 14:24:27.000000 dsmlibrary_viz-0.0.3/setup.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-13 09:19:24.035555 dsmlibrary_viz-0.0.4/
+-rw-r--r--   0 naii       (501) staff       (20)     1066 2023-07-12 12:08:08.000000 dsmlibrary_viz-0.0.4/LICENSE
+-rw-r--r--   0 naii       (501) staff       (20)     1054 2023-07-13 09:19:24.034811 dsmlibrary_viz-0.0.4/PKG-INFO
+-rw-r--r--   0 naii       (501) staff       (20)      355 2023-07-12 14:26:15.000000 dsmlibrary_viz-0.0.4/README.md
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-13 09:19:24.029926 dsmlibrary_viz-0.0.4/dsmlibrary_viz/
+-rw-r--r--   0 naii       (501) staff       (20)      160 2023-07-13 09:19:22.000000 dsmlibrary_viz-0.0.4/dsmlibrary_viz/__init__.py
+-rw-r--r--   0 naii       (501) staff       (20)     2255 2023-07-12 14:14:40.000000 dsmlibrary_viz-0.0.4/dsmlibrary_viz/base.py
+-rw-r--r--   0 naii       (501) staff       (20)     2221 2023-07-13 09:19:09.000000 dsmlibrary_viz-0.0.4/dsmlibrary_viz/data_viz.py
+-rw-r--r--   0 naii       (501) staff       (20)      619 2023-07-12 15:26:02.000000 dsmlibrary_viz-0.0.4/dsmlibrary_viz/utils.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-07-13 09:19:24.033854 dsmlibrary_viz-0.0.4/dsmlibrary_viz.egg-info/
+-rw-r--r--   0 naii       (501) staff       (20)     1054 2023-07-13 09:19:24.000000 dsmlibrary_viz-0.0.4/dsmlibrary_viz.egg-info/PKG-INFO
+-rw-r--r--   0 naii       (501) staff       (20)      316 2023-07-13 09:19:24.000000 dsmlibrary_viz-0.0.4/dsmlibrary_viz.egg-info/SOURCES.txt
+-rw-r--r--   0 naii       (501) staff       (20)        1 2023-07-13 09:19:24.000000 dsmlibrary_viz-0.0.4/dsmlibrary_viz.egg-info/dependency_links.txt
+-rw-r--r--   0 naii       (501) staff       (20)       28 2023-07-13 09:19:24.000000 dsmlibrary_viz-0.0.4/dsmlibrary_viz.egg-info/requires.txt
+-rw-r--r--   0 naii       (501) staff       (20)       15 2023-07-13 09:19:24.000000 dsmlibrary_viz-0.0.4/dsmlibrary_viz.egg-info/top_level.txt
+-rw-r--r--   0 naii       (501) staff       (20)       38 2023-07-13 09:19:24.035728 dsmlibrary_viz-0.0.4/setup.cfg
+-rw-r--r--   0 naii       (501) staff       (20)     1410 2023-07-12 14:24:27.000000 dsmlibrary_viz-0.0.4/setup.py
```

### Comparing `dsmlibrary_viz-0.0.3/LICENSE` & `dsmlibrary_viz-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dsmlibrary_viz-0.0.3/PKG-INFO` & `dsmlibrary_viz-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsmlibrary_viz
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple way to use Dataset. for dsm
 Home-page: https://github.com/storemesh/dsmlibrary-viz
 Author: DigitalStoreMesh Co.,Ltd
 Author-email: contact@storemesh.com
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dsmlibrary_viz-0.0.3/dsmlibrary_viz/base.py` & `dsmlibrary_viz-0.0.4/dsmlibrary_viz/base.py`

 * *Files identical despite different names*

### Comparing `dsmlibrary_viz-0.0.3/dsmlibrary_viz/data_viz.py` & `dsmlibrary_viz-0.0.4/dsmlibrary_viz/data_viz.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         return f"s3://dataplatform/{osd_key}/*/*.parquet"
     
     def _find_fileID3(self, match):
         match = match.group()
         _file_id = match.split(':')[-1]
         meta = self.get_meta_file(file_id=_file_id)
         osd_key = meta.get('s3_key')
-        return f"s3://dataplatform/{osd_key}/*/*/*.parquet",
+        return f"s3://dataplatform/{osd_key}/*/*/*.parquet"
 
 
     def _query(self, query_str):
         _storage_options = self._storage_options
         query = f"""
         load 'httpfs';
         SET s3_endpoint='{_storage_options.get('client_kwargs',{}).get('endpoint_url', "").replace("http://","")}';
```

### Comparing `dsmlibrary_viz-0.0.3/dsmlibrary_viz/utils.py` & `dsmlibrary_viz-0.0.4/dsmlibrary_viz/utils.py`

 * *Files identical despite different names*

### Comparing `dsmlibrary_viz-0.0.3/dsmlibrary_viz.egg-info/PKG-INFO` & `dsmlibrary_viz-0.0.4/dsmlibrary_viz.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsmlibrary-viz
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple way to use Dataset. for dsm
 Home-page: https://github.com/storemesh/dsmlibrary-viz
 Author: DigitalStoreMesh Co.,Ltd
 Author-email: contact@storemesh.com
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dsmlibrary_viz-0.0.3/setup.py` & `dsmlibrary_viz-0.0.4/setup.py`

 * *Files identical despite different names*

