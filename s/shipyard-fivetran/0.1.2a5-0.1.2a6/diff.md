# Comparing `tmp/shipyard_fivetran-0.1.2a5.tar.gz` & `tmp/shipyard_fivetran-0.1.2a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_fivetran-0.1.2a5.tar", max compression
+gzip compressed data, was "shipyard_fivetran-0.1.2a6.tar", max compression
```

## Comparing `shipyard_fivetran-0.1.2a5.tar` & `shipyard_fivetran-0.1.2a6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      508 2023-07-12 21:53:42.938315 shipyard_fivetran-0.1.2a5/pyproject.toml
--rw-r--r--   0        0        0       37 2023-06-21 19:54:18.755231 shipyard_fivetran-0.1.2a5/shipyard_fivetran/__init__.py
--rw-r--r--   0        0        0      257 2023-06-21 19:54:18.755602 shipyard_fivetran-0.1.2a5/shipyard_fivetran/cli/authtest.py
--rw-r--r--   0        0        0     3012 2023-07-10 20:44:53.454669 shipyard_fivetran-0.1.2a5/shipyard_fivetran/cli/sync.py
--rw-r--r--   0        0        0     2150 2023-07-10 20:44:53.455303 shipyard_fivetran-0.1.2a5/shipyard_fivetran/cli/update_connector.py
--rw-r--r--   0        0        0     9921 2023-06-21 19:54:18.755987 shipyard_fivetran-0.1.2a5/shipyard_fivetran/fivetran.py
--rw-r--r--   0        0        0      596 1970-01-01 00:00:00.000000 shipyard_fivetran-0.1.2a5/PKG-INFO
+-rw-r--r--   0        0        0      508 2023-07-12 21:56:26.250521 shipyard_fivetran-0.1.2a6/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-06-21 19:54:18.755231 shipyard_fivetran-0.1.2a6/shipyard_fivetran/__init__.py
+-rw-r--r--   0        0        0      257 2023-06-21 19:54:18.755602 shipyard_fivetran-0.1.2a6/shipyard_fivetran/cli/authtest.py
+-rw-r--r--   0        0        0     3012 2023-07-10 20:44:53.454669 shipyard_fivetran-0.1.2a6/shipyard_fivetran/cli/sync.py
+-rw-r--r--   0        0        0     2150 2023-07-10 20:44:53.455303 shipyard_fivetran-0.1.2a6/shipyard_fivetran/cli/update_connector.py
+-rw-r--r--   0        0        0     9921 2023-06-21 19:54:18.755987 shipyard_fivetran-0.1.2a6/shipyard_fivetran/fivetran.py
+-rw-r--r--   0        0        0      596 1970-01-01 00:00:00.000000 shipyard_fivetran-0.1.2a6/PKG-INFO
```

### Comparing `shipyard_fivetran-0.1.2a5/shipyard_fivetran/cli/sync.py` & `shipyard_fivetran-0.1.2a6/shipyard_fivetran/cli/sync.py`

 * *Files identical despite different names*

### Comparing `shipyard_fivetran-0.1.2a5/shipyard_fivetran/cli/update_connector.py` & `shipyard_fivetran-0.1.2a6/shipyard_fivetran/cli/update_connector.py`

 * *Files identical despite different names*

### Comparing `shipyard_fivetran-0.1.2a5/shipyard_fivetran/fivetran.py` & `shipyard_fivetran-0.1.2a6/shipyard_fivetran/fivetran.py`

 * *Files identical despite different names*

### Comparing `shipyard_fivetran-0.1.2a5/PKG-INFO` & `shipyard_fivetran-0.1.2a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: shipyard-fivetran
-Version: 0.1.2a5
+Version: 0.1.2a6
 Summary: A local client for connecting and working with Fivetran
 License: Apache 2.0
 Author: JR
 Author-email: johnathan.rodriguez@shipyardapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pytz (==2023.3)
 Requires-Dist: requests (==2.31.0)
-Requires-Dist: shipyard-templates (==0.1.7)
+Requires-Dist: shipyard-templates (==0.2.0)
```

