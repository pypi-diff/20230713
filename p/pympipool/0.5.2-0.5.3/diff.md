# Comparing `tmp/pympipool-0.5.2.tar.gz` & `tmp/pympipool-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pympipool-0.5.2.tar", last modified: Wed Jul 12 00:54:24 2023, max compression
+gzip compressed data, was "pympipool-0.5.3.tar", last modified: Thu Jul 13 04:07:03 2023, max compression
```

## Comparing `pympipool-0.5.2.tar` & `pympipool-0.5.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:54:24.716657 pympipool-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-12 00:54:21.000000 pympipool-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-12 00:54:21.000000 pympipool-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-12 00:54:24.716657 pympipool-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-07-12 00:54:21.000000 pympipool-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:54:24.716657 pympipool-0.5.2/pympipool/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-12 00:54:21.000000 pympipool-0.5.2/pympipool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-12 00:54:24.716657 pympipool-0.5.2/pympipool/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:54:24.712656 pympipool-0.5.2/pympipool/executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 00:54:21.000000 pympipool-0.5.2/pympipool/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-12 00:54:21.000000 pympipool-0.5.2/pympipool/executor/mpiexec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-12 00:54:21.000000 pympipool-0.5.2/pympipool/executor/mpipool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:54:24.712656 pympipool-0.5.2/pympipool/share/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 00:54:21.000000 pympipool-0.5.2/pympipool/share/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-12 00:54:21.000000 pympipool-0.5.2/pympipool/share/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-07-12 00:54:21.000000 pympipool-0.5.2/pympipool/share/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-07-12 00:54:21.000000 pympipool-0.5.2/pympipool/share/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-07-12 00:54:21.000000 pympipool-0.5.2/pympipool/share/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-12 00:54:21.000000 pympipool-0.5.2/pympipool/share/serial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:54:24.712656 pympipool-0.5.2/pympipool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-12 00:54:24.000000 pympipool-0.5.2/pympipool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-12 00:54:24.000000 pympipool-0.5.2/pympipool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 00:54:24.000000 pympipool-0.5.2/pympipool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-12 00:54:24.000000 pympipool-0.5.2/pympipool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 00:54:24.000000 pympipool-0.5.2/pympipool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-12 00:54:24.716657 pympipool-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-12 00:54:24.000000 pympipool-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 00:54:24.716657 pympipool-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-12 00:54:21.000000 pympipool-0.5.2/tests/test_communicator_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-07-12 00:54:21.000000 pympipool-0.5.2/tests/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-12 00:54:21.000000 pympipool-0.5.2/tests/test_future.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-12 00:54:21.000000 pympipool-0.5.2/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-12 00:54:21.000000 pympipool-0.5.2/tests/test_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-12 00:54:21.000000 pympipool-0.5.2/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-12 00:54:21.000000 pympipool-0.5.2/tests/test_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-12 00:54:21.000000 pympipool-0.5.2/tests/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-12 00:54:21.000000 pympipool-0.5.2/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-12 00:54:21.000000 pympipool-0.5.2/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-12 00:54:21.000000 pympipool-0.5.2/tests/test_worker_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-12 00:54:21.000000 pympipool-0.5.2/tests/test_zmq.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-12 00:54:21.000000 pympipool-0.5.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 04:07:03.163276 pympipool-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-13 04:07:00.000000 pympipool-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-13 04:07:00.000000 pympipool-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-13 04:07:03.163276 pympipool-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-07-13 04:07:00.000000 pympipool-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 04:07:03.163276 pympipool-0.5.3/pympipool/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-13 04:07:00.000000 pympipool-0.5.3/pympipool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-13 04:07:03.163276 pympipool-0.5.3/pympipool/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 04:07:03.159276 pympipool-0.5.3/pympipool/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 04:07:00.000000 pympipool-0.5.3/pympipool/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-13 04:07:00.000000 pympipool-0.5.3/pympipool/executor/mpiexec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-13 04:07:00.000000 pympipool-0.5.3/pympipool/executor/mpipool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 04:07:03.159276 pympipool-0.5.3/pympipool/share/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 04:07:00.000000 pympipool-0.5.3/pympipool/share/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-13 04:07:00.000000 pympipool-0.5.3/pympipool/share/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-07-13 04:07:00.000000 pympipool-0.5.3/pympipool/share/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-07-13 04:07:00.000000 pympipool-0.5.3/pympipool/share/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-07-13 04:07:00.000000 pympipool-0.5.3/pympipool/share/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-07-13 04:07:00.000000 pympipool-0.5.3/pympipool/share/serial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 04:07:03.159276 pympipool-0.5.3/pympipool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-13 04:07:03.000000 pympipool-0.5.3/pympipool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-13 04:07:03.000000 pympipool-0.5.3/pympipool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 04:07:03.000000 pympipool-0.5.3/pympipool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 04:07:03.000000 pympipool-0.5.3/pympipool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 04:07:03.000000 pympipool-0.5.3/pympipool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-13 04:07:03.163276 pympipool-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-13 04:07:02.000000 pympipool-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 04:07:03.163276 pympipool-0.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-13 04:07:00.000000 pympipool-0.5.3/tests/test_communicator_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-07-13 04:07:00.000000 pympipool-0.5.3/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-13 04:07:00.000000 pympipool-0.5.3/tests/test_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-13 04:07:00.000000 pympipool-0.5.3/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-13 04:07:00.000000 pympipool-0.5.3/tests/test_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-13 04:07:00.000000 pympipool-0.5.3/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-13 04:07:00.000000 pympipool-0.5.3/tests/test_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-13 04:07:00.000000 pympipool-0.5.3/tests/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-13 04:07:00.000000 pympipool-0.5.3/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-13 04:07:00.000000 pympipool-0.5.3/tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-13 04:07:00.000000 pympipool-0.5.3/tests/test_worker_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-13 04:07:00.000000 pympipool-0.5.3/tests/test_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-13 04:07:00.000000 pympipool-0.5.3/versioneer.py
```

### Comparing `pympipool-0.5.2/LICENSE` & `pympipool-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.2/PKG-INFO` & `pympipool-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.5.2
+Version: 0.5.3
 Summary: pympipool - scale python functions over multiple compute nodes
 Home-page: https://github.com/jan-janssen/pympipool
 Author-email: jan.janssen@outlook.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pympipool-0.5.2/README.md` & `pympipool-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.2/pympipool/executor/mpiexec.py` & `pympipool-0.5.3/pympipool/executor/mpiexec.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.2/pympipool/executor/mpipool.py` & `pympipool-0.5.3/pympipool/executor/mpipool.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.2/pympipool/share/communication.py` & `pympipool-0.5.3/pympipool/share/communication.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import subprocess
 
 import cloudpickle
 import zmq
 
 
 class SocketInterface(object):
