# Comparing `tmp/fair_cli-0.9.1.tar.gz` & `tmp/fair_cli-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fair_cli-0.9.1.tar", max compression
+gzip compressed data, was "fair_cli-0.9.2.tar", max compression
```

## Comparing `fair_cli-0.9.1.tar` & `fair_cli-0.9.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1855 2023-06-21 19:13:33.324048 fair_cli-0.9.1/CHANGELOG.md
--rw-r--r--   0        0        0     1358 2023-07-12 10:02:05.198104 fair_cli-0.9.1/CITATION.cff
--rw-r--r--   0        0        0     1314 2023-06-12 13:03:22.463351 fair_cli-0.9.1/LICENSE
--rw-r--r--   0        0        0    11363 2023-06-21 19:13:33.324484 fair_cli-0.9.1/README.md
--rw-r--r--   0        0        0     1976 2023-06-12 13:03:22.464552 fair_cli-0.9.1/fair/__init__.py
--rw-r--r--   0        0        0    23763 2023-07-12 09:43:39.260687 fair_cli-0.9.1/fair/cli.py
--rw-r--r--   0        0        0     9447 2023-07-11 16:34:34.113605 fair_cli-0.9.1/fair/common.py
--rw-r--r--   0        0        0    30704 2023-07-11 16:34:34.113863 fair_cli-0.9.1/fair/configuration/__init__.py
--rw-r--r--   0        0        0     3450 2023-07-08 08:05:57.895747 fair_cli-0.9.1/fair/configuration/validation.py
--rw-r--r--   0        0        0     5358 2023-06-21 19:13:33.327099 fair_cli-0.9.1/fair/exceptions.py
--rw-r--r--   0        0        0    10127 2023-06-21 19:13:33.327168 fair_cli-0.9.1/fair/files.txt
--rw-r--r--   0        0        0     4773 2023-07-11 16:34:34.114027 fair_cli-0.9.1/fair/history.py
--rw-r--r--   0        0        0     6506 2023-07-11 14:54:18.134530 fair_cli-0.9.1/fair/identifiers.py
--rw-r--r--   0        0        0     3035 2023-07-11 16:34:34.114175 fair_cli-0.9.1/fair/logging.py
--rw-r--r--   0        0        0    11136 2023-07-11 14:54:18.134725 fair_cli-0.9.1/fair/register.py
--rw-r--r--   0        0        0      161 2023-06-21 19:13:33.327663 fair_cli-0.9.1/fair/registry/__init__.py
--rw-r--r--   0        0        0     1249 2023-06-12 13:03:22.465501 fair_cli-0.9.1/fair/registry/file_formats.json
--rw-r--r--   0        0        0      138 2023-07-11 16:34:34.114333 fair_cli-0.9.1/fair/registry/file_types.py
--rw-r--r--   0        0        0    18004 2023-07-11 16:34:34.114556 fair_cli-0.9.1/fair/registry/requests.py
--rw-r--r--   0        0        0    15020 2023-07-11 16:34:34.114766 fair_cli-0.9.1/fair/registry/server.py
--rw-r--r--   0        0        0    24284 2023-07-11 16:34:34.115007 fair_cli-0.9.1/fair/registry/storage.py
--rw-r--r--   0        0        0    42144 2023-07-11 20:37:03.466251 fair_cli-0.9.1/fair/registry/sync.py
--rw-r--r--   0        0        0     4752 2023-06-21 19:13:33.329007 fair_cli-0.9.1/fair/registry/versioning.py
--rw-r--r--   0        0        0     2302 2023-06-21 19:13:33.329217 fair_cli-0.9.1/fair/run.py
--rw-r--r--   0        0        0    58739 2023-07-12 09:43:39.261073 fair_cli-0.9.1/fair/session.py
--rw-r--r--   0        0        0    16498 2023-07-11 16:34:34.115607 fair_cli-0.9.1/fair/staging.py
--rw-r--r--   0        0        0      526 2023-07-11 16:34:34.115767 fair_cli-0.9.1/fair/templates/__init__.py
--rw-r--r--   0        0        0      296 2023-06-12 13:03:22.466514 fair_cli-0.9.1/fair/templates/config.jinja
--rw-r--r--   0        0        0      136 2023-06-12 13:03:22.466556 fair_cli-0.9.1/fair/templates/hist.jinja
--rw-r--r--   0        0        0     3244 2023-07-11 16:34:34.115922 fair_cli-0.9.1/fair/testing.py
--rw-r--r--   0        0        0    54257 2023-07-12 10:02:05.198485 fair_cli-0.9.1/fair/user_config/__init__.py
--rw-r--r--   0        0        0     4830 2023-06-21 19:13:33.330469 fair_cli-0.9.1/fair/user_config/globbing.py
--rw-r--r--   0        0        0     9205 2023-07-11 16:34:34.116474 fair_cli-0.9.1/fair/user_config/validation.py
--rw-r--r--   0        0        0     5087 2023-06-21 19:13:33.330678 fair_cli-0.9.1/fair/utilities.py
--rw-r--r--   0        0        0     1465 2023-06-21 19:13:33.330742 fair_cli-0.9.1/fair/virtualenv.py
--rw-r--r--   0        0        0     2496 2023-07-12 10:02:05.198667 fair_cli-0.9.1/pyproject.toml
--rw-r--r--   0        0        0    13295 1970-01-01 00:00:00.000000 fair_cli-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1855 2023-06-21 19:13:33.324048 fair_cli-0.9.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1358 2023-07-12 22:46:38.902397 fair_cli-0.9.2/CITATION.cff
+-rw-r--r--   0        0        0     1314 2023-06-12 13:03:22.463351 fair_cli-0.9.2/LICENSE
+-rw-r--r--   0        0        0    11363 2023-06-21 19:13:33.324484 fair_cli-0.9.2/README.md
+-rw-r--r--   0        0        0     1976 2023-06-12 13:03:22.464552 fair_cli-0.9.2/fair/__init__.py
+-rw-r--r--   0        0        0    23763 2023-07-12 09:43:39.260687 fair_cli-0.9.2/fair/cli.py
+-rw-r--r--   0        0        0     9447 2023-07-11 16:34:34.113605 fair_cli-0.9.2/fair/common.py
+-rw-r--r--   0        0        0    30704 2023-07-11 16:34:34.113863 fair_cli-0.9.2/fair/configuration/__init__.py
+-rw-r--r--   0        0        0     3450 2023-07-08 08:05:57.895747 fair_cli-0.9.2/fair/configuration/validation.py
+-rw-r--r--   0        0        0     5358 2023-06-21 19:13:33.327099 fair_cli-0.9.2/fair/exceptions.py
+-rw-r--r--   0        0        0    10127 2023-06-21 19:13:33.327168 fair_cli-0.9.2/fair/files.txt
+-rw-r--r--   0        0        0     4773 2023-07-11 16:34:34.114027 fair_cli-0.9.2/fair/history.py
+-rw-r--r--   0        0        0     6506 2023-07-11 14:54:18.134530 fair_cli-0.9.2/fair/identifiers.py
+-rw-r--r--   0        0        0     3035 2023-07-11 16:34:34.114175 fair_cli-0.9.2/fair/logging.py
+-rw-r--r--   0        0        0    11136 2023-07-11 14:54:18.134725 fair_cli-0.9.2/fair/register.py
+-rw-r--r--   0        0        0      161 2023-06-21 19:13:33.327663 fair_cli-0.9.2/fair/registry/__init__.py
+-rw-r--r--   0        0        0     1249 2023-06-12 13:03:22.465501 fair_cli-0.9.2/fair/registry/file_formats.json
+-rw-r--r--   0        0        0      138 2023-07-11 16:34:34.114333 fair_cli-0.9.2/fair/registry/file_types.py
+-rw-r--r--   0        0        0    18004 2023-07-11 16:34:34.114556 fair_cli-0.9.2/fair/registry/requests.py
+-rw-r--r--   0        0        0    15020 2023-07-11 16:34:34.114766 fair_cli-0.9.2/fair/registry/server.py
+-rw-r--r--   0        0        0    24284 2023-07-11 16:34:34.115007 fair_cli-0.9.2/fair/registry/storage.py
+-rw-r--r--   0        0        0    42144 2023-07-11 20:37:03.466251 fair_cli-0.9.2/fair/registry/sync.py
+-rw-r--r--   0        0        0     4752 2023-06-21 19:13:33.329007 fair_cli-0.9.2/fair/registry/versioning.py
+-rw-r--r--   0        0        0     2302 2023-06-21 19:13:33.329217 fair_cli-0.9.2/fair/run.py
+-rw-r--r--   0        0        0    58740 2023-07-12 22:46:38.903146 fair_cli-0.9.2/fair/session.py
+-rw-r--r--   0        0        0    16498 2023-07-11 16:34:34.115607 fair_cli-0.9.2/fair/staging.py
+-rw-r--r--   0        0        0      526 2023-07-11 16:34:34.115767 fair_cli-0.9.2/fair/templates/__init__.py
+-rw-r--r--   0        0        0      296 2023-06-12 13:03:22.466514 fair_cli-0.9.2/fair/templates/config.jinja
+-rw-r--r--   0        0        0      136 2023-06-12 13:03:22.466556 fair_cli-0.9.2/fair/templates/hist.jinja
+-rw-r--r--   0        0        0     3244 2023-07-11 16:34:34.115922 fair_cli-0.9.2/fair/testing.py
+-rw-r--r--   0        0        0    54257 2023-07-12 10:02:05.198485 fair_cli-0.9.2/fair/user_config/__init__.py
+-rw-r--r--   0        0        0     4830 2023-06-21 19:13:33.330469 fair_cli-0.9.2/fair/user_config/globbing.py
+-rw-r--r--   0        0        0     9205 2023-07-11 16:34:34.116474 fair_cli-0.9.2/fair/user_config/validation.py
+-rw-r--r--   0        0        0     5087 2023-06-21 19:13:33.330678 fair_cli-0.9.2/fair/utilities.py
+-rw-r--r--   0        0        0     1465 2023-06-21 19:13:33.330742 fair_cli-0.9.2/fair/virtualenv.py
+-rw-r--r--   0        0        0     2496 2023-07-12 22:46:38.903604 fair_cli-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0    13295 1970-01-01 00:00:00.000000 fair_cli-0.9.2/PKG-INFO
```

### Comparing `fair_cli-0.9.1/CHANGELOG.md` & `fair_cli-0.9.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `fair_cli-0.9.1/CITATION.cff` & `fair_cli-0.9.2/CITATION.cff`

 * *Files 0% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 - FAIR
 - Data Management
 - Provenance
 license: BSD-2-Clause
 message: If you use this software, please cite it using these metadata.
 repository-code: https://github.com/FAIRDataPipeline/FAIR-CLI/
 title: "The FAIR Data Pipeline command line tool"
