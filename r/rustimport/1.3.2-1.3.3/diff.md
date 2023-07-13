# Comparing `tmp/rustimport-1.3.2.tar.gz` & `tmp/rustimport-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rustimport-1.3.2.tar", last modified: Thu Jun 29 15:56:48 2023, max compression
+gzip compressed data, was "rustimport-1.3.3.tar", last modified: Thu Jul 13 13:36:56 2023, max compression
```

## Comparing `rustimport-1.3.2.tar` & `rustimport-1.3.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:56:48.737987 rustimport-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-29 15:56:37.000000 rustimport-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-29 15:56:37.000000 rustimport-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-06-29 15:56:48.737987 rustimport-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-06-29 15:56:37.000000 rustimport-1.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 15:56:37.000000 rustimport-1.3.2/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:56:48.733987 rustimport-1.3.2/rustimport/
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-06-29 15:56:37.000000 rustimport-1.3.2/rustimport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-06-29 15:56:37.000000 rustimport-1.3.2/rustimport/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-29 15:56:37.000000 rustimport-1.3.2/rustimport/checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-06-29 15:56:37.000000 rustimport-1.3.2/rustimport/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-29 15:56:37.000000 rustimport-1.3.2/rustimport/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-29 15:56:37.000000 rustimport-1.3.2/rustimport/find.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-29 15:56:37.000000 rustimport-1.3.2/rustimport/import_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-06-29 15:56:37.000000 rustimport-1.3.2/rustimport/importable.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-29 15:56:37.000000 rustimport-1.3.2/rustimport/load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:56:48.737987 rustimport-1.3.2/rustimport/pre_processing/
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-29 15:56:37.000000 rustimport-1.3.2/rustimport/pre_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-29 15:56:37.000000 rustimport-1.3.2/rustimport/pre_processing/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-29 15:56:37.000000 rustimport-1.3.2/rustimport/pre_processing/pyo3_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-06-29 15:56:37.000000 rustimport-1.3.2/rustimport/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:56:48.737987 rustimport-1.3.2/rustimport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-06-29 15:56:48.000000 rustimport-1.3.2/rustimport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-29 15:56:48.000000 rustimport-1.3.2/rustimport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 15:56:48.000000 rustimport-1.3.2/rustimport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 15:56:48.000000 rustimport-1.3.2/rustimport.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 15:56:48.000000 rustimport-1.3.2/rustimport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 15:56:48.000000 rustimport-1.3.2/rustimport.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 15:56:48.737987 rustimport-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-29 15:56:37.000000 rustimport-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:56:48.737987 rustimport-1.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-29 15:56:37.000000 rustimport-1.3.2/tests/run_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-06-29 15:56:37.000000 rustimport-1.3.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-29 15:56:37.000000 rustimport-1.3.2/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:36:56.883315 rustimport-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-13 13:36:43.000000 rustimport-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 13:36:43.000000 rustimport-1.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-07-13 13:36:56.883315 rustimport-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-07-13 13:36:43.000000 rustimport-1.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 13:36:43.000000 rustimport-1.3.3/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:36:56.875315 rustimport-1.3.3/rustimport/
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-07-13 13:36:43.000000 rustimport-1.3.3/rustimport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-13 13:36:43.000000 rustimport-1.3.3/rustimport/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-07-13 13:36:43.000000 rustimport-1.3.3/rustimport/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-13 13:36:43.000000 rustimport-1.3.3/rustimport/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-13 13:36:43.000000 rustimport-1.3.3/rustimport/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-13 13:36:43.000000 rustimport-1.3.3/rustimport/find.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-13 13:36:43.000000 rustimport-1.3.3/rustimport/import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-07-13 13:36:43.000000 rustimport-1.3.3/rustimport/importable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-13 13:36:43.000000 rustimport-1.3.3/rustimport/load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:36:56.879315 rustimport-1.3.3/rustimport/pre_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-07-13 13:36:43.000000 rustimport-1.3.3/rustimport/pre_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-13 13:36:43.000000 rustimport-1.3.3/rustimport/pre_processing/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-07-13 13:36:43.000000 rustimport-1.3.3/rustimport/pre_processing/pyo3_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-13 13:36:43.000000 rustimport-1.3.3/rustimport/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:36:56.879315 rustimport-1.3.3/rustimport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-07-13 13:36:56.000000 rustimport-1.3.3/rustimport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-13 13:36:56.000000 rustimport-1.3.3/rustimport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 13:36:56.000000 rustimport-1.3.3/rustimport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 13:36:56.000000 rustimport-1.3.3/rustimport.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-13 13:36:56.000000 rustimport-1.3.3/rustimport.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 13:36:56.000000 rustimport-1.3.3/rustimport.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 13:36:56.883315 rustimport-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-13 13:36:43.000000 rustimport-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:36:56.879315 rustimport-1.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-13 13:36:43.000000 rustimport-1.3.3/tests/run_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-07-13 13:36:43.000000 rustimport-1.3.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-13 13:36:43.000000 rustimport-1.3.3/tests/test_examples.py
```

### Comparing `rustimport-1.3.2/LICENSE` & `rustimport-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rustimport-1.3.2/PKG-INFO` & `rustimport-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustimport
-Version: 1.3.2
+Version: 1.3.3
 Summary: Import Rust files directly from Python!
 Home-page: https://github.com/mityax/rustimport
 Author: mityax
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `rustimport-1.3.2/README.md` & `rustimport-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `rustimport-1.3.2/rustimport/__init__.py` & `rustimport-1.3.3/rustimport/__init__.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.3.2/rustimport/__main__.py` & `rustimport-1.3.3/rustimport/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,20 +54,20 @@
 crate-type = ["cdylib"]
 
 [dependencies]
 pyo3 = { version = "0.18.3", features = ["extension-module"] }
 """
 
 
-def create_extension(name: str):
+def create_extension(name: str, cwd: str = '.'):
     if not re.match(r'^[a-zA-Z]\w*(\.rs)?$', name):
         raise ValueError(f"Invalid extension name: {name}. The name may only contain letters (preferably lowercase), "
                          f"numbers and underscores and should start with a letter.")
 
-    path = os.path.realpath(name)
+    path = os.path.realpath(os.path.join(cwd, name))
     name = os.path.splitext(os.path.basename(name))[0]
 
     if path.endswith(".rs"):
         with open(path, 'w+') as f:
             f.write(rust_lib_template.replace('{{EXTENSION_NAME}}', name))
     else:
         src_dir = os.path.join(path, 'src')
```

### Comparing `rustimport-1.3.2/rustimport/checksum.py` & `rustimport-1.3.3/rustimport/checksum.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.3.2/rustimport/compiler.py` & `rustimport-1.3.3/rustimport/compiler.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.3.2/rustimport/error_handling.py` & `rustimport-1.3.3/rustimport/error_handling.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.3.2/rustimport/find.py` & `rustimport-1.3.3/rustimport/find.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.3.2/rustimport/import_hook.py` & `rustimport-1.3.3/rustimport/import_hook.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.3.2/rustimport/importable.py` & `rustimport-1.3.3/rustimport/importable.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import hashlib
 import logging
 import os.path
 import shutil
 import sysconfig
 import types
 from functools import cached_property
-from typing import Optional, List, Type
+from typing import Optional, List, Type, Set
 
 from rustimport import load, BuildError, settings
 from rustimport.checksum import is_checksum_valid, save_checksum
 from rustimport.compiler import Cargo
 from rustimport.error_handling import notify_potential_failure_reason
 from rustimport.pre_processing import Preprocessor
 
@@ -250,29 +250,47 @@
         save_checksum(self.extension_path, self.dependencies, release=release)
 
     def _copy_source_to_build_dir(self) -> str:
         """
         Copies the source crate or workspace into the temporary build directory
         and return the root path (i.e. to the workspace directory if we're in a
         workspace, to the crate otherwise).
