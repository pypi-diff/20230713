# Comparing `tmp/yetl-framework-1.6.6.dev5.tar.gz` & `tmp/yetl-framework-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-1.6.6.dev5.tar", last modified: Tue Jul 11 19:14:18 2023, max compression
+gzip compressed data, was "yetl-framework-1.7.0.tar", last modified: Thu Jul 13 18:34:37 2023, max compression
```

## Comparing `yetl-framework-1.6.6.dev5.tar` & `yetl-framework-1.7.0.tar`

### file list

```diff
@@ -1,46 +1,51 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-11 19:14:18.460569 yetl-framework-1.6.6.dev5/
--rw-r--r--   0 vsts      (1001) docker     (123)     1098 2023-07-11 19:14:18.460569 yetl-framework-1.6.6.dev5/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      596 2023-07-11 19:13:21.000000 yetl-framework-1.6.6.dev5/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-11 19:14:18.460569 yetl-framework-1.6.6.dev5/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1251 2023-07-11 19:13:21.000000 yetl-framework-1.6.6.dev5/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-11 19:14:18.456570 yetl-framework-1.6.6.dev5/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-07-11 19:13:21.000000 yetl-framework-1.6.6.dev5/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1141 2023-07-11 19:13:21.000000 yetl-framework-1.6.6.dev5/yetl/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-11 19:14:18.456570 yetl-framework-1.6.6.dev5/yetl/cli/
--rw-r--r--   0 vsts      (1001) docker     (123)     2845 2023-07-11 19:13:21.000000 yetl-framework-1.6.6.dev5/yetl/cli/_init.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-11 19:14:18.456570 yetl-framework-1.6.6.dev5/yetl/cli/metadata_provider/
--rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-07-11 19:13:21.000000 yetl-framework-1.6.6.dev5/yetl/cli/metadata_provider/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16742 2023-07-11 19:13:21.000000 yetl-framework-1.6.6.dev5/yetl/cli/metadata_provider/_xlsx.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-11 19:14:18.460569 yetl-framework-1.6.6.dev5/yetl/config/
--rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-07-11 19:13:21.000000 yetl-framework-1.6.6.dev5/yetl/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3284 2023-07-11 19:13:21.000000 yetl-framework-1.6.6.dev5/yetl/config/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2195 2023-07-11 19:13:21.000000 yetl-framework-1.6.6.dev5/yetl/config/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-07-11 19:13:21.000000 yetl-framework-1.6.6.dev5/yetl/config/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-07-11 19:13:21.000000 yetl-framework-1.6.6.dev5/yetl/config/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1309 2023-07-11 19:13:21.000000 yetl-framework-1.6.6.dev5/yetl/config/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-07-11 19:13:21.000000 yetl-framework-1.6.6.dev5/yetl/config/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-07-11 19:13:21.000000 yetl-framework-1.6.6.dev5/yetl/config/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10168 2023-07-11 19:13:21.000000 yetl-framework-1.6.6.dev5/yetl/config/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-07-11 19:13:21.000000 yetl-framework-1.6.6.dev5/yetl/config/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5064 2023-07-11 19:13:21.000000 yetl-framework-1.6.6.dev5/yetl/config/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17636 2023-07-11 19:13:21.000000 yetl-framework-1.6.6.dev5/yetl/config/deltalake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-11 19:14:18.460569 yetl-framework-1.6.6.dev5/yetl/config/table/
--rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-07-11 19:13:21.000000 yetl-framework-1.6.6.dev5/yetl/config/table/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4980 2023-07-11 19:13:21.000000 yetl-framework-1.6.6.dev5/yetl/config/table/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-07-11 19:13:21.000000 yetl-framework-1.6.6.dev5/yetl/config/table/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6603 2023-07-11 19:13:21.000000 yetl-framework-1.6.6.dev5/yetl/config/table/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4712 2023-07-11 19:13:21.000000 yetl-framework-1.6.6.dev5/yetl/config/table/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-07-11 19:13:21.000000 yetl-framework-1.6.6.dev5/yetl/config/table/_table_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-07-11 19:13:21.000000 yetl-framework-1.6.6.dev5/yetl/config/table/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-11 19:14:18.460569 yetl-framework-1.6.6.dev5/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      167 2023-07-11 19:13:21.000000 yetl-framework-1.6.6.dev5/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1312 2023-07-11 19:13:21.000000 yetl-framework-1.6.6.dev5/yetl/workflow/_dlt.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-07-11 19:13:21.000000 yetl-framework-1.6.6.dev5/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-07-11 19:13:21.000000 yetl-framework-1.6.6.dev5/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-11 19:14:18.460569 yetl-framework-1.6.6.dev5/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     1098 2023-07-11 19:14:18.000000 yetl-framework-1.6.6.dev5/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      999 2023-07-11 19:14:18.000000 yetl-framework-1.6.6.dev5/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-11 19:14:18.000000 yetl-framework-1.6.6.dev5/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-11 19:14:18.000000 yetl-framework-1.6.6.dev5/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       73 2023-07-11 19:14:18.000000 yetl-framework-1.6.6.dev5/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-07-11 19:14:18.000000 yetl-framework-1.6.6.dev5/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 18:34:37.933685 yetl-framework-1.7.0/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1094 2023-07-13 18:34:37.933685 yetl-framework-1.7.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      596 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-13 18:34:37.933685 yetl-framework-1.7.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1237 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 18:34:37.929685 yetl-framework-1.7.0/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1141 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 18:34:37.929685 yetl-framework-1.7.0/yetl/_resources/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/_resources/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      299 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/_resources/logging.yaml
+-rw-r--r--   0 vsts      (1001) docker     (123)      500 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/_resources/project.yaml
+-rw-r--r--   0 vsts      (1001) docker     (123)    14649 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/_resources/sibytes_yetl_pipeline_schema.json
+-rw-r--r--   0 vsts      (1001) docker     (123)     2654 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/_resources/sibytes_yetl_project_schema.json
+-rw-r--r--   0 vsts      (1001) docker     (123)    14649 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/_resources/sibytes_yetl_tables_schema.json
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 18:34:37.933685 yetl-framework-1.7.0/yetl/config/
+-rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3362 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/config/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2195 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/config/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/config/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/config/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1309 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/config/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/config/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/config/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10168 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/config/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/config/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5064 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/config/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17636 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/config/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 18:34:37.933685 yetl-framework-1.7.0/yetl/config/table/
+-rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/config/table/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4980 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/config/table/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/config/table/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6603 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/config/table/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4712 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/config/table/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/config/table/_table_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/config/table/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 18:34:37.933685 yetl-framework-1.7.0/yetl/validation/
+-rw-r--r--   0 vsts      (1001) docker     (123)      353 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/validation/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1555 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/validation/_validate.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 18:34:37.933685 yetl-framework-1.7.0/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      167 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1312 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/workflow/_dlt.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-07-13 18:33:32.000000 yetl-framework-1.7.0/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-13 18:34:37.933685 yetl-framework-1.7.0/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1094 2023-07-13 18:34:37.000000 yetl-framework-1.7.0/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1262 2023-07-13 18:34:37.000000 yetl-framework-1.7.0/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-13 18:34:37.000000 yetl-framework-1.7.0/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-13 18:34:37.000000 yetl-framework-1.7.0/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       92 2023-07-13 18:34:37.000000 yetl-framework-1.7.0/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-07-13 18:34:37.000000 yetl-framework-1.7.0/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-1.6.6.dev5/PKG-INFO` & `yetl-framework-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.6.6.dev5
+Version: 1.7.0
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 
 # What Is Yetl
 
 Website: https://www.yetl.io/