-version: 0.9.1
+version: 0.9.2
```

### Comparing `fair_cli-0.9.1/LICENSE` & `fair_cli-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fair_cli-0.9.1/README.md` & `fair_cli-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `fair_cli-0.9.1/fair/__init__.py` & `fair_cli-0.9.2/fair/__init__.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.9.1/fair/cli.py` & `fair_cli-0.9.2/fair/cli.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.9.1/fair/common.py` & `fair_cli-0.9.2/fair/common.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.9.1/fair/configuration/__init__.py` & `fair_cli-0.9.2/fair/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.9.1/fair/configuration/validation.py` & `fair_cli-0.9.2/fair/configuration/validation.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.9.1/fair/exceptions.py` & `fair_cli-0.9.2/fair/exceptions.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.9.1/fair/files.txt` & `fair_cli-0.9.2/fair/files.txt`

 * *Files identical despite different names*

### Comparing `fair_cli-0.9.1/fair/history.py` & `fair_cli-0.9.2/fair/history.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.9.1/fair/identifiers.py` & `fair_cli-0.9.2/fair/identifiers.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.9.1/fair/logging.py` & `fair_cli-0.9.2/fair/logging.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.9.1/fair/register.py` & `fair_cli-0.9.2/fair/register.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.9.1/fair/registry/file_formats.json` & `fair_cli-0.9.2/fair/registry/file_formats.json`

 * *Files identical despite different names*

