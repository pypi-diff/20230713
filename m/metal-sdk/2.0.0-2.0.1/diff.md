# Comparing `tmp/metal_sdk-2.0.0.tar.gz` & `tmp/metal_sdk-2.0.1.tar.gz`

## Comparing `metal_sdk-2.0.0.tar` & `metal_sdk-2.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/examples/example.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/examples/example_async.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/src/metal_sdk/__init__.py
--rw-r--r--   0        0        0     6891 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/src/metal_sdk/metal.py
--rw-r--r--   0        0        0     7038 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/src/metal_sdk/metal_async.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/src/metal_sdk/motorhead.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/src/metal_sdk/motorhead_async.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/src/metal_sdk/typings.py
--rw-r--r--   0        0        0     9558 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/tests/test_metal.py
--rw-r--r--   0        0        0     9969 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/tests/test_metal_async.py
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/tests/test_motorhead.py
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/tests/test_motorhead_async.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/tests/fixtures/sample.csv
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/.gitignore
--rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/LICENSE
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/README.md
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 metal_sdk-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 metal_sdk-2.0.1/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 metal_sdk-2.0.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 metal_sdk-2.0.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 metal_sdk-2.0.1/examples/example.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 metal_sdk-2.0.1/examples/example_async.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 metal_sdk-2.0.1/src/metal_sdk/__init__.py
+-rw-r--r--   0        0        0     6894 2020-02-02 00:00:00.000000 metal_sdk-2.0.1/src/metal_sdk/metal.py
+-rw-r--r--   0        0        0     7041 2020-02-02 00:00:00.000000 metal_sdk-2.0.1/src/metal_sdk/metal_async.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 metal_sdk-2.0.1/src/metal_sdk/motorhead.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 metal_sdk-2.0.1/src/metal_sdk/motorhead_async.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 metal_sdk-2.0.1/src/metal_sdk/typings.py
+-rw-r--r--   0        0        0     9558 2020-02-02 00:00:00.000000 metal_sdk-2.0.1/tests/test_metal.py
+-rw-r--r--   0        0        0     9969 2020-02-02 00:00:00.000000 metal_sdk-2.0.1/tests/test_metal_async.py
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 metal_sdk-2.0.1/tests/test_motorhead.py
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 metal_sdk-2.0.1/tests/test_motorhead_async.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 metal_sdk-2.0.1/tests/fixtures/sample.csv
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 metal_sdk-2.0.1/.gitignore
+-rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 metal_sdk-2.0.1/LICENSE
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 metal_sdk-2.0.1/README.md
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 metal_sdk-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 metal_sdk-2.0.1/PKG-INFO
```

### Comparing `metal_sdk-2.0.0/.github/workflows/publish.yml` & `metal_sdk-2.0.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `metal_sdk-2.0.0/.github/workflows/test.yml` & `metal_sdk-2.0.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `metal_sdk-2.0.0/examples/example.py` & `metal_sdk-2.0.1/examples/example.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-2.0.0/examples/example_async.py` & `metal_sdk-2.0.1/examples/example_async.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-2.0.0/src/metal_sdk/metal.py` & `metal_sdk-2.0.1/src/metal_sdk/metal.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
         """
         Implement your filename sanitation method here.
         """
         sanitized_filename = filename.replace(' ', '_')  # Simplified example
         return sanitized_filename
 
     def __create_resource(self, index_id, filename, file_type, file_size):
-        url = f'{self.base_url}/indexes/{index_id}/files'
+        url = f'{self.base_url}/v1/indexes/{index_id}/files'
         payload = {
             'fileName': self.__sanitize_filename(filename),
             'fileType': file_type,
         }
         headers = {'x-metal-file-size': str(file_size)}
 
         res = self.request("post", url, json=payload, headers=headers)
```

### Comparing `metal_sdk-2.0.0/src/metal_sdk/metal_async.py` & `metal_sdk-2.0.1/src/metal_sdk/metal_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
         """
         Implement your filename sanitation method here.
         """
         sanitized_filename = filename.replace(' ', '_')  # Simplified example
         return sanitized_filename
 
     async def __create_resource(self, index_id, filename, file_type, file_size):
-        url = f'{self.base_url}/indexes/{index_id}/files'
+        url = f'{self.base_url}/v1/indexes/{index_id}/files'
         payload = {
             'fileName': self.__sanitize_filename(filename),
             'fileType': file_type,
         }
         headers = {'x-metal-file-size': str(file_size)}
 
         res = await self.request("post", url, json=payload, headers=headers)
```

### Comparing `metal_sdk-2.0.0/src/metal_sdk/motorhead.py` & `metal_sdk-2.0.1/src/metal_sdk/motorhead.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-2.0.0/src/metal_sdk/motorhead_async.py` & `metal_sdk-2.0.1/src/metal_sdk/motorhead_async.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-2.0.0/src/metal_sdk/typings.py` & `metal_sdk-2.0.1/src/metal_sdk/typings.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-2.0.0/tests/test_metal.py` & `metal_sdk-2.0.1/tests/test_metal.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-2.0.0/tests/test_metal_async.py` & `metal_sdk-2.0.1/tests/test_metal_async.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-2.0.0/tests/test_motorhead.py` & `metal_sdk-2.0.1/tests/test_motorhead.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-2.0.0/tests/test_motorhead_async.py` & `metal_sdk-2.0.1/tests/test_motorhead_async.py`

 * *Files identical despite different names*

### Comparing `metal_sdk-2.0.0/.gitignore` & `metal_sdk-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `metal_sdk-2.0.0/LICENSE` & `metal_sdk-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `metal_sdk-2.0.0/README.md` & `metal_sdk-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `metal_sdk-2.0.0/pyproject.toml` & `metal_sdk-2.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "metal_sdk"
-version = "2.0.0"
+version = "2.0.1"
 authors = [
   { name="Metal Technologies Inc", email="james@getmetal.io" },
 ]
 description = "SDK for getmetal.io"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `metal_sdk-2.0.0/PKG-INFO` & `metal_sdk-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metal_sdk
-Version: 2.0.0
+Version: 2.0.1
 Summary: SDK for getmetal.io
 Project-URL: Github, https://github.com/getmetal/metal-python
 Author-email: Metal Technologies Inc <james@getmetal.io>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