```

### Comparing `yetl-framework-1.6.6.dev5/README.md` & `yetl-framework-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev5/setup.py` & `yetl-framework-1.7.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,44 @@
 import pathlib
-from setuptools import setup
+from setuptools import setup, find_packages
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="1.6.6.dev5",
+    version="1.7.0",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
     },
     author="Shaun Ryan",
     author_email="shaun_chiburi@hotmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
-    ],
-    packages=[
-        "yetl",
-        "yetl.cli",
-        "yetl.cli.metadata_provider",
-        "yetl.config",
-        "yetl.config.table",
-        "yetl.workflow",
-
+        "Programming Language :: Python :: 3.10",
     ],
+    package_dir={"": "."},
+    packages=find_packages(),
+    package_data={"yetl._resources": ["*.json", "*.yaml"]},
     install_requires=[
           'PyYAML',
           'jinja2',
           'pydantic==1.10.6',
+          'jsonschema==4.16.0',
           'typer',
           'pandas',
           'openpyxl',
           'delta-spark',
           'pyspark'
       ],
     zip_safe=False
```

### Comparing `yetl-framework-1.6.6.dev5/yetl/__main__.py` & `yetl-framework-1.7.0/yetl/__main__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev5/yetl/config/__init__.py` & `yetl-framework-1.7.0/yetl/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev5/yetl/config/_config.py` & `yetl-framework-1.7.0/yetl/config/_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from ._timeslice import Timeslice
 from ._tables import Tables, _INDEX_WILDCARD, KeyContants
 from ._stage_type import StageType
 from ._utils import abs_config_path, load_yaml, get_config_path, check_version
 from ._logging_config import configure_logging
 import logging
 from ._project import Project
