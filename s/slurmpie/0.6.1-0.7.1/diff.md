# Comparing `tmp/slurmpie-0.6.1.tar.gz` & `tmp/slurmpie-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/slurmpie-0.6.1.tar", last modified: Fri Nov 18 14:07:14 2022, max compression
+gzip compressed data, was "dist/slurmpie-0.7.1.tar", last modified: Thu Jul 13 11:29:04 2023, max compression
```

## Comparing `slurmpie-0.6.1.tar` & `slurmpie-0.7.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 14:07:14.000000 slurmpie-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-11-18 14:07:14.000000 slurmpie-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      883 2022-11-18 14:06:56.000000 slurmpie-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-11-18 14:07:14.000000 slurmpie-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      668 2022-11-18 14:06:56.000000 slurmpie-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 14:07:14.000000 slurmpie-0.6.1/slurmpie/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 14:06:56.000000 slurmpie-0.6.1/slurmpie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21816 2022-11-18 14:06:56.000000 slurmpie-0.6.1/slurmpie/slurmpie.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 14:07:14.000000 slurmpie-0.6.1/slurmpie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-11-18 14:07:14.000000 slurmpie-0.6.1/slurmpie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-11-18 14:07:14.000000 slurmpie-0.6.1/slurmpie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-18 14:07:14.000000 slurmpie-0.6.1/slurmpie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-18 14:07:14.000000 slurmpie-0.6.1/slurmpie.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 14:07:14.000000 slurmpie-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 14:06:56.000000 slurmpie-0.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8994 2022-11-18 14:06:56.000000 slurmpie-0.6.1/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (121)     5010 2022-11-18 14:06:56.000000 slurmpie-0.6.1/tests/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:29:04.000000 slurmpie-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-13 11:28:13.000000 slurmpie-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-13 11:29:04.000000 slurmpie-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-13 11:28:13.000000 slurmpie-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-13 11:29:04.000000 slurmpie-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-13 11:28:13.000000 slurmpie-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:29:04.000000 slurmpie-0.7.1/slurmpie/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:28:13.000000 slurmpie-0.7.1/slurmpie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22424 2023-07-13 11:28:13.000000 slurmpie-0.7.1/slurmpie/slurmpie.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:29:04.000000 slurmpie-0.7.1/slurmpie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-13 11:29:02.000000 slurmpie-0.7.1/slurmpie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-13 11:29:03.000000 slurmpie-0.7.1/slurmpie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 11:29:02.000000 slurmpie-0.7.1/slurmpie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 11:29:02.000000 slurmpie-0.7.1/slurmpie.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:29:04.000000 slurmpie-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:28:13.000000 slurmpie-0.7.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-07-13 11:28:13.000000 slurmpie-0.7.1/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-07-13 11:28:13.000000 slurmpie-0.7.1/tests/test_pipeline.py
```

### Comparing `slurmpie-0.6.1/PKG-INFO` & `slurmpie-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurmpie
-Version: 0.6.1
+Version: 0.7.1
 Summary: Package to interact with SLURM
 Home-page: https://github.com/svdvoort/slurmpie
 Author: Sebastian van der Voort
 Author-email: Svdvoort@users.noreply.github.com
 License: UNKNOWN
 Description: # slurmpie
```

### Comparing `slurmpie-0.6.1/README.md` & `slurmpie-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `slurmpie-0.6.1/setup.py` & `slurmpie-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="slurmpie",
-    version="0.6.1",
+    version="0.7.1",
     author="Sebastian van der Voort",
     author_email="Svdvoort@users.noreply.github.com",
     description="Package to interact with SLURM",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/svdvoort/slurmpie",
     packages=setuptools.find_packages(),
```

### Comparing `slurmpie-0.6.1/slurmpie/slurmpie.py` & `slurmpie-0.7.1/slurmpie/slurmpie.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import itertools
 import math
 import numbers
 import os
 import re
 import subprocess
