# Comparing `tmp/whiffle_client-0.2.0.tar.gz` & `tmp/whiffle_client-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/whiffle/hindcasting/whiffle-client/dist/.tmp-55yuhyal/whiffle_client-0.2.0.tar", last modified: Tue Jul 11 09:52:22 2023, max compression
+gzip compressed data, was "/builds/whiffle/hindcasting/whiffle-client/dist/.tmp-ts2eoey2/whiffle_client-0.2.1.tar", last modified: Thu Jul 13 13:40:46 2023, max compression
```

## Comparing `whiffle_client-0.2.0.tar` & `whiffle_client-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:52:22.000000 whiffle_client-0.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-07-11 09:52:17.000000 whiffle_client-0.2.0/LICENCE.txt
--rw-rw-rw-   0 root         (0) root         (0)      121 2023-07-11 09:52:17.000000 whiffle_client-0.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1333 2023-07-11 09:52:22.000000 whiffle_client-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-07-11 09:52:17.000000 whiffle_client-0.2.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      994 2023-07-11 09:52:17.000000 whiffle_client-0.2.0/USER_README.md
--rw-rw-rw-   0 root         (0) root         (0)      834 2023-07-11 09:52:17.000000 whiffle_client-0.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 09:52:22.000000 whiffle_client-0.2.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:52:22.000000 whiffle_client-0.2.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3922 2023-07-11 09:52:17.000000 whiffle_client-0.2.0/tests/test_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:52:22.000000 whiffle_client-0.2.0/whiffle_client/
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-07-11 09:52:17.000000 whiffle_client-0.2.0/whiffle_client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7093 2023-07-11 09:52:17.000000 whiffle_client-0.2.0/whiffle_client/client.py
--rw-rw-rw-   0 root         (0) root         (0)     3057 2023-07-11 09:52:17.000000 whiffle_client-0.2.0/whiffle_client/entrypoints.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:52:22.000000 whiffle_client-0.2.0/whiffle_client/resources/
--rw-rw-rw-   0 root         (0) root         (0)     2624 2023-07-11 09:52:17.000000 whiffle_client-0.2.0/whiffle_client/resources/example_generic_params.json
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-11 09:52:17.000000 whiffle_client-0.2.0/whiffle_client/resources/whiffle_config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 09:52:22.000000 whiffle_client-0.2.0/whiffle_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1333 2023-07-11 09:52:22.000000 whiffle_client-0.2.0/whiffle_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      494 2023-07-11 09:52:22.000000 whiffle_client-0.2.0/whiffle_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 09:52:22.000000 whiffle_client-0.2.0/whiffle_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-07-11 09:52:22.000000 whiffle_client-0.2.0/whiffle_client.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-07-11 09:52:22.000000 whiffle_client-0.2.0/whiffle_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-11 09:52:22.000000 whiffle_client-0.2.0/whiffle_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 13:40:46.000000 whiffle_client-0.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-07-13 13:40:40.000000 whiffle_client-0.2.1/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-07-13 13:40:40.000000 whiffle_client-0.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1333 2023-07-13 13:40:46.000000 whiffle_client-0.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-07-13 13:40:40.000000 whiffle_client-0.2.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      994 2023-07-13 13:40:40.000000 whiffle_client-0.2.1/USER_README.md
+-rw-rw-rw-   0 root         (0) root         (0)      834 2023-07-13 13:40:40.000000 whiffle_client-0.2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-13 13:40:46.000000 whiffle_client-0.2.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 13:40:46.000000 whiffle_client-0.2.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3922 2023-07-13 13:40:40.000000 whiffle_client-0.2.1/tests/test_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 13:40:46.000000 whiffle_client-0.2.1/whiffle_client/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-07-13 13:40:40.000000 whiffle_client-0.2.1/whiffle_client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7093 2023-07-13 13:40:40.000000 whiffle_client-0.2.1/whiffle_client/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3057 2023-07-13 13:40:40.000000 whiffle_client-0.2.1/whiffle_client/entrypoints.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 13:40:46.000000 whiffle_client-0.2.1/whiffle_client/resources/
+-rw-rw-rw-   0 root         (0) root         (0)     2624 2023-07-13 13:40:40.000000 whiffle_client-0.2.1/whiffle_client/resources/example_generic_params.json
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-13 13:40:40.000000 whiffle_client-0.2.1/whiffle_client/resources/whiffle_config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 13:40:46.000000 whiffle_client-0.2.1/whiffle_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1333 2023-07-13 13:40:46.000000 whiffle_client-0.2.1/whiffle_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      494 2023-07-13 13:40:46.000000 whiffle_client-0.2.1/whiffle_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 13:40:46.000000 whiffle_client-0.2.1/whiffle_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-07-13 13:40:46.000000 whiffle_client-0.2.1/whiffle_client.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-07-13 13:40:46.000000 whiffle_client-0.2.1/whiffle_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-13 13:40:46.000000 whiffle_client-0.2.1/whiffle_client.egg-info/top_level.txt
```

### Comparing `whiffle_client-0.2.0/LICENCE.txt` & `whiffle_client-0.2.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.2.0/PKG-INFO` & `whiffle_client-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whiffle_client
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python based web client to interact with Whiffle services
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

### Comparing `whiffle_client-0.2.0/README.md` & `whiffle_client-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.2.0/USER_README.md` & `whiffle_client-0.2.1/USER_README.md`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.2.0/pyproject.toml` & `whiffle_client-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.2.0/tests/test_client.py` & `whiffle_client-0.2.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.2.0/whiffle_client/client.py` & `whiffle_client-0.2.1/whiffle_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         )
         if lon != None and lat != None:
             return res.json()
         return res.json()
 
     def download(self, task_id, filename=None):
         if filename == None:
-            filename = task_id + ".tar"
+            filename = task_id + ".zip"
         res = self._create_request(
             self.session.get,
             "/api/aspforge/tasks/{}/download".format(task_id),
             stream=True,
         )
         self._download_write_chunks(filename, res)
 
@@ -178,15 +178,15 @@
     def communicate(self, task_id=None, filename=None):
         if task_id == None:
             task_id = self.get_tasks()[-1]["task_id"]
         print(f"Poll for status of task_id: {task_id}")
 
         # Output
         if filename is None:
-            filename = task_id + ".tar"
+            filename = task_id + ".zip"
 
         # Initialize poll parameters
         status = self.get_status(task_id)
         while status not in ["successful", "failed"]:
             time.sleep(5)
             status = self.get_status(task_id)
             progress = self.get_progress(task_id)
```

### Comparing `whiffle_client-0.2.0/whiffle_client/entrypoints.py` & `whiffle_client-0.2.1/whiffle_client/entrypoints.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.2.0/whiffle_client/resources/example_generic_params.json` & `whiffle_client-0.2.1/whiffle_client/resources/example_generic_params.json`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.2.0/whiffle_client.egg-info/PKG-INFO` & `whiffle_client-0.2.1/whiffle_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whiffle-client
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python based web client to interact with Whiffle services
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