+from ..validation import validate_tables
 
 
 class Config:
     def __init__(
         self,
         project: str,
         pipeline: str,
@@ -44,16 +45,18 @@
         return pipeline
 
     def _load_tables(self, timeslice: Timeslice):
         tables_config = self._load_pipeline(self.pipeline)
         tables_path = tables_config[KeyContants.TABLES.value]
         tables_path = abs_config_path(self.project.pipelines, tables_path)
 
-        data = load_yaml(tables_path)
+        data: dict = load_yaml(tables_path)
+        validate_tables(data)
         check_version(data)
+
         tables_config[KeyContants.TABLES.value] = data
         tables_config[KeyContants.TIMESLICE.value] = timeslice
         tables_config[KeyContants.CONFIG_PATH.value] = self.project.pipelines
         tables_config[KeyContants.PROJECT.value] = self.project
 
         tables = Tables(table_data=tables_config)
         return tables
```

### Comparing `yetl-framework-1.6.6.dev5/yetl/config/_decorators.py` & `yetl-framework-1.7.0/yetl/config/_decorators.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev5/yetl/config/_logging_config.py` & `yetl-framework-1.7.0/yetl/config/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev5/yetl/config/_project.py` & `yetl-framework-1.7.0/yetl/config/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev5/yetl/config/_spark_context.py` & `yetl-framework-1.7.0/yetl/config/_spark_context.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev5/yetl/config/_tables.py` & `yetl-framework-1.7.0/yetl/config/_tables.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev5/yetl/config/_timeslice.py` & `yetl-framework-1.7.0/yetl/config/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev5/yetl/config/_utils.py` & `yetl-framework-1.7.0/yetl/config/_utils.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev5/yetl/config/deltalake.py` & `yetl-framework-1.7.0/yetl/config/deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev5/yetl/config/table/_deltalake.py` & `yetl-framework-1.7.0/yetl/config/table/_deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev5/yetl/config/table/_factory.py` & `yetl-framework-1.7.0/yetl/config/table/_factory.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev5/yetl/config/table/_read.py` & `yetl-framework-1.7.0/yetl/config/table/_read.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev5/yetl/config/table/_table.py` & `yetl-framework-1.7.0/yetl/config/table/_table.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev5/yetl/workflow/_dlt.py` & `yetl-framework-1.7.0/yetl/workflow/_dlt.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev5/yetl/workflow/_multi_threaded.py` & `yetl-framework-1.7.0/yetl/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.6.6.dev5/yetl_framework.egg-info/PKG-INFO` & `yetl-framework-1.7.0/yetl_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.6.6.dev5
+Version: 1.7.0
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 
 # What Is Yetl
 
 Website: https://www.yetl.io/
```

### Comparing `yetl-framework-1.6.6.dev5/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-1.7.0/yetl_framework.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 README.md
 setup.py
-yetl/__init__.py
-yetl/__main__.py
-yetl/cli/_init.py
-yetl/cli/metadata_provider/__init__.py
-yetl/cli/metadata_provider/_xlsx.py
-yetl/config/__init__.py
-yetl/config/_config.py
-yetl/config/_decorators.py
-yetl/config/_logging_config.py
-yetl/config/_project.py
-yetl/config/_spark_context.py
-yetl/config/_stage_type.py
-yetl/config/_table_mapping.py
-yetl/config/_tables.py
-yetl/config/_timeslice.py
-yetl/config/_utils.py
-yetl/config/deltalake.py
-yetl/config/table/__init__.py
-yetl/config/table/_deltalake.py
-yetl/config/table/_factory.py
-yetl/config/table/_read.py
-yetl/config/table/_table.py
-yetl/config/table/_table_type.py
-yetl/config/table/_write.py
-yetl/workflow/__init__.py
-yetl/workflow/_dlt.py
-yetl/workflow/_multi_threaded.py
-yetl/workflow/_notebook.py
+./yetl/__init__.py
+./yetl/__main__.py
+./yetl/_resources/__init__.py
+./yetl/_resources/logging.yaml
+./yetl/_resources/project.yaml
+./yetl/_resources/sibytes_yetl_pipeline_schema.json
+./yetl/_resources/sibytes_yetl_project_schema.json
+./yetl/_resources/sibytes_yetl_tables_schema.json
+./yetl/config/__init__.py
+./yetl/config/_config.py
+./yetl/config/_decorators.py
+./yetl/config/_logging_config.py
+./yetl/config/_project.py
+./yetl/config/_spark_context.py
+./yetl/config/_stage_type.py
+./yetl/config/_table_mapping.py
+./yetl/config/_tables.py
+./yetl/config/_timeslice.py
+./yetl/config/_utils.py
+./yetl/config/deltalake.py
+./yetl/config/table/__init__.py
+./yetl/config/table/_deltalake.py
+./yetl/config/table/_factory.py
+./yetl/config/table/_read.py
+./yetl/config/table/_table.py
+./yetl/config/table/_table_type.py
+./yetl/config/table/_write.py
+./yetl/validation/__init__.py
+./yetl/validation/_validate.py
+./yetl/workflow/__init__.py
+./yetl/workflow/_dlt.py
+./yetl/workflow/_multi_threaded.py
+./yetl/workflow/_notebook.py
 yetl_framework.egg-info/PKG-INFO
 yetl_framework.egg-info/SOURCES.txt
 yetl_framework.egg-info/dependency_links.txt
 yetl_framework.egg-info/not-zip-safe
 yetl_framework.egg-info/requires.txt
 yetl_framework.egg-info/top_level.txt
```

