# Comparing `tmp/taskbadger-0.5.0.tar.gz` & `tmp/taskbadger-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskbadger-0.5.0.tar", max compression
+gzip compressed data, was "taskbadger-0.6.0.tar", max compression
```

## Comparing `taskbadger-0.5.0.tar` & `taskbadger-0.6.0.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0    11357 2023-06-01 14:47:47.951661 taskbadger-0.5.0/LICENSE
--rw-r--r--   0        0        0     1716 2023-06-01 14:47:47.951661 taskbadger-0.5.0/README.md
--rw-r--r--   0        0        0     1808 2023-06-01 14:47:47.955661 taskbadger-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      482 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/__init__.py
--rw-r--r--   0        0        0     5153 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/cli.py
--rw-r--r--   0        0        0     3253 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/config.py
--rw-r--r--   0        0        0      299 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/exceptions.py
--rw-r--r--   0        0        0     2158 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/integrations.py
--rw-r--r--   0        0        0      155 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/__init__.py
--rw-r--r--   0        0        0       47 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/api/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/api/action_endpoints/__init__.py
--rw-r--r--   0        0        0     3318 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/api/action_endpoints/action_cancel.py
--rw-r--r--   0        0        0     5393 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/api/action_endpoints/action_create.py
--rw-r--r--   0        0        0     5005 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/api/action_endpoints/action_get.py
--rw-r--r--   0        0        0     5097 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/api/action_endpoints/action_list.py
--rw-r--r--   0        0        0     5676 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/api/action_endpoints/action_partial_update.py
--rw-r--r--   0        0        0     5556 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/api/action_endpoints/action_update.py
--rw-r--r--   0        0        0        0 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/api/task_endpoints/__init__.py
--rw-r--r--   0        0        0     3123 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/api/task_endpoints/task_cancel.py
--rw-r--r--   0        0        0     5770 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/api/task_endpoints/task_create.py
--rw-r--r--   0        0        0     4662 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/api/task_endpoints/task_get.py
--rw-r--r--   0        0        0     5872 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/api/task_endpoints/task_list.py
--rw-r--r--   0        0        0     5359 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/api/task_endpoints/task_partial_update.py
--rw-r--r--   0        0        0     5167 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/api/task_endpoints/task_update.py
--rw-r--r--   0        0        0     2673 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/client.py
--rw-r--r--   0        0        0      282 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/errors.py
--rw-r--r--   0        0        0     1022 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/models/__init__.py
--rw-r--r--   0        0        0     3234 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/models/action.py
--rw-r--r--   0        0        0     1152 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/models/action_config.py
--rw-r--r--   0        0        0     2405 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/models/action_request.py
--rw-r--r--   0        0        0     1190 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/models/action_request_config.py
--rw-r--r--   0        0        0     2590 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/models/paginated_task_list.py
--rw-r--r--   0        0        0     2638 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/models/patched_action_request.py
--rw-r--r--   0        0        0     1228 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/models/patched_action_request_config.py
--rw-r--r--   0        0        0     6107 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/models/patched_task_request.py
--rw-r--r--   0        0        0     1222 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/models/patched_task_request_data.py
--rw-r--r--   0        0        0      339 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/models/status_enum.py
--rw-r--r--   0        0        0     7435 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/models/task.py
--rw-r--r--   0        0        0     1146 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/models/task_data.py
--rw-r--r--   0        0        0     5965 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/models/task_request.py
--rw-r--r--   0        0        0     1184 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/models/task_request_data.py
--rw-r--r--   0        0        0       26 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/py.typed
--rw-r--r--   0        0        0      974 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/internal/types.py
--rw-r--r--   0        0        0     1185 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/safe_sdk.py
--rw-r--r--   0        0        0    10444 2023-06-01 14:47:47.955661 taskbadger-0.5.0/taskbadger/sdk.py
--rw-r--r--   0        0        0     3131 1970-01-01 00:00:00.000000 taskbadger-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-13 13:29:49.161963 taskbadger-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1714 2023-07-13 13:29:49.161963 taskbadger-0.6.0/README.md
+-rw-r--r--   0        0        0     1808 2023-07-13 13:29:49.161963 taskbadger-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      482 2023-07-13 13:29:49.161963 taskbadger-0.6.0/taskbadger/__init__.py
+-rw-r--r--   0        0        0     5430 2023-07-13 13:29:49.161963 taskbadger-0.6.0/taskbadger/cli.py
+-rw-r--r--   0        0        0     3253 2023-07-13 13:29:49.161963 taskbadger-0.6.0/taskbadger/config.py
+-rw-r--r--   0        0        0      299 2023-07-13 13:29:49.161963 taskbadger-0.6.0/taskbadger/exceptions.py
+-rw-r--r--   0        0        0     2158 2023-07-13 13:29:49.161963 taskbadger-0.6.0/taskbadger/integrations.py
+-rw-r--r--   0        0        0      155 2023-07-13 13:29:49.161963 taskbadger-0.6.0/taskbadger/internal/__init__.py
+-rw-r--r--   0        0        0       47 2023-07-13 13:29:49.161963 taskbadger-0.6.0/taskbadger/internal/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 13:29:49.161963 taskbadger-0.6.0/taskbadger/internal/api/action_endpoints/__init__.py
+-rw-r--r--   0        0        0     3318 2023-07-13 13:29:49.161963 taskbadger-0.6.0/taskbadger/internal/api/action_endpoints/action_cancel.py
+-rw-r--r--   0        0        0     5393 2023-07-13 13:29:49.161963 taskbadger-0.6.0/taskbadger/internal/api/action_endpoints/action_create.py
+-rw-r--r--   0        0        0     5005 2023-07-13 13:29:49.161963 taskbadger-0.6.0/taskbadger/internal/api/action_endpoints/action_get.py
+-rw-r--r--   0        0        0     5097 2023-07-13 13:29:49.161963 taskbadger-0.6.0/taskbadger/internal/api/action_endpoints/action_list.py
+-rw-r--r--   0        0        0     5676 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/api/action_endpoints/action_partial_update.py
+-rw-r--r--   0        0        0     5556 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/api/action_endpoints/action_update.py
+-rw-r--r--   0        0        0        0 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/api/task_endpoints/__init__.py
+-rw-r--r--   0        0        0     3123 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/api/task_endpoints/task_cancel.py
+-rw-r--r--   0        0        0     5770 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/api/task_endpoints/task_create.py
+-rw-r--r--   0        0        0     4662 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/api/task_endpoints/task_get.py
+-rw-r--r--   0        0        0     5872 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/api/task_endpoints/task_list.py
+-rw-r--r--   0        0        0     5359 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/api/task_endpoints/task_partial_update.py
+-rw-r--r--   0        0        0     5167 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/api/task_endpoints/task_update.py
+-rw-r--r--   0        0        0     2673 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/client.py
+-rw-r--r--   0        0        0      282 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/errors.py
+-rw-r--r--   0        0        0     1022 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/models/__init__.py
+-rw-r--r--   0        0        0     3234 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/models/action.py
+-rw-r--r--   0        0        0     1152 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/models/action_config.py
+-rw-r--r--   0        0        0     2405 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/models/action_request.py
+-rw-r--r--   0        0        0     1190 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/models/action_request_config.py
+-rw-r--r--   0        0        0     2590 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/models/paginated_task_list.py
+-rw-r--r--   0        0        0     2638 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/models/patched_action_request.py
+-rw-r--r--   0        0        0     1228 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/models/patched_action_request_config.py
+-rw-r--r--   0        0        0     6107 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/models/patched_task_request.py
+-rw-r--r--   0        0        0     1222 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/models/patched_task_request_data.py
+-rw-r--r--   0        0        0      339 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/models/status_enum.py
+-rw-r--r--   0        0        0     7435 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/models/task.py
+-rw-r--r--   0        0        0     1146 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/models/task_data.py
+-rw-r--r--   0        0        0     5965 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/models/task_request.py
+-rw-r--r--   0        0        0     1184 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/models/task_request_data.py
+-rw-r--r--   0        0        0       26 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/py.typed
+-rw-r--r--   0        0        0      974 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/internal/types.py
+-rw-r--r--   0        0        0     2415 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/process.py
+-rw-r--r--   0        0        0     1185 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/safe_sdk.py
+-rw-r--r--   0        0        0    10444 2023-07-13 13:29:49.165963 taskbadger-0.6.0/taskbadger/sdk.py
+-rw-r--r--   0        0        0     3129 1970-01-01 00:00:00.000000 taskbadger-0.6.0/PKG-INFO
```

### Comparing `taskbadger-0.5.0/LICENSE` & `taskbadger-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/README.md` & `taskbadger-0.6.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -79,11 +79,11 @@
 ```
 
 #### Usage Examples
 
 The CLI `run` command executes your command whilst creating and updating a Task Badger task.
 
 ```shell