-    def __init__(self):
+    def __init__(self, queue_adapter=None, queue_adapter_kwargs=None):
         self._context = zmq.Context()
         self._socket = self._context.socket(zmq.PAIR)
         self._process = None
+        self._queue_adapter = queue_adapter
+        self._queue_adapter_kwargs = queue_adapter_kwargs
 
     def send_dict(self, input_dict):
         self._socket.send(cloudpickle.dumps(input_dict))
 
     def receive_dict(self):
         output = cloudpickle.loads(self._socket.recv())
         if "result" in output.keys():
@@ -24,30 +26,42 @@
     def send_and_receive_dict(self, input_dict):
         self.send_dict(input_dict=input_dict)
         return self.receive_dict()
 
     def bind_to_random_port(self):
         return self._socket.bind_to_random_port("tcp://*")
 
-    def bootup(self, command_lst, cwd=None):
-        self._process = subprocess.Popen(
-            args=command_lst,
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
-            stdin=subprocess.PIPE,
-            cwd=cwd,
-        )
+    def bootup(self, command_lst, cwd=None, cores=None):
+        if self._queue_adapter is not None:
+            self._queue_adapter.submit_job(
+                working_directory=cwd,
+                cores=cores,
+                command=" ".join(command_lst),
+                **self._queue_adapter_kwargs
+            )
+        else:
+            self._process = subprocess.Popen(
+                args=command_lst,
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+                stdin=subprocess.PIPE,
+                cwd=cwd,
+            )
 
     def shutdown(self, wait=True):
         result = None
         if self._process is not None and self._process.poll() is None:
             result = self.send_and_receive_dict(
                 input_dict={"shutdown": True, "wait": wait}
             )
             self._process_close(wait=wait)
