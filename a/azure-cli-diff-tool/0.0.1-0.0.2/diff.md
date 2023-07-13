# Comparing `tmp/azure-cli-diff-tool-0.0.1.tar.gz` & `tmp/azure-cli-diff-tool-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-cli-diff-tool-0.0.1.tar", last modified: Tue Jul 11 03:07:11 2023, max compression
+gzip compressed data, was "azure-cli-diff-tool-0.0.2.tar", last modified: Thu Jul 13 06:47:17 2023, max compression
```

## Comparing `azure-cli-diff-tool-0.0.1.tar` & `azure-cli-diff-tool-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-07-11 03:07:11.366397 azure-cli-diff-tool-0.0.1/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3301 2023-07-11 03:07:11.366397 azure-cli-diff-tool-0.0.1/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3032 2023-07-11 03:06:53.000000 azure-cli-diff-tool-0.0.1/README.rst
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-07-11 03:07:11.366397 azure-cli-diff-tool-0.0.1/azureCliDiffTool/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6273 2023-07-11 03:06:53.000000 azure-cli-diff-tool-0.0.1/azureCliDiffTool/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3151 2023-07-11 03:06:53.000000 azure-cli-diff-tool-0.0.1/azureCliDiffTool/_const.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-07-11 03:07:11.366397 azure-cli-diff-tool-0.0.1/azureCliDiffTool/data/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      164 2023-07-11 03:06:53.000000 azure-cli-diff-tool-0.0.1/azureCliDiffTool/data/blob_config.ini
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      540 2023-07-11 03:06:53.000000 azure-cli-diff-tool-0.0.1/azureCliDiffTool/data/meta_change_whitelist.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12819 2023-07-11 03:06:53.000000 azure-cli-diff-tool-0.0.1/azureCliDiffTool/meta_change.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    16658 2023-07-11 03:06:53.000000 azure-cli-diff-tool-0.0.1/azureCliDiffTool/meta_change_detect.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8727 2023-07-11 03:06:53.000000 azure-cli-diff-tool-0.0.1/azureCliDiffTool/utils.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-07-11 03:07:11.366397 azure-cli-diff-tool-0.0.1/azure_cli_diff_tool.egg-info/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3301 2023-07-11 03:07:11.000000 azure-cli-diff-tool-0.0.1/azure_cli_diff_tool.egg-info/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      472 2023-07-11 03:07:11.000000 azure-cli-diff-tool-0.0.1/azure_cli_diff_tool.egg-info/SOURCES.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2023-07-11 03:07:11.000000 azure-cli-diff-tool-0.0.1/azure_cli_diff_tool.egg-info/dependency_links.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       18 2023-07-11 03:07:11.000000 azure-cli-diff-tool-0.0.1/azure_cli_diff_tool.egg-info/requires.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       17 2023-07-11 03:07:11.000000 azure-cli-diff-tool-0.0.1/azure_cli_diff_tool.egg-info/top_level.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2023-07-11 03:07:11.366397 azure-cli-diff-tool-0.0.1/setup.cfg
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1399 2023-07-11 03:06:53.000000 azure-cli-diff-tool-0.0.1/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-07-13 06:47:17.492990 azure-cli-diff-tool-0.0.2/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3466 2023-07-13 06:47:17.492990 azure-cli-diff-tool-0.0.2/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3050 2023-07-13 06:47:11.000000 azure-cli-diff-tool-0.0.2/README.rst
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-07-13 06:47:17.488990 azure-cli-diff-tool-0.0.2/azure_cli_diff_tool/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6291 2023-07-13 06:47:11.000000 azure-cli-diff-tool-0.0.2/azure_cli_diff_tool/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3151 2023-07-13 06:47:11.000000 azure-cli-diff-tool-0.0.2/azure_cli_diff_tool/_const.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-07-13 06:47:17.492990 azure-cli-diff-tool-0.0.2/azure_cli_diff_tool/data/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      164 2023-07-13 06:47:11.000000 azure-cli-diff-tool-0.0.2/azure_cli_diff_tool/data/blob_config.ini
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      540 2023-07-13 06:47:11.000000 azure-cli-diff-tool-0.0.2/azure_cli_diff_tool/data/meta_change_whitelist.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12819 2023-07-13 06:47:11.000000 azure-cli-diff-tool-0.0.2/azure_cli_diff_tool/meta_change.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    16658 2023-07-13 06:47:11.000000 azure-cli-diff-tool-0.0.2/azure_cli_diff_tool/meta_change_detect.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8727 2023-07-13 06:47:11.000000 azure-cli-diff-tool-0.0.2/azure_cli_diff_tool/utils.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-07-13 06:47:17.492990 azure-cli-diff-tool-0.0.2/azure_cli_diff_tool.egg-info/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3466 2023-07-13 06:47:17.000000 azure-cli-diff-tool-0.0.2/azure_cli_diff_tool.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      493 2023-07-13 06:47:17.000000 azure-cli-diff-tool-0.0.2/azure_cli_diff_tool.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2023-07-13 06:47:17.000000 azure-cli-diff-tool-0.0.2/azure_cli_diff_tool.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       18 2023-07-13 06:47:17.000000 azure-cli-diff-tool-0.0.2/azure_cli_diff_tool.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       20 2023-07-13 06:47:17.000000 azure-cli-diff-tool-0.0.2/azure_cli_diff_tool.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2023-07-13 06:47:17.492990 azure-cli-diff-tool-0.0.2/setup.cfg
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1405 2023-07-13 06:47:11.000000 azure-cli-diff-tool-0.0.2/setup.py
```

### Comparing `azure-cli-diff-tool-0.0.1/PKG-INFO` & `azure-cli-diff-tool-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: azure-cli-diff-tool
-Version: 0.0.1
+Version: 0.0.2
 Summary: A tool for cli metadata management
 Author: Microsoft Corporation
 Author-email: azpycli@microsoft.com
 License: MIT
 