-$ taskbadger run "demo task" --action "error email to:me@test.com" -- path/to/script.sh
+$ taskbadger run "demo task" --action error email to:me@test.com -- path/to/script.sh
 
 Task created: https://taskbadger.net/public/tasks/xyz/
 ```
```

### Comparing `taskbadger-0.5.0/pyproject.toml` & `taskbadger-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskbadger"
-version = "0.5.0"
+version = "0.6.0"
 description = "The official Python SDK for Task Badger"
 license = "Apache-2.0"
 
 authors = []
 
 readme = "README.md"
 packages = [
```

### Comparing `taskbadger-0.5.0/taskbadger/cli.py` & `taskbadger-0.6.0/taskbadger/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-import subprocess
-import time
-from datetime import datetime
 from typing import Optional, Tuple
 
 import typer
 from rich import print
 from rich.console import Console
 
 from taskbadger import Action, StatusEnum, Task, __version__, integrations
 from taskbadger.config import get_config, write_config
 from taskbadger.exceptions import ConfigurationError
+from taskbadger.process import ProcessRunner
 
 app = typer.Typer(
     rich_markup_mode="rich",
     context_settings={"help_option_names": ["-h", "--help"]},
 )
 
 
@@ -45,14 +43,15 @@
         (None, None, None),
         "--action",
         "-a",
         metavar="<trigger integration config>",
         show_default=False,
         help="Action definition e.g. 'success,error email to:me@email.com'",
     ),