+        elif self._queue_adapter is not None and self._socket is not None:
+            result = self.send_and_receive_dict(
+                input_dict={"shutdown": True, "wait": wait}
+            )
         if self._socket is not None:
             self._socket.close()
         if self._context is not None:
             self._context.term()
         self._process = None
         self._socket = None
         self._context = None
```

### Comparing `pympipool-0.5.2/pympipool/share/executor.py` & `pympipool-0.5.3/pympipool/share/executor.py`

 * *Files 18% similar despite different names*

```diff
@@ -92,19 +92,29 @@
     def __init__(
         self,
         cores,
         oversubscribe=False,
         enable_flux_backend=False,
         init_function=None,
         cwd=None,
+        queue_adapter=None,
+        queue_adapter_kwargs=None,
     ):
         super().__init__()
         self._process = Thread(
             target=execute_parallel_tasks,
-            args=(self._future_queue, cores, oversubscribe, enable_flux_backend, cwd),
+            kwargs={
+                "future_queue": self._future_queue,
+                "cores": cores,
+                "oversubscribe": oversubscribe,
+                "enable_flux_backend": enable_flux_backend,
+                "cwd": cwd,
+                "queue_adapter": queue_adapter,
+                "queue_adapter_kwargs": queue_adapter_kwargs,
+            },
         )
         self._process.start()
         if init_function is not None:
             self._future_queue.put(
                 {"init": True, "fn": init_function, "args": (), "kwargs": {}}
             )
 
@@ -113,21 +123,25 @@
     def __init__(
         self,
         max_workers=1,
         oversubscribe=False,
         enable_flux_backend=False,
         cwd=None,
         sleep_interval=0.1,
+        queue_adapter=None,
+        queue_adapter_kwargs=None,
     ):
         super().__init__()
         self._process = Thread(
             target=execute_serial_tasks,
-            args=(
-                self._future_queue,
-                max_workers,
-                oversubscribe,
-                enable_flux_backend,
-                cwd,
-                sleep_interval,
-            ),
+            kwargs={
+                "future_queue": self._future_queue,
+                "cores": max_workers,
+                "oversubscribe": oversubscribe,
+                "enable_flux_backend": enable_flux_backend,
+                "cwd": cwd,
+                "sleep_interval": sleep_interval,
+                "queue_adapter": queue_adapter,
+                "queue_adapter_kwargs": queue_adapter_kwargs,
+            },
         )
         self._process.start()
```

### Comparing `pympipool-0.5.2/pympipool/share/parallel.py` & `pympipool-0.5.3/pympipool/share/parallel.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.2/pympipool/share/pool.py` & `pympipool-0.5.3/pympipool/share/pool.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from pympipool.share.communication import SocketInterface
 from pympipool.share.serial import get_parallel_subprocess_command, cloudpickle_register
 
 
 class PoolBase(object):
-    def __init__(self):
+    def __init__(self, queue_adapter=None, queue_adapter_kwargs=None):
         self._future_dict = {}
-        self._interface = SocketInterface()
+        self._interface = SocketInterface(
+            queue_adapter=queue_adapter, queue_adapter_kwargs=queue_adapter_kwargs
+        )
         cloudpickle_register(ind=3)
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.shutdown(wait=True)
@@ -47,26 +49,32 @@
 
     def __init__(
         self,
         max_workers=1,
         oversubscribe=False,
         enable_flux_backend=False,
         cwd=None,
+        queue_adapter=None,
+        queue_adapter_kwargs=None,
     ):
