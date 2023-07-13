# Comparing `tmp/ob-metaflow-extensions-1.1.9rc0.tar.gz` & `tmp/ob-metaflow-extensions-1.1.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ob-metaflow-extensions-1.1.9rc0.tar", last modified: Tue Jan 31 01:08:04 2023, max compression
+gzip compressed data, was "ob-metaflow-extensions-1.1.9rc1.tar", last modified: Tue Jan 31 01:53:20 2023, max compression
```

## Comparing `ob-metaflow-extensions-1.1.9rc0.tar` & `ob-metaflow-extensions-1.1.9rc1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 01:08:04.419441 ob-metaflow-extensions-1.1.9rc0/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-01-31 01:08:04.419441 ob-metaflow-extensions-1.1.9rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-01-31 01:07:49.000000 ob-metaflow-extensions-1.1.9rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 01:08:04.411441 ob-metaflow-extensions-1.1.9rc0/metaflow_extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 01:08:04.415441 ob-metaflow-extensions-1.1.9rc0/metaflow_extensions/outerbounds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 01:07:49.000000 ob-metaflow-extensions-1.1.9rc0/metaflow_extensions/outerbounds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 01:08:04.415441 ob-metaflow-extensions-1.1.9rc0/metaflow_extensions/outerbounds/config/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-01-31 01:07:49.000000 ob-metaflow-extensions-1.1.9rc0/metaflow_extensions/outerbounds/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 01:08:04.415441 ob-metaflow-extensions-1.1.9rc0/metaflow_extensions/outerbounds/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-01-31 01:07:49.000000 ob-metaflow-extensions-1.1.9rc0/metaflow_extensions/outerbounds/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-01-31 01:07:49.000000 ob-metaflow-extensions-1.1.9rc0/metaflow_extensions/outerbounds/plugins/auth_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 01:08:04.415441 ob-metaflow-extensions-1.1.9rc0/metaflow_extensions/outerbounds/plugins/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-31 01:07:49.000000 ob-metaflow-extensions-1.1.9rc0/metaflow_extensions/outerbounds/plugins/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-01-31 01:07:49.000000 ob-metaflow-extensions-1.1.9rc0/metaflow_extensions/outerbounds/plugins/kubernetes/kubernetes_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 01:08:04.415441 ob-metaflow-extensions-1.1.9rc0/metaflow_extensions/outerbounds/toplevel/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-01-31 01:07:49.000000 ob-metaflow-extensions-1.1.9rc0/metaflow_extensions/outerbounds/toplevel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 01:08:04.415441 ob-metaflow-extensions-1.1.9rc0/metaflow_extensions/outerbounds/toplevel/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 01:08:04.419441 ob-metaflow-extensions-1.1.9rc0/metaflow_extensions/outerbounds/toplevel/plugins/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-31 01:07:49.000000 ob-metaflow-extensions-1.1.9rc0/metaflow_extensions/outerbounds/toplevel/plugins/kubernetes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 01:08:04.419441 ob-metaflow-extensions-1.1.9rc0/ob_metaflow_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-01-31 01:08:04.000000 ob-metaflow-extensions-1.1.9rc0/ob_metaflow_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-01-31 01:08:04.000000 ob-metaflow-extensions-1.1.9rc0/ob_metaflow_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 01:08:04.000000 ob-metaflow-extensions-1.1.9rc0/ob_metaflow_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-01-31 01:08:04.000000 ob-metaflow-extensions-1.1.9rc0/ob_metaflow_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-31 01:08:04.000000 ob-metaflow-extensions-1.1.9rc0/ob_metaflow_extensions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 01:08:04.419441 ob-metaflow-extensions-1.1.9rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-01-31 01:07:49.000000 ob-metaflow-extensions-1.1.9rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 01:53:20.065642 ob-metaflow-extensions-1.1.9rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-01-31 01:53:20.065642 ob-metaflow-extensions-1.1.9rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-01-31 01:53:09.000000 ob-metaflow-extensions-1.1.9rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 01:53:20.061642 ob-metaflow-extensions-1.1.9rc1/metaflow_extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 01:53:20.065642 ob-metaflow-extensions-1.1.9rc1/metaflow_extensions/outerbounds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 01:53:09.000000 ob-metaflow-extensions-1.1.9rc1/metaflow_extensions/outerbounds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 01:53:20.065642 ob-metaflow-extensions-1.1.9rc1/metaflow_extensions/outerbounds/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-01-31 01:53:09.000000 ob-metaflow-extensions-1.1.9rc1/metaflow_extensions/outerbounds/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 01:53:20.065642 ob-metaflow-extensions-1.1.9rc1/metaflow_extensions/outerbounds/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-01-31 01:53:09.000000 ob-metaflow-extensions-1.1.9rc1/metaflow_extensions/outerbounds/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-01-31 01:53:09.000000 ob-metaflow-extensions-1.1.9rc1/metaflow_extensions/outerbounds/plugins/auth_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 01:53:20.065642 ob-metaflow-extensions-1.1.9rc1/metaflow_extensions/outerbounds/plugins/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-31 01:53:09.000000 ob-metaflow-extensions-1.1.9rc1/metaflow_extensions/outerbounds/plugins/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-01-31 01:53:09.000000 ob-metaflow-extensions-1.1.9rc1/metaflow_extensions/outerbounds/plugins/kubernetes/kubernetes_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 01:53:20.065642 ob-metaflow-extensions-1.1.9rc1/metaflow_extensions/outerbounds/toplevel/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-01-31 01:53:09.000000 ob-metaflow-extensions-1.1.9rc1/metaflow_extensions/outerbounds/toplevel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 01:53:20.065642 ob-metaflow-extensions-1.1.9rc1/metaflow_extensions/outerbounds/toplevel/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 01:53:20.065642 ob-metaflow-extensions-1.1.9rc1/metaflow_extensions/outerbounds/toplevel/plugins/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-31 01:53:09.000000 ob-metaflow-extensions-1.1.9rc1/metaflow_extensions/outerbounds/toplevel/plugins/kubernetes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 01:53:20.065642 ob-metaflow-extensions-1.1.9rc1/ob_metaflow_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-01-31 01:53:19.000000 ob-metaflow-extensions-1.1.9rc1/ob_metaflow_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-01-31 01:53:20.000000 ob-metaflow-extensions-1.1.9rc1/ob_metaflow_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 01:53:19.000000 ob-metaflow-extensions-1.1.9rc1/ob_metaflow_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-01-31 01:53:19.000000 ob-metaflow-extensions-1.1.9rc1/ob_metaflow_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-31 01:53:19.000000 ob-metaflow-extensions-1.1.9rc1/ob_metaflow_extensions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 01:53:20.065642 ob-metaflow-extensions-1.1.9rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-01-31 01:53:09.000000 ob-metaflow-extensions-1.1.9rc1/setup.py
```

### Comparing `ob-metaflow-extensions-1.1.9rc0/metaflow_extensions/outerbounds/plugins/__init__.py` & `ob-metaflow-extensions-1.1.9rc1/metaflow_extensions/outerbounds/plugins/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,8 +52,8 @@
                 return session.client(module, **client_params)
         if with_error:
             return boto3.client(module, **client_params), ClientError
         else:
             return boto3.client(module, **client_params)
 
 
-AWS_CLIENT_PROVIDERS_DESC = [("obp", ".outerbounds.plugins.ObpAuthProvider")]
+AWS_CLIENT_PROVIDERS_DESC = [("obp", ".ObpAuthProvider")]
```

### Comparing `ob-metaflow-extensions-1.1.9rc0/metaflow_extensions/outerbounds/plugins/auth_server.py` & `ob-metaflow-extensions-1.1.9rc1/metaflow_extensions/outerbounds/plugins/auth_server.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-extensions-1.1.9rc0/metaflow_extensions/outerbounds/plugins/kubernetes/kubernetes_client.py` & `ob-metaflow-extensions-1.1.9rc1/metaflow_extensions/outerbounds/plugins/kubernetes/kubernetes_client.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-extensions-1.1.9rc0/ob_metaflow_extensions.egg-info/SOURCES.txt` & `ob-metaflow-extensions-1.1.9rc1/ob_metaflow_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ob-metaflow-extensions-1.1.9rc0/setup.py` & `ob-metaflow-extensions-1.1.9rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 from pathlib import Path
 
 
-version = "1.1.9rc0"
+version = "1.1.9rc1"
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="ob-metaflow-extensions",
     version=version,
     description="Outerbounds Platform Extensions for Metaflow",
```

