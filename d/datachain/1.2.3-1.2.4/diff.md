# Comparing `tmp/datachain-1.2.3.tar.gz` & `tmp/datachain-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datachain-1.2.3.tar", max compression
+gzip compressed data, was "datachain-1.2.4.tar", max compression
```

## Comparing `datachain-1.2.3.tar` & `datachain-1.2.4.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0    35060 2023-03-26 22:49:34.715348 datachain-1.2.3/LICENSE
--rw-r--r--   0        0        0        0 2023-03-26 22:49:34.715403 datachain-1.2.3/README.md
--rw-r--r--   0        0        0      187 2023-03-27 10:55:56.699305 datachain-1.2.3/datachain/__init__.py
--rw-r--r--   0        0        0      120 2023-06-01 01:19:09.359858 datachain-1.2.3/datachain/config/__init__.py
--rw-r--r--   0        0        0     2749 2023-07-05 12:28:32.475128 datachain-1.2.3/datachain/config/logging.py
--rw-r--r--   0        0        0      752 2023-07-05 12:28:32.475276 datachain-1.2.3/datachain/config/params.py
--rw-r--r--   0        0        0       32 2023-03-26 22:49:34.715707 datachain-1.2.3/datachain/core/__init__.py
--rw-r--r--   0        0        0    19005 2023-07-05 12:32:35.621608 datachain-1.2.3/datachain/core/common.py
--rw-r--r--   0        0        0     3044 2023-03-27 10:29:58.237300 datachain-1.2.3/datachain/core/lazy.py
--rw-r--r--   0        0        0     2243 2023-03-31 01:27:20.943629 datachain-1.2.3/datachain/core/sync.py
--rw-r--r--   0        0        0      479 2023-07-05 12:28:32.475949 datachain-1.2.3/datachain/sources/__init__.py
--rw-r--r--   0        0        0     3919 2023-07-05 12:28:32.476031 datachain-1.2.3/datachain/sources/_utils.py
--rw-r--r--   0        0        0       32 2023-07-05 12:28:32.476123 datachain-1.2.3/datachain/sources/bytes/__init__.py
--rw-r--r--   0        0        0     1338 2023-07-05 12:28:32.476184 datachain-1.2.3/datachain/sources/bytes/_pandas.py
--rw-r--r--   0        0        0      816 2023-07-05 12:28:32.476234 datachain-1.2.3/datachain/sources/file.py
--rw-r--r--   0        0        0       32 2023-07-05 12:28:32.476296 datachain-1.2.3/datachain/sources/files/__init__.py
--rw-r--r--   0        0        0     1038 2023-07-05 12:28:32.476354 datachain-1.2.3/datachain/sources/files/_file.py
--rw-r--r--   0        0        0     1135 2023-07-05 12:28:32.476414 datachain-1.2.3/datachain/sources/files/_ftp.py
--rw-r--r--   0        0        0      859 2023-07-05 12:28:32.476467 datachain-1.2.3/datachain/sources/files/_http.py
--rw-r--r--   0        0        0      624 2023-07-05 12:28:32.476517 datachain-1.2.3/datachain/sources/files/_jsonfile.py
--rw-r--r--   0        0        0      442 2023-07-05 12:28:32.476571 datachain-1.2.3/datachain/sources/files/_local.py
--rw-r--r--   0        0        0     2825 2023-07-05 12:28:32.476628 datachain-1.2.3/datachain/sources/files/_pandas.py
--rw-r--r--   0        0        0     1281 2023-07-05 12:28:32.476685 datachain-1.2.3/datachain/sources/files/_sftp.py
--rw-r--r--   0        0        0     1232 2023-07-05 12:28:32.476753 datachain-1.2.3/datachain/sources/ftp.py
--rw-r--r--   0        0        0     1847 2023-07-05 12:28:32.476807 datachain-1.2.3/datachain/sources/http.py
--rw-r--r--   0        0        0       32 2023-07-05 12:28:32.476886 datachain-1.2.3/datachain/sources/query/__init__.py
--rw-r--r--   0        0        0     3050 2023-07-10 09:51:33.411623 datachain-1.2.3/datachain/sources/query/_pandas.py
--rw-r--r--   0        0        0     1348 2023-07-05 12:28:32.476989 datachain-1.2.3/datachain/sources/sftp.py
--rw-r--r--   0        0        0     2139 2023-07-05 12:28:32.477051 datachain-1.2.3/datachain/sources/sharepoint.py
--rw-r--r--   0        0        0     2473 2023-07-05 12:28:32.477107 datachain-1.2.3/datachain/sources/sql.py
--rw-r--r--   0        0        0      353 2023-07-05 12:28:32.477181 datachain-1.2.3/datachain/sources/utils/__init__.py
--rw-r--r--   0        0        0     2241 2023-07-05 12:28:32.477233 datachain-1.2.3/datachain/sources/utils/_column.py
--rw-r--r--   0        0        0     4577 2023-07-05 12:28:32.477292 datachain-1.2.3/datachain/sources/utils/_dataframe.py
--rw-r--r--   0        0        0      410 2023-07-05 12:28:32.477347 datachain-1.2.3/datachain/sources/utils/_func.py
--rw-r--r--   0        0        0      567 2023-07-05 12:28:32.477401 datachain-1.2.3/datachain/sources/utils/utils.py
--rw-r--r--   0        0        0      617 2023-03-28 17:59:32.602567 datachain-1.2.3/datachain/utils/func.py
--rw-r--r--   0        0        0     2019 2023-07-10 09:52:02.809513 datachain-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     2005 1970-01-01 00:00:00.000000 datachain-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0    35060 2023-05-23 08:21:28.841649 datachain-1.2.4/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-23 08:21:28.841716 datachain-1.2.4/README.md
+-rw-r--r--   0        0        0      187 2023-06-13 09:20:37.750539 datachain-1.2.4/datachain/__init__.py
+-rw-r--r--   0        0        0      120 2023-06-01 00:25:14.448453 datachain-1.2.4/datachain/config/__init__.py
+-rw-r--r--   0        0        0     2749 2023-06-06 13:28:01.504285 datachain-1.2.4/datachain/config/logging.py
+-rw-r--r--   0        0        0      752 2023-06-01 03:30:25.805131 datachain-1.2.4/datachain/config/params.py
+-rw-r--r--   0        0        0       32 2023-05-23 08:21:28.842314 datachain-1.2.4/datachain/core/__init__.py
+-rw-r--r--   0        0        0    19033 2023-07-13 10:21:21.395837 datachain-1.2.4/datachain/core/common.py
+-rw-r--r--   0        0        0     3044 2023-05-23 08:21:28.842591 datachain-1.2.4/datachain/core/lazy.py
+-rw-r--r--   0        0        0     2243 2023-05-23 08:21:28.842704 datachain-1.2.4/datachain/core/sync.py
+-rw-r--r--   0        0        0      479 2023-06-13 09:20:30.929115 datachain-1.2.4/datachain/sources/__init__.py
+-rw-r--r--   0        0        0     3994 2023-07-13 08:14:37.048344 datachain-1.2.4/datachain/sources/_utils.py
+-rw-r--r--   0        0        0       32 2023-05-31 14:27:33.000000 datachain-1.2.4/datachain/sources/bytes/__init__.py
+-rw-r--r--   0        0        0     1338 2023-06-06 08:42:46.052456 datachain-1.2.4/datachain/sources/bytes/_pandas.py
+-rw-r--r--   0        0        0      816 2023-06-06 08:22:54.813123 datachain-1.2.4/datachain/sources/file.py
+-rw-r--r--   0        0        0       32 2023-06-01 00:28:56.000000 datachain-1.2.4/datachain/sources/files/__init__.py
+-rw-r--r--   0        0        0     1038 2023-06-06 10:10:23.465279 datachain-1.2.4/datachain/sources/files/_file.py
+-rw-r--r--   0        0        0     1135 2023-06-06 10:15:30.554275 datachain-1.2.4/datachain/sources/files/_ftp.py
+-rw-r--r--   0        0        0      859 2023-06-06 08:39:33.394438 datachain-1.2.4/datachain/sources/files/_http.py
+-rw-r--r--   0        0        0      624 2023-06-06 08:22:54.828168 datachain-1.2.4/datachain/sources/files/_jsonfile.py
+-rw-r--r--   0        0        0      442 2023-03-31 02:13:33.000000 datachain-1.2.4/datachain/sources/files/_local.py
+-rw-r--r--   0        0        0     2825 2023-06-06 09:42:09.908877 datachain-1.2.4/datachain/sources/files/_pandas.py
+-rw-r--r--   0        0        0     1281 2023-06-06 08:45:42.480612 datachain-1.2.4/datachain/sources/files/_sftp.py
+-rw-r--r--   0        0        0     1232 2023-06-06 08:22:54.812738 datachain-1.2.4/datachain/sources/ftp.py
+-rw-r--r--   0        0        0     1847 2023-06-06 10:10:48.078320 datachain-1.2.4/datachain/sources/http.py
+-rw-r--r--   0        0        0       32 2023-05-31 12:23:56.000000 datachain-1.2.4/datachain/sources/query/__init__.py
+-rw-r--r--   0        0        0     3050 2023-07-13 08:14:37.041607 datachain-1.2.4/datachain/sources/query/_pandas.py
+-rw-r--r--   0        0        0     1348 2023-06-06 08:44:01.909822 datachain-1.2.4/datachain/sources/sftp.py
+-rw-r--r--   0        0        0     2139 2023-06-07 08:18:06.637078 datachain-1.2.4/datachain/sources/sharepoint.py
+-rw-r--r--   0        0        0     2473 2023-06-06 08:22:54.813016 datachain-1.2.4/datachain/sources/sql.py
+-rw-r--r--   0        0        0      353 2023-06-06 08:09:47.500631 datachain-1.2.4/datachain/sources/utils/__init__.py
+-rw-r--r--   0        0        0     2241 2023-06-06 08:12:04.292242 datachain-1.2.4/datachain/sources/utils/_column.py
+-rw-r--r--   0        0        0     4577 2023-06-06 08:12:39.732515 datachain-1.2.4/datachain/sources/utils/_dataframe.py
+-rw-r--r--   0        0        0      410 2023-02-06 12:21:00.337713 datachain-1.2.4/datachain/sources/utils/_func.py
+-rw-r--r--   0        0        0      567 2023-06-06 08:23:42.203847 datachain-1.2.4/datachain/sources/utils/utils.py
+-rw-r--r--   0        0        0      617 2023-05-23 08:21:28.842996 datachain-1.2.4/datachain/utils/func.py
+-rw-r--r--   0        0        0     2019 2023-07-13 10:21:58.314602 datachain-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1788 1970-01-01 00:00:00.000000 datachain-1.2.4/setup.py
+-rw-r--r--   0        0        0     1990 1970-01-01 00:00:00.000000 datachain-1.2.4/PKG-INFO
```

### Comparing `datachain-1.2.3/LICENSE` & `datachain-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `datachain-1.2.3/datachain/config/logging.py` & `datachain-1.2.4/datachain/config/logging.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.3/datachain/config/params.py` & `datachain-1.2.4/datachain/config/params.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.3/datachain/core/common.py` & `datachain-1.2.4/datachain/core/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """@Author: Rayane AMROUCHE
 
 Common classes.
 """
 
 from __future__ import annotations
 
+import copy
 import json
 import uuid
 import inspect
 
 try:
     from IPython.display import display  # type: ignore
 except ImportError:
@@ -404,15 +405,15 @@
             **kwds (Any): Keyword arguments for the extractor.
 
         Returns:
             Any: The arguments to pass to the extractor function.
         """
         if key is not None:
             try:
-                params = Params.config.copy()[key]
+                params = copy.deepcopy(Params.config)[key]
             except KeyError as _:
                 params = {}
         else:
             params = {}
         params.update(kwds)
         extractor_func = getattr(extractor, "func", extractor)
         sign = inspect.signature(extractor_func).bind(*args, **params)
@@ -458,15 +459,15 @@
             **kwds (Any): Keyword arguments for the extractor.
 
         Returns:
             Any: The original data.
         """
         if key is not None:
             try:
-                params = Params.config.copy()[key]
+                params = copy.deepcopy(Params.config)[key]
             except KeyError as _:
                 params = {}
         else:
             params = {}
         params.update(kwds)
         loader_func = getattr(loader, "func", loader)
         sign = inspect.signature(_transform).bind(self, loader_func, args, params)
```