+    capture_output: bool = typer.Option(False, help="Capture stdout and stderr."),
 ):
     """Execute a command using the CLI and create a Task to track its outcome.
 
     This command makes it easy to track a process's outcome using Task Badger.
 
     It will create a Task prior to executing your command and will update
     the Task status when you command exits.
@@ -77,41 +76,52 @@
         )
     except Exception as e:
         err_console.print(f"Error creating task: {e}")
         task = None
     else:
         print(f"Task created: {task.public_url}")
     env = {"TASKBADGER_TASK_ID": task.id} if task else None
-    last_update = datetime.utcnow()
     try:
-        process = subprocess.Popen(ctx.args, env=env, shell=True)
-        while process.poll() is None:
-            try:
-                time.sleep(0.1)
-                if task and _should_update_task(last_update, update_frequency):
-                    last_update = datetime.utcnow()
-                    task.ping()
-            except Exception as e:
-                err_console.print(f"Error updating task status: {e}")
+        process = ProcessRunner(ctx.args, env, capture_output=capture_output, update_frequency=update_frequency)
+        for output in process.run():
+            _update_task(task, **(output or {}))
     except Exception as e:
-        task and task.error(data={"exception": str(e)})
+        _update_task(task, exception=str(e))
         raise typer.Exit(1)
 
     if task:
         if process.returncode == 0:
             task.success(value=100)
         else:
-            task.error(data={"return_code": process.returncode})
+            _update_task(task, status=StatusEnum.ERROR, return_code=process.returncode)
 
     if process.returncode != 0:
         raise typer.Exit(process.returncode)
 
 
-def _should_update_task(last_update: datetime, update_frequency_seconds):
-    return (datetime.utcnow() - last_update).total_seconds() >= update_frequency_seconds
+def _update_task(task, status=None, **data_kwargs):
+    """Update the task and merge the data"""
+    if not task:
+        return
+
+    task_data = task.data or {}
+    for key, value in data_kwargs.items():
+        if key in ("stdout", "stderr"):
+            if key in task_data and value:
+                task_data[key] += value
+            elif value:
+                task_data[key] = value
+        else:
+            task_data[key] = value
+
+    print(task_data)
+    try:
+        task.update(status=status, data=task_data or None)
+    except Exception as e:
+        err_console.print(f"Error updating task status: {e}")
 
 
 @app.command()
 def configure(ctx: typer.Context):
     """Update CLI configuration."""
     config = ctx.meta["tb_config"]
     config.organization_slug = typer.prompt(f"Organization slug", default=config.organization_slug)
```

### Comparing `taskbadger-0.5.0/taskbadger/config.py` & `taskbadger-0.6.0/taskbadger/config.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/taskbadger/integrations.py` & `taskbadger-0.6.0/taskbadger/integrations.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/taskbadger/internal/api/action_endpoints/action_cancel.py` & `taskbadger-0.6.0/taskbadger/internal/api/action_endpoints/action_cancel.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/taskbadger/internal/api/action_endpoints/action_create.py` & `taskbadger-0.6.0/taskbadger/internal/api/action_endpoints/action_create.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/taskbadger/internal/api/action_endpoints/action_get.py` & `taskbadger-0.6.0/taskbadger/internal/api/action_endpoints/action_get.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/taskbadger/internal/api/action_endpoints/action_list.py` & `taskbadger-0.6.0/taskbadger/internal/api/action_endpoints/action_list.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/taskbadger/internal/api/action_endpoints/action_partial_update.py` & `taskbadger-0.6.0/taskbadger/internal/api/action_endpoints/action_partial_update.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/taskbadger/internal/api/action_endpoints/action_update.py` & `taskbadger-0.6.0/taskbadger/internal/api/action_endpoints/action_update.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/taskbadger/internal/api/task_endpoints/task_cancel.py` & `taskbadger-0.6.0/taskbadger/internal/api/task_endpoints/task_cancel.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/taskbadger/internal/api/task_endpoints/task_create.py` & `taskbadger-0.6.0/taskbadger/internal/api/task_endpoints/task_create.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/taskbadger/internal/api/task_endpoints/task_get.py` & `taskbadger-0.6.0/taskbadger/internal/api/task_endpoints/task_get.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/taskbadger/internal/api/task_endpoints/task_list.py` & `taskbadger-0.6.0/taskbadger/internal/api/task_endpoints/task_list.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/taskbadger/internal/api/task_endpoints/task_partial_update.py` & `taskbadger-0.6.0/taskbadger/internal/api/task_endpoints/task_partial_update.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/taskbadger/internal/api/task_endpoints/task_update.py` & `taskbadger-0.6.0/taskbadger/internal/api/task_endpoints/task_update.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/taskbadger/internal/client.py` & `taskbadger-0.6.0/taskbadger/internal/client.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/taskbadger/internal/models/__init__.py` & `taskbadger-0.6.0/taskbadger/internal/models/__init__.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/taskbadger/internal/models/action.py` & `taskbadger-0.6.0/taskbadger/internal/models/action.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/taskbadger/internal/models/action_config.py` & `taskbadger-0.6.0/taskbadger/internal/models/action_config.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/taskbadger/internal/models/action_request.py` & `taskbadger-0.6.0/taskbadger/internal/models/action_request.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/taskbadger/internal/models/action_request_config.py` & `taskbadger-0.6.0/taskbadger/internal/models/action_request_config.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/taskbadger/internal/models/paginated_task_list.py` & `taskbadger-0.6.0/taskbadger/internal/models/paginated_task_list.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/taskbadger/internal/models/patched_action_request.py` & `taskbadger-0.6.0/taskbadger/internal/models/patched_action_request.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/taskbadger/internal/models/patched_action_request_config.py` & `taskbadger-0.6.0/taskbadger/internal/models/patched_action_request_config.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/taskbadger/internal/models/patched_task_request.py` & `taskbadger-0.6.0/taskbadger/internal/models/patched_task_request.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/taskbadger/internal/models/patched_task_request_data.py` & `taskbadger-0.6.0/taskbadger/internal/models/patched_task_request_data.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/taskbadger/internal/models/task.py` & `taskbadger-0.6.0/taskbadger/internal/models/task.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/taskbadger/internal/models/task_data.py` & `taskbadger-0.6.0/taskbadger/internal/models/task_data.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/taskbadger/internal/models/task_request.py` & `taskbadger-0.6.0/taskbadger/internal/models/task_request.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/taskbadger/internal/models/task_request_data.py` & `taskbadger-0.6.0/taskbadger/internal/models/task_request_data.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/taskbadger/internal/types.py` & `taskbadger-0.6.0/taskbadger/internal/types.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/taskbadger/safe_sdk.py` & `taskbadger-0.6.0/taskbadger/safe_sdk.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/taskbadger/sdk.py` & `taskbadger-0.6.0/taskbadger/sdk.py`

 * *Files identical despite different names*

### Comparing `taskbadger-0.5.0/PKG-INFO` & `taskbadger-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskbadger
-Version: 0.5.0
+Version: 0.6.0
 Summary: The official Python SDK for Task Badger
 Home-page: https://taskbadger.net/
 License: Apache-2.0
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -111,12 +111,12 @@
 ```
 
 #### Usage Examples
 
 The CLI `run` command executes your command whilst creating and updating a Task Badger task.
 
 ```shell
-$ taskbadger run "demo task" --action "error email to:me@test.com" -- path/to/script.sh
+$ taskbadger run "demo task" --action error email to:me@test.com -- path/to/script.sh
 
 Task created: https://taskbadger.net/public/tasks/xyz/
 ```
```

