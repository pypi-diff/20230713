# Comparing `tmp/faasmctl-0.3.4.tar.gz` & `tmp/faasmctl-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faasmctl-0.3.4.tar", last modified: Wed Jul 12 10:32:54 2023, max compression
+gzip compressed data, was "faasmctl-0.3.5.tar", last modified: Thu Jul 13 10:01:14 2023, max compression
```

## Comparing `faasmctl-0.3.4.tar` & `faasmctl-0.3.5.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:32:54.481671 faasmctl-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-12 10:29:59.000000 faasmctl-0.3.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-12 10:32:54.481671 faasmctl-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-12 10:29:59.000000 faasmctl-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:32:54.473671 faasmctl-0.3.4/faasmctl/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:32:54.477671 faasmctl-0.3.4/faasmctl/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/tasks/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/tasks/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/tasks/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/tasks/flush.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/tasks/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/tasks/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/tasks/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/tasks/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:32:54.481671 faasmctl-0.3.4/faasmctl/util/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/faasm.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/flush.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:32:54.481671 faasmctl-0.3.4/faasmctl/util/gen_proto/
--rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-12 10:32:38.000000 faasmctl-0.3.4/faasmctl/util/gen_proto/faabric_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-12 10:32:38.000000 faasmctl-0.3.4/faasmctl/util/gen_proto/planner_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/message.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/planner.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-12 10:29:59.000000 faasmctl-0.3.4/faasmctl/util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 10:32:54.477671 faasmctl-0.3.4/faasmctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-12 10:32:54.000000 faasmctl-0.3.4/faasmctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-12 10:32:54.000000 faasmctl-0.3.4/faasmctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 10:32:54.000000 faasmctl-0.3.4/faasmctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 10:32:54.000000 faasmctl-0.3.4/faasmctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 10:32:54.000000 faasmctl-0.3.4/faasmctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 10:32:54.000000 faasmctl-0.3.4/faasmctl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-12 10:29:59.000000 faasmctl-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 10:32:54.481671 faasmctl-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:01:14.397753 faasmctl-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-13 09:58:43.000000 faasmctl-0.3.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-13 10:01:14.397753 faasmctl-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-13 09:58:43.000000 faasmctl-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:01:14.393753 faasmctl-0.3.5/faasmctl/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-13 09:58:43.000000 faasmctl-0.3.5/faasmctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-13 09:58:43.000000 faasmctl-0.3.5/faasmctl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:01:14.393753 faasmctl-0.3.5/faasmctl/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-13 09:58:43.000000 faasmctl-0.3.5/faasmctl/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-13 09:58:43.000000 faasmctl-0.3.5/faasmctl/tasks/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-13 09:58:43.000000 faasmctl-0.3.5/faasmctl/tasks/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-13 09:58:43.000000 faasmctl-0.3.5/faasmctl/tasks/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-13 09:58:43.000000 faasmctl-0.3.5/faasmctl/tasks/flush.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-13 09:58:43.000000 faasmctl-0.3.5/faasmctl/tasks/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-13 09:58:43.000000 faasmctl-0.3.5/faasmctl/tasks/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-13 09:58:43.000000 faasmctl-0.3.5/faasmctl/tasks/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-13 09:58:43.000000 faasmctl-0.3.5/faasmctl/tasks/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-13 09:58:43.000000 faasmctl-0.3.5/faasmctl/tasks/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:01:14.397753 faasmctl-0.3.5/faasmctl/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-13 09:58:43.000000 faasmctl-0.3.5/faasmctl/util/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-13 09:58:43.000000 faasmctl-0.3.5/faasmctl/util/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-13 09:58:43.000000 faasmctl-0.3.5/faasmctl/util/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-13 09:58:43.000000 faasmctl-0.3.5/faasmctl/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-07-13 09:58:43.000000 faasmctl-0.3.5/faasmctl/util/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-13 09:58:43.000000 faasmctl-0.3.5/faasmctl/util/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-13 09:58:43.000000 faasmctl-0.3.5/faasmctl/util/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-13 09:58:43.000000 faasmctl-0.3.5/faasmctl/util/faasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-13 09:58:43.000000 faasmctl-0.3.5/faasmctl/util/flush.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:01:14.397753 faasmctl-0.3.5/faasmctl/util/gen_proto/
+-rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-13 10:01:05.000000 faasmctl-0.3.5/faasmctl/util/gen_proto/faabric_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-13 10:01:05.000000 faasmctl-0.3.5/faasmctl/util/gen_proto/planner_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-13 09:58:43.000000 faasmctl-0.3.5/faasmctl/util/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-13 09:58:43.000000 faasmctl-0.3.5/faasmctl/util/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-13 09:58:43.000000 faasmctl-0.3.5/faasmctl/util/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-13 09:58:43.000000 faasmctl-0.3.5/faasmctl/util/planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-13 09:58:43.000000 faasmctl-0.3.5/faasmctl/util/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-13 09:58:43.000000 faasmctl-0.3.5/faasmctl/util/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 09:58:43.000000 faasmctl-0.3.5/faasmctl/util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:01:14.393753 faasmctl-0.3.5/faasmctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-13 10:01:14.000000 faasmctl-0.3.5/faasmctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-13 10:01:14.000000 faasmctl-0.3.5/faasmctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 10:01:14.000000 faasmctl-0.3.5/faasmctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-13 10:01:14.000000 faasmctl-0.3.5/faasmctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-13 10:01:14.000000 faasmctl-0.3.5/faasmctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 10:01:14.000000 faasmctl-0.3.5/faasmctl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-13 09:58:43.000000 faasmctl-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 10:01:14.397753 faasmctl-0.3.5/setup.cfg
```

### Comparing `faasmctl-0.3.4/LICENSE.md` & `faasmctl-0.3.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.4/PKG-INFO` & `faasmctl-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.3.4
+Version: 0.3.5
 Summary: Command line tool to deploy, manage, and interact with Faasm
 Author-email: Faasm Team <foo@bar.com>
 Project-URL: Homepage, https://github.com/faasm/faasmctl
 Project-URL: Bug Tracker, https://github.com/faasm/faasmctl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -17,15 +17,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.3.4