+
+        Note: This method also deletes entities contained in the target directory
+              should they appear to no longer be in the source directory.
         """
 
         src_path = self.__workspace_path or self.__crate_path
         output_path = os.path.join(  # e.g. `/output/path/myworkspace` or `/output/path/mycrate` respectively
             self.build_tempdir,
             os.path.basename(self.__workspace_path or self.__crate_path)
         )
 
-        def ignore(src: str, names: List[str]) -> List[str]:
-            if src == src_path and 'target' in names:
-                return ['target']  # do not copy the root "target" folder as it may be huge and slow
-            return []
-
         os.makedirs(output_path, exist_ok=True)
-        shutil.copytree(src_path, output_path, ignore=ignore, dirs_exist_ok=True)
+
+        def ignore(src: str, names: List[str]) -> Set[str]:
+            # Do not copy the root "target" folder as it may be huge and slow:
+            return {'target'} if src == src_path else set()
+
+        # Track the copied files, so we can delete files that are no longer in the source directory:
+        copied_files = set()
+
+        def copy_function(src, dst):
+            shutil.copy2(src, dst)
+            copied_files.add(dst)
+
+        shutil.copytree(src_path, output_path, ignore=ignore, copy_function=copy_function, dirs_exist_ok=True)
+
+        # Delete files that are no longer in the source directory:
+        for root, dirs, files in os.walk(output_path, topdown=True):
+            dirs[:] = set(dirs) - ignore(root, dirs)  # remove ignored directories from the walk
+
+            for file in files:
+                if (abs_path := os.path.join(root, file)) not in copied_files:
+                    os.remove(abs_path)
 
         return output_path
 
     def _preprocess(self, crate_output_subdirectory: str) -> Preprocessor.PreprocessorResult:
         """
         Calls [Preprocessor.process()] on the crate, updates the source files
         with the result and returns the result for further usage.
```

### Comparing `rustimport-1.3.2/rustimport/load.py` & `rustimport-1.3.3/rustimport/load.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.3.2/rustimport/pre_processing/__init__.py` & `rustimport-1.3.3/rustimport/pre_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.3.2/rustimport/pre_processing/base.py` & `rustimport-1.3.3/rustimport/pre_processing/base.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.3.2/rustimport/pre_processing/pyo3_template.py` & `rustimport-1.3.3/rustimport/pre_processing/pyo3_template.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.3.2/rustimport/settings.py` & `rustimport-1.3.3/rustimport/settings.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.3.2/rustimport.egg-info/PKG-INFO` & `rustimport-1.3.3/rustimport.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustimport
-Version: 1.3.2
+Version: 1.3.3
 Summary: Import Rust files directly from Python!
 Home-page: https://github.com/mityax/rustimport
 Author: mityax
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `rustimport-1.3.2/rustimport.egg-info/SOURCES.txt` & `rustimport-1.3.3/rustimport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rustimport-1.3.2/setup.py` & `rustimport-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.3.2/tests/test_cli.py` & `rustimport-1.3.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.3.2/tests/test_examples.py` & `rustimport-1.3.3/tests/test_examples.py`

 * *Files identical despite different names*