### Comparing `fair_cli-0.9.1/fair/registry/requests.py` & `fair_cli-0.9.2/fair/registry/requests.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.9.1/fair/registry/server.py` & `fair_cli-0.9.2/fair/registry/server.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.9.1/fair/registry/storage.py` & `fair_cli-0.9.2/fair/registry/storage.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.9.1/fair/registry/sync.py` & `fair_cli-0.9.2/fair/registry/sync.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.9.1/fair/registry/versioning.py` & `fair_cli-0.9.2/fair/registry/versioning.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.9.1/fair/run.py` & `fair_cli-0.9.2/fair/run.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.9.1/fair/session.py` & `fair_cli-0.9.2/fair/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1450,15 +1450,15 @@
                         if _storage_location:
                             _storage_root_url = _storage_location["storage_root"]
                             _storage_location_path = _storage_location["path"]
                             _storage_root = fdp_req.url_get(_storage_root_url, _token)
                             if _storage_root:
                                 _root = _storage_root["root"]
                                 if "file://" in _root:
-                                    click.echo(f"Data Product: {data_product} is located {_root}{os.pathsep}{_storage_location_path}")
+                                    click.echo(f"Data Product: {data_product} is located {_root}{os.path.sep}{_storage_location_path}")
                                 else:
                                     click.echo(f"Data Product: {data_product} is located {_root}/{_storage_location_path}")
             else:
                 click.echo(f"Data Product {data_product} could not be found on {_registry}")
         else:
             click.echo(f"Namespace {namespace} not found on {_registry}")
