# Comparing `tmp/pympipool-0.5.3.tar.gz` & `tmp/pympipool-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pympipool-0.5.3.tar", last modified: Thu Jul 13 04:07:03 2023, max compression
+gzip compressed data, was "pympipool-0.5.4.tar", last modified: Thu Jul 13 16:24:32 2023, max compression
```

## Comparing `pympipool-0.5.3.tar` & `pympipool-0.5.4.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 04:07:03.163276 pympipool-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-13 04:07:00.000000 pympipool-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-13 04:07:00.000000 pympipool-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-13 04:07:03.163276 pympipool-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-07-13 04:07:00.000000 pympipool-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 04:07:03.163276 pympipool-0.5.3/pympipool/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-13 04:07:00.000000 pympipool-0.5.3/pympipool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-13 04:07:03.163276 pympipool-0.5.3/pympipool/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 04:07:03.159276 pympipool-0.5.3/pympipool/executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 04:07:00.000000 pympipool-0.5.3/pympipool/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-13 04:07:00.000000 pympipool-0.5.3/pympipool/executor/mpiexec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-13 04:07:00.000000 pympipool-0.5.3/pympipool/executor/mpipool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 04:07:03.159276 pympipool-0.5.3/pympipool/share/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 04:07:00.000000 pympipool-0.5.3/pympipool/share/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-13 04:07:00.000000 pympipool-0.5.3/pympipool/share/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-07-13 04:07:00.000000 pympipool-0.5.3/pympipool/share/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-07-13 04:07:00.000000 pympipool-0.5.3/pympipool/share/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-07-13 04:07:00.000000 pympipool-0.5.3/pympipool/share/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-07-13 04:07:00.000000 pympipool-0.5.3/pympipool/share/serial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 04:07:03.159276 pympipool-0.5.3/pympipool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-13 04:07:03.000000 pympipool-0.5.3/pympipool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-13 04:07:03.000000 pympipool-0.5.3/pympipool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 04:07:03.000000 pympipool-0.5.3/pympipool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 04:07:03.000000 pympipool-0.5.3/pympipool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 04:07:03.000000 pympipool-0.5.3/pympipool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-13 04:07:03.163276 pympipool-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-13 04:07:02.000000 pympipool-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 04:07:03.163276 pympipool-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-13 04:07:00.000000 pympipool-0.5.3/tests/test_communicator_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-07-13 04:07:00.000000 pympipool-0.5.3/tests/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-13 04:07:00.000000 pympipool-0.5.3/tests/test_future.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-13 04:07:00.000000 pympipool-0.5.3/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-13 04:07:00.000000 pympipool-0.5.3/tests/test_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-13 04:07:00.000000 pympipool-0.5.3/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-13 04:07:00.000000 pympipool-0.5.3/tests/test_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-13 04:07:00.000000 pympipool-0.5.3/tests/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-13 04:07:00.000000 pympipool-0.5.3/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-13 04:07:00.000000 pympipool-0.5.3/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-13 04:07:00.000000 pympipool-0.5.3/tests/test_worker_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-13 04:07:00.000000 pympipool-0.5.3/tests/test_zmq.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-13 04:07:00.000000 pympipool-0.5.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:24:32.490979 pympipool-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-13 16:24:28.000000 pympipool-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-13 16:24:28.000000 pympipool-0.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-13 16:24:32.490979 pympipool-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-07-13 16:24:28.000000 pympipool-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:24:32.490979 pympipool-0.5.4/pympipool/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-13 16:24:28.000000 pympipool-0.5.4/pympipool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-13 16:24:32.490979 pympipool-0.5.4/pympipool/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:24:32.486979 pympipool-0.5.4/pympipool/external_interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:24:28.000000 pympipool-0.5.4/pympipool/external_interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-07-13 16:24:28.000000 pympipool-0.5.4/pympipool/external_interfaces/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-07-13 16:24:28.000000 pympipool-0.5.4/pympipool/external_interfaces/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-07-13 16:24:28.000000 pympipool-0.5.4/pympipool/external_interfaces/pool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:24:32.490979 pympipool-0.5.4/pympipool/parallel_executors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:24:28.000000 pympipool-0.5.4/pympipool/parallel_executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-13 16:24:28.000000 pympipool-0.5.4/pympipool/parallel_executors/mpiexec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-13 16:24:28.000000 pympipool-0.5.4/pympipool/parallel_executors/mpipool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:24:32.490979 pympipool-0.5.4/pympipool/shared_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:24:28.000000 pympipool-0.5.4/pympipool/shared_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-07-13 16:24:28.000000 pympipool-0.5.4/pympipool/shared_functions/external_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-07-13 16:24:28.000000 pympipool-0.5.4/pympipool/shared_functions/parallel_executors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:24:32.486979 pympipool-0.5.4/pympipool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-13 16:24:32.000000 pympipool-0.5.4/pympipool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-13 16:24:32.000000 pympipool-0.5.4/pympipool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:24:32.000000 pympipool-0.5.4/pympipool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 16:24:32.000000 pympipool-0.5.4/pympipool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 16:24:32.000000 pympipool-0.5.4/pympipool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-13 16:24:32.490979 pympipool-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-13 16:24:32.000000 pympipool-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:24:32.490979 pympipool-0.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-13 16:24:28.000000 pympipool-0.5.4/tests/test_communicator_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-13 16:24:28.000000 pympipool-0.5.4/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-13 16:24:28.000000 pympipool-0.5.4/tests/test_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-13 16:24:28.000000 pympipool-0.5.4/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-13 16:24:28.000000 pympipool-0.5.4/tests/test_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-13 16:24:28.000000 pympipool-0.5.4/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-13 16:24:28.000000 pympipool-0.5.4/tests/test_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-13 16:24:28.000000 pympipool-0.5.4/tests/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-13 16:24:28.000000 pympipool-0.5.4/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-13 16:24:28.000000 pympipool-0.5.4/tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-13 16:24:28.000000 pympipool-0.5.4/tests/test_worker_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-13 16:24:28.000000 pympipool-0.5.4/tests/test_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-13 16:24:28.000000 pympipool-0.5.4/versioneer.py
```

### Comparing `pympipool-0.5.3/LICENSE` & `pympipool-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.3/PKG-INFO` & `pympipool-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.5.3
+Version: 0.5.4
 Summary: pympipool - scale python functions over multiple compute nodes
 Home-page: https://github.com/jan-janssen/pympipool
 Author-email: jan.janssen@outlook.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pympipool-0.5.3/README.md` & `pympipool-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.3/pympipool/executor/mpiexec.py` & `pympipool-0.5.4/pympipool/parallel_executors/mpiexec.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import pickle
 import sys
 
 import cloudpickle
 
