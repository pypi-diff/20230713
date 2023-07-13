# Comparing `tmp/taskbadger-0.6.0.tar.gz` & `tmp/taskbadger-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskbadger-0.6.0.tar", max compression
+gzip compressed data, was "taskbadger-0.6.1.tar", max compression
```

## Comparing `taskbadger-0.6.0.tar` & `taskbadger-0.6.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    11357 2023-07-13 13:29:49.161963 taskbadger-0.6.0/LICENSE
--rw-r--r--   0        0        0     1714 2023-07-13 13:29:49.161963 taskbadger-0.6.0/README.md
--rw-r--r--   0        0        0     1808 2023-07-13 13:29:49.161963 taskbadger-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      482 2023-07-13 13:29:49.161963 taskbadger-0.6.0/taskbadger/__init__.py
--rw-r--r--   0        0        0     5430 2023-07-13 13:29:49.161963 taskbadger-0.6.0/taskbadger/cli.py
--rw-r--r--   0        0        0     3253 2023-07-13 13:29:49.161963 taskbadger-0.6.0/taskbadger/config.py
--rw-r--r--   0        0        0      299 2023-07-13 13:29:49.161963 taskbadger-0.6.0/taskbadger/exceptions.py
--rw-r--r--   0        0        0     2158 2023-07-13 13:29:49.161963 taskbadger-0.6.0/taskbadger/integrations.py
--rw-r--r--   0        0        0      155 2023-07-13 13:29:49.161963 taskbadger-0.6.0/taskbadger/internal/__init__.py
--rw-r--r--   0        0        0       47 2023-07-13 13:29:49.161963 taskbadger-0.6.0/taskbadger/internal/api/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 13:29:49.161963 taskbadger-0.6.0/taskbadger/internal/api/action_endpoints/__init__.py
--rw-r--r--   0        0        0     3318 2023-07-13 13:29:49.161963 taskbadger-0.6.0/taskbadger/internal/api/action_endpoints/action_cancel.py
--rw-r--r--   0        0        0     5393 2023-07-13 13:29:49.161963 taskbadger-0.6.0/taskbadger/internal/api/action_endpoints/action_create.py
--rw-r--r--   0        0        0     5005 2023-07-13 13:29:49.161963 taskbadger-0.6.0/taskbadger/internal/api/action_endpoints/action_get.py
--rw-r--r--   0        0        0     5097 2023-07-13 13:29:49.161963 taskbadger-0.6.0/taskbadger/internal/api/action_endpoints/action_list.py
--rw-r--r--   0        0        0     5676 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/api/action_endpoints/action_partial_update.py
--rw-r--r--   0        0        0     5556 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/api/action_endpoints/action_update.py
--rw-r--r--   0        0        0        0 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/api/task_endpoints/__init__.py
--rw-r--r--   0        0        0     3123 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/api/task_endpoints/task_cancel.py
--rw-r--r--   0        0        0     5770 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/api/task_endpoints/task_create.py
--rw-r--r--   0        0        0     4662 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/api/task_endpoints/task_get.py
--rw-r--r--   0        0        0     5872 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/api/task_endpoints/task_list.py
--rw-r--r--   0        0        0     5359 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/api/task_endpoints/task_partial_update.py
--rw-r--r--   0        0        0     5167 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/api/task_endpoints/task_update.py
--rw-r--r--   0        0        0     2673 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/client.py
--rw-r--r--   0        0        0      282 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/errors.py
--rw-r--r--   0        0        0     1022 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/models/__init__.py
--rw-r--r--   0        0        0     3234 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/models/action.py
--rw-r--r--   0        0        0     1152 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/models/action_config.py
--rw-r--r--   0        0        0     2405 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/models/action_request.py
--rw-r--r--   0        0        0     1190 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/models/action_request_config.py
--rw-r--r--   0        0        0     2590 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/models/paginated_task_list.py
--rw-r--r--   0        0        0     2638 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/models/patched_action_request.py
--rw-r--r--   0        0        0     1228 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/models/patched_action_request_config.py
--rw-r--r--   0        0        0     6107 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/models/patched_task_request.py
--rw-r--r--   0        0        0     1222 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/models/patched_task_request_data.py
--rw-r--r--   0        0        0      339 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/models/status_enum.py
--rw-r--r--   0        0        0     7435 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/models/task.py
--rw-r--r--   0        0        0     1146 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/models/task_data.py
--rw-r--r--   0        0        0     5965 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/models/task_request.py
--rw-r--r--   0        0        0     1184 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/models/task_request_data.py
--rw-r--r--   0        0        0       26 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/py.typed
--rw-r--r--   0        0        0      974 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/types.py
--rw-r--r--   0        0        0     2415 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/process.py
--rw-r--r--   0        0        0     1185 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/safe_sdk.py
--rw-r--r--   0        0        0    10444 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/sdk.py
--rw-r--r--   0        0        0     3129 1970-01-01 00:00:00.000000 taskbadger-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-13 13:56:57.056078 taskbadger-0.6.1/LICENSE
+-rw-r--r--   0        0        0     1714 2023-07-13 13:56:57.056078 taskbadger-0.6.1/README.md
+-rw-r--r--   0        0        0     1808 2023-07-13 13:56:57.056078 taskbadger-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      482 2023-07-13 13:56:57.056078 taskbadger-0.6.1/taskbadger/__init__.py
+-rw-r--r--   0        0        0     5409 2023-07-13 13:56:57.056078 taskbadger-0.6.1/taskbadger/cli.py
+-rw-r--r--   0        0        0     3253 2023-07-13 13:56:57.056078 taskbadger-0.6.1/taskbadger/config.py
+-rw-r--r--   0        0        0      299 2023-07-13 13:56:57.056078 taskbadger-0.6.1/taskbadger/exceptions.py
+-rw-r--r--   0        0        0     2158 2023-07-13 13:56:57.056078 taskbadger-0.6.1/taskbadger/integrations.py
+-rw-r--r--   0        0        0      155 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/__init__.py
+-rw-r--r--   0        0        0       47 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/api/action_endpoints/__init__.py
+-rw-r--r--   0        0        0     3318 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/api/action_endpoints/action_cancel.py
+-rw-r--r--   0        0        0     5393 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/api/action_endpoints/action_create.py
+-rw-r--r--   0        0        0     5005 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/api/action_endpoints/action_get.py
+-rw-r--r--   0        0        0     5097 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/api/action_endpoints/action_list.py
+-rw-r--r--   0        0        0     5676 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/api/action_endpoints/action_partial_update.py
+-rw-r--r--   0        0        0     5556 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/api/action_endpoints/action_update.py
+-rw-r--r--   0        0        0        0 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/api/task_endpoints/__init__.py
+-rw-r--r--   0        0        0     3123 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/api/task_endpoints/task_cancel.py
+-rw-r--r--   0        0        0     5770 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/api/task_endpoints/task_create.py
+-rw-r--r--   0        0        0     4662 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/api/task_endpoints/task_get.py
+-rw-r--r--   0        0        0     5872 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/api/task_endpoints/task_list.py
+-rw-r--r--   0        0        0     5359 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/api/task_endpoints/task_partial_update.py
+-rw-r--r--   0        0        0     5167 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/api/task_endpoints/task_update.py
+-rw-r--r--   0        0        0     2673 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/client.py
+-rw-r--r--   0        0        0      282 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/errors.py
+-rw-r--r--   0        0        0     1022 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/models/__init__.py
+-rw-r--r--   0        0        0     3234 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/models/action.py
+-rw-r--r--   0        0        0     1152 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/models/action_config.py
+-rw-r--r--   0        0        0     2405 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/models/action_request.py
+-rw-r--r--   0        0        0     1190 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/models/action_request_config.py
+-rw-r--r--   0        0        0     2590 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/models/paginated_task_list.py
+-rw-r--r--   0        0        0     2638 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/models/patched_action_request.py
+-rw-r--r--   0        0        0     1228 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/models/patched_action_request_config.py
+-rw-r--r--   0        0        0     6107 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/models/patched_task_request.py
+-rw-r--r--   0        0        0     1222 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/models/patched_task_request_data.py
+-rw-r--r--   0        0        0      339 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/models/status_enum.py
+-rw-r--r--   0        0        0     7435 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/models/task.py
+-rw-r--r--   0        0        0     1146 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/models/task_data.py
+-rw-r--r--   0        0        0     5965 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/models/task_request.py
+-rw-r--r--   0        0        0     1184 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/models/task_request_data.py
+-rw-r--r--   0        0        0       26 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/py.typed
+-rw-r--r--   0        0        0      974 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/internal/types.py
+-rw-r--r--   0        0        0     2415 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/process.py
+-rw-r--r--   0        0        0     1185 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/safe_sdk.py
+-rw-r--r--   0        0        0    10444 2023-07-13 13:56:57.060078 taskbadger-0.6.1/taskbadger/sdk.py
+-rw-r--r--   0        0        0     3129 1970-01-01 00:00:00.000000 taskbadger-0.6.1/PKG-INFO
```

### Comparing `taskbadger-0.6.0/LICENSE` & `taskbadger-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/README.md` & `taskbadger-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/pyproject.toml` & `taskbadger-0.6.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskbadger"
-version = "0.6.0"
+version = "0.6.1"
 description = "The official Python SDK for Task Badger"
 license = "Apache-2.0"
 
 authors = []
 
 readme = "README.md"
 packages = [
```

### Comparing `taskbadger-0.6.0/taskbadger/cli.py` & `taskbadger-0.6.1/taskbadger/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,14 @@
             if key in task_data and value:
                 task_data[key] += value
             elif value:
                 task_data[key] = value
         else:
             task_data[key] = value
 
-    print(task_data)
     try:
         task.update(status=status, data=task_data or None)
     except Exception as e:
         err_console.print(f"Error updating task status: {e}")
 
 
 @app.command()
```

### Comparing `taskbadger-0.6.0/taskbadger/config.py` & `taskbadger-0.6.1/taskbadger/config.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/integrations.py` & `taskbadger-0.6.1/taskbadger/integrations.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/internal/api/action_endpoints/action_cancel.py` & `taskbadger-0.6.1/taskbadger/internal/api/action_endpoints/action_cancel.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/internal/api/action_endpoints/action_create.py` & `taskbadger-0.6.1/taskbadger/internal/api/action_endpoints/action_create.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/internal/api/action_endpoints/action_get.py` & `taskbadger-0.6.1/taskbadger/internal/api/action_endpoints/action_get.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/internal/api/action_endpoints/action_list.py` & `taskbadger-0.6.1/taskbadger/internal/api/action_endpoints/action_list.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/internal/api/action_endpoints/action_partial_update.py` & `taskbadger-0.6.1/taskbadger/internal/api/action_endpoints/action_partial_update.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/internal/api/action_endpoints/action_update.py` & `taskbadger-0.6.1/taskbadger/internal/api/action_endpoints/action_update.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/internal/api/task_endpoints/task_cancel.py` & `taskbadger-0.6.1/taskbadger/internal/api/task_endpoints/task_cancel.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/internal/api/task_endpoints/task_create.py` & `taskbadger-0.6.1/taskbadger/internal/api/task_endpoints/task_create.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/internal/api/task_endpoints/task_get.py` & `taskbadger-0.6.1/taskbadger/internal/api/task_endpoints/task_get.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/internal/api/task_endpoints/task_list.py` & `taskbadger-0.6.1/taskbadger/internal/api/task_endpoints/task_list.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/internal/api/task_endpoints/task_partial_update.py` & `taskbadger-0.6.1/taskbadger/internal/api/task_endpoints/task_partial_update.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/internal/api/task_endpoints/task_update.py` & `taskbadger-0.6.1/taskbadger/internal/api/task_endpoints/task_update.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/internal/client.py` & `taskbadger-0.6.1/taskbadger/internal/client.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/internal/models/__init__.py` & `taskbadger-0.6.1/taskbadger/internal/models/__init__.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/internal/models/action.py` & `taskbadger-0.6.1/taskbadger/internal/models/action.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/internal/models/action_config.py` & `taskbadger-0.6.1/taskbadger/internal/models/action_config.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/internal/models/action_request.py` & `taskbadger-0.6.1/taskbadger/internal/models/action_request.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/internal/models/action_request_config.py` & `taskbadger-0.6.1/taskbadger/internal/models/action_request_config.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/internal/models/paginated_task_list.py` & `taskbadger-0.6.1/taskbadger/internal/models/paginated_task_list.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/internal/models/patched_action_request.py` & `taskbadger-0.6.1/taskbadger/internal/models/patched_action_request.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/internal/models/patched_action_request_config.py` & `taskbadger-0.6.1/taskbadger/internal/models/patched_action_request_config.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/internal/models/patched_task_request.py` & `taskbadger-0.6.1/taskbadger/internal/models/patched_task_request.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/internal/models/patched_task_request_data.py` & `taskbadger-0.6.1/taskbadger/internal/models/patched_task_request_data.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/internal/models/task.py` & `taskbadger-0.6.1/taskbadger/internal/models/task.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/internal/models/task_data.py` & `taskbadger-0.6.1/taskbadger/internal/models/task_data.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/internal/models/task_request.py` & `taskbadger-0.6.1/taskbadger/internal/models/task_request.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/internal/models/task_request_data.py` & `taskbadger-0.6.1/taskbadger/internal/models/task_request_data.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/internal/types.py` & `taskbadger-0.6.1/taskbadger/internal/types.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/process.py` & `taskbadger-0.6.1/taskbadger/process.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/safe_sdk.py` & `taskbadger-0.6.1/taskbadger/safe_sdk.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/taskbadger/sdk.py` & `taskbadger-0.6.1/taskbadger/sdk.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.6.0/PKG-INFO` & `taskbadger-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskbadger
-Version: 0.6.0
+Version: 0.6.1
 Summary: The official Python SDK for Task Badger
 Home-page: https://taskbadger.net/
 License: Apache-2.0
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