-Microsoft Azure CLI Diff Tools (azureCliDiffTool)
-=================================================
+Microsoft Azure CLI Diff Tools (azure-cli-diff-tool)
+=======================================================
 
-The ``azureCliDiffTool`` is designed to aid azure-cli users in diffing metadata files to see its updates through historical versions for Azure CLI command modules and extensions.
+The ``azure-cli-diff-tool`` is designed to aid azure-cli users in diffing metadata files to see its updates through historical versions for Azure CLI command modules and extensions.
 
 Setting up your environment
 +++++++++++++++++++++++++++++++++++++++
 
 1. Install Python 3.6+ from http://python.org. Please note that the version of Python that comes preinstalled on OSX is 2.7.
 
 3. Create a new virtual environment for Python in the root of your clone. You can do this by running:
@@ -48,15 +48,15 @@
 
     OSX/Linux (bash):
 
     ::
 
         source env/bin/activate
 
-5. Install ``azureCliDiffTool`` by running:
+5. Install ``azure-cli-diff-tool`` by running:
 
     ::
 
         pip install azure-cli-diff-tool
 
 Reporting issues and feedback
 +++++++++++++++++++++++++++++
@@ -74,15 +74,15 @@
 follow the instructions provided in `Microsoft Azure Projects Contribution Guidelines <http://azure.github.io/guidelines.html>`__.
 
 License
 +++++++
 
 ::
 
-    Azure CLI Diff Tools (azureCliDiffTool)
+    Azure CLI Diff Tools (azure-cli-diff-tool)
 
     Copyright (c) Microsoft Corporation
     All rights reserved.
 
     MIT License
 
     Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the ""Software""), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -92,11 +92,15 @@
     THE SOFTWARE IS PROVIDED *AS IS*, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.::
 
 
 .. :changelog:
 
 Release History
 ===============
+0.0.2
+++++++
+* Change time consuming into info log level
+* Adjust pkg name according to https://peps.python.org/pep-0008/#package-and-module-names
 
 0.0.1
 ++++++
 * Initial release
```

### Comparing `azure-cli-diff-tool-0.0.1/README.rst` & `azure-cli-diff-tool-0.0.2/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-Microsoft Azure CLI Diff Tools (azureCliDiffTool)
-=================================================
+Microsoft Azure CLI Diff Tools (azure-cli-diff-tool)
+=======================================================
 
-The ``azureCliDiffTool`` is designed to aid azure-cli users in diffing metadata files to see its updates through historical versions for Azure CLI command modules and extensions.
+The ``azure-cli-diff-tool`` is designed to aid azure-cli users in diffing metadata files to see its updates through historical versions for Azure CLI command modules and extensions.
 
 Setting up your environment
 +++++++++++++++++++++++++++++++++++++++
 
 1. Install Python 3.6+ from http://python.org. Please note that the version of Python that comes preinstalled on OSX is 2.7.
 
 3. Create a new virtual environment for Python in the root of your clone. You can do this by running:
