# Comparing `tmp/pipekit_sdk-0.0.1.tar.gz` & `tmp/pipekit_sdk-0.0.2.tar.gz`

## Comparing `pipekit_sdk-0.0.1.tar` & `pipekit_sdk-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipekit_sdk-0.0.1/src/pipekit_sdk/__init__.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 pipekit_sdk-0.0.1/src/pipekit_sdk/helpers.py
--rw-r--r--   0        0        0    12205 2020-02-02 00:00:00.000000 pipekit_sdk-0.0.1/src/pipekit_sdk/service.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pipekit_sdk-0.0.1/.gitignore
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 pipekit_sdk-0.0.1/LICENSE
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 pipekit_sdk-0.0.1/README.md
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 pipekit_sdk-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 pipekit_sdk-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipekit_sdk-0.0.2/src/pipekit_sdk/__init__.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 pipekit_sdk-0.0.2/src/pipekit_sdk/helpers.py
+-rw-r--r--   0        0        0    12205 2020-02-02 00:00:00.000000 pipekit_sdk-0.0.2/src/pipekit_sdk/service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pipekit_sdk-0.0.2/tests/.gitkeep
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pipekit_sdk-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 pipekit_sdk-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 pipekit_sdk-0.0.2/README.md
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 pipekit_sdk-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 pipekit_sdk-0.0.2/PKG-INFO
```

### Comparing `pipekit_sdk-0.0.1/src/pipekit_sdk/helpers.py` & `pipekit_sdk-0.0.2/src/pipekit_sdk/helpers.py`

 * *Files identical despite different names*

### Comparing `pipekit_sdk-0.0.1/src/pipekit_sdk/service.py` & `pipekit_sdk-0.0.2/src/pipekit_sdk/service.py`

 * *Files identical despite different names*

### Comparing `pipekit_sdk-0.0.1/LICENSE` & `pipekit_sdk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pipekit_sdk-0.0.1/README.md` & `pipekit_sdk-0.0.2/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -56,8 +56,8 @@
         A >> [B, C] >> D
 
 # submit the workflow to pipekit
 pipe_run = pipekit.submit(w, "<cluster-name>")
 
 # let's tail logs
 pipekit.print_logs(pipe_run["uuid"])
-```
+```
```

### Comparing `pipekit_sdk-0.0.1/PKG-INFO` & `pipekit_sdk-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pipekit-sdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: Pipekit Python SDK
 Author-email: Aleksa Trajkovic <aleksa@pipekit.io>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
-Requires-Dist: hera
+Requires-Dist: hera>=5.5.2
 Description-Content-Type: text/markdown
 
 # Pipekit Python SDK
 
 ## Installation
 
 ```bash
@@ -68,8 +68,8 @@
         A >> [B, C] >> D
 
 # submit the workflow to pipekit
 pipe_run = pipekit.submit(w, "<cluster-name>")
 
 # let's tail logs
 pipekit.print_logs(pipe_run["uuid"])
-```
+```
```

