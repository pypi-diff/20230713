# Comparing `tmp/faasmctl-0.3.6.tar.gz` & `tmp/faasmctl-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faasmctl-0.3.6.tar", last modified: Thu Jul 13 11:14:48 2023, max compression
+gzip compressed data, was "faasmctl-0.3.7.tar", last modified: Thu Jul 13 11:45:14 2023, max compression
```

## Comparing `faasmctl-0.3.6.tar` & `faasmctl-0.3.7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:14:48.689128 faasmctl-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-13 11:12:44.000000 faasmctl-0.3.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-13 11:14:48.689128 faasmctl-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-13 11:12:44.000000 faasmctl-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:14:48.669128 faasmctl-0.3.6/faasmctl/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-13 11:12:44.000000 faasmctl-0.3.6/faasmctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-13 11:12:44.000000 faasmctl-0.3.6/faasmctl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:14:48.677128 faasmctl-0.3.6/faasmctl/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-13 11:12:44.000000 faasmctl-0.3.6/faasmctl/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-13 11:12:44.000000 faasmctl-0.3.6/faasmctl/tasks/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-13 11:12:44.000000 faasmctl-0.3.6/faasmctl/tasks/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-13 11:12:44.000000 faasmctl-0.3.6/faasmctl/tasks/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-13 11:12:44.000000 faasmctl-0.3.6/faasmctl/tasks/flush.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-13 11:12:44.000000 faasmctl-0.3.6/faasmctl/tasks/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-13 11:12:44.000000 faasmctl-0.3.6/faasmctl/tasks/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-13 11:12:44.000000 faasmctl-0.3.6/faasmctl/tasks/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-13 11:12:44.000000 faasmctl-0.3.6/faasmctl/tasks/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-13 11:12:44.000000 faasmctl-0.3.6/faasmctl/tasks/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:14:48.689128 faasmctl-0.3.6/faasmctl/util/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-13 11:12:44.000000 faasmctl-0.3.6/faasmctl/util/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-13 11:12:44.000000 faasmctl-0.3.6/faasmctl/util/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-07-13 11:12:44.000000 faasmctl-0.3.6/faasmctl/util/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-13 11:12:44.000000 faasmctl-0.3.6/faasmctl/util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-07-13 11:12:44.000000 faasmctl-0.3.6/faasmctl/util/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-13 11:12:44.000000 faasmctl-0.3.6/faasmctl/util/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-13 11:12:44.000000 faasmctl-0.3.6/faasmctl/util/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-13 11:12:44.000000 faasmctl-0.3.6/faasmctl/util/faasm.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-13 11:12:44.000000 faasmctl-0.3.6/faasmctl/util/flush.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:14:48.689128 faasmctl-0.3.6/faasmctl/util/gen_proto/
--rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-13 11:14:33.000000 faasmctl-0.3.6/faasmctl/util/gen_proto/faabric_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-13 11:14:33.000000 faasmctl-0.3.6/faasmctl/util/gen_proto/planner_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-13 11:12:44.000000 faasmctl-0.3.6/faasmctl/util/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-13 11:12:44.000000 faasmctl-0.3.6/faasmctl/util/message.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-13 11:12:44.000000 faasmctl-0.3.6/faasmctl/util/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-13 11:12:44.000000 faasmctl-0.3.6/faasmctl/util/planner.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-13 11:12:44.000000 faasmctl-0.3.6/faasmctl/util/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-13 11:12:44.000000 faasmctl-0.3.6/faasmctl/util/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 11:12:44.000000 faasmctl-0.3.6/faasmctl/util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:14:48.673128 faasmctl-0.3.6/faasmctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-13 11:14:48.000000 faasmctl-0.3.6/faasmctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-13 11:14:48.000000 faasmctl-0.3.6/faasmctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 11:14:48.000000 faasmctl-0.3.6/faasmctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-13 11:14:48.000000 faasmctl-0.3.6/faasmctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-13 11:14:48.000000 faasmctl-0.3.6/faasmctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 11:14:48.000000 faasmctl-0.3.6/faasmctl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-13 11:12:44.000000 faasmctl-0.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 11:14:48.689128 faasmctl-0.3.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:45:14.509302 faasmctl-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-13 11:43:12.000000 faasmctl-0.3.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-13 11:45:14.509302 faasmctl-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-13 11:43:12.000000 faasmctl-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:45:14.505302 faasmctl-0.3.7/faasmctl/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-13 11:43:12.000000 faasmctl-0.3.7/faasmctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-13 11:43:12.000000 faasmctl-0.3.7/faasmctl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:45:14.509302 faasmctl-0.3.7/faasmctl/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-13 11:43:12.000000 faasmctl-0.3.7/faasmctl/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-13 11:43:12.000000 faasmctl-0.3.7/faasmctl/tasks/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-13 11:43:12.000000 faasmctl-0.3.7/faasmctl/tasks/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-13 11:43:12.000000 faasmctl-0.3.7/faasmctl/tasks/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-13 11:43:12.000000 faasmctl-0.3.7/faasmctl/tasks/flush.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-13 11:43:12.000000 faasmctl-0.3.7/faasmctl/tasks/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-13 11:43:12.000000 faasmctl-0.3.7/faasmctl/tasks/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-13 11:43:12.000000 faasmctl-0.3.7/faasmctl/tasks/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-13 11:43:12.000000 faasmctl-0.3.7/faasmctl/tasks/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-13 11:43:12.000000 faasmctl-0.3.7/faasmctl/tasks/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:45:14.509302 faasmctl-0.3.7/faasmctl/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-13 11:43:12.000000 faasmctl-0.3.7/faasmctl/util/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-13 11:43:12.000000 faasmctl-0.3.7/faasmctl/util/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-07-13 11:43:12.000000 faasmctl-0.3.7/faasmctl/util/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-13 11:43:12.000000 faasmctl-0.3.7/faasmctl/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-07-13 11:43:12.000000 faasmctl-0.3.7/faasmctl/util/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-13 11:43:12.000000 faasmctl-0.3.7/faasmctl/util/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-13 11:43:12.000000 faasmctl-0.3.7/faasmctl/util/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-13 11:43:12.000000 faasmctl-0.3.7/faasmctl/util/faasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-13 11:43:12.000000 faasmctl-0.3.7/faasmctl/util/flush.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:45:14.509302 faasmctl-0.3.7/faasmctl/util/gen_proto/
+-rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-13 11:45:05.000000 faasmctl-0.3.7/faasmctl/util/gen_proto/faabric_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-13 11:45:05.000000 faasmctl-0.3.7/faasmctl/util/gen_proto/planner_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-13 11:43:12.000000 faasmctl-0.3.7/faasmctl/util/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-13 11:43:12.000000 faasmctl-0.3.7/faasmctl/util/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-13 11:43:12.000000 faasmctl-0.3.7/faasmctl/util/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-13 11:43:12.000000 faasmctl-0.3.7/faasmctl/util/planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-13 11:43:12.000000 faasmctl-0.3.7/faasmctl/util/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-13 11:43:12.000000 faasmctl-0.3.7/faasmctl/util/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 11:43:12.000000 faasmctl-0.3.7/faasmctl/util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:45:14.505302 faasmctl-0.3.7/faasmctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-13 11:45:14.000000 faasmctl-0.3.7/faasmctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-13 11:45:14.000000 faasmctl-0.3.7/faasmctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 11:45:14.000000 faasmctl-0.3.7/faasmctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-13 11:45:14.000000 faasmctl-0.3.7/faasmctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-13 11:45:14.000000 faasmctl-0.3.7/faasmctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 11:45:14.000000 faasmctl-0.3.7/faasmctl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-13 11:43:12.000000 faasmctl-0.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 11:45:14.509302 faasmctl-0.3.7/setup.cfg
```

### Comparing `faasmctl-0.3.6/LICENSE.md` & `faasmctl-0.3.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.6/PKG-INFO` & `faasmctl-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.3.6
+Version: 0.3.7
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
-pip install faasmctl==0.3.6
+pip install faasmctl==0.3.7
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.3.6/README.md` & `faasmctl-0.3.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.3.6
+pip install faasmctl==0.3.7
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.3.6/faasmctl/tasks/cli.py` & `faasmctl-0.3.7/faasmctl/tasks/cli.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.6/faasmctl/tasks/delete.py` & `faasmctl-0.3.7/faasmctl/tasks/delete.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.6/faasmctl/tasks/deploy.py` & `faasmctl-0.3.7/faasmctl/tasks/deploy.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.6/faasmctl/tasks/flush.py` & `faasmctl-0.3.7/faasmctl/tasks/flush.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.6/faasmctl/tasks/invoke.py` & `faasmctl-0.3.7/faasmctl/tasks/invoke.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.6/faasmctl/tasks/logs.py` & `faasmctl-0.3.7/faasmctl/tasks/logs.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.6/faasmctl/tasks/restart.py` & `faasmctl-0.3.7/faasmctl/tasks/restart.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.6/faasmctl/tasks/status.py` & `faasmctl-0.3.7/faasmctl/tasks/status.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.6/faasmctl/util/compose.py` & `faasmctl-0.3.7/faasmctl/util/compose.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.6/faasmctl/util/config.py` & `faasmctl-0.3.7/faasmctl/util/config.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.6/faasmctl/util/deploy.py` & `faasmctl-0.3.7/faasmctl/util/deploy.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.6/faasmctl/util/docker.py` & `faasmctl-0.3.7/faasmctl/util/docker.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,12 +11,13 @@
     faasmctl can be invoked both from outside and inside a docker container.
     When invoked from inside a docker container, faasmctl can only be used to
     interact with a cluster running on docker compose. In that case, we need to
     use a different IP for the services in the cluster. Fortunately, Faasm
     sets certain env. vars when running inside a container. This function
     checks for them and returns True if successful
     """
+    print("ENVIRON: {}".format(environ))
     for env_var in IN_DOCKER_ENV_VARS:
         if env_var in environ and environ[env_var] == "on":
             return True
 
     return False
```

### Comparing `faasmctl-0.3.6/faasmctl/util/flush.py` & `faasmctl-0.3.7/faasmctl/util/flush.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.6/faasmctl/util/gen_proto/faabric_pb2.py` & `faasmctl-0.3.7/faasmctl/util/gen_proto/faabric_pb2.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.6/faasmctl/util/gen_proto/planner_pb2.py` & `faasmctl-0.3.7/faasmctl/util/gen_proto/planner_pb2.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.6/faasmctl/util/invoke.py` & `faasmctl-0.3.7/faasmctl/util/invoke.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.6/faasmctl/util/planner.py` & `faasmctl-0.3.7/faasmctl/util/planner.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.6/faasmctl/util/upload.py` & `faasmctl-0.3.7/faasmctl/util/upload.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.6/faasmctl.egg-info/PKG-INFO` & `faasmctl-0.3.7/faasmctl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.3.6
+Version: 0.3.7
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
-pip install faasmctl==0.3.6
+pip install faasmctl==0.3.7
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.3.6/faasmctl.egg-info/SOURCES.txt` & `faasmctl-0.3.7/faasmctl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.6/pyproject.toml` & `faasmctl-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "faasmctl"
-version = "0.3.6"
+version = "0.3.7"
 authors = [
   { name="Faasm Team", email="foo@bar.com" },
 ]
 description = "Command line tool to deploy, manage, and interact with Faasm"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