-from typing import Dict, Tuple, Union
+from typing import Dict, Tuple, Union, List
 
 
 class Job:
     _newid = itertools.count()
 
     def __init__(
         self,
@@ -21,14 +21,15 @@
         gres: dict = {},
         logfile_directory: str = "",
         mail_address: str = "",
         mail_type: str = "",
         memory_size: Union[str, int] = "",
         name: str = "",
         nodes: int = -1,
+        nodelist: str = "",
         output_file: str = "",
         partition: str = "",
         tasks: int = -1,
         time: str = "",
         workdir: str = "",
     ):
         """
@@ -51,14 +52,15 @@
             mail_address (str, optional): Mail address to send notifications to.
             mail_type (str, optional): Specify for which events a notification should be send.
              One of: NONE, BEGIN, END, FAIL, REQUEUE, ALL
             memory_size (str or int): Specify memory requirement for job.
              See :func:`slurmpie.slurmpie.Job.memory_size` for the specification.
             name (str, optional): The name of the job.
             nodes (int, optional): Number of nodes to use for the job.
+            nodelist (str, optional): Request specific host nodes for job.
             output_file (str, optional): File path for the slurm output file.
             partition (str, optional): Name of the partition to which to submit the job.
             tasks (int, optional): Number of tasks.
             time (str, optional): The expected/maximum wall time for the job.
              Needs to be specified in the SLURM format, one of:
              "minutes", "minutes:seconds", "hours:minutes:seconds",
              "days-hours", "days-hours:minutes" and "days-hours:minutes:seconds"
@@ -71,14 +73,15 @@
         self._array = ""
         self._dependencies = ""
         self._gpus = ""
         self._gres = ""
         self._memory_size = ""
         self._memory_units = None
         self._id = next(Job._newid)
+        self._nodelist = ""
 
         self.script = script
         self.script_is_file = script_is_file
 
         self.array = array
         self.cpus_per_task = cpus_per_task
         self.dependencies = ""
@@ -295,14 +298,31 @@
         if isinstance(array_spec, list):
             array_spec = [str(i_spec) for i_spec in array_spec]
             array_spec = ",".join(array_spec)
 
         self._array = self._format_argument_list(self._array, array_spec)
 
     @property
+    def nodelist(self) -> str:
+        """
+        List of nodes to run the job on.
+
+        When you want to run a job on a specific node (that is not specified by a queue),
+        you can use this argument to specify the exact nodes you want to run
+        the job on.
+        """
+
+        return self._nodelist
+
+    @nodelist.setter
+    def nodelist(self, nodelist_spec: str):
+        self._nodelist = nodelist_spec
+
+
+    @property
     def gpus(self) -> str:
         """
         The gpus to request from the SLURM jobs.
 
         Just like the gres resources, one can request the gpu resources for the job.
         This is configuration dependent, so make sure your cluster supports this.
         The configuration has to be applied in the same way as for gres.
@@ -357,14 +377,15 @@
             "name": "job-name",
             "nodes": "nodes",
             "output_file": "output",
             "partition": "partition",
             "tasks": "ntasks",
             "time": "time",
             "workdir": "chdir",
+            "nodelist": "nodelist"
         }
 
         # We set parsable to easily get job id
         command = ["sbatch", "--parsable"]
 
         for attribute_name, bash_argument in sorted(
             command_mapping.items(), key=lambda x: x[0].lower()
```

### Comparing `slurmpie-0.6.1/slurmpie.egg-info/PKG-INFO` & `slurmpie-0.7.1/slurmpie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurmpie
-Version: 0.6.1
+Version: 0.7.1
 Summary: Package to interact with SLURM
 Home-page: https://github.com/svdvoort/slurmpie
 Author: Sebastian van der Voort
 Author-email: Svdvoort@users.noreply.github.com
 License: UNKNOWN
 Description: # slurmpie
```

### Comparing `slurmpie-0.6.1/tests/test_jobs.py` & `slurmpie-0.7.1/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `slurmpie-0.6.1/tests/test_pipeline.py` & `slurmpie-0.7.1/tests/test_pipeline.py`

 * *Files identical despite different names*

