# Comparing `tmp/capsulecorp-0.1.2.tar.gz` & `tmp/capsulecorp-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capsulecorp-0.1.2.tar", last modified: Wed Jul 12 13:54:57 2023, max compression
+gzip compressed data, was "capsulecorp-0.1.3.tar", last modified: Thu Jul 13 16:38:13 2023, max compression
```

## Comparing `capsulecorp-0.1.2.tar` & `capsulecorp-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-12 13:54:57.441418 capsulecorp-0.1.2/
--rw-r--r--   0 daless383   (502) staff       (20)    11357 2023-02-13 20:25:15.000000 capsulecorp-0.1.2/LICENSE
--rw-r--r--   0 daless383   (502) staff       (20)      461 2023-07-12 13:54:57.440772 capsulecorp-0.1.2/PKG-INFO
--rw-r--r--   0 daless383   (502) staff       (20)       99 2023-02-13 20:25:15.000000 capsulecorp-0.1.2/README.md
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-12 13:54:57.429823 capsulecorp-0.1.2/capsulecorp/
--rw-r--r--   0 daless383   (502) staff       (20)       63 2023-02-14 15:14:02.000000 capsulecorp-0.1.2/capsulecorp/__init__.py
--rw-r--r--   0 daless383   (502) staff       (20)     7967 2023-05-04 16:53:29.000000 capsulecorp-0.1.2/capsulecorp/query_driver.py
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-12 13:54:57.439509 capsulecorp-0.1.2/capsulecorp/utilities/
--rw-r--r--   0 daless383   (502) staff       (20)        0 2023-07-10 14:36:34.000000 capsulecorp-0.1.2/capsulecorp/utilities/__init__.py
--rw-r--r--   0 daless383   (502) staff       (20)     5882 2023-07-10 18:54:59.000000 capsulecorp-0.1.2/capsulecorp/utilities/databricks_utils.py
--rw-r--r--   0 daless383   (502) staff       (20)     1441 2023-07-10 20:48:28.000000 capsulecorp-0.1.2/capsulecorp/utilities/github_utils.py
--rw-r--r--   0 daless383   (502) staff       (20)     2320 2023-05-18 14:36:49.000000 capsulecorp-0.1.2/capsulecorp/utilities/slack_utils.py
--rw-r--r--   0 daless383   (502) staff       (20)    14740 2023-07-06 17:37:40.000000 capsulecorp-0.1.2/capsulecorp/utils.py
--rw-r--r--   0 daless383   (502) staff       (20)      269 2023-07-12 13:53:46.000000 capsulecorp-0.1.2/capsulecorp/version.py
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-12 13:54:57.434827 capsulecorp-0.1.2/capsulecorp.egg-info/
--rw-r--r--   0 daless383   (502) staff       (20)      461 2023-07-12 13:54:56.000000 capsulecorp-0.1.2/capsulecorp.egg-info/PKG-INFO
--rw-r--r--   0 daless383   (502) staff       (20)      462 2023-07-12 13:54:57.000000 capsulecorp-0.1.2/capsulecorp.egg-info/SOURCES.txt
--rw-r--r--   0 daless383   (502) staff       (20)        1 2023-07-12 13:54:56.000000 capsulecorp-0.1.2/capsulecorp.egg-info/dependency_links.txt
--rw-r--r--   0 daless383   (502) staff       (20)      106 2023-07-12 13:54:57.000000 capsulecorp-0.1.2/capsulecorp.egg-info/requires.txt
--rw-r--r--   0 daless383   (502) staff       (20)       12 2023-07-12 13:54:57.000000 capsulecorp-0.1.2/capsulecorp.egg-info/top_level.txt
--rw-r--r--   0 daless383   (502) staff       (20)       86 2023-02-14 15:04:49.000000 capsulecorp-0.1.2/pyproject.toml
--rw-r--r--   0 daless383   (502) staff       (20)       38 2023-07-12 13:54:57.441630 capsulecorp-0.1.2/setup.cfg
--rw-r--r--   0 daless383   (502) staff       (20)     6621 2023-07-12 13:53:07.000000 capsulecorp-0.1.2/setup.py
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-13 16:38:13.389714 capsulecorp-0.1.3/
+-rw-r--r--   0 daless383   (502) staff       (20)    11357 2023-02-13 20:25:15.000000 capsulecorp-0.1.3/LICENSE
+-rw-r--r--   0 daless383   (502) staff       (20)      461 2023-07-13 16:38:13.388980 capsulecorp-0.1.3/PKG-INFO
+-rw-r--r--   0 daless383   (502) staff       (20)       99 2023-02-13 20:25:15.000000 capsulecorp-0.1.3/README.md
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-13 16:38:13.374502 capsulecorp-0.1.3/capsulecorp/
+-rw-r--r--   0 daless383   (502) staff       (20)       63 2023-02-14 15:14:02.000000 capsulecorp-0.1.3/capsulecorp/__init__.py
+-rw-r--r--   0 daless383   (502) staff       (20)     7967 2023-05-04 16:53:29.000000 capsulecorp-0.1.3/capsulecorp/query_driver.py
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-13 16:38:13.387205 capsulecorp-0.1.3/capsulecorp/utilities/
+-rw-r--r--   0 daless383   (502) staff       (20)        0 2023-07-13 15:20:45.000000 capsulecorp-0.1.3/capsulecorp/utilities/__init__.py
+-rw-r--r--   0 daless383   (502) staff       (20)     7717 2023-07-13 16:29:38.000000 capsulecorp-0.1.3/capsulecorp/utilities/databricks_utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)     1441 2023-07-10 20:48:28.000000 capsulecorp-0.1.3/capsulecorp/utilities/github_utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)     2320 2023-05-18 14:36:49.000000 capsulecorp-0.1.3/capsulecorp/utilities/slack_utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)    14740 2023-07-06 17:37:40.000000 capsulecorp-0.1.3/capsulecorp/utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)      269 2023-07-13 14:23:27.000000 capsulecorp-0.1.3/capsulecorp/version.py
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-13 16:38:13.380462 capsulecorp-0.1.3/capsulecorp.egg-info/
+-rw-r--r--   0 daless383   (502) staff       (20)      461 2023-07-13 16:38:12.000000 capsulecorp-0.1.3/capsulecorp.egg-info/PKG-INFO
+-rw-r--r--   0 daless383   (502) staff       (20)      462 2023-07-13 16:38:13.000000 capsulecorp-0.1.3/capsulecorp.egg-info/SOURCES.txt
+-rw-r--r--   0 daless383   (502) staff       (20)        1 2023-07-13 16:38:12.000000 capsulecorp-0.1.3/capsulecorp.egg-info/dependency_links.txt
+-rw-r--r--   0 daless383   (502) staff       (20)      106 2023-07-13 16:38:13.000000 capsulecorp-0.1.3/capsulecorp.egg-info/requires.txt
+-rw-r--r--   0 daless383   (502) staff       (20)       12 2023-07-13 16:38:13.000000 capsulecorp-0.1.3/capsulecorp.egg-info/top_level.txt
+-rw-r--r--   0 daless383   (502) staff       (20)       86 2023-02-14 15:04:49.000000 capsulecorp-0.1.3/pyproject.toml
+-rw-r--r--   0 daless383   (502) staff       (20)       38 2023-07-13 16:38:13.390142 capsulecorp-0.1.3/setup.cfg
+-rw-r--r--   0 daless383   (502) staff       (20)     6621 2023-07-12 13:53:07.000000 capsulecorp-0.1.3/setup.py
```

### Comparing `capsulecorp-0.1.2/LICENSE` & `capsulecorp-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.2/capsulecorp/query_driver.py` & `capsulecorp-0.1.3/capsulecorp/query_driver.py`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.2/capsulecorp/utilities/databricks_utils.py` & `capsulecorp-0.1.3/capsulecorp/utilities/databricks_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -182,7 +182,58 @@
     databricks_client = ApiClient(host=host, token=token, verify=True)
     workspace_service = WorkspaceService(databricks_client)
     # Import the source code as the new DataBricks notebook
     workspace_service.import_workspace(
         notebook_path, "SOURCE", "PYTHON", source_code, True)
 
     return
+
+
+def does_dir_exist(host, token, user, notebook_path):
+    """
+        This method will determine whether the directory in a notebook path
+        exists.
+
+        Args:
+            host (str): URL of DataBricks workspace
+            token (str): DataBricks API token
+            user (str): databricks user path
+            notebook_path (str): location of notebook
+
+        Returns:
+            boolean
+    """
+    # Parse the directory name from the full notebook path
+    dir_name = os.path.dirname(notebook_path.split(user)[1])
+    # Initialize DataBricks API Client and Workspace API
+    databricks_client = ApiClient(host=host, token=token, verify=True)
+    workspace_service = WorkspaceService(databricks_client)
+    # Grab the workspace objects for the provided user
+    workspace_objects = workspace_service.list(user)
+    # Return a boolean for whether the directory exists iin the workspace
+    return any([
+        user + dir_name == i["path"]
+        for i in workspace_objects["objects"]
+        if i["object_type"] == "DIRECTORY"])
+
+
+def make_dir(host, token, user, notebook_path):
+    """
+        This method will make a databricks directory given user and notebook
+        path information.
+
+        Args:
+            host (str): URL of DataBricks workspace
+            token (str): DataBricks API token
+            user (str): databricks user path
+            notebook_path (str): location of notebook
+
+        Returns:
+
+    """
+    # Parse the directory name from the full notebook path
+    dir_name = os.path.dirname(notebook_path.split(user)[1])
+    # Initialize DataBricks API Client and Workspace API
+    databricks_client = ApiClient(host=host, token=token, verify=True)
+    workspace_service = WorkspaceService(databricks_client)
+    # Make the directory
+    return workspace_service.mkdirs(user + dir_name)
```

### Comparing `capsulecorp-0.1.2/capsulecorp/utilities/github_utils.py` & `capsulecorp-0.1.3/capsulecorp/utilities/github_utils.py`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.2/capsulecorp/utilities/slack_utils.py` & `capsulecorp-0.1.3/capsulecorp/utilities/slack_utils.py`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.2/capsulecorp/utils.py` & `capsulecorp-0.1.3/capsulecorp/utils.py`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.2/setup.py` & `capsulecorp-0.1.3/setup.py`

 * *Files identical despite different names*

