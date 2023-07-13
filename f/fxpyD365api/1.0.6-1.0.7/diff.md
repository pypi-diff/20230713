# Comparing `tmp/fxpyD365api-1.0.6.tar.gz` & `tmp/fxpyD365api-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fxpyD365api-1.0.6.tar", last modified: Fri Mar 17 09:48:53 2023, max compression
+gzip compressed data, was "dist/fxpyD365api-1.0.7.tar", last modified: Thu Jul 13 07:51:12 2023, max compression
```

## Comparing `fxpyD365api-1.0.6.tar` & `fxpyD365api-1.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 yz         (501) staff       (20)        0 2023-03-17 09:48:53.000000 fxpyD365api-1.0.6/
--rw-r--r--   0 yz         (501) staff       (20)      545 2023-03-17 09:48:53.000000 fxpyD365api-1.0.6/PKG-INFO
-drwxr-xr-x   0 yz         (501) staff       (20)        0 2023-03-17 09:48:53.000000 fxpyD365api-1.0.6/fxpyD365api.egg-info/
--rw-r--r--   0 yz         (501) staff       (20)      545 2023-03-17 09:48:52.000000 fxpyD365api-1.0.6/fxpyD365api.egg-info/PKG-INFO
--rw-r--r--   0 yz         (501) staff       (20)        1 2021-06-15 06:53:32.000000 fxpyD365api-1.0.6/fxpyD365api.egg-info/not-zip-safe
--rw-r--r--   0 yz         (501) staff       (20)      250 2023-03-17 09:48:52.000000 fxpyD365api-1.0.6/fxpyD365api.egg-info/SOURCES.txt
--rw-r--r--   0 yz         (501) staff       (20)       14 2023-03-17 09:48:52.000000 fxpyD365api-1.0.6/fxpyD365api.egg-info/requires.txt
--rw-r--r--   0 yz         (501) staff       (20)       12 2023-03-17 09:48:52.000000 fxpyD365api-1.0.6/fxpyD365api.egg-info/top_level.txt
--rw-r--r--   0 yz         (501) staff       (20)        1 2023-03-17 09:48:52.000000 fxpyD365api-1.0.6/fxpyD365api.egg-info/dependency_links.txt
--rw-r--r--   0 yz         (501) staff       (20)       13 2021-03-29 06:33:22.000000 fxpyD365api-1.0.6/README.md
--rw-r--r--   0 yz         (501) staff       (20)      896 2021-06-14 13:33:01.000000 fxpyD365api-1.0.6/setup.py
--rw-r--r--   0 yz         (501) staff       (20)       38 2023-03-17 09:48:53.000000 fxpyD365api-1.0.6/setup.cfg
-drwxr-xr-x   0 yz         (501) staff       (20)        0 2023-03-17 09:48:53.000000 fxpyD365api-1.0.6/fxpyD365api/
--rw-r--r--   0 yz         (501) staff       (20)     9345 2023-03-17 09:48:30.000000 fxpyD365api-1.0.6/fxpyD365api/__init__.py
+drwxr-xr-x   0 yz         (501) staff       (20)        0 2023-07-13 07:51:12.000000 fxpyD365api-1.0.7/
+-rw-r--r--   0 yz         (501) staff       (20)      545 2023-07-13 07:51:12.000000 fxpyD365api-1.0.7/PKG-INFO
+drwxr-xr-x   0 yz         (501) staff       (20)        0 2023-07-13 07:51:12.000000 fxpyD365api-1.0.7/fxpyD365api.egg-info/
+-rw-r--r--   0 yz         (501) staff       (20)      545 2023-07-13 07:51:12.000000 fxpyD365api-1.0.7/fxpyD365api.egg-info/PKG-INFO
+-rw-r--r--   0 yz         (501) staff       (20)        1 2021-06-15 06:53:32.000000 fxpyD365api-1.0.7/fxpyD365api.egg-info/not-zip-safe
+-rw-r--r--   0 yz         (501) staff       (20)      250 2023-07-13 07:51:12.000000 fxpyD365api-1.0.7/fxpyD365api.egg-info/SOURCES.txt
+-rw-r--r--   0 yz         (501) staff       (20)       14 2023-07-13 07:51:12.000000 fxpyD365api-1.0.7/fxpyD365api.egg-info/requires.txt
+-rw-r--r--   0 yz         (501) staff       (20)       12 2023-07-13 07:51:12.000000 fxpyD365api-1.0.7/fxpyD365api.egg-info/top_level.txt
+-rw-r--r--   0 yz         (501) staff       (20)        1 2023-07-13 07:51:12.000000 fxpyD365api-1.0.7/fxpyD365api.egg-info/dependency_links.txt
+-rw-r--r--   0 yz         (501) staff       (20)       13 2021-03-29 06:33:22.000000 fxpyD365api-1.0.7/README.md
+-rw-r--r--   0 yz         (501) staff       (20)      896 2021-06-14 13:33:01.000000 fxpyD365api-1.0.7/setup.py
+-rw-r--r--   0 yz         (501) staff       (20)       38 2023-07-13 07:51:12.000000 fxpyD365api-1.0.7/setup.cfg
+drwxr-xr-x   0 yz         (501) staff       (20)        0 2023-07-13 07:51:12.000000 fxpyD365api-1.0.7/fxpyD365api/
+-rw-r--r--   0 yz         (501) staff       (20)     9345 2023-07-13 07:50:23.000000 fxpyD365api-1.0.7/fxpyD365api/__init__.py
```

### Comparing `fxpyD365api-1.0.6/PKG-INFO` & `fxpyD365api-1.0.7/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: fxpyD365api
-Version: 1.0.6
+Version: 1.0.7
 Summary: Wrapper classes for working with Dynamics 365 web API entities.
 Home-page: https://github.com/flexitdev/fxpyD365api
 Author: Flexit developers
 Author-email: westma@flexit.no
 License: BSD
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `fxpyD365api-1.0.6/fxpyD365api.egg-info/PKG-INFO` & `fxpyD365api-1.0.7/fxpyD365api.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: fxpyD365api
-Version: 1.0.6
+Version: 1.0.7
 Summary: Wrapper classes for working with Dynamics 365 web API entities.
 Home-page: https://github.com/flexitdev/fxpyD365api
 Author: Flexit developers
 Author-email: westma@flexit.no
 License: BSD
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `fxpyD365api-1.0.6/setup.py` & `fxpyD365api-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `fxpyD365api-1.0.6/fxpyD365api/__init__.py` & `fxpyD365api-1.0.7/fxpyD365api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,15 @@
         :param annotations: string, e.g. "*", will include all annotations for related objects
         :return: response object
         """
         headers = self.headers.copy()
         headers.update({'Prefer': 'return=representation'})
         if annotations:
             headers = self._update_prefer_header(headers, 'odata.include-annotations', f'"{annotations}"')
-        return requests.post(self.api_url, headers=headers, json=json.dumps(data))
+        return requests.post(self.api_url, headers=headers, data=json.dumps(data))
 
     def retrieve(self, entity_id, select=None, annotations=None, query_dict=None):
         params = {}
         if select:
             params['$select'] = select
         if query_dict:
             params.update(query_dict)
```