@@ -40,15 +40,15 @@
 
     OSX/Linux (bash):
 
     ::
 
         source env/bin/activate
 
-5. Install ``azureCliDiffTool`` by running:
+5. Install ``azure-cli-diff-tool`` by running:
 
     ::
 
         pip install azure-cli-diff-tool
 
 Reporting issues and feedback
 +++++++++++++++++++++++++++++
@@ -66,15 +66,15 @@
 follow the instructions provided in `Microsoft Azure Projects Contribution Guidelines <http://azure.github.io/guidelines.html>`__.
 
 License
 +++++++
 
 ::
 
-    Azure CLI Diff Tools (azureCliDiffTool)
+    Azure CLI Diff Tools (azure-cli-diff-tool)
 
     Copyright (c) Microsoft Corporation
     All rights reserved.
 
     MIT License
 
     Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the ""Software""), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `azure-cli-diff-tool-0.0.1/azureCliDiffTool/__init__.py` & `azure-cli-diff-tool-0.0.2/azure_cli_diff_tool/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import logging
 from deepdiff import DeepDiff
 from .meta_change_detect import MetaChangeDetect
 from .utils import get_blob_config, load_blob_config_file, get_target_version_modules, get_target_version_module, \
     extract_module_name_from_meta_file, export_meta_changes_to_csv, export_meta_changes_to_json, \
     export_meta_changes_to_dict
 
-__VERSION__ = '0.0.1'
+__VERSION__ = '0.0.2'
 
 logger = logging.getLogger(__name__)
 
 
 class DiffExportFormat(Enum):
     DICT = "dict"
     TEXT = "text"
@@ -80,23 +80,23 @@
     download_base_start = time.time()
     if target_module:
         base_version_module_list = get_target_version_module(blob_url, path_prefix, base_version,
                                                              target_module, use_cache)
     else:
         base_version_module_list = get_target_version_modules(blob_url, path_prefix, index_file, base_version, use_cache)
     download_base_end = time.time()
-    print("base version {} meta files download using {} sec".format(base_version,
+    logger.info("base version {} meta files download using {} sec".format(base_version,
                                                                           download_base_end - download_base_start))
     if target_module:
         get_target_version_module(blob_url, path_prefix, diff_version,
                                   target_module, use_cache)
     else:
         get_target_version_modules(blob_url, path_prefix, index_file, diff_version, use_cache)
     download_target_end = time.time()
-    print("diff version {} meta files download using {} sec".format(diff_version,
+    logger.info("diff version {} meta files download using {} sec".format(diff_version,
                                                                           download_target_end - download_base_end))
     version_diffs = []
     for _, base_meta_file_full_path, base_meta_file in base_version_module_list:
         module_name = extract_module_name_from_meta_file(base_meta_file)
         if not module_name:
             continue
         if target_module and module_name != target_module:
@@ -125,11 +125,11 @@
         detected_changes.check_deep_diffs()
         diff_objs = detected_changes.export_meta_changes(only_break, "dict")
         mod_obj = {"module": module_name}
         for obj in diff_objs:
             obj.update(mod_obj)
             version_diffs.append(obj)
     meta_change_end = time.time()
-    print("meta file diffs using {} sec".format(meta_change_end - download_target_end))
+    logger.info("meta file diffs using {} sec".format(meta_change_end - download_target_end))
     if output_type == "dict":
         return export_meta_changes_to_dict(version_diffs, version_diff_file)
     return export_meta_changes_to_csv(version_diffs, version_diff_file)
```

### Comparing `azure-cli-diff-tool-0.0.1/azureCliDiffTool/_const.py` & `azure-cli-diff-tool-0.0.2/azure_cli_diff_tool/_const.py`

 * *Files identical despite different names*

### Comparing `azure-cli-diff-tool-0.0.1/azureCliDiffTool/data/meta_change_whitelist.txt` & `azure-cli-diff-tool-0.0.2/azure_cli_diff_tool/data/meta_change_whitelist.txt`

 * *Files identical despite different names*

### Comparing `azure-cli-diff-tool-0.0.1/azureCliDiffTool/meta_change.py` & `azure-cli-diff-tool-0.0.2/azure_cli_diff_tool/meta_change.py`

 * *Files identical despite different names*

