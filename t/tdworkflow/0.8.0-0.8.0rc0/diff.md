# Comparing `tmp/tdworkflow-0.8.0.tar.gz` & `tmp/tdworkflow-0.8.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdworkflow-0.8.0.tar", last modified: Wed May 31 17:57:00 2023, max compression
+gzip compressed data, was "tdworkflow-0.8.0rc0.tar", last modified: Wed May 31 04:08:05 2023, max compression
```

## Comparing `tdworkflow-0.8.0.tar` & `tdworkflow-0.8.0rc0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:57:00.709496 tdworkflow-0.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:57:00.701496 tdworkflow-0.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:57:00.705496 tdworkflow-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/.github/workflows/pythonapp.yml
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-05-31 17:57:00.709496 tdworkflow-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:57:00.705496 tdworkflow-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:57:00.705496 tdworkflow-0.8.0/docs/references/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/docs/references/client.rst
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/docs/references/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/docs/references/misc.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/docs/references/model.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-31 17:57:00.709496 tdworkflow-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:57:00.709496 tdworkflow-0.8.0/tdworkflow/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/tdworkflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/tdworkflow/attempt.py
--rw-r--r--   0 runner    (1001) docker     (123)    39145 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/tdworkflow/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/tdworkflow/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/tdworkflow/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/tdworkflow/project.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/tdworkflow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/tdworkflow/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/tdworkflow/revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/tdworkflow/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/tdworkflow/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/tdworkflow/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/tdworkflow/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/tdworkflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:57:00.709496 tdworkflow-0.8.0/tdworkflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-05-31 17:57:00.000000 tdworkflow-0.8.0/tdworkflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-31 17:57:00.000000 tdworkflow-0.8.0/tdworkflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 17:57:00.000000 tdworkflow-0.8.0/tdworkflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-31 17:57:00.000000 tdworkflow-0.8.0/tdworkflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 17:57:00.000000 tdworkflow-0.8.0/tdworkflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:57:00.709496 tdworkflow-0.8.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:57:00.705496 tdworkflow-0.8.0/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:57:00.709496 tdworkflow-0.8.0/tests/resources/sample_project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/tests/resources/sample_project/.digdag
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:57:00.709496 tdworkflow-0.8.0/tests/resources/sample_project/ignore_dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/tests/resources/sample_project/ignore_dir/dummy
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/tests/resources/sample_project/main.dig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:57:00.709496 tdworkflow-0.8.0/tests/resources/sample_project/py_scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:57:00.709496 tdworkflow-0.8.0/tests/resources/sample_project/py_scripts/__ignoredir__/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/tests/resources/sample_project/py_scripts/__ignoredir__/dummy
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/tests/resources/sample_project/py_scripts/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)    24529 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-31 17:56:44.000000 tdworkflow-0.8.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:08:05.928309 tdworkflow-0.8.0rc0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:08:05.920309 tdworkflow-0.8.0rc0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:08:05.924309 tdworkflow-0.8.0rc0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/.github/workflows/pythonapp.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-05-31 04:08:05.928309 tdworkflow-0.8.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:08:05.924309 tdworkflow-0.8.0rc0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:08:05.924309 tdworkflow-0.8.0rc0/docs/references/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/docs/references/client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/docs/references/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/docs/references/misc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/docs/references/model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-31 04:08:05.928309 tdworkflow-0.8.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:08:05.928309 tdworkflow-0.8.0rc0/tdworkflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tdworkflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tdworkflow/attempt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37083 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tdworkflow/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tdworkflow/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tdworkflow/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tdworkflow/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tdworkflow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tdworkflow/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tdworkflow/revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tdworkflow/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tdworkflow/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tdworkflow/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tdworkflow/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tdworkflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:08:05.928309 tdworkflow-0.8.0rc0/tdworkflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-05-31 04:08:05.000000 tdworkflow-0.8.0rc0/tdworkflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-31 04:08:05.000000 tdworkflow-0.8.0rc0/tdworkflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 04:08:05.000000 tdworkflow-0.8.0rc0/tdworkflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-31 04:08:05.000000 tdworkflow-0.8.0rc0/tdworkflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 04:08:05.000000 tdworkflow-0.8.0rc0/tdworkflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:08:05.928309 tdworkflow-0.8.0rc0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:08:05.920309 tdworkflow-0.8.0rc0/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:08:05.928309 tdworkflow-0.8.0rc0/tests/resources/sample_project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tests/resources/sample_project/.digdag
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:08:05.928309 tdworkflow-0.8.0rc0/tests/resources/sample_project/ignore_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tests/resources/sample_project/ignore_dir/dummy
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tests/resources/sample_project/main.dig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:08:05.928309 tdworkflow-0.8.0rc0/tests/resources/sample_project/py_scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:08:05.928309 tdworkflow-0.8.0rc0/tests/resources/sample_project/py_scripts/__ignoredir__/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tests/resources/sample_project/py_scripts/__ignoredir__/dummy
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tests/resources/sample_project/py_scripts/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24529 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-31 04:07:48.000000 tdworkflow-0.8.0rc0/tests/test_util.py
```

### Comparing `tdworkflow-0.8.0/.github/workflows/pythonapp.yml` & `tdworkflow-0.8.0rc0/.github/workflows/pythonapp.yml`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.0/.github/workflows/pythonpublish.yml` & `tdworkflow-0.8.0rc0/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.0/.gitignore` & `tdworkflow-0.8.0rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.0/.readthedocs.yml` & `tdworkflow-0.8.0rc0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.0/CHANGES.rst` & `tdworkflow-0.8.0rc0/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.0/LICENSE` & `tdworkflow-0.8.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.0/PKG-INFO` & `tdworkflow-0.8.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdworkflow
-Version: 0.8.0
+Version: 0.8.0rc0
 Summary: Unofficial Treasure Workflow API client
 Home-page: https://github.com/chezou/tdworkflow
 Author: Aki Ariga
 Author-email: chezou@gmail.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `tdworkflow-0.8.0/README.rst` & `tdworkflow-0.8.0rc0/README.rst`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.0/docs/Makefile` & `tdworkflow-0.8.0rc0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.0/docs/conf.py` & `tdworkflow-0.8.0rc0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.0/docs/make.bat` & `tdworkflow-0.8.0rc0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.0/docs/references/model.rst` & `tdworkflow-0.8.0rc0/docs/references/model.rst`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.0/setup.cfg` & `tdworkflow-0.8.0rc0/setup.cfg`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.0/tdworkflow/attempt.py` & `tdworkflow-0.8.0rc0/tdworkflow/attempt.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,27 +24,24 @@
     params: Optional[Dict[str, Any]] = None
     createdAt: Optional[datetime] = None
     finishedAt: Optional[datetime] = None
     status: str = ""
 
     def __post_init__(self) -> None:
         self.id = int(self.id)
-        if self.sessionTime and isinstance(self.sessionTime, str):
-            self.sessionTime = parse_iso8601(self.sessionTime)
+        self.sessionTime = parse_iso8601(self.sessionTime)  # type: ignore
         if self.project and isinstance(self.project, dict):
             self.project = Project(**self.project)
         if self.workflow and isinstance(self.workflow, dict):
             self.workflow = Workflow(**self.workflow)
         self.done = bool(self.done)
         self.success = bool(self.success)
         self.cancelRequested = bool(self.cancelRequested)
-        if self.createdAt and isinstance(self.createdAt, str):
-            self.createdAt = parse_iso8601(self.createdAt)
-        if self.finishedAt and isinstance(self.finishedAt, str):
-            self.finishedAt = parse_iso8601(self.finishedAt)
+        self.createdAt = parse_iso8601(self.createdAt)  # type: ignore
+        self.finishedAt = parse_iso8601(self.finishedAt)  # type: ignore
         self.status = self.status
 
     @property
     def session_id(self) -> int:
         return self.sessionId
 
     @property
```

