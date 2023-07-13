# Comparing `tmp/tdworkflow-0.8.1.tar.gz` & `tmp/tdworkflow-0.8.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdworkflow-0.8.1.tar", last modified: Thu Jul 13 14:55:19 2023, max compression
+gzip compressed data, was "tdworkflow-0.8.1rc0.tar", last modified: Thu Jul 13 14:53:48 2023, max compression
```

## Comparing `tdworkflow-0.8.1.tar` & `tdworkflow-0.8.1rc0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:55:19.813247 tdworkflow-0.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:55:19.805246 tdworkflow-0.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:55:19.809247 tdworkflow-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/.github/workflows/pythonapp.yml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17742 2023-07-13 14:55:19.813247 tdworkflow-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:55:19.809247 tdworkflow-0.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:55:19.809247 tdworkflow-0.8.1/docs/references/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/docs/references/client.rst
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/docs/references/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/docs/references/misc.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/docs/references/model.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 14:55:19.813247 tdworkflow-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:55:19.809247 tdworkflow-0.8.1/tdworkflow/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/tdworkflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/tdworkflow/attempt.py
--rw-r--r--   0 runner    (1001) docker     (123)    39145 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/tdworkflow/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/tdworkflow/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/tdworkflow/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/tdworkflow/project.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/tdworkflow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/tdworkflow/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/tdworkflow/revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/tdworkflow/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/tdworkflow/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/tdworkflow/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/tdworkflow/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/tdworkflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:55:19.809247 tdworkflow-0.8.1/tdworkflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17742 2023-07-13 14:55:19.000000 tdworkflow-0.8.1/tdworkflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-13 14:55:19.000000 tdworkflow-0.8.1/tdworkflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:55:19.000000 tdworkflow-0.8.1/tdworkflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-13 14:55:19.000000 tdworkflow-0.8.1/tdworkflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-13 14:55:19.000000 tdworkflow-0.8.1/tdworkflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:55:19.809247 tdworkflow-0.8.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:55:19.805246 tdworkflow-0.8.1/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:55:19.809247 tdworkflow-0.8.1/tests/resources/sample_project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/tests/resources/sample_project/.digdag
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:55:19.809247 tdworkflow-0.8.1/tests/resources/sample_project/ignore_dir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/tests/resources/sample_project/ignore_dir/dummy
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/tests/resources/sample_project/main.dig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:55:19.809247 tdworkflow-0.8.1/tests/resources/sample_project/py_scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:55:19.809247 tdworkflow-0.8.1/tests/resources/sample_project/py_scripts/__ignoredir__/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/tests/resources/sample_project/py_scripts/__ignoredir__/dummy
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/tests/resources/sample_project/py_scripts/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)    24529 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-13 14:55:00.000000 tdworkflow-0.8.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:53:48.928925 tdworkflow-0.8.1rc0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:53:48.920925 tdworkflow-0.8.1rc0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:53:48.924925 tdworkflow-0.8.1rc0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/.github/workflows/pythonapp.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17745 2023-07-13 14:53:48.928925 tdworkflow-0.8.1rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:53:48.924925 tdworkflow-0.8.1rc0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:53:48.924925 tdworkflow-0.8.1rc0/docs/references/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/docs/references/client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/docs/references/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/docs/references/misc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/docs/references/model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 14:53:48.928925 tdworkflow-0.8.1rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:53:48.928925 tdworkflow-0.8.1rc0/tdworkflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/tdworkflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/tdworkflow/attempt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39145 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/tdworkflow/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/tdworkflow/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/tdworkflow/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/tdworkflow/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/tdworkflow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/tdworkflow/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/tdworkflow/revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/tdworkflow/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/tdworkflow/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/tdworkflow/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/tdworkflow/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/tdworkflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:53:48.928925 tdworkflow-0.8.1rc0/tdworkflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17745 2023-07-13 14:53:48.000000 tdworkflow-0.8.1rc0/tdworkflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-13 14:53:48.000000 tdworkflow-0.8.1rc0/tdworkflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:53:48.000000 tdworkflow-0.8.1rc0/tdworkflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-13 14:53:48.000000 tdworkflow-0.8.1rc0/tdworkflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-13 14:53:48.000000 tdworkflow-0.8.1rc0/tdworkflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:53:48.928925 tdworkflow-0.8.1rc0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:53:48.920925 tdworkflow-0.8.1rc0/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:53:48.928925 tdworkflow-0.8.1rc0/tests/resources/sample_project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/tests/resources/sample_project/.digdag
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:53:48.928925 tdworkflow-0.8.1rc0/tests/resources/sample_project/ignore_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/tests/resources/sample_project/ignore_dir/dummy
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/tests/resources/sample_project/main.dig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:53:48.928925 tdworkflow-0.8.1rc0/tests/resources/sample_project/py_scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:53:48.928925 tdworkflow-0.8.1rc0/tests/resources/sample_project/py_scripts/__ignoredir__/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/tests/resources/sample_project/py_scripts/__ignoredir__/dummy
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/tests/resources/sample_project/py_scripts/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24529 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-13 14:53:31.000000 tdworkflow-0.8.1rc0/tests/test_util.py
```

### Comparing `tdworkflow-0.8.1/.github/workflows/pythonapp.yml` & `tdworkflow-0.8.1rc0/.github/workflows/pythonapp.yml`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.1/.github/workflows/pythonpublish.yml` & `tdworkflow-0.8.1rc0/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.1/.gitignore` & `tdworkflow-0.8.1rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.1/.readthedocs.yml` & `tdworkflow-0.8.1rc0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.1/CHANGES.rst` & `tdworkflow-0.8.1rc0/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.1/LICENSE` & `tdworkflow-0.8.1rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.1/PKG-INFO` & `tdworkflow-0.8.1rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdworkflow
-Version: 0.8.1
+Version: 0.8.1rc0
 Summary: Unofficial Treasure Workflow API client
 Author-email: Aki Ariga <chezou@gmail.com>
 Maintainer-email: Aki Ariga <chezou@gmail.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `tdworkflow-0.8.1/README.rst` & `tdworkflow-0.8.1rc0/README.rst`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.1/docs/Makefile` & `tdworkflow-0.8.1rc0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.1/docs/conf.py` & `tdworkflow-0.8.1rc0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.1/docs/make.bat` & `tdworkflow-0.8.1rc0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.1/docs/references/model.rst` & `tdworkflow-0.8.1rc0/docs/references/model.rst`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.1/pyproject.toml` & `tdworkflow-0.8.1rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.1/tdworkflow/attempt.py` & `tdworkflow-0.8.1rc0/tdworkflow/attempt.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.1/tdworkflow/client.py` & `tdworkflow-0.8.1rc0/tdworkflow/client.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.1/tdworkflow/log.py` & `tdworkflow-0.8.1rc0/tdworkflow/log.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.1/tdworkflow/project.py` & `tdworkflow-0.8.1rc0/tdworkflow/project.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.1/tdworkflow/resource.py` & `tdworkflow-0.8.1rc0/tdworkflow/resource.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.1/tdworkflow/revision.py` & `tdworkflow-0.8.1rc0/tdworkflow/revision.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.1/tdworkflow/schedule.py` & `tdworkflow-0.8.1rc0/tdworkflow/schedule.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.1/tdworkflow/session.py` & `tdworkflow-0.8.1rc0/tdworkflow/session.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.1/tdworkflow/task.py` & `tdworkflow-0.8.1rc0/tdworkflow/task.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.1/tdworkflow/util.py` & `tdworkflow-0.8.1rc0/tdworkflow/util.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.1/tdworkflow/workflow.py` & `tdworkflow-0.8.1rc0/tdworkflow/workflow.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.1/tdworkflow.egg-info/PKG-INFO` & `tdworkflow-0.8.1rc0/tdworkflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdworkflow
-Version: 0.8.1
+Version: 0.8.1rc0
 Summary: Unofficial Treasure Workflow API client
 Author-email: Aki Ariga <chezou@gmail.com>
 Maintainer-email: Aki Ariga <chezou@gmail.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `tdworkflow-0.8.1/tdworkflow.egg-info/SOURCES.txt` & `tdworkflow-0.8.1rc0/tdworkflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.1/tests/test_client.py` & `tdworkflow-0.8.1rc0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `tdworkflow-0.8.1/tests/test_util.py` & `tdworkflow-0.8.1rc0/tests/test_util.py`

 * *Files identical despite different names*