### Comparing `azure-cli-diff-tool-0.0.1/azureCliDiffTool/meta_change_detect.py` & `azure-cli-diff-tool-0.0.2/azure_cli_diff_tool/meta_change_detect.py`

 * *Files identical despite different names*

### Comparing `azure-cli-diff-tool-0.0.1/azureCliDiffTool/utils.py` & `azure-cli-diff-tool-0.0.2/azure_cli_diff_tool/utils.py`

 * *Files identical despite different names*

### Comparing `azure-cli-diff-tool-0.0.1/azure_cli_diff_tool.egg-info/PKG-INFO` & `azure-cli-diff-tool-0.0.2/azure_cli_diff_tool.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: azure-cli-diff-tool
-Version: 0.0.1
+Version: 0.0.2
 Summary: A tool for cli metadata management
 Author: Microsoft Corporation
 Author-email: azpycli@microsoft.com
 License: MIT
 
-Microsoft Azure CLI Diff Tools (azureCliDiffTool)
-=================================================
+Microsoft Azure CLI Diff Tools (azure-cli-diff-tool)
+=======================================================
 
-The ``azureCliDiffTool`` is designed to aid azure-cli users in diffing metadata files to see its updates through historical versions for Azure CLI command modules and extensions.
+The ``azure-cli-diff-tool`` is designed to aid azure-cli users in diffing metadata files to see its updates through historical versions for Azure CLI command modules and extensions.
 
 Setting up your environment
 +++++++++++++++++++++++++++++++++++++++
 
 1. Install Python 3.6+ from http://python.org. Please note that the version of Python that comes preinstalled on OSX is 2.7.
 
 3. Create a new virtual environment for Python in the root of your clone. You can do this by running:
@@ -48,15 +48,15 @@
 
     OSX/Linux (bash):
 
     ::
 
         source env/bin/activate
 
-5. Install ``azureCliDiffTool`` by running:
+5. Install ``azure-cli-diff-tool`` by running:
 
     ::
 
         pip install azure-cli-diff-tool
 
 Reporting issues and feedback
 +++++++++++++++++++++++++++++
@@ -74,15 +74,15 @@
 follow the instructions provided in `Microsoft Azure Projects Contribution Guidelines <http://azure.github.io/guidelines.html>`__.
 
 License
 +++++++
 
 ::
 
-    Azure CLI Diff Tools (azureCliDiffTool)
+    Azure CLI Diff Tools (azure-cli-diff-tool)
 
     Copyright (c) Microsoft Corporation
     All rights reserved.
 
     MIT License
 
     Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the ""Software""), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -92,11 +92,15 @@
     THE SOFTWARE IS PROVIDED *AS IS*, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.::
 
 
 .. :changelog:
 
 Release History
 ===============
+0.0.2
+++++++
+* Change time consuming into info log level
+* Adjust pkg name according to https://peps.python.org/pep-0008/#package-and-module-names
 
 0.0.1
 ++++++
 * Initial release
```

### Comparing `azure-cli-diff-tool-0.0.1/setup.py` & `azure-cli-diff-tool-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 """Azure Command Diff Tools package that can be installed using setuptools"""
 import os
 import re
 from setuptools import setup, find_packages
 
 diff_tool_path = os.path.dirname(os.path.realpath(__file__))
-with open(os.path.join(diff_tool_path, 'azureCliDiffTool', '__init__.py'), 'r') as version_file:
+with open(os.path.join(diff_tool_path, 'azure_cli_diff_tool', '__init__.py'), 'r') as version_file:
     __VERSION__ = re.search(r'^__VERSION__\s*=\s*[\'"]([^\'"]*)[\'"]',
                             version_file.read(), re.MULTILINE).group(1)
 
 with open('README.rst', 'r', encoding='utf-8') as f:
     README = f.read()
 with open('HISTORY.rst', 'r', encoding='utf-8') as f:
     HISTORY = f.read()
@@ -28,10 +28,10 @@
       license='MIT',
       author='Microsoft Corporation',
       author_email='azpycli@microsoft.com',
       packages=find_packages(),
       include_package_data=True,
       install_requires=["deepdiff", "requests"],
       package_data={
-        "azureCliDiffTool": ["data/*"]
+        "azure_cli_diff_tool": ["data/*"]
       }
       )
```