### Comparing `tdworkflow-0.8.0/tdworkflow/client.py` & `tdworkflow-0.8.0rc0/tdworkflow/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import os
 import time
 import uuid
 from datetime import datetime
 from typing import Any, BinaryIO, Callable, Dict, List, Optional, Tuple, Union, cast
 
 import requests
-from mypy_extensions import DefaultArg
 from requests.adapters import HTTPAdapter
 from urllib3.util.retry import Retry
 
 import tdworkflow
 
 from . import exceptions
 from .attempt import Attempt
@@ -24,25 +23,17 @@
 from .session import Session
 from .task import Task
 from .util import archive_files, to_iso8601
 from .workflow import Workflow
 
 logger = logging.getLogger(__name__)
 
-GetResponse = Union[Dict[str, Any], bytes]
-PostResponse = Optional[Union[Dict[str, Any], bytes]]
-PutResponse = Optional[Dict[str, Any]]
-DeleteResponse = Optional[Dict[str, Any]]
-Params = Dict[str, Union[str, bool, int, None]]
-DataType = Union[str, Dict[str, Any], List[Tuple[Any]], BinaryIO]
-ListOfDict = Dict[str, List[Dict[str, Any]]]
-
 
 class WorkflowAPI:
-    get: Callable[[str, DefaultArg(Params, "params")], GetResponse]
+    get: Callable
 
     def workflows(
         self,
         name_pattern: Optional[str] = None,
         search_project_name: bool = False,
         order: Optional[str] = None,
         count: Optional[int] = None,
@@ -70,57 +61,47 @@
             params["search_project_name"] = search_project_name
         if order:
             params["order"] = order
         if count:
             params["count"] = count
         if last_id:
             params["last_id"] = last_id
-        res = cast(ListOfDict, self.get("workflows", params=params))
+        res = self.get("workflows", params=params)
         if len(res) > 0:
             return [Workflow.from_api_repr(**wf) for wf in res["workflows"]]
         else:
             return []
 
     def workflow(self, workflow: Union[int, Workflow]) -> Workflow:
         """Get a specific workflow
 
         :param workflow: Id for workflow or Workflow object
         :type workflow: Union[int, Workflow]
         :return: A workflow
         :rtype: Workflow
         """
         workflow_id = workflow.id if isinstance(workflow, Workflow) else workflow
-        res = cast(Dict[str, Any], self.get(f"workflows/{workflow_id}"))
+        res = self.get(f"workflows/{workflow_id}")
         return Workflow.from_api_repr(**res)
 
 
 class ProjectAPI:
-    get: Callable[
-        [str, DefaultArg(Params, "params"), DefaultArg(bool, "content")], GetResponse
-    ]
-    put: Callable[
-        [
-            str,
-            DefaultArg(DataType, "data"),
-            DefaultArg(Dict[str, Any], "_json"),
-            DefaultArg(Dict[str, str], "params"),
-        ],
-        PutResponse,
-    ]
-    delete: Callable[[Any], DeleteResponse]
+    get: Callable
+    put: Callable
+    delete: Callable
 
     def project(self, project: Union[int, Project]) -> Project:
         """Get a project
 
         :param project: Project id or Project object
         :type project: Union[int, Project]
         :return: A Project
         """
         project_id = project.id if isinstance(project, Project) else project
-        r = cast(Dict[str, Any], self.get(f"projects/{project_id}"))
+        r = self.get(f"projects/{project_id}")
         return Project.from_api_repr(**r)
 
     def projects(
         self,
         name: Optional[str] = None,
         name_pattern: Optional[str] = None,
         count: Optional[int] = None,
@@ -145,15 +126,15 @@
         if name_pattern:
             params["name_pattern"] = name_pattern
         if count:
             params["count"] = count
         if last_id:
             params["last_id"] = last_id
 
-        res = cast(ListOfDict, self.get("projects", params=params))
+        res = self.get("projects", params=params)
         if res:
             return [Project.from_api_repr(**proj) for proj in res["projects"]]
         else:
             return []
 
     def project_workflows(
         self,
@@ -177,17 +158,15 @@
             workflow_name = (
                 workflow.name if isinstance(workflow, Workflow) else workflow
             )
             params["workflow"] = workflow_name
         if revision:
             params["revision"] = revision
         project_id = project.id if isinstance(project, Project) else project
-        r = cast(
-            ListOfDict, self.get(f"projects/{project_id}/workflows", params=params)
-        )
+        r = self.get(f"projects/{project_id}/workflows", params=params)
         if r:
             return [Workflow.from_api_repr(**wf) for wf in r["workflows"]]
         else:
             return []
 
     def create_project(
         self,
@@ -219,15 +198,15 @@
             ".pyc",
         ]
         if exclude_patterns:
             exclude_patterns.extend(default_excludes)
         else:
             exclude_patterns = default_excludes
         data = archive_files(target_dir, exclude_patterns)
-        r = cast(Dict[str, Any], self.put("projects", params=params, data=data))
+        r = self.put("projects", params=params, data=data)
 
         if r:
             return Project.from_api_repr(**r)
         else:
             raise ValueError("Unable to crate project")
 
     def delete_project(self, project: Union[int, Project]) -> bool:
@@ -252,20 +231,17 @@
         """Download a project and save as a file (tar.gz)
 
         :param project: Project id or Project object
         :param file_path: Target file path to be saved in tar.gz
         :param revision: Revision name
         :return: ``True`` if succeeded
         """
-        params = {"revision": revision} if revision else {}  # type: Params
+        params = {"revision": revision} if revision else {}
         project_id = project.id if isinstance(project, Project) else project
-        res = cast(
-            bytes,
-            self.get(f"projects/{project_id}/archive", params=params, content=True),
-        )
+        res = self.get(f"projects/{project_id}/archive", params=params, content=True)
 
         # File will be downloaded as tar.gz format
         with open(file_path, "wb") as f:
             f.write(res)
 
         return True
 
@@ -284,15 +260,15 @@
     def project_revisions(self, project: Union[int, Project]) -> List[Revision]:
         """List revisions associated with Project
 
         :param project: Project id or Project object
         :return: List of Revision
         """
         project_id = project.id if isinstance(project, Project) else project
-        res = cast(ListOfDict, self.get(f"projects/{project_id}/revisions"))
+        res = self.get(f"projects/{project_id}/revisions")
         if res:
             return [Revision.from_api_repr(**rev) for rev in res["revisions"]]
         else:
             return []
 
     def project_schedules(
         self,
@@ -312,17 +288,15 @@
             workflow_name = (
                 workflow.name if isinstance(workflow, Workflow) else workflow
             )
             params["workflow"] = workflow_name
         if last_id:
             params["last_id"] = last_id
         project_id = project.id if isinstance(project, Project) else project
-        res = cast(
-            ListOfDict, self.get(f"projects/{project_id}/schedules", params=params)
-        )
+        res = self.get(f"projects/{project_id}/schedules", params=params)
         if res:
             return [Schedule.from_api_repr(**s) for s in res["schedules"]]
         else:
             return []
 
     def set_secrets(
         self, project: Union[int, Project], secrets: Dict[str, str]
@@ -354,17 +328,15 @@
 
         :param project: Project ID or Project object
         :type project: Union[int, Project]
         :return: The list of secret keys
         :rtype: List[str]
         """
         project_id = project.id if isinstance(project, Project) else project
-        r = cast(
-            Dict[str, List[Dict[str, str]]], self.get(f"projects/{project_id}/secrets/")
-        )
+        r = self.get(f"projects/{project_id}/secrets/")
         if r is None or len(r) == 0:
             return []
         else:
             return [e["key"] for e in r["secrets"]]
 
     def delete_secret(self, project: Union[int, Project], key: str) -> bool:
         """Delete secret key
@@ -434,35 +406,25 @@
             )
             params["workflow"] = workflow_name
         if last_id:
             params["last_id"] = last_id
         if page_size:
             params["page_size"] = page_size
         project_id = project.id if isinstance(project, Project) else project
-        r = cast(ListOfDict, self.get(f"projects/{project_id}/sessions"))
+        r = self.get(f"projects/{project_id}/sessions")
         if r:
             return [Session.from_api_repr(**s) for s in r["sessions"]]
         else:
             return []
 
 
 class AttemptAPI:
-    get: Callable[[str, DefaultArg(Params, "params")], GetResponse]
-    put: Callable[
-        [
-            str,
-            DefaultArg(DataType, "data"),
-            DefaultArg(Dict[str, Any], "_json"),
-            DefaultArg(Dict[str, str], "params"),
-        ],
-        PutResponse,
-    ]
-    post: Callable[
-        [str, DefaultArg(Any, "body"), DefaultArg(bool, "content")], PostResponse
-    ]
+    get: Callable
+    put: Callable
+    post: Callable
 
     def attempts(
         self,
         project: Optional[Union[str, Project]] = None,
         workflow: Optional[Union[str, Workflow]] = None,
         include_retried: Optional[bool] = None,
         last_id: Optional[int] = None,
@@ -495,15 +457,15 @@
         if include_retried:
             params.update({"include_retried": include_retried})
         if last_id:
             params.update({"last_id": last_id})
         if page_size:
             params.update({"page_size": page_size})
 
-        r = cast(Optional[ListOfDict], self.get("attempts", params=params))
+        r = self.get("attempts", params=params)
         res = (
             [Attempt.from_api_repr(**attempt) for attempt in r["attempts"]] if r else []
         )
         return res
 
     def attempt(
         self, attempt: Union[int, Attempt], inplace: bool = False
@@ -513,15 +475,15 @@
         :param attempt: Attempt ID or Attempt object
         :type attempt: int
         :param inplace: If True, do operation inplace and return None
         :return: Attempt object
         :rtype: :class:`Attempt`
         """
         attempt_id = attempt.id if isinstance(attempt, Attempt) else attempt
-        r = cast(Dict[str, Any], self.get(f"attempts/{attempt_id}"))
+        r = self.get(f"attempts/{attempt_id}")
         if not r:
             raise ValueError(f"Unable to find attempt id {attempt_id}")
 
         if inplace:
             if isinstance(attempt, int):
                 raise ValueError(f"Unable to use inplace with integer value {attempt=}")
             else:
@@ -534,27 +496,27 @@
         """Get tasks of a session
 
         :param attempt: Attempt id or Attempt object
         :return: List of :class:`Task`
         """
 
         attempt_id = attempt.id if isinstance(attempt, Attempt) else attempt
-        r = cast(Optional[ListOfDict], self.get(f"attempts/{attempt_id}/tasks"))
+        r = self.get(f"attempts/{attempt_id}/tasks")
         res = [Task.from_api_repr(**task) for task in r["tasks"]] if r else []
         return res
 
     def retried_attempts(self, attempt: Union[int, Attempt]) -> List[Attempt]:
         """Get retried attempt list
 
         :param attempt: Attempt id or Attempt object
         :return: List of Attempt
         """
 
         attempt_id = attempt.id if isinstance(attempt, Attempt) else attempt
-        r = cast(Optional[ListOfDict], self.get(f"attempts/{attempt_id}/retries"))
+        r = self.get(f"attempts/{attempt_id}/retries")
         res = [Attempt(**attempt) for attempt in r["attempts"]] if r else []
         return res
 
     def start_attempt(
         self,
         workflow: Union[int, Workflow],
         session_time: Optional[str] = None,
@@ -566,15 +528,17 @@
         :param workflow: Workflow id or Workflow object
         :param session_time: Session time, optional Default: ``datetime.datetime.now()``
         :param retry_attempt_name: Retry attempt name, optional
         :param workflow_params: Extra workflow parameters
         :return:
         """
         workflow_id = workflow.id if isinstance(workflow, Workflow) else workflow
-        _params = {"workflowId": workflow_id}  # type: Dict[str, Any]
+        _params = {
+            "workflowId": workflow_id
+        }  # type: Dict[str, Union[str, int, Dict, None]]
         workflow_params = workflow_params if workflow_params else {}
         _params.update({"params": workflow_params})
         if not session_time:
             session_time = to_iso8601(datetime.now())
         if retry_attempt_name:
             _params.update({"retryAttemptName": retry_attempt_name})
 
@@ -623,39 +587,37 @@
             time.sleep(wait_interval)
             self.attempt(attempt, inplace=True)
 
         return attempt
 
 
 class ScheduleAPI:
-    get: Callable[[str, DefaultArg(Params, "params")], GetResponse]
-    post: Callable[
-        [str, DefaultArg(Any, "body"), DefaultArg(bool, "content")], PostResponse
-    ]
+    get: Callable
+    post: Callable
 
     def schedules(self, last_id: Optional[int] = None) -> List[Schedule]:
         """List schedules
 
         :param last_id: List schedules whose id is grater than this id for pagination.
         :return: List of Schedule
         """
-        r = cast(ListOfDict, self.get("schedules", params={"last_id": last_id}))
+        r = self.get("schedules", params={"last_id": last_id})
         if r:
             return [Schedule.from_api_repr(**s) for s in r["schedules"]]
         else:
             return []
 
     def schedule(self, schedule: Union[int, Schedule]) -> Schedule:
         """Get a schedule
 
         :param schedule: Schedule id or Schedule object
         :return: Schedule
         """
         schedule_id = schedule.id if isinstance(schedule, Schedule) else schedule
-        r = cast(Dict[str, Any], self.get(f"schedules/{schedule_id}"))
+        r = self.get(f"schedules/{schedule_id}")
         if r:
             return Schedule.from_api_repr(**r)
         else:
             raise ValueError(f"Unable to find schedule id: {schedule_id}")
 
     def backfill_schedule(
         self,
@@ -681,43 +643,41 @@
         if attempt_name:
             params["attemptName"] = attempt_name
         if count:
             params["count"] = count
         params["dryRun"] = dry_run
 
         schedule_id = schedule.id if isinstance(schedule, Schedule) else schedule
-        r = cast(
-            Dict[str, Any], self.post(f"schedules/{schedule_id}/backfill", body=params)
-        )
+        r = self.post(f"schedules/{schedule_id}/backfill", body=params)
         if r:
             return ScheduleAttempt.from_api_repr(**r)
         else:
             raise ValueError(f"Unable to backfill for schedule: {schedule_id}")
 
     def disable_schedule(self, schedule: Union[int, Schedule]) -> Schedule:
         """Disable a schedule
 
         :param schedule: Schedule ID or Schedule object
         :return: New Schedule
         """
         schedule_id = schedule.id if isinstance(schedule, Schedule) else schedule
-        r = cast(Dict[str, Any], self.post(f"schedules/{schedule_id}/disable"))
+        r = self.post(f"schedules/{schedule_id}/disable")
         if r:
             return Schedule.from_api_repr(**r)
         else:
             raise ValueError(f"Unable to disable schedule id: {schedule_id}")
 
     def enable_schedule(self, schedule: Union[int, Schedule]) -> Schedule:
         """Enable a schedule
 
         :param schedule: Schedule ID or Schedule object
         :return: New Schedule
         """
         schedule_id = schedule.id if isinstance(schedule, Schedule) else schedule
-        r = cast(Dict[str, Any], self.post(f"schedules/{schedule_id}/enable"))
+        r = self.post(f"schedules/{schedule_id}/enable")
         if r:
             return Schedule.from_api_repr(**r)
         else:
             raise ValueError(f"Unable to enable schedule id: {schedule_id}")
 
     def skip_schedule(
         self,
@@ -741,42 +701,40 @@
             params["fromTime"] = to_iso8601(from_time)
         if next_time:
             params["nextTime"] = next_time
         if next_run_time:
             params["nextRunTime"] = to_iso8601(next_run_time)
         params["dryRun"] = dry_run
         schedule_id = schedule.id if isinstance(schedule, Schedule) else schedule
-        r = cast(
-            Dict[str, Any], self.post(f"schedules/{schedule_id}/skip", body=params)
-        )
+        r = self.post(f"schedules/{schedule_id}/skip", body=params)
         if r:
             return Schedule.from_api_repr(**r)
         else:
             raise ValueError(f"Unable to skip schedule id: {schedule_id}")
 
 
 class SessionAPI:
-    get: Callable[[str, DefaultArg(Params, "params"), DefaultArg(bool, "content")], Any]
+    get: Callable
 
     def sessions(
         self, last_id: Optional[int] = None, page_size: Optional[int] = None
     ) -> List[Session]:
         """List sessions
 
         :param last_id: List sessions whose id is grater than this id for pagination
         :param page_size: Number of sessions to return
         :return: List of Session
         """
-        params = {}  # type: Params
+        params = {}
         if last_id:
             params["last_id"] = last_id
         if page_size:
             params["page_size"] = page_size
 
-        r = cast(ListOfDict, self.get("sessions", params=params))
+        r = self.get("sessions", params=params)
         if r:
             return [Session(**s) for s in r["sessions"]]
         else:
             return []
 
     def session(self, session: Union[int, Session]) -> Session:
         """Get a session
@@ -800,32 +758,30 @@
         """Get attempts of a session
 
         :param session: Session ID or Session object
         :param last_id: List attempts whose id is grater than this id for pagination
         :param page_size: Number of attempts to return
         :return: List of Attempt
         """
-        params = {}  # type: Params
+        params = {}
         if last_id:
             params["last_id"] = last_id
         if page_size:
             params["page_size"] = page_size
 
         session_id = session.id if isinstance(session, Session) else session
         r = self.get(f"sessions/{session_id}/attempts", params=params)
         if r:
             return [Attempt.from_api_repr(**e) for e in r["attempts"]]
         else:
             return []
 
 
 class LogAPI:
-    get: Callable[
-        [str, DefaultArg(Params, "params"), DefaultArg(bool, "content")], GetResponse
-    ]
+    get: Callable
 
     def log_files(
         self,
         attempt: Union[Attempt, int],
         task: Optional[str] = None,
         direct_download: Optional[bool] = None,
     ) -> List[LogFile]:
@@ -839,15 +795,15 @@
         params = {}  # type: Dict[str, Union[int, str, bool, None]]
         if task:
             params["task"] = task
         if direct_download:
             params["direct_download"] = True
 
         attempt_id = attempt.id if isinstance(attempt, Attempt) else attempt
-        r = cast(ListOfDict, self.get(f"logs/{attempt_id}/files"))
+        r = self.get(f"logs/{attempt_id}/files")
         if r:
             return [LogFile.from_api_repr(**l) for l in r["files"]]
         else:
             return []
 
     def log_file(
         self, attempt: Union[Attempt, int], file: Union[LogFile, str]
@@ -857,15 +813,15 @@
         :param attempt: Target Attempt id or Attempt object
         :param file: LogFile name or LogFile object
         :return: Log string
         """
 
         attempt_id = attempt.id if isinstance(attempt, Attempt) else attempt
         file_name = file.file_name if isinstance(file, LogFile) else file
-        r = cast(bytes, self.get(f"logs/{attempt_id}/files/{file_name}", content=True))
+        r = self.get(f"logs/{attempt_id}/files/{file_name}", content=True)
         if r:
             gzfile = io.BytesIO(r)
             with gzip.open(gzfile, "rt") as f:
                 return f.read()
         else:
             raise ValueError(f"Unable to get file: {file_name}")
 
@@ -977,22 +933,22 @@
         """
         :return: Established session
         :rtype: requests.Session
         """
         return self._http
 
     def get(
-        self, path: str, params: Optional[Params] = None, content: bool = False
-    ) -> GetResponse:
+        self, path: str, params: Optional[Dict[str, str]] = None, content: bool = False
+    ) -> Union[Dict[str, str], bytes]:
         """GET operator for REST API
 
         :param path: Treasure Workflow API path
         :type path: str
         :param params: Query parameters, defaults to None
-        :type params: Optional[Dict[str, Union[str, bool, int, None]]], optional
+        :type params: Optional[Dict[str, str]], optional
         :param content: Return content body without parsing JSON if ``True``
         :type content: bool
         :return: Response data in JSON or bytes
         :rtype: Union[Dict[str, str], bytes]
         """
         url = f"{self.api_base}{path}"
         r = self.http.get(url, params=params)
@@ -1000,58 +956,58 @@
 
         if not 200 <= r.status_code < 300:
             exceptions.raise_response_error(r)
 
         if content:
             return r.content
         else:
-            return cast(Dict[str, Any], r.json())
+            return r.json()
 
     def post(
-        self, path: str, body: Optional[Dict[str, Any]] = None, content: bool = False
-    ) -> PostResponse:
+        self, path: str, body: Optional[Dict[str, str]] = None, content: bool = False
+    ) -> Optional[Union[Dict[str, str], bytes]]:
         """POST operator for REST API
 
         :param path: Treasure Workflow API path
         :type path: str
         :param body: Content body in dictionary to be passed in JSON
-        :type body: Optional[Dict[str, Any]], optional
+        :type body: Optional[Dict[str, str]], optional
         :param content: Return content body without parsing JSON if ``True``
         :type content: bool
         :return: ``True`` if succeeded
         """
         url = f"{self.api_base}{path}"
         r = self.http.post(url, json=body)
         logger.debug(f"{r.status_code!r}\n{r.content!r}")
 
         if not 200 <= r.status_code < 300:
             exceptions.raise_response_error(r)
 
         if content:
             return r.content
         elif r.content and "application/json" in r.headers.get("Content-Type", ""):
-            return cast(Dict[str, str], r.json())
+            return r.json()
 
         return None
 
     def put(
         self,
         path: str,
-        data: Optional[DataType] = None,
-        _json: Optional[Dict[str, Any]] = None,
+        data: Optional[Union[str, Dict, List[Tuple], BinaryIO]] = None,
+        _json: Optional[Dict[str, str]] = None,
         params: Optional[Dict[str, str]] = None,
-    ) -> PutResponse:
+    ) -> Optional[Dict[str, str]]:
         """PUT operator for REST API
 
         :param path: Treasure Workflow API path
         :type path: str
         :param data: Content body
         :type data: Optional[str, Union[Dict, List[Tuple], BinaryIO]], optional
         :param _json: Content body as JSON
-        :type _json: Optional[Dict[str, Any]], optional
+        :type _json: Optional[Dict[str, str]], optional
         :param params: Query parameters
         :type params: Optional[Dict[str, str]], optional
         :return: Response content
         :rtype: Dict[str,str]
         """
         url = f"{self.api_base}{path}"
         headers = {}
@@ -1064,21 +1020,21 @@
         r = self.http.put(url, data=data, headers=headers, params=params)  # type: ignore
         logger.debug(f"{r.status_code!r}\n{r.content!r}")
 
         if not 200 <= r.status_code < 300:
             exceptions.raise_response_error(r)
 
         if r.content and "application/json" in r.headers.get("Content-Type", ""):
-            return cast(Dict[str, str], r.json())
+            return r.json()
 
         return None
 
     def delete(
         self, path: str, params: Optional[Dict[str, str]] = None
-    ) -> DeleteResponse:
+    ) -> Optional[Dict[str, str]]:
         """DELETE operator for REST API
 
         :param path: Treasure Workflow API path
         :type path: str
         :param params: Query parameters, defaults to None
         :type params: Optional[Dict[str, str]], optional
         :return: ``True`` if succeeded
@@ -1089,10 +1045,10 @@
         r = self.http.delete(url, params=params)
         logger.debug(f"{r.status_code!r}\n{r.content!r}")
 
         if not 200 <= r.status_code < 300:
             exceptions.raise_response_error(r)
 
         if r.content and "application/json" in r.headers.get("Content-Type", ""):
-            return cast(Dict[str, str], r.json())
+            return r.json()
 
         return None
```

### Comparing `tdworkflow-0.8.0/tdworkflow/log.py` & `tdworkflow-0.8.0rc0/tdworkflow/log.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,15 @@
     taskName: str
     direct: Dict[Any, Any]
     fileSize: int
     agentId: str
     fileTime: Optional[datetime] = None
 
     def __post_init__(self) -> None:
-        if self.fileTime and isinstance(self.fileTime, str):
-            self.fileTime = parse_iso8601(self.fileTime)
+        self.fileTime = parse_iso8601(self.fileTime)  # type: ignore
 
     @property
     def file_name(self) -> str:
         return self.fileName
 
     @property
     def taks_name(self) -> str:
```

### Comparing `tdworkflow-0.8.0/tdworkflow/project.py` & `tdworkflow-0.8.0rc0/tdworkflow/project.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,20 +15,17 @@
     archiveMd5: str = ""
     createdAt: Optional[datetime] = None
     deletedAt: Optional[datetime] = None
     updatedAt: Optional[datetime] = None
 
     def __post_init__(self) -> None:
         self.id = int(self.id)
-        if self.createdAt and isinstance(self.createdAt, str):
-            self.createdAt = parse_iso8601(self.createdAt)
-        if self.deletedAt and isinstance(self.deletedAt, str):
-            self.deletedAt = parse_iso8601(self.deletedAt)
-        if self.updatedAt and isinstance(self.updatedAt, str):
-            self.updatedAt = parse_iso8601(self.updatedAt)
+        self.createdAt = parse_iso8601(self.createdAt)  # type: ignore
+        self.deletedAt = parse_iso8601(self.deletedAt)  # type: ignore
+        self.updatedAt = parse_iso8601(self.updatedAt)  # type: ignore
 
     @property
     def archive_type(self) -> str:
         return self.archiveType
 
     @property
     def archive_md5(self) -> str:
```

### Comparing `tdworkflow-0.8.0/tdworkflow/revision.py` & `tdworkflow-0.8.0rc0/tdworkflow/revision.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,16 +11,15 @@
     revision: str
     createdAt: Optional[datetime] = None
     archiveType: str = ""
     archiveMd5: str = ""
     userInfo: Optional[Dict[str, Any]] = None
 
     def __post_init__(self) -> None:
-        if self.createdAt and isinstance(self.createdAt, str):
-            self.createdAt = parse_iso8601(self.createdAt)
+        self.createdAt = parse_iso8601(self.createdAt)  # type: ignore
 
     @property
     def archive_type(self) -> str:
         return self.archiveType
 
     @property
     def archive_md5(self) -> str:
```

### Comparing `tdworkflow-0.8.0/tdworkflow/schedule.py` & `tdworkflow-0.8.0rc0/tdworkflow/schedule.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,26 +20,20 @@
     updatedAt: Optional[datetime] = None
     disabledAt: Optional[datetime] = None
     nextScheduleTime: Optional[NextSchedule] = None
     nextRunTime: Optional[datetime] = None
 
     def __post_init__(self) -> None:
         self.id = int(self.id)
-        if self.project and isinstance(self.project, dict):
-            self.project = Project(**self.project)
-        if self.workflow and isinstance(self.workflow, dict):
-            self.workflow = Workflow(**self.workflow)
-        if self.createdAt and isinstance(self.createdAt, str):
-            self.createdAt = parse_iso8601(self.createdAt)
-        if self.updatedAt and isinstance(self.updatedAt, str):
-            self.updatedAt = parse_iso8601(self.updatedAt)
-        if self.disabledAt and isinstance(self.disabledAt, str):
-            self.disabledAt = parse_iso8601(self.disabledAt)
-        if self.nextRunTime and isinstance(self.nextRunTime, str):
-            self.nextRunTime = parse_iso8601(self.nextRunTime)
+        self.project = Project(**self.project)  # type: ignore
+        self.workflow = Workflow(**self.workflow)  # type: ignore
+        self.createdAt = parse_iso8601(self.createdAt)  # type: ignore
+        self.updatedAt = parse_iso8601(self.updatedAt)  # type: ignore
+        self.disabledAt = parse_iso8601(self.disabledAt)  # type: ignore
+        self.nextRunTime = parse_iso8601(self.nextRunTime)  # type: ignore
 
     @property
     def created_at(self) -> Optional[datetime]:
         return self.createdAt
 
     @property
     def updated_at(self) -> Optional[datetime]:
@@ -63,14 +57,10 @@
     id: int
     attempts: List[Attempt]
     project: Optional[Project] = None
     workflow: Optional[Workflow] = None
 
     def __post_init__(self) -> None:
         self.id = int(self.id)
-        self.attempts = [
-            Attempt(**att) if isinstance(att, dict) else att for att in self.attempts
-        ]
-        if self.project and isinstance(self.project, dict):
-            self.project = Project(**self.project)
-        if self.workflow and isinstance(self.workflow, dict):
-            self.workflow = Workflow(**self.workflow)
+        self.attempts = [Attempt(**att) for att in self.attempts]  # type: ignore
+        self.project = Project(**self.project)  # type: ignore
+        self.workflow = Project(**self.workflow)  # type: ignore
```

### Comparing `tdworkflow-0.8.0/tdworkflow/task.py` & `tdworkflow-0.8.0rc0/tdworkflow/task.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,22 +23,19 @@
     error: Optional[Dict[str, Any]] = None
     startedAt: Optional[datetime] = None
     cancelRequested: bool = False
     isGroup: bool = False
 
     def __post_init__(self) -> None:
         self.id = int(self.id)
-        if self.updatedAt and isinstance(self.updatedAt, str):
-            self.updatedAt = parse_iso8601(self.updatedAt)
+        self.updatedAt = parse_iso8601(self.updatedAt)  # type: ignore
         self.parentId = int(self.parentId) if self.parentId else None
         self.upstreams = [int(_id) for _id in self.upstreams] if self.upstreams else []
-        if self.retryAt and isinstance(self.retryAt, str):
-            self.retryAt = parse_iso8601(self.retryAt)
-        if self.startedAt and isinstance(self.startedAt, str):
-            self.startedAt = parse_iso8601(self.startedAt)
+        self.retryAt = parse_iso8601(self.retryAt)  # type: ignore
+        self.startedAt = parse_iso8601(self.startedAt)  # type: ignore
 
     @property
     def updated_at(self) -> Optional[datetime]:
         return self.updatedAt
 
     @property
     def full_name(self) -> str:
@@ -74,11 +71,11 @@
 
     @property
     def group(self) -> bool:
         return self.isGroup
 
 
 class TaskEncoder(json.JSONEncoder):
-    def default(self, obj: Any) -> Any:
+    def default(self, obj):
         if isinstance(obj, Task):
             return obj.__dict__
         return json.JSONEncoder.default(self, obj)
```

### Comparing `tdworkflow-0.8.0/tdworkflow/util.py` & `tdworkflow-0.8.0rc0/tdworkflow/util.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.0/tdworkflow/workflow.py` & `tdworkflow-0.8.0rc0/tdworkflow/workflow.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,22 +17,18 @@
     revision: str = ""
     createdAt: Optional[datetime] = None
     deletedAt: Optional[datetime] = None
     updatedAt: Optional[datetime] = None
 
     def __post_init__(self) -> None:
         self.id = int(self.id)
-        if self.project and isinstance(self.project, dict):
-            self.project = Project(**self.project)
-        if self.createdAt and isinstance(self.createdAt, str):
-            self.createdAt = parse_iso8601(self.createdAt)
-        if self.deletedAt and isinstance(self.deletedAt, str):
-            self.deletedAt = parse_iso8601(self.deletedAt)
-        if self.updatedAt and isinstance(self.updatedAt, str):
-            self.updatedAt = parse_iso8601(self.updatedAt)
+        self.project = Project(**self.project) if self.project else None  # type: ignore
+        self.createdAt = parse_iso8601(self.createdAt)  # type: ignore
+        self.deletedAt = parse_iso8601(self.deletedAt)  # type: ignore
+        self.updatedAt = parse_iso8601(self.updatedAt)  # type: ignore
 
     @property
     def created_at(self) -> Optional[datetime]:
         return self.createdAt
 
     @property
     def deleted_at(self) -> Optional[datetime]:
```

### Comparing `tdworkflow-0.8.0/tdworkflow.egg-info/PKG-INFO` & `tdworkflow-0.8.0rc0/tdworkflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdworkflow
-Version: 0.8.0
+Version: 0.8.0rc0
 Summary: Unofficial Treasure Workflow API client
 Home-page: https://github.com/chezou/tdworkflow
 Author: Aki Ariga
 Author-email: chezou@gmail.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `tdworkflow-0.8.0/tdworkflow.egg-info/SOURCES.txt` & `tdworkflow-0.8.0rc0/tdworkflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.0/tests/test_client.py` & `tdworkflow-0.8.0rc0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.0/tests/test_util.py` & `tdworkflow-0.8.0rc0/tests/test_util.py`

 * *Files identical despite different names*

