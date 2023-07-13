# Comparing `tmp/idbadapter-1.8.tar.gz` & `tmp/idbadapter-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idbadapter-1.8.tar", last modified: Wed Jul 12 15:18:52 2023, max compression
+gzip compressed data, was "idbadapter-1.9.tar", last modified: Thu Jul 13 10:57:44 2023, max compression
```

## Comparing `idbadapter-1.8.tar` & `idbadapter-1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 15:18:52.375835 idbadapter-1.8/
--rw-rw-rw-   0        0        0    11558 2023-06-20 07:34:13.000000 idbadapter-1.8/LICENSE
--rw-rw-rw-   0        0        0      695 2023-07-12 15:18:52.375835 idbadapter-1.8/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-06-20 07:34:13.000000 idbadapter-1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 15:18:52.341720 idbadapter-1.8/idbadapter/
--rw-rw-rw-   0        0        0       61 2023-06-20 07:34:13.000000 idbadapter-1.8/idbadapter/__init__.py
--rw-rw-rw-   0        0        0    12044 2023-07-12 15:10:41.000000 idbadapter-1.8/idbadapter/schedule_loader.py
-drwxrwxrwx   0        0        0        0 2023-07-12 15:18:52.368811 idbadapter-1.8/idbadapter.egg-info/
--rw-rw-rw-   0        0        0      695 2023-07-12 15:18:52.000000 idbadapter-1.8/idbadapter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-07-12 15:18:52.000000 idbadapter-1.8/idbadapter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 15:18:52.000000 idbadapter-1.8/idbadapter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-12 15:18:52.000000 idbadapter-1.8/idbadapter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-12 15:18:52.000000 idbadapter-1.8/idbadapter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 15:18:52.379847 idbadapter-1.8/setup.cfg
--rw-rw-rw-   0        0        0      987 2023-07-12 15:18:49.000000 idbadapter-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 10:57:44.647962 idbadapter-1.9/
+-rw-rw-rw-   0        0        0    11558 2023-06-20 07:34:13.000000 idbadapter-1.9/LICENSE
+-rw-rw-rw-   0        0        0      695 2023-07-13 10:57:44.648967 idbadapter-1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-06-20 07:34:13.000000 idbadapter-1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 10:57:44.617864 idbadapter-1.9/idbadapter/
+-rw-rw-rw-   0        0        0       61 2023-06-20 07:34:13.000000 idbadapter-1.9/idbadapter/__init__.py
+-rw-rw-rw-   0        0        0    12028 2023-07-13 10:56:58.000000 idbadapter-1.9/idbadapter/schedule_loader.py
+drwxrwxrwx   0        0        0        0 2023-07-13 10:57:44.646959 idbadapter-1.9/idbadapter.egg-info/
+-rw-rw-rw-   0        0        0      695 2023-07-13 10:57:44.000000 idbadapter-1.9/idbadapter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-07-13 10:57:44.000000 idbadapter-1.9/idbadapter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 10:57:44.000000 idbadapter-1.9/idbadapter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-13 10:57:44.000000 idbadapter-1.9/idbadapter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-13 10:57:44.000000 idbadapter-1.9/idbadapter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 10:57:44.651978 idbadapter-1.9/setup.cfg
+-rw-rw-rw-   0        0        0      987 2023-07-13 10:57:42.000000 idbadapter-1.9/setup.py
```

### Comparing `idbadapter-1.8/LICENSE` & `idbadapter-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `idbadapter-1.8/PKG-INFO` & `idbadapter-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 1.8
+Version: 1.9
 Summary: Сache module for batch loading of data
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-1.8/idbadapter/schedule_loader.py` & `idbadapter-1.9/idbadapter/schedule_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         }
         if res_type not in queries:
             raise ValueError(f"Incorrect work_type argument. {res_type}")
         
         data = json.dumps({"body": queries[res_type]})        
         response = self.session.post(urljoin(self.url, "query/select"), data=data)
         
-        return [k[0] for k in response.json()]
+        return response.json()
         
     def get_works_names(self, work_type=GRANULARY):
         query = f"SELECT DISTINCT name FROM {work_type['table']}"
         df = self._execute_query(query)
         return df
     
     def _get_works_ids_by_names(self, work_name_list):
```

### Comparing `idbadapter-1.8/idbadapter.egg-info/PKG-INFO` & `idbadapter-1.9/idbadapter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 1.8
+Version: 1.9
 Summary: Сache module for batch loading of data
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-1.8/setup.py` & `idbadapter-1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 
 from distutils.core import setup
 
-version = '1.8'
+version = '1.9'
 
 long_description = "Сache module for batch loading of data"
 
 setup(name='idbadapter',
-      version='1.8',
+      version='1.9',
       description='Сache module for batch loading of data',
       long_description=long_description,
       url="https://github.com/AnatolyPershinov/gpn_cache_module",
       download_url='https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip',
       author='Anatoly Pershinov',
       author_email='anatoliypershinov@gmail.com',
       packages=['idbadapter'],
```