-from pympipool.share.communication import (
+from pympipool.external_interfaces.communication import (
     connect_to_socket_interface,
     send_result,
     close_connection,
     receive_instruction,
 )
-from pympipool.share.parallel import call_funct, parse_arguments
+from pympipool.shared_functions.parallel_executors import call_funct, parse_arguments
 
 
 def main():
     from mpi4py import MPI
 
     MPI.pickle.__init__(
         cloudpickle.dumps,
```

### Comparing `pympipool-0.5.3/pympipool/executor/mpipool.py` & `pympipool-0.5.4/pympipool/parallel_executors/mpipool.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import pickle
 import sys
 
 import cloudpickle
 
-from pympipool.share.communication import (
+from pympipool.external_interfaces.communication import (
     connect_to_socket_interface,
     send_result,
     close_connection,
     receive_instruction,
 )
-from pympipool.share.parallel import (
+from pympipool.shared_functions.parallel_executors import (
     parse_arguments,
     parse_socket_communication,
 )
 
 
 def main():
     from mpi4py import MPI
```

### Comparing `pympipool-0.5.3/pympipool/share/parallel.py` & `pympipool-0.5.4/pympipool/shared_functions/parallel_executors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,28 @@
 import inspect
-from tqdm import tqdm
 
+from tqdm import tqdm
 
-def parse_arguments(argument_lst):
-    argument_dict = {
-        "total_cores": "--cores-total",
-        "zmqport": "--zmqport",
-        "cores_per_task": "--cores-per-task",
-        "host": "--host",
-    }
-    parse_dict = {"host": "localhost"}
-    parse_dict.update(
-        {
-            k: argument_lst[argument_lst.index(v) + 1]
-            for k, v in argument_dict.items()
-            if v in argument_lst
-        }
-    )
-    return parse_dict
 
+def call_funct(input_dict, funct=None, memory=None):
+    if funct is None:
 
-def wrap(funct, number_of_cores_per_communicator=1):
-    def functwrapped(*args, **kwargs):
-        from mpi4py import MPI
+        def funct(*args, **kwargs):
+            return args[0].__call__(*args[1:], **kwargs)
 
-        MPI.COMM_WORLD.Barrier()
-        rank = MPI.COMM_WORLD.Get_rank()
-        comm_new = MPI.COMM_WORLD.Split(
-            rank // number_of_cores_per_communicator,
-            rank % number_of_cores_per_communicator,
+    funct_args = inspect.getfullargspec(input_dict["fn"]).args
+    if memory is not None:
+        input_dict["kwargs"].update(
+            _update_dict_delta(
+                dict_input=memory,
+                dict_output=input_dict["kwargs"],
+                keys_possible_lst=funct_args,
+            )
         )
-        comm_new.Barrier()
-        return funct(*args, comm=comm_new, **kwargs)
-
-    return functwrapped
+    return funct(input_dict["fn"], *input_dict["args"], **input_dict["kwargs"])
 
 
 def map_funct(executor, funct, lst, chunksize=1, cores_per_task=1, map_flag=True):
     if cores_per_task == 1:
         if map_flag:
             results = executor.map(funct, lst, chunksize=chunksize)
         else:
@@ -46,51 +31,60 @@
     else:
         lst_parallel = []
         for input_parameter in lst:
             for _ in range(cores_per_task):
                 lst_parallel.append(input_parameter)
         if map_flag:
             results = executor.map(
-                wrap(funct=funct, number_of_cores_per_communicator=cores_per_task),
+                _wrap(funct=funct, number_of_cores_per_communicator=cores_per_task),
                 lst_parallel,
                 chunksize=chunksize,
             )
         else:
             results = executor.starmap(
-                wrap(funct=funct, number_of_cores_per_communicator=cores_per_task),
+                _wrap(funct=funct, number_of_cores_per_communicator=cores_per_task),
                 lst_parallel,
                 chunksize=chunksize,
             )
         return list(tqdm(results, desc="Tasks", total=len(lst_parallel)))[
             ::cores_per_task
         ]
 
 
-def call_funct(input_dict, funct=None, memory=None):
-    if funct is None:
+def parse_arguments(argument_lst):
+    """
+    Simple function to parse command line arguments
 
-        def funct(*args, **kwargs):
-            return args[0].__call__(*args[1:], **kwargs)
+    Args:
+        argument_lst (list): list of arguments as strings
 
-    funct_args = inspect.getfullargspec(input_dict["fn"]).args
-    if memory is not None:
-        input_dict["kwargs"].update(
-            update_dict_delta(
-                dict_input=memory,
-                dict_output=input_dict["kwargs"],
-                keys_possible_lst=funct_args,
-            )
-        )
-    return funct(input_dict["fn"], *input_dict["args"], **input_dict["kwargs"])
+    Returns:
+        dict: dictionary with the parsed arguments and their corresponding values
+    """
+    argument_dict = {
+        "total_cores": "--cores-total",
+        "zmqport": "--zmqport",
+        "cores_per_task": "--cores-per-task",
+        "host": "--host",
+    }
+    parse_dict = {"host": "localhost"}
+    parse_dict.update(
+        {
+            k: argument_lst[argument_lst.index(v) + 1]
+            for k, v in argument_dict.items()
+            if v in argument_lst
+        }
+    )
+    return parse_dict
 
 
 def parse_socket_communication(executor, input_dict, future_dict, cores_per_task=1):
     if "shutdown" in input_dict.keys() and input_dict["shutdown"]:
         executor.shutdown(wait=input_dict["wait"])
-        done_dict = update_futures(future_dict=future_dict)
+        done_dict = _update_futures(future_dict=future_dict)
         # If close "shutdown" is communicated the process is shutdown.
         if done_dict is not None and len(done_dict) > 0:
             return {"exit": True, "result": done_dict}
         else:
             return {"exit": True}
     elif "fn" in input_dict.keys() and "iterable" in input_dict.keys():
         # If a function "fn" and a list or arguments "iterable" are communicated,
@@ -119,36 +113,52 @@
         future = call_funct(input_dict=input_dict, funct=executor.submit)
         future_hash = hash(future)
         future_dict[future_hash] = future
         return {"result": future_hash}
     elif "update" in input_dict.keys():
         # If update "update" is communicated pympipool checks for asynchronously submitted
         # functions which have completed in the meantime and communicates their results.
-        done_dict = update_futures(
+        done_dict = _update_futures(
             future_dict=future_dict, hash_lst=input_dict["update"]
         )
         return {"result": done_dict}
     elif "cancel" in input_dict.keys():
         for k in input_dict["cancel"]:
             future_dict[k].cancel()
         return {"result": True}
 
 
-def update_dict_delta(dict_input, dict_output, keys_possible_lst):
+def _update_dict_delta(dict_input, dict_output, keys_possible_lst):
     return {
         k: v
         for k, v in dict_input.items()
         if k in keys_possible_lst and k not in dict_output.keys()
     }
 
 
-def update_futures(future_dict, hash_lst=None):
+def _update_futures(future_dict, hash_lst=None):
     if hash_lst is None:
         hash_lst = list(future_dict.keys())
     done_dict = {
         k: f.result()
         for k, f in {k: future_dict[k] for k in hash_lst}.items()
         if f.done()
     }
     for k in done_dict.keys():
         del future_dict[k]
     return done_dict
+
+
+def _wrap(funct, number_of_cores_per_communicator=1):
+    def functwrapped(*args, **kwargs):
+        from mpi4py import MPI
+
+        MPI.COMM_WORLD.Barrier()
+        rank = MPI.COMM_WORLD.Get_rank()
+        comm_new = MPI.COMM_WORLD.Split(
+            rank // number_of_cores_per_communicator,
+            rank % number_of_cores_per_communicator,
+        )
+        comm_new.Barrier()
+        return funct(*args, comm=comm_new, **kwargs)
+
+    return functwrapped
```

### Comparing `pympipool-0.5.3/pympipool/share/serial.py` & `pympipool-0.5.4/pympipool/shared_functions/external_interfaces.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,44 +2,90 @@
 import os
 import socket
 import time
 import queue
 
 import cloudpickle
 
-from pympipool.share.communication import SocketInterface
+from pympipool.external_interfaces.communication import SocketInterface
+
+
+def cancel_items_in_queue(que):
+    while True:
+        try:
+            item = que.get_nowait()
+            if isinstance(item, dict) and "future" in item.keys():
+                item["future"].cancel()
+        except queue.Empty:
+            break
+
+
+def cloudpickle_register(ind=2):
+    # Cloudpickle can either pickle by value or pickle by reference. The functions which are communicated have to
+    # be pickled by value rather than by reference, so the module which calls the map function is pickled by value.
+    # https://github.com/cloudpipe/cloudpickle#overriding-pickles-serialization-mechanism-for-importable-constructs
+    # inspect can help to find the module which is calling pympipool
+    # https://docs.python.org/3/library/inspect.html
+    # to learn more about inspect another good read is:
+    # http://pymotw.com/2/inspect/index.html#module-inspect
+    # 1 refers to 1 level higher than the map function
+    try:  # When executed in a jupyter notebook this can cause a ValueError - in this case we just ignore it.
+        cloudpickle.register_pickle_by_value(inspect.getmodule(inspect.stack()[ind][0]))
+    except ValueError:
+        pass
 
 
 def command_line_options(
     hostname,
     port_selected,
     path,
     cores,
     cores_per_task=1,
     oversubscribe=False,
     enable_flux_backend=False,
+    enable_slurm_backend=False,
     enable_mpi4py_backend=True,
     enable_multi_host=False,
 ):
+    """
+    Translate the individual parameters to command line options.
+
+    Args:
+        hostname (str): name of the host where the SocketInterface instance runs the client process should conenct to.
+        port_selected (int): port the SocketInterface instance runs on.
+        path (str): path to the python script which should be executed as client process.
+        cores (int): defines the total number of MPI ranks to use
+        cores_per_task (int): number of MPI ranks per task - defaults to 1
+        oversubscribe (bool): enable of disable the oversubscribe feature of OpenMPI - defaults to False
+        enable_flux_backend (bool): enable the flux-framework as backend - defaults to False
+        enable_slurm_backend (bool): enable the SLURM queueing system as backend - defaults to False
+        enable_mpi4py_backend (bool): enable the mpi4py.futures module - defaults to True
+        enable_multi_host (bool): communicate the host to connect to - defaults to False
+
+    Returns:
+        list: list of strings to be executed on the command line
+    """
     if enable_flux_backend:
         command_lst = ["flux", "run"]
+    elif enable_slurm_backend:
+        command_lst = ["srun"]
     else:
         command_lst = ["mpiexec"]
     if oversubscribe:
         command_lst += ["--oversubscribe"]
     if cores_per_task == 1 and enable_mpi4py_backend:
         command_lst += ["-n", str(cores), "python", "-m", "mpi4py.futures"]
     elif cores_per_task > 1 and enable_mpi4py_backend:
         # Running MPI parallel tasks within the map() requires mpi4py to use mpi spawn:
         # https://github.com/mpi4py/mpi4py/issues/324
         command_lst += ["-n", "1", "python"]
     else:
         command_lst += ["-n", str(cores), "python"]
     command_lst += [path]
-    if enable_flux_backend or enable_multi_host:
+    if enable_flux_backend or enable_slurm_backend or enable_multi_host:
         command_lst += [
             "--host",
             hostname,
         ]
     command_lst += [
         "--zmqport",
         str(port_selected),
@@ -50,173 +96,200 @@
             str(cores_per_task),
             "--cores-total",
             str(cores),
         ]
     return command_lst
 
 
-def get_parallel_subprocess_command(
-    port_selected,
-    cores,
-    cores_per_task=1,
-    oversubscribe=False,
-    enable_flux_backend=False,
-    enable_mpi4py_backend=True,
-    enable_multi_host=False,
-):
-    if enable_mpi4py_backend:
-        executable = "mpipool.py"
-    else:
-        executable = "mpiexec.py"
-    command_lst = command_line_options(
-        hostname=socket.gethostname(),
-        port_selected=port_selected,
-        path=os.path.abspath(os.path.join(__file__, "../../executor", executable)),
-        cores=cores,
-        cores_per_task=cores_per_task,
-        oversubscribe=oversubscribe,
-        enable_flux_backend=enable_flux_backend,
-        enable_mpi4py_backend=enable_mpi4py_backend,
-        enable_multi_host=enable_multi_host,
-    )
-    return command_lst
-
-
-def execute_parallel_tasks_loop(interface, future_queue):
-    while True:
-        task_dict = future_queue.get()
-        if "shutdown" in task_dict.keys() and task_dict["shutdown"]:
-            interface.shutdown(wait=task_dict["wait"])
-            break
-        elif "fn" in task_dict.keys() and "future" in task_dict.keys():
-            f = task_dict.pop("future")
-            if f.set_running_or_notify_cancel():
-                f.set_result(interface.send_and_receive_dict(input_dict=task_dict))
-        elif "fn" in task_dict.keys() and "init" in task_dict.keys():
-            interface.send_dict(input_dict=task_dict)
-
-
-def execute_serial_tasks_loop(interface, future_queue, future_dict, sleep_interval=0.1):
-    while True:
-        try:
-            task_dict = future_queue.get_nowait()
-        except queue.Empty:
-            pass
-        else:
-            if "shutdown" in task_dict.keys() and task_dict["shutdown"]:
-                done_dict = interface.shutdown(wait=task_dict["wait"])
-                if isinstance(done_dict, dict):
-                    for k, v in done_dict.items():
-                        if k in future_dict.keys() and not future_dict[k].cancelled():
-                            future_dict.pop(k).set_result(v)
-                break
-            elif "fn" in task_dict.keys() and "future" in task_dict.keys():
-                f = task_dict.pop("future")
-                future_hash = interface.send_and_receive_dict(input_dict=task_dict)
-                future_dict[future_hash] = f
-        update_future_dict(
-            interface=interface, future_dict=future_dict, sleep_interval=sleep_interval
-        )
-
-
 def execute_parallel_tasks(
     future_queue,
     cores,
     oversubscribe=False,
     enable_flux_backend=False,
+    enable_slurm_backend=False,
     cwd=None,
     queue_adapter=None,
     queue_adapter_kwargs=None,
 ):
+    """
+    Execute a single tasks in parallel using the message passing interface (MPI).
+
+    Args:
+       future_queue (queue.Queue): task queue of dictionary objects which are submitted to the parallel process
+       cores (int): defines the total number of MPI ranks to use
+       oversubscribe (bool): enable of disable the oversubscribe feature of OpenMPI - defaults to False
+       enable_flux_backend (bool): enable the flux-framework as backend - defaults to False
+       enable_slurm_backend (bool): enable the SLURM queueing system as backend - defaults to False
+       cwd (str/None): current working directory where the parallel python task is executed
+       queue_adapter (pysqa.queueadapter.QueueAdapter): generalized interface to various queuing systems
+       queue_adapter_kwargs (dict/None): keyword arguments for the submit_job() function of the queue adapter
+    """
     interface = SocketInterface(
         queue_adapter=queue_adapter, queue_adapter_kwargs=queue_adapter_kwargs
     )
     interface.bootup(
         command_lst=get_parallel_subprocess_command(
             port_selected=interface.bind_to_random_port(),
             cores=cores,
             cores_per_task=1,
             oversubscribe=oversubscribe,
             enable_flux_backend=enable_flux_backend,
+            enable_slurm_backend=enable_slurm_backend,
             enable_mpi4py_backend=False,
             enable_multi_host=queue_adapter is not None,
         ),
         cwd=cwd,
         cores=cores,
     )
-    execute_parallel_tasks_loop(interface=interface, future_queue=future_queue)
+    _execute_parallel_tasks_loop(interface=interface, future_queue=future_queue)
 
 
 def execute_serial_tasks(
     future_queue,
     cores,
     oversubscribe=False,
     enable_flux_backend=False,
+    enable_slurm_backend=False,
     cwd=None,
     sleep_interval=0.1,
     queue_adapter=None,
     queue_adapter_kwargs=None,
 ):
+    """
+    Execute a single tasks in serial.
+
+    Args:
+       future_queue (queue.Queue): task queue of dictionary objects which are submitted to the parallel process
+       cores (int): defines the total number of MPI ranks to use
+       oversubscribe (bool): enable of disable the oversubscribe feature of OpenMPI - defaults to False
+       enable_flux_backend (bool): enable the flux-framework as backend - defaults to False
+       enable_slurm_backend (bool): enable the SLURM queueing system as backend - defaults to False
+       cwd (str/None): current working directory where the parallel python task is executed
+       sleep_interval (float):
+       queue_adapter (pysqa.queueadapter.QueueAdapter): generalized interface to various queuing systems
+       queue_adapter_kwargs (dict/None): keyword arguments for the submit_job() function of the queue adapter
+    """
     future_dict = {}
     interface = SocketInterface(
         queue_adapter=queue_adapter, queue_adapter_kwargs=queue_adapter_kwargs
     )
     interface.bootup(
         command_lst=get_parallel_subprocess_command(
             port_selected=interface.bind_to_random_port(),
             cores=cores,
             cores_per_task=1,
             oversubscribe=oversubscribe,
             enable_flux_backend=enable_flux_backend,
+            enable_slurm_backend=enable_slurm_backend,
             enable_mpi4py_backend=True,
             enable_multi_host=queue_adapter is not None,
         ),
         cwd=cwd,
         cores=cores,
     )
-    execute_serial_tasks_loop(
+    _execute_serial_tasks_loop(
         interface=interface,
         future_queue=future_queue,
         future_dict=future_dict,
         sleep_interval=sleep_interval,
     )
 
 
-def update_future_dict(interface, future_dict, sleep_interval=0.1):
+def get_parallel_subprocess_command(
+    port_selected,
+    cores,
+    cores_per_task=1,
+    oversubscribe=False,
+    enable_flux_backend=False,
+    enable_slurm_backend=False,
+    enable_mpi4py_backend=True,
+    enable_multi_host=False,
+):
+    """
+    Translate the individual parameters to command line options.
+
+    Args:
+        port_selected (int): port the SocketInterface instance runs on.
+        cores (int): defines the total number of MPI ranks to use
+        cores_per_task (int): number of MPI ranks per task - defaults to 1
+        oversubscribe (bool): enable of disable the oversubscribe feature of OpenMPI - defaults to False
+        enable_flux_backend (bool): enable the flux-framework as backend - defaults to False
+        enable_slurm_backend (bool): enable the SLURM queueing system as backend - defaults to False
+        enable_mpi4py_backend (bool): enable the mpi4py.futures module - defaults to True
+        enable_multi_host (bool): communicate the host to connect to - defaults to False
+
+    Returns:
+        list: list of strings to be executed on the command line
+    """
+    if enable_mpi4py_backend:
+        executable = "mpipool.py"
+    else:
+        executable = "mpiexec.py"
+    return command_line_options(
+        hostname=socket.gethostname(),
+        port_selected=port_selected,
+        path=os.path.abspath(
+            os.path.join(__file__, "../../parallel_executors", executable)
+        ),
+        cores=cores,
+        cores_per_task=cores_per_task,
+        oversubscribe=oversubscribe,
+        enable_flux_backend=enable_flux_backend,
+        enable_slurm_backend=enable_slurm_backend,
+        enable_mpi4py_backend=enable_mpi4py_backend,
+        enable_multi_host=enable_multi_host,
+    )
+
+
+def _execute_parallel_tasks_loop(interface, future_queue):
+    while True:
+        task_dict = future_queue.get()
+        if "shutdown" in task_dict.keys() and task_dict["shutdown"]:
+            interface.shutdown(wait=task_dict["wait"])
+            break
+        elif "fn" in task_dict.keys() and "future" in task_dict.keys():
+            f = task_dict.pop("future")
+            if f.set_running_or_notify_cancel():
+                f.set_result(interface.send_and_receive_dict(input_dict=task_dict))
+        elif "fn" in task_dict.keys() and "init" in task_dict.keys():
+            interface.send_dict(input_dict=task_dict)
+
+
+def _execute_serial_tasks_loop(
+    interface, future_queue, future_dict, sleep_interval=0.1
+):
+    while True:
+        try:
+            task_dict = future_queue.get_nowait()
+        except queue.Empty:
+            pass
+        else:
+            if "shutdown" in task_dict.keys() and task_dict["shutdown"]:
+                done_dict = interface.shutdown(wait=task_dict["wait"])
+                if isinstance(done_dict, dict):
+                    for k, v in done_dict.items():
+                        if k in future_dict.keys() and not future_dict[k].cancelled():
+                            future_dict.pop(k).set_result(v)
+                break
+            elif "fn" in task_dict.keys() and "future" in task_dict.keys():
+                f = task_dict.pop("future")
+                future_hash = interface.send_and_receive_dict(input_dict=task_dict)
+                future_dict[future_hash] = f
+        _update_future_dict(
+            interface=interface, future_dict=future_dict, sleep_interval=sleep_interval
+        )
+
+
+def _update_future_dict(interface, future_dict, sleep_interval=0.1):
     time.sleep(sleep_interval)
     hash_to_update = [h for h, f in future_dict.items() if not f.done()]
     hash_to_cancel = [h for h, f in future_dict.items() if f.cancelled()]
     if len(hash_to_update) > 0:
         for k, v in interface.send_and_receive_dict(
             input_dict={"update": hash_to_update}
         ).items():
             future_dict.pop(k).set_result(v)
     if len(hash_to_cancel) > 0 and interface.send_and_receive_dict(
         input_dict={"cancel": hash_to_cancel}
     ):
         for h in hash_to_cancel:
             del future_dict[h]
-
-
-def cloudpickle_register(ind=2):
-    # Cloudpickle can either pickle by value or pickle by reference. The functions which are communicated have to
-    # be pickled by value rather than by reference, so the module which calls the map function is pickled by value.
-    # https://github.com/cloudpipe/cloudpickle#overriding-pickles-serialization-mechanism-for-importable-constructs
-    # inspect can help to find the module which is calling pympipool
-    # https://docs.python.org/3/library/inspect.html
-    # to learn more about inspect another good read is:
-    # http://pymotw.com/2/inspect/index.html#module-inspect
-    # 1 refers to 1 level higher than the map function
-    try:  # When executed in a jupyter notebook this can cause a ValueError - in this case we just ignore it.
-        cloudpickle.register_pickle_by_value(inspect.getmodule(inspect.stack()[ind][0]))
-    except ValueError:
-        pass
-
-
-def cancel_items_in_queue(que):
-    while True:
-        try:
-            item = que.get_nowait()
-            if isinstance(item, dict) and "future" in item.keys():
-                item["future"].cancel()
-        except queue.Empty:
-            break
```

### Comparing `pympipool-0.5.3/pympipool.egg-info/PKG-INFO` & `pympipool-0.5.4/pympipool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.5.3
+Version: 0.5.4
 Summary: pympipool - scale python functions over multiple compute nodes
 Home-page: https://github.com/jan-janssen/pympipool
 Author-email: jan.janssen@outlook.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pympipool-0.5.3/setup.py` & `pympipool-0.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.3/tests/test_communicator_split.py` & `pympipool-0.5.4/tests/test_communicator_split.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.3/tests/test_executor.py` & `pympipool-0.5.4/tests/test_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 from concurrent.futures import ThreadPoolExecutor
-from pympipool.share.parallel import map_funct, parse_socket_communication, call_funct
+from pympipool.shared_functions.parallel_executors import map_funct, parse_socket_communication, call_funct
 
 
 def function_multi_args(a, b):
     return a + b
 
 
 class TestExecutor(unittest.TestCase):
```

### Comparing `pympipool-0.5.3/tests/test_future.py` & `pympipool-0.5.4/tests/test_future.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.3/tests/test_interface.py` & `pympipool-0.5.4/tests/test_interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import unittest
-from pympipool.share.communication import SocketInterface
-from pympipool.share.serial import get_parallel_subprocess_command, cloudpickle_register
+from pympipool.external_interfaces.communication import SocketInterface
+from pympipool.shared_functions.external_interfaces import get_parallel_subprocess_command, cloudpickle_register
 
 
 def calc(i):
     return np.array(i ** 2)
 
 
 class TestInterface(unittest.TestCase):
```

### Comparing `pympipool-0.5.3/tests/test_multitask.py` & `pympipool-0.5.4/tests/test_multitask.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import unittest
 from queue import Queue
 from time import sleep
 from pympipool import PoolExecutor
-from pympipool.share.serial import execute_serial_tasks, cloudpickle_register
+from pympipool.shared_functions.external_interfaces import execute_serial_tasks, cloudpickle_register
 from concurrent.futures import Future
 
 
 def calc(i):
     return np.array(i ** 2)
```

### Comparing `pympipool-0.5.3/tests/test_parse.py` & `pympipool-0.5.4/tests/test_parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
-from pympipool.executor.mpipool import parse_arguments
-from pympipool.share.serial import command_line_options
+from pympipool.parallel_executors.mpipool import parse_arguments
+from pympipool.shared_functions.external_interfaces import command_line_options
 
 
 class TestParser(unittest.TestCase):
     def test_command_local(self):
         result_dict = {
             'host': 'localhost',
             'total_cores': '2',
```

### Comparing `pympipool-0.5.3/tests/test_pool.py` & `pympipool-0.5.4/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.3/tests/test_queue.py` & `pympipool-0.5.4/tests/test_queue.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from concurrent.futures import Future, CancelledError
 from queue import Queue
-from pympipool.share.serial import cancel_items_in_queue
+from pympipool.shared_functions.external_interfaces import cancel_items_in_queue
 
 
 class TestQueue(unittest.TestCase):
     def test_cancel_items_in_queue(self):
         q = Queue()
         fs1 = Future()
         fs2 = Future()
```

### Comparing `pympipool-0.5.3/tests/test_task.py` & `pympipool-0.5.4/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.3/tests/test_worker.py` & `pympipool-0.5.4/tests/test_worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import unittest
 from queue import Queue
 from time import sleep
 from concurrent.futures import CancelledError
 from pympipool import Executor
-from pympipool.share.serial import execute_parallel_tasks, cloudpickle_register
+from pympipool.shared_functions.external_interfaces import execute_parallel_tasks, cloudpickle_register
 from concurrent.futures import Future
 
 
 def calc(i):
     return np.array(i ** 2)
```

### Comparing `pympipool-0.5.3/tests/test_worker_memory.py` & `pympipool-0.5.4/tests/test_worker_memory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 import numpy as np
 from queue import Queue
 from pympipool import Executor
-from pympipool.share.parallel import call_funct
-from pympipool.share.serial import execute_parallel_tasks, cloudpickle_register
+from pympipool.shared_functions.parallel_executors import call_funct
+from pympipool.shared_functions.external_interfaces import execute_parallel_tasks, cloudpickle_register
 from concurrent.futures import Future
 
 
 def get_global(memory=None):
     return memory
```

### Comparing `pympipool-0.5.3/tests/test_zmq.py` & `pympipool-0.5.4/tests/test_zmq.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 import zmq
-from pympipool.share.communication import (
+from pympipool.external_interfaces.communication import (
     connect_to_socket_interface,
     close_connection,
     send_result,
     receive_instruction
 )
```

### Comparing `pympipool-0.5.3/versioneer.py` & `pympipool-0.5.4/versioneer.py`

 * *Files identical despite different names*