+pip install faasmctl==0.3.5
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.3.4/README.md` & `faasmctl-0.3.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.3.4
+pip install faasmctl==0.3.5
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.3.4/faasmctl/tasks/cli.py` & `faasmctl-0.3.5/faasmctl/tasks/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     By default, if --cmd is set to None, we will get a shell into the
     container. If the --cmd argument is set, we execute the cmd string
 
     Parameters:
     - cmd (str): command to run in the CLI container
     - ini_file (str): path to the cluster's INI file
     """
-    do_run_cmd("faasm", cmd, ini_file)
+    do_run_cmd("faasm-cli", cmd, ini_file)
 
 
 @task
 def cpp(ctx, cmd=None, ini_file=None):
     """
     Run a command in the CPP CLI container
```

### Comparing `faasmctl-0.3.4/faasmctl/tasks/delete.py` & `faasmctl-0.3.5/faasmctl/tasks/delete.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.4/faasmctl/tasks/deploy.py` & `faasmctl-0.3.5/faasmctl/tasks/deploy.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.4/faasmctl/tasks/flush.py` & `faasmctl-0.3.5/faasmctl/tasks/flush.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.4/faasmctl/tasks/invoke.py` & `faasmctl-0.3.5/faasmctl/tasks/invoke.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.4/faasmctl/tasks/logs.py` & `faasmctl-0.3.5/faasmctl/tasks/logs.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.4/faasmctl/tasks/status.py` & `faasmctl-0.3.5/faasmctl/tasks/status.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.4/faasmctl/util/compose.py` & `faasmctl-0.3.5/faasmctl/util/compose.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.4/faasmctl/util/config.py` & `faasmctl-0.3.5/faasmctl/util/config.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.4/faasmctl/util/deploy.py` & `faasmctl-0.3.5/faasmctl/util/deploy.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.4/faasmctl/util/docker.py` & `faasmctl-0.3.5/faasmctl/util/docker.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.4/faasmctl/util/flush.py` & `faasmctl-0.3.5/faasmctl/util/flush.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.4/faasmctl/util/gen_proto/faabric_pb2.py` & `faasmctl-0.3.5/faasmctl/util/gen_proto/faabric_pb2.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.4/faasmctl/util/gen_proto/planner_pb2.py` & `faasmctl-0.3.5/faasmctl/util/gen_proto/planner_pb2.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.4/faasmctl/util/invoke.py` & `faasmctl-0.3.5/faasmctl/util/invoke.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.4/faasmctl/util/planner.py` & `faasmctl-0.3.5/faasmctl/util/planner.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.4/faasmctl/util/upload.py` & `faasmctl-0.3.5/faasmctl/util/upload.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.4/faasmctl.egg-info/PKG-INFO` & `faasmctl-0.3.5/faasmctl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.3.4
+Version: 0.3.5
 Summary: Command line tool to deploy, manage, and interact with Faasm
 Author-email: Faasm Team <foo@bar.com>
 Project-URL: Homepage, https://github.com/faasm/faasmctl
 Project-URL: Bug Tracker, https://github.com/faasm/faasmctl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -17,15 +17,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.3.4
+pip install faasmctl==0.3.5
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.3.4/faasmctl.egg-info/SOURCES.txt` & `faasmctl-0.3.5/faasmctl.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 faasmctl/tasks/__init__.py
 faasmctl/tasks/cli.py
 faasmctl/tasks/delete.py
 faasmctl/tasks/deploy.py
 faasmctl/tasks/flush.py
 faasmctl/tasks/invoke.py
 faasmctl/tasks/logs.py
+faasmctl/tasks/restart.py
 faasmctl/tasks/status.py
 faasmctl/tasks/upload.py
 faasmctl/util/backend.py
 faasmctl/util/batch.py
 faasmctl/util/compose.py
 faasmctl/util/config.py
 faasmctl/util/deploy.py
```

### Comparing `faasmctl-0.3.4/pyproject.toml` & `faasmctl-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "faasmctl"
-version = "0.3.4"
+version = "0.3.5"
 authors = [
   { name="Faasm Team", email="foo@bar.com" },
 ]
 description = "Command line tool to deploy, manage, and interact with Faasm"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