### Comparing `datachain-1.2.3/datachain/core/lazy.py` & `datachain-1.2.4/datachain/core/lazy.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.3/datachain/core/sync.py` & `datachain-1.2.4/datachain/core/sync.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.3/datachain/sources/_utils.py` & `datachain-1.2.4/datachain/sources/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,16 +108,17 @@
 
     Args:
         kwds (dict): keyword arguments dict.
 
     Returns:
         Tuple[dict, dict]: request params, non-request params.
     """
-    read_file_params = {}
-    for param in kwds.items():
+    whole_dict = kwds.copy()
+    read_file_params = kwds.copy()
+    for param in whole_dict.keys():
         if param in [
             "params",
             "data",
             "headers",
             "cookies",
             "files",
             "auth",
@@ -125,17 +126,20 @@
             "allow_redirects",
             "proxies",
             "hooks",
             "stream",
             "verify",
             "cert",
             "json",
+            "request_type"
         ]:
-            read_file_params[param] = kwds[param]
             del kwds[param]
+        else:
+            del read_file_params[param]
+
     return read_file_params, kwds
 
 
 def missing_lib(m_lib: str, m_source: str):
     """_summary_
 
     Args:
```

### Comparing `datachain-1.2.3/datachain/sources/bytes/_pandas.py` & `datachain-1.2.4/datachain/sources/bytes/_pandas.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.3/datachain/sources/file.py` & `datachain-1.2.4/datachain/sources/file.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.3/datachain/sources/files/_file.py` & `datachain-1.2.4/datachain/sources/files/_file.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.3/datachain/sources/files/_ftp.py` & `datachain-1.2.4/datachain/sources/files/_ftp.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.3/datachain/sources/files/_http.py` & `datachain-1.2.4/datachain/sources/files/_http.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.3/datachain/sources/files/_jsonfile.py` & `datachain-1.2.4/datachain/sources/files/_jsonfile.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.3/datachain/sources/files/_pandas.py` & `datachain-1.2.4/datachain/sources/files/_pandas.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.3/datachain/sources/files/_sftp.py` & `datachain-1.2.4/datachain/sources/files/_sftp.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.3/datachain/sources/ftp.py` & `datachain-1.2.4/datachain/sources/ftp.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.3/datachain/sources/http.py` & `datachain-1.2.4/datachain/sources/http.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.3/datachain/sources/query/_pandas.py` & `datachain-1.2.4/datachain/sources/query/_pandas.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.3/datachain/sources/sftp.py` & `datachain-1.2.4/datachain/sources/sftp.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.3/datachain/sources/sharepoint.py` & `datachain-1.2.4/datachain/sources/sharepoint.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.3/datachain/sources/sql.py` & `datachain-1.2.4/datachain/sources/sql.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.3/datachain/sources/utils/_column.py` & `datachain-1.2.4/datachain/sources/utils/_column.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.3/datachain/sources/utils/_dataframe.py` & `datachain-1.2.4/datachain/sources/utils/_dataframe.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.3/datachain/sources/utils/utils.py` & `datachain-1.2.4/datachain/sources/utils/utils.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.3/datachain/utils/func.py` & `datachain-1.2.4/datachain/utils/func.py`

 * *Files identical despite different names*

### Comparing `datachain-1.2.3/pyproject.toml` & `datachain-1.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datachain"
-version = "1.2.3"
+version = "1.2.4"
 description = "Tools to build data pipelines."
 authors = ["Rayane AMROUCHE <rayaneamrouche@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 packages = [{ include = "datachain" }, { include = "datachain/**/*.py" }]
```

### Comparing `datachain-1.2.3/PKG-INFO` & `datachain-1.2.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datachain
-Version: 1.2.3
+Version: 1.2.4
 Summary: Tools to build data pipelines.
 License: GPL-3.0-or-later
 Author: Rayane AMROUCHE
 Author-email: rayaneamrouche@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -18,25 +18,25 @@
 Provides-Extra: mysql
 Provides-Extra: pgsql
 Provides-Extra: salesforce
 Provides-Extra: sftp
 Provides-Extra: sharepoint
 Provides-Extra: snowflake
 Provides-Extra: tabular
-Requires-Dist: azure-common (>=1.1.28,<2.0.0) ; extra == "sharepoint"
-Requires-Dist: azure-storage-blob (>=12.14.1,<13.0.0) ; extra == "sharepoint"
-Requires-Dist: azure-storage-common (>=2.1.0,<3.0.0) ; extra == "sharepoint"
-Requires-Dist: cryptography (==38.0.4) ; extra == "snowflake"
-Requires-Dist: mysqlclient (>=2.1.1,<3.0.0) ; extra == "mysql"
-Requires-Dist: pandas (>=1.0.0,<2.0.0) ; extra == "tabular"
-Requires-Dist: paramiko (>=3.2.0,<4.0.0) ; extra == "sftp"
-Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0) ; extra == "pgsql"
-Requires-Dist: python-dotenv (>=1.0.0,<2.0.0) ; extra == "sharepoint" or extra == "salesforce" or extra == "mysql" or extra == "pgsql" or extra == "kaggle" or extra == "sftp" or extra == "ftp"
-Requires-Dist: requests (>=2.31.0,<3.0.0) ; extra == "http"
-Requires-Dist: shareplum (>=0.5.1,<0.6.0) ; extra == "sharepoint"
-Requires-Dist: simple-salesforce (>=1.12.2,<2.0.0) ; extra == "salesforce"
-Requires-Dist: snowflake-connector-python (>=2.9.0,<3.0.0) ; extra == "snowflake"
-Requires-Dist: snowflake-sqlalchemy (>=1.4.4,<2.0.0) ; extra == "snowflake"
-Requires-Dist: sqlalchemy (==1.4.46) ; extra == "snowflake" or extra == "mysql" or extra == "pgsql"
+Requires-Dist: azure-common (>=1.1.28,<2.0.0); extra == "sharepoint"
+Requires-Dist: azure-storage-blob (>=12.14.1,<13.0.0); extra == "sharepoint"
+Requires-Dist: azure-storage-common (>=2.1.0,<3.0.0); extra == "sharepoint"
+Requires-Dist: cryptography (==38.0.4); extra == "snowflake"
+Requires-Dist: mysqlclient (>=2.1.1,<3.0.0); extra == "mysql"
+Requires-Dist: pandas (>=1.0.0,<2.0.0); extra == "tabular"
+Requires-Dist: paramiko (>=3.2.0,<4.0.0); extra == "sftp"
+Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0); extra == "pgsql"
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0); extra == "sharepoint" or extra == "salesforce" or extra == "mysql" or extra == "pgsql" or extra == "kaggle" or extra == "sftp" or extra == "ftp"
+Requires-Dist: requests (>=2.31.0,<3.0.0); extra == "http"
+Requires-Dist: shareplum (>=0.5.1,<0.6.0); extra == "sharepoint"
+Requires-Dist: simple-salesforce (>=1.12.2,<2.0.0); extra == "salesforce"
+Requires-Dist: snowflake-connector-python (>=2.9.0,<3.0.0); extra == "snowflake"
+Requires-Dist: snowflake-sqlalchemy (>=1.4.4,<2.0.0); extra == "snowflake"
+Requires-Dist: sqlalchemy (==1.4.46); extra == "snowflake" or extra == "mysql" or extra == "pgsql"
 Description-Content-Type: text/markdown
```