-        super().__init__()
+        super().__init__(
+            queue_adapter=queue_adapter, queue_adapter_kwargs=queue_adapter_kwargs
+        )
         self._interface.bootup(
             command_lst=get_parallel_subprocess_command(
                 port_selected=self._interface.bind_to_random_port(),
                 cores=max_workers,
                 cores_per_task=1,
                 oversubscribe=oversubscribe,
                 enable_flux_backend=enable_flux_backend,
                 enable_mpi4py_backend=True,
+                enable_multi_host=queue_adapter is not None,
             ),
             cwd=cwd,
+            cores=max_workers,
         )
 
     def map(self, func, iterable, chunksize=None):
         """
         Map a given function on a list of attributes.
 
         Args:
@@ -141,26 +149,32 @@
 
     def __init__(
         self,
         max_ranks=1,
         ranks_per_task=1,
         oversubscribe=False,
         cwd=None,
+        queue_adapter=None,
+        queue_adapter_kwargs=None,
     ):
-        super().__init__()
+        super().__init__(
+            queue_adapter=queue_adapter, queue_adapter_kwargs=queue_adapter_kwargs
+        )
         self._interface.bootup(
             command_lst=get_parallel_subprocess_command(
                 port_selected=self._interface.bind_to_random_port(),
                 cores=max_ranks,
                 cores_per_task=ranks_per_task,
                 oversubscribe=oversubscribe,
                 enable_flux_backend=False,
                 enable_mpi4py_backend=True,
+                enable_multi_host=queue_adapter is not None,
             ),
             cwd=cwd,
+            cores=max_ranks,
         )
 
     def map(self, func, iterable, chunksize=None):
         """
         Map a given function on a list of attributes.
 
         Args:
```

### Comparing `pympipool-0.5.2/pympipool/share/serial.py` & `pympipool-0.5.3/pympipool/share/serial.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     port_selected,
     path,
     cores,
     cores_per_task=1,
     oversubscribe=False,
     enable_flux_backend=False,
     enable_mpi4py_backend=True,
+    enable_multi_host=False,
 ):
     if enable_flux_backend:
         command_lst = ["flux", "run"]
     else:
         command_lst = ["mpiexec"]
     if oversubscribe:
         command_lst += ["--oversubscribe"]
@@ -30,15 +31,15 @@
     elif cores_per_task > 1 and enable_mpi4py_backend:
         # Running MPI parallel tasks within the map() requires mpi4py to use mpi spawn:
         # https://github.com/mpi4py/mpi4py/issues/324
         command_lst += ["-n", "1", "python"]
     else:
         command_lst += ["-n", str(cores), "python"]
     command_lst += [path]