```

### Comparing `fair_cli-0.9.1/fair/staging.py` & `fair_cli-0.9.2/fair/staging.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.9.1/fair/templates/__init__.py` & `fair_cli-0.9.2/fair/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.9.1/fair/testing.py` & `fair_cli-0.9.2/fair/testing.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.9.1/fair/user_config/__init__.py` & `fair_cli-0.9.2/fair/user_config/__init__.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.9.1/fair/user_config/globbing.py` & `fair_cli-0.9.2/fair/user_config/globbing.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.9.1/fair/user_config/validation.py` & `fair_cli-0.9.2/fair/user_config/validation.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.9.1/fair/utilities.py` & `fair_cli-0.9.2/fair/utilities.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.9.1/fair/virtualenv.py` & `fair_cli-0.9.2/fair/virtualenv.py`

 * *Files identical despite different names*

### Comparing `fair_cli-0.9.1/pyproject.toml` & `fair_cli-0.9.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   "Environment :: Console",
   "Operating System :: POSIX :: Linux",
   "Operating System :: MacOS",
   "Operating System :: OS Independent",
 ]
 description = "Synchronization interface for the SCRC FAIR Data Pipeline registry"
 name = "fair-cli"
-version = "0.9.1"
+version = "0.9.2"
 
 homepage = "https://www.fairdatapipeline.org/"
 
 repository = "https://github.com/FAIRDataPipeline/FAIR-CLI"
 
 documentation = "https://www.fairdatapipeline.org/docs/interface/fdp/"
```

### Comparing `fair_cli-0.9.1/PKG-INFO` & `fair_cli-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair-cli
-Version: 0.9.1
+Version: 0.9.2
 Summary: Synchronization interface for the SCRC FAIR Data Pipeline registry
 Home-page: https://www.fairdatapipeline.org/
 License: BSD-2-Clause
 Keywords: FAIR Data Pipeline,FAIR,Data Management,Provenance
 Author: Richard Reeve
 Author-email: richard.reeve@glasgow.ac.uk
 Requires-Python: >=3.8.0,<4.0.0
```