-    if enable_flux_backend:
+    if enable_flux_backend or enable_multi_host:
         command_lst += [
             "--host",
             hostname,
         ]
     command_lst += [
         "--zmqport",
         str(port_selected),
@@ -56,101 +57,132 @@
 def get_parallel_subprocess_command(
     port_selected,
     cores,
     cores_per_task=1,
     oversubscribe=False,
     enable_flux_backend=False,
     enable_mpi4py_backend=True,
+    enable_multi_host=False,
 ):
     if enable_mpi4py_backend:
         executable = "mpipool.py"
     else:
         executable = "mpiexec.py"
     command_lst = command_line_options(
         hostname=socket.gethostname(),
         port_selected=port_selected,
         path=os.path.abspath(os.path.join(__file__, "../../executor", executable)),
         cores=cores,
         cores_per_task=cores_per_task,
         oversubscribe=oversubscribe,
         enable_flux_backend=enable_flux_backend,
         enable_mpi4py_backend=enable_mpi4py_backend,
+        enable_multi_host=enable_multi_host,
     )
     return command_lst
 
 
+def execute_parallel_tasks_loop(interface, future_queue):
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
+def execute_serial_tasks_loop(interface, future_queue, future_dict, sleep_interval=0.1):
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
+        update_future_dict(
+            interface=interface, future_dict=future_dict, sleep_interval=sleep_interval
+        )
+
+
 def execute_parallel_tasks(
-    future_queue, cores, oversubscribe=False, enable_flux_backend=False, cwd=None
+    future_queue,
+    cores,
+    oversubscribe=False,
+    enable_flux_backend=False,
+    cwd=None,
+    queue_adapter=None,
+    queue_adapter_kwargs=None,
 ):
-    interface = SocketInterface()
+    interface = SocketInterface(
+        queue_adapter=queue_adapter, queue_adapter_kwargs=queue_adapter_kwargs
+    )
     interface.bootup(
         command_lst=get_parallel_subprocess_command(
             port_selected=interface.bind_to_random_port(),
             cores=cores,
             cores_per_task=1,
             oversubscribe=oversubscribe,
             enable_flux_backend=enable_flux_backend,
             enable_mpi4py_backend=False,
+            enable_multi_host=queue_adapter is not None,
         ),
         cwd=cwd,
+        cores=cores,
     )
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
+    execute_parallel_tasks_loop(interface=interface, future_queue=future_queue)
 
 
 def execute_serial_tasks(
     future_queue,
     cores,
     oversubscribe=False,
     enable_flux_backend=False,
     cwd=None,
     sleep_interval=0.1,
+    queue_adapter=None,
+    queue_adapter_kwargs=None,
 ):
     future_dict = {}
-    interface = SocketInterface()
+    interface = SocketInterface(
+        queue_adapter=queue_adapter, queue_adapter_kwargs=queue_adapter_kwargs
+    )
     interface.bootup(
         command_lst=get_parallel_subprocess_command(
             port_selected=interface.bind_to_random_port(),
             cores=cores,
             cores_per_task=1,
             oversubscribe=oversubscribe,
             enable_flux_backend=enable_flux_backend,
             enable_mpi4py_backend=True,
+            enable_multi_host=queue_adapter is not None,
         ),
         cwd=cwd,
+        cores=cores,
+    )
+    execute_serial_tasks_loop(
+        interface=interface,
+        future_queue=future_queue,
+        future_dict=future_dict,
+        sleep_interval=sleep_interval,
     )
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
 
 
 def update_future_dict(interface, future_dict, sleep_interval=0.1):
     time.sleep(sleep_interval)
     hash_to_update = [h for h, f in future_dict.items() if not f.done()]
     hash_to_cancel = [h for h, f in future_dict.items() if f.cancelled()]
     if len(hash_to_update) > 0:
```

### Comparing `pympipool-0.5.2/pympipool.egg-info/PKG-INFO` & `pympipool-0.5.3/pympipool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.5.2
+Version: 0.5.3
 Summary: pympipool - scale python functions over multiple compute nodes
 Home-page: https://github.com/jan-janssen/pympipool
 Author-email: jan.janssen@outlook.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pympipool-0.5.2/pympipool.egg-info/SOURCES.txt` & `pympipool-0.5.3/pympipool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.2/setup.py` & `pympipool-0.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.2/tests/test_communicator_split.py` & `pympipool-0.5.3/tests/test_communicator_split.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.2/tests/test_executor.py` & `pympipool-0.5.3/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.2/tests/test_future.py` & `pympipool-0.5.3/tests/test_future.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.2/tests/test_interface.py` & `pympipool-0.5.3/tests/test_interface.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     return np.array(i ** 2)
 
 
 class TestInterface(unittest.TestCase):
     def test_interface(self):
         cloudpickle_register(ind=1)
         task_dict = {"fn": calc, 'args': (), "kwargs": {"i": 2}}
-        interface = SocketInterface()
+        interface = SocketInterface(queue_adapter=None, queue_adapter_kwargs=None)
         interface.bootup(
             command_lst=get_parallel_subprocess_command(
                 port_selected=interface.bind_to_random_port(),
                 cores=1,
                 cores_per_task=1,
                 oversubscribe=False,
                 enable_flux_backend=False,
```

### Comparing `pympipool-0.5.2/tests/test_multitask.py` & `pympipool-0.5.3/tests/test_multitask.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.2/tests/test_parse.py` & `pympipool-0.5.3/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.2/tests/test_pool.py` & `pympipool-0.5.3/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.2/tests/test_queue.py` & `pympipool-0.5.3/tests/test_queue.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.2/tests/test_task.py` & `pympipool-0.5.3/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.2/tests/test_worker.py` & `pympipool-0.5.3/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.2/tests/test_worker_memory.py` & `pympipool-0.5.3/tests/test_worker_memory.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.2/tests/test_zmq.py` & `pympipool-0.5.3/tests/test_zmq.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.5.2/versioneer.py` & `pympipool-0.5.3/versioneer.py`

 * *Files identical despite different names*

