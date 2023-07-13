# Comparing `tmp/deadpool_executor-2023.7.5.tar.gz` & `tmp/deadpool_executor-2023.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deadpool_executor-2023.7.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "deadpool_executor-2023.7.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `deadpool_executor-2023.7.5.tar` & `deadpool_executor-2023.7.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       66 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.5/.coveragerc
--rw-r--r--   0        0        0    34523 2022-10-24 05:21:18.405196 deadpool_executor-2023.7.5/LICENSE
--rw-r--r--   0        0        0    23161 2023-07-12 20:43:26.395603 deadpool_executor-2023.7.5/README.rst
--rw-r--r--   0        0        0       86 2023-07-12 11:42:09.927732 deadpool_executor-2023.7.5/covstart.pth
--rw-r--r--   0        0        0    24234 2023-07-12 20:43:46.151456 deadpool_executor-2023.7.5/deadpool.py
--rw-r--r--   0        0        0      477 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.5/examples/callbacks.py
--rw-r--r--   0        0        0      751 2023-07-09 23:58:41.948872 deadpool_executor-2023.7.5/examples/entrypoint.py
--rw-r--r--   0        0        0      961 2023-07-12 14:22:32.777642 deadpool_executor-2023.7.5/examples/leftover.py
--rw-r--r--   0        0        0      737 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.5/examples/priorities.py
--rw-r--r--   0        0        0     1230 2023-07-12 20:43:26.399603 deadpool_executor-2023.7.5/noxfile.py
--rw-r--r--   0        0        0     1335 2023-07-12 20:43:26.399603 deadpool_executor-2023.7.5/pyproject.toml
--rw-r--r--   0        0        0      183 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.5/tests/conftest.py
--rw-r--r--   0        0        0    10238 2023-07-12 20:43:26.399603 deadpool_executor-2023.7.5/tests/test_deadpool.py
--rw-r--r--   0        0        0    24240 1970-01-01 00:00:00.000000 deadpool_executor-2023.7.5/PKG-INFO
+-rw-r--r--   0        0        0       66 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.6/.coveragerc
+-rw-r--r--   0        0        0    34523 2022-10-24 05:21:18.405196 deadpool_executor-2023.7.6/LICENSE
+-rw-r--r--   0        0        0    24687 2023-07-12 21:30:05.391425 deadpool_executor-2023.7.6/README.rst
+-rw-r--r--   0        0        0       86 2023-07-12 11:42:09.927732 deadpool_executor-2023.7.6/covstart.pth
+-rw-r--r--   0        0        0    25248 2023-07-13 13:46:37.647452 deadpool_executor-2023.7.6/deadpool.py
+-rw-r--r--   0        0        0      477 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.6/examples/callbacks.py
+-rw-r--r--   0        0        0      751 2023-07-09 23:58:41.948872 deadpool_executor-2023.7.6/examples/entrypoint.py
+-rw-r--r--   0        0        0      961 2023-07-12 14:22:32.777642 deadpool_executor-2023.7.6/examples/leftover.py
+-rw-r--r--   0        0        0      737 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.6/examples/priorities.py
+-rw-r--r--   0        0        0     1230 2023-07-12 20:43:26.399603 deadpool_executor-2023.7.6/noxfile.py
+-rw-r--r--   0        0        0     1335 2023-07-12 20:43:26.399603 deadpool_executor-2023.7.6/pyproject.toml
+-rw-r--r--   0        0        0      183 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.6/tests/conftest.py
+-rw-r--r--   0        0        0    12647 2023-07-13 13:46:28.639510 deadpool_executor-2023.7.6/tests/test_deadpool.py
+-rw-r--r--   0        0        0    25766 1970-01-01 00:00:00.000000 deadpool_executor-2023.7.6/PKG-INFO
```

### Comparing `deadpool_executor-2023.7.5/LICENSE` & `deadpool_executor-2023.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `deadpool_executor-2023.7.5/README.rst` & `deadpool_executor-2023.7.6/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -60,14 +60,18 @@
 ------------
 
 The python package name is *deadpool-executor*, so to install
 you must type ``$ pip install deadpool-executor``. The import
 name is *deadpool*, so in your Python code you must type
 ``import deadpool`` to use it.
 
+I try quite hard to keep dependencies to a minimum. Currently
+``Deadpool`` has no dependencies other than ``psutil`` which
+is simply too useful to avoid for this library.
+
 Why would I want to use this?
 -----------------------------
 
 I created ``Deadpool`` because I became frustrated with the
 stdlib `ProcessPoolExecutor`_, and various other community
 implementations of process pools. In particular, I had a use-case
 that required a high server uptime, but also had variable and
@@ -100,75 +104,105 @@
 -----------------------------------------
 
 ``Deadpool`` is generally similar to `ProcessPoolExecutor`_ since it executes
 tasks in subprocesses, and implements the standard ``Executor`` abstract
 interface. We can draw a few comparisons to the stdlib pool to guide
 your decision process about whether this makes sense for your use-case:
 
-- ``Deadpool`` precreates all subprocesses up to the pool size.
+Similarities
+^^^^^^^^^^^^
+
 - ``Deadpool`` also supports the
   ``max_tasks_per_child`` parameter (a new feature in
   Python 3.11, although it was available in `multiprocessing.Pool`_
   since Python 3.2).
-- ``Deadpool`` tasks can have priorities. When the executor chooses
-  the next pending task to schedule to a subprocess, it chooses the
-  pending task with the highest priority. This gives you a way of
-  prioritizing certain kinds of tasks. For example, you might give
-  UI-sensitive tasks a higher priority to deliver a more snappy
-  user experience to your users.
+- The "initializer" callback in ``Deadpool`` works the same.
 - ``Deadpool`` defaults to the `forkserver <https://docs.python.org/3.11/library/multiprocessing.html#contexts-and-start-methods>`_ multiprocessing
   context, unlike the stdlib pool which defaults to ``fork`` on
   Linux. It's just a setting though, you can change it in the same way as
   with the stdlib pool. Like the stdlib, I strongly advise you to avoid
   using ``fork`` because propagation threads and locks via fork is
-  going to ruin your day eventually.
-- ``Deadpool`` can ask the system allocator (Linux only) to return
-  unused memory back to the OS based on exceeding a max threshold RSS.
-  For long-running pools and modern
-  kernels, the system memory allocator can hold onto unused memory
-  for a surprisingly long time, and coupled with bloat due to
-  memory fragmentation, this can result in carrying very large
-  RSS values in your pool. The ``max_tasks_per_child`` helps with
-  this because a subprocess is entirely erased when the max is
-  reached, but it does mean that periodically there will be a small
-  latency penalty from constructing the replacement subprocess. In
-  my opinion, ``max_tasks_per_child`` is appropriate for when you
-  know or suspect there's a real memory leak somewhere in your code
-  (or a 3rd-party package!), and the easiest way to deal with that
-  right now is just to periodically remove a process.
-- ``Deadpool`` tasks can have timeouts. When a task hits the timeout,
-  the underlying subprocess in the pool is killed with ``SIGKILL``.
-  The entire process tree of that subprocess is killed. Your application
-  logic needs to handle this. The ``finalizer`` will not run.
-- ``Deadpool`` tasks can have priorities. The priority is set in the
-  ``submit()`` call. See the examples later in this document for further
-  discussion on priorities.
-- The shutdown parameters ``wait`` and ``cancel_futures`` can behave
-  differently to how they work in the _ProcessPoolExecutor. This is
-  discussed in more detail later in this document.
+  going to ruin your day eventually. While this is a difference to the
+  default behaviour of the stdlib pool, it's not a difference in
+  behaviour to the stdlib pool when you use the ``forkserver`` context
+  which is the recommended context for multiprocessing.
+
+Differences in existing behaviour
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+``Deadpool`` differs from the stdlib pool in the following ways:
+
 - If a ``Deadpool`` subprocess in the pool is killed by some
   external actor, for example, the OS runs out of memory and the
   `OOM killer`_ kills a pool subprocess that is using too much memory,
   ``Deadpool`` does not care and further operation is unaffected.
   ``Deadpool`` will not, and indeed cannot raise
   `BrokenProcessPool <https://docs.python.org/3/library/concurrent.futures.html?highlight=broken%20process%20pool#concurrent.futures.process.BrokenProcessPool>`_ or
   `BrokenExecutor <https://docs.python.org/3/library/concurrent.futures.html?highlight=broken%20process%20pool#concurrent.futures.BrokenExecutor>`_.
+- ``Deadpool`` precreates all subprocesses up to the pool size on
+  creation.
+- ``Deadpool`` tasks can have priorities. When the executor chooses
+  the next pending task to schedule to a subprocess, it chooses the
+  pending task with the highest priority. This gives you a way of
+  prioritizing certain kinds of tasks. For example, you might give
+  UI-sensitive tasks a higher priority to deliver a more snappy
+  user experience to your users. The priority can be specified in
+  the ``submit`` call.
+- The shutdown parameters ``wait`` and ``cancel_futures`` can behave
+  differently to how they work in the `ProcessPoolExecutor`_. This is
+  discussed in more detail later in this document.
+- ``Deadpool`` currently only works on Linux. There isn't any specific
+  reason it can't work on other platforms. The malloc trim feature also
+  requires a glibc system, so probably won't work on Alpine.
+
+New features in Deadpool
+^^^^^^^^^^^^^^^^^^^^^^^^
+
+``Deadpool`` has the following features that are not present in the
+stdlib pool:
+
+- With ``Deadpool`` you can provider a "finalizer" callback that will
+  fire before a subprocess is shut down or killed. The finalizer callback
+  might be executed in a different thread than the main thread of the
+  subprocess, so don't rely on the callback running in the main
+  subprocess thread. There are certain circumstances where the finalizer
+  will not run at all, such as when the subprocess is killed by the OS
+  due to an out-of-memory (OOM) condition. So don't design your application
+  such that the finalizer is required to run for correct operation.
+- Even though ``Deadpool`` typically uses a hard kill to remove
+  subprocesses, it does still run any handlers registered with
+  ``atexit``.
+- ``Deadpool`` tasks can have timeouts. When a task hits the timeout,
+  the underlying subprocess in the pool is killed with ``SIGKILL``.
+  The entire process tree of that subprocess is killed. Your application
+  logic needs to handle this. The ``finalizer`` will not run.
 - ``Deadpool`` also allows a ``finalizer``, with corresponding
   ``finalargs``, that will be called after a task is executed on
   a subprocess, but before the subprocess terminates. It is
   analogous to the ``initializer`` and ``initargs`` parameters.
   Just like the ``initializer`` callable, the ``finalizer``
   callable is executed inside the subprocess. It is not guaranteed that
   the finalizer will always run. If a process is killed, e.g. due to a
   timeout or any other reason, the finalizer will not run. The finalizer
   could be used for things like flushing pending monitoring messages,
   such as traces and so on.
-- ``Deadpool`` currently only works on Linux. There isn't any specific
-  reason it can't work on other platforms. The malloc trim feature also
-  requires a glibc system, so probably won't work on Alpine.
+- ``Deadpool`` can ask the system allocator (Linux only) to return
+  unused memory back to the OS based on exceeding a max threshold RSS.
+  For long-running pools and modern
+  kernels, the system memory allocator can hold onto unused memory
+  for a surprisingly long time, and coupled with bloat due to
+  memory fragmentation, this can result in carrying very large
+  RSS values in your pool. The ``max_tasks_per_child`` helps with
+  this because a subprocess is entirely erased when the max is
+  reached, but it does mean that periodically there will be a small
+  latency penalty from constructing the replacement subprocess. In
+  my opinion, ``max_tasks_per_child`` is appropriate for when you
+  know or suspect there's a real memory leak somewhere in your code
+  (or a 3rd-party package!), and the easiest way to deal with that
+  right now is just to periodically remove a process.
 
 Show me some code
 -----------------
 
 Simple case
 ^^^^^^^^^^^
 
@@ -212,14 +246,18 @@
 
     with deadpool.Deadpool() as exe:
         fut = exe.submit(f, deadpool_timeout=1.0)
 
         with pytest.raises(deadpool.TimeoutError)
             fut.result()
 
+The parameter ``deadpool_timeout`` is special and consumed by ``Deadpool``
+in the call. You can't use a parameter with this name in your function 
+kwargs.
+
 Handling OOM killed situations
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. code-block:: python
 
     import time
     import deadpool
@@ -232,17 +270,17 @@
 
         try:
             result = fut.result()
         except deadpool.ProcessError:
             print("Oh no someone killed my task!")
 
 
-As long as the OOM killer terminates the subprocess (and not the main process),
-which is likely because it'll be your subprocess that is using too much
-memory, this will not hurt the pool, and it will be able to receive and
+As long as the OOM killer terminates merely a subprocess (and not the main
+process), which is likely because it'll be your subprocess that is using too
+much memory, this will not hurt the pool, and it will be able to receive and
 process more tasks. Note that this event will show up as a ``ProcessError``
 exception when accessing the future, so you have a way of at least tracking
 these events.
 
 Design Details
 --------------
```

### Comparing `deadpool_executor-2023.7.5/deadpool.py` & `deadpool_executor-2023.7.6/deadpool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,25 @@
 """
 Deadpool
 ========
 
+Important design considerations:
+
+Backpressure
+------------
+
+To allow backpressure when submitting work to the pool, we make
+the ``submit`` method block when the number of pending tasks is
+greater than the ``max_workers`` parameter. This has consequences,
+basically it means the main thread is blocked and nothing else
+can happen until it unblocks by getting space in the queue.
+
+Deadpool itself needs to do actions around job management, so
+this is why we have a separate "supervisor" thread for each
+worker process.
 
 """
 import concurrent.futures
 import ctypes
 import logging
 import multiprocessing as mp
 import os
@@ -21,15 +35,15 @@
 from dataclasses import dataclass, field
 from multiprocessing.connection import Connection
 from queue import Empty, PriorityQueue, Queue, SimpleQueue
 from typing import Callable, Optional, Tuple
 
 import psutil
 
-__version__ = "2023.7.5"
+__version__ = "2023.7.6"
 __all__ = [
     "Deadpool",
     "Future",
     "CancelledError",
     "TimeoutError",
     "ProcessError",
     "PoolClosed",
@@ -339,25 +353,36 @@
             if wp.tasks_ran_counter >= self.max_tasks_per_child:
                 logger.debug(f"Worker {wp.pid} hit max tasks per child.")
                 wp.shutdown(wait=False)
                 self.add_worker_to_pool()
                 return
 
         if self.max_worker_memory_bytes is not None:
-            if wp.get_rss_bytes() >= self.max_worker_memory_bytes:
+            mem = wp.get_rss_bytes()
+            logger.debug(f"Worker {wp.pid} has {mem} bytes of RSS memory.")
+            if mem >= self.max_worker_memory_bytes:
+                logger.debug(f"Worker {wp.pid} hit max memory threshold.")
                 wp.shutdown(wait=False)
                 self.add_worker_to_pool()
                 return
 
         self.workers.put(wp)
 
     def run_task(self, fn, args, kwargs, timeout, fut: Future):
         try:
             worker: WorkerProcess = self.get_process()
-            worker.submit_job((fn, args, kwargs, timeout))
+            try:
+                worker.submit_job((fn, args, kwargs, timeout))
+            except (pickle.PicklingError, AttributeError) as e:
+                # If the user passed in a function or params that can't
+                # be pickled, use the future to communicate the error.
+                fut.set_exception(e)
+                self.done_with_process(worker)
+                return
+
             fut.pid = worker.pid
             self.running_futs.add(fut)
 
             while True:
                 if worker.results_are_available():
                     try:
                         results = worker.get_results()
@@ -418,15 +443,16 @@
             try:
                 self.running_jobs.get_nowait()
             except Empty:  # pragma: no cover
                 logger.warning("Weird error, did not expect running jobs to be empty")
 
     def submit(
         self,
-        __fn: Callable,
+        fn: Callable,
+        /,
         *args,
         deadpool_timeout=None,
         deadpool_priority=0,
         **kwargs,
     ) -> Future:
         if deadpool_priority < 0:  # pragma: no cover
             raise ValueError(
@@ -436,15 +462,15 @@
         if self.closed:
             raise PoolClosed("The pool is closed. No more tasks can be submitted.")
 
         fut = Future()
         self.submitted_jobs.put(
             PrioritizedItem(
                 priority=deadpool_priority,
-                item=(__fn, args, kwargs, deadpool_timeout, fut),
+                item=(fn, args, kwargs, deadpool_timeout, fut),
             )
         )
         return fut
 
     def shutdown(self, wait: bool = True, *, cancel_futures: bool = False) -> None:
         logger.debug(f"shutdown: {wait=} {cancel_futures=}")
 
@@ -541,15 +567,15 @@
 def kill_proc_tree(
     pid,
     sig=signal.SIGTERM,
     include_parent=True,
     timeout=None,
     on_terminate=None,
     allow_kill_self=False,
-):  # pragma: no cover
+):
     """Kill a process tree (including grandchildren) with signal
     "sig" and return a (gone, still_alive) tuple.
     "on_terminate", if specified, is a callback function which is
     called as soon as a child terminates.
     """
     if not allow_kill_self and pid == os.getpid():
         raise ValueError("Won't kill myself")
```

### Comparing `deadpool_executor-2023.7.5/examples/entrypoint.py` & `deadpool_executor-2023.7.6/examples/entrypoint.py`

 * *Files identical despite different names*

### Comparing `deadpool_executor-2023.7.5/examples/leftover.py` & `deadpool_executor-2023.7.6/examples/leftover.py`

 * *Files identical despite different names*

### Comparing `deadpool_executor-2023.7.5/examples/priorities.py` & `deadpool_executor-2023.7.6/examples/priorities.py`

 * *Files identical despite different names*

### Comparing `deadpool_executor-2023.7.5/noxfile.py` & `deadpool_executor-2023.7.6/noxfile.py`

 * *Files identical despite different names*

### Comparing `deadpool_executor-2023.7.5/pyproject.toml` & `deadpool_executor-2023.7.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deadpool_executor-2023.7.5/tests/test_deadpool.py` & `deadpool_executor-2023.7.6/tests/test_deadpool.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import asyncio
 import logging
 import os
 import queue
 import signal
 import sys
 import time
-import unittest
 from concurrent.futures import CancelledError, as_completed
 from contextlib import contextmanager
 from functools import partial
 
 import pytest
 
 import deadpool
@@ -403,14 +402,94 @@
 
 
 def test_trim_memory():
     """Just testing it doesn't fail."""
     deadpool.trim_memory()
 
 
+leak_test_accumulator = bytearray()
+
+
+def leak_bytes(n):
+    leak_test_accumulator.extend(bytearray(n))
+
+
+def leaker(n):
+    leak_bytes(n)
+    return os.getpid()
+
+
+def test_max_memory(logging_initializer):
+    # Verify that the memory threshold feature in deadpool
+    # works as expected. This test will run 20 functions, 10
+    # of which will consume 1MB of memory. The other 10 will
+    # consume 0.1MB of memory. The memory threshold is set to
+    # 1.5MB, so the first 10 functions should cause their workers
+    # to be replaced by new workers, while the other 10 functions
+    # should be able to run without requiring their workers to be
+    # replaced. So we'll count the total number of subprocess PID
+    # values seen by a task, and verify the result.
+
+    leak_test_accumulator.clear()
+    with deadpool.Deadpool(
+        initializer=logging_initializer,
+        max_workers=1,
+        max_worker_memory_bytes=100_000_000,
+    ) as exe:
+        futs = []
+        for _ in range(10):
+            futs.append(exe.submit(leaker, 150_000_000))
+            futs.append(exe.submit(leaker, 100_000))
+
+        pids = set(f.result() for f in deadpool.as_completed(futs))
+
+    # We should see 11 unique PIDs, because the first 10 functions
+    # should have caused their workers to be replaced, while their
+    # replacements should have been able to run the remaining 10
+    # functions without being replaced.
+    assert len(pids) == 11
+
+
+def test_can_pickle_nested_function():
+    # Verify that deadpool raises a ValueError
+    # if the function can't be pickled.
+    def f():
+        pass
+
+    with deadpool.Deadpool() as exe:
+        fut = exe.submit(f)
+
+        with pytest.raises(AttributeError, match="Can't pickle local object"):
+            fut.result()
+
+
+def test_can_pickle_nested_function_cf():
+    """Check that stdlib works the same way."""
+    from concurrent.futures import ProcessPoolExecutor
+
+    def f():
+        pass
+
+    with ProcessPoolExecutor() as exe:
+        fut = exe.submit(f)
+
+        with pytest.raises(AttributeError, match="Can't pickle local object"):
+            fut.result()
+
+
+def test_can_pickle_lambda_function():
+    # Verify that deadpool raises a ValueError
+    # if the function can't be pickled.
+    with deadpool.Deadpool() as exe:
+        fut = exe.submit(lambda: 123)
+
+        with pytest.raises(AttributeError, match="Can't pickle local object"):
+            fut.result()
+
+
 @contextmanager
 def elapsed():
     t0 = time.perf_counter()
     try:
         yield
     finally:
         t1 = time.perf_counter()
```

### Comparing `deadpool_executor-2023.7.5/PKG-INFO` & `deadpool_executor-2023.7.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deadpool-executor
-Version: 2023.7.5
+Version: 2023.7.6
 Summary: Deadpool
 Author-email: Caleb Hattingh <caleb.hattingh@gmail.com>
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
@@ -85,14 +85,18 @@
 ------------
 
 The python package name is *deadpool-executor*, so to install
 you must type ``$ pip install deadpool-executor``. The import
 name is *deadpool*, so in your Python code you must type
 ``import deadpool`` to use it.
 
+I try quite hard to keep dependencies to a minimum. Currently
+``Deadpool`` has no dependencies other than ``psutil`` which
+is simply too useful to avoid for this library.
+
 Why would I want to use this?
 -----------------------------
 
 I created ``Deadpool`` because I became frustrated with the
 stdlib `ProcessPoolExecutor`_, and various other community
 implementations of process pools. In particular, I had a use-case
 that required a high server uptime, but also had variable and
@@ -125,75 +129,105 @@
 -----------------------------------------
 
 ``Deadpool`` is generally similar to `ProcessPoolExecutor`_ since it executes
 tasks in subprocesses, and implements the standard ``Executor`` abstract
 interface. We can draw a few comparisons to the stdlib pool to guide
 your decision process about whether this makes sense for your use-case:
 
-- ``Deadpool`` precreates all subprocesses up to the pool size.
+Similarities
+^^^^^^^^^^^^
+
 - ``Deadpool`` also supports the
   ``max_tasks_per_child`` parameter (a new feature in
   Python 3.11, although it was available in `multiprocessing.Pool`_
   since Python 3.2).
-- ``Deadpool`` tasks can have priorities. When the executor chooses
-  the next pending task to schedule to a subprocess, it chooses the
-  pending task with the highest priority. This gives you a way of
-  prioritizing certain kinds of tasks. For example, you might give
-  UI-sensitive tasks a higher priority to deliver a more snappy
-  user experience to your users.
+- The "initializer" callback in ``Deadpool`` works the same.
 - ``Deadpool`` defaults to the `forkserver <https://docs.python.org/3.11/library/multiprocessing.html#contexts-and-start-methods>`_ multiprocessing
   context, unlike the stdlib pool which defaults to ``fork`` on
   Linux. It's just a setting though, you can change it in the same way as
   with the stdlib pool. Like the stdlib, I strongly advise you to avoid
   using ``fork`` because propagation threads and locks via fork is
-  going to ruin your day eventually.
-- ``Deadpool`` can ask the system allocator (Linux only) to return
-  unused memory back to the OS based on exceeding a max threshold RSS.
-  For long-running pools and modern
-  kernels, the system memory allocator can hold onto unused memory
-  for a surprisingly long time, and coupled with bloat due to
-  memory fragmentation, this can result in carrying very large
-  RSS values in your pool. The ``max_tasks_per_child`` helps with
-  this because a subprocess is entirely erased when the max is
-  reached, but it does mean that periodically there will be a small
-  latency penalty from constructing the replacement subprocess. In
-  my opinion, ``max_tasks_per_child`` is appropriate for when you
-  know or suspect there's a real memory leak somewhere in your code
-  (or a 3rd-party package!), and the easiest way to deal with that
-  right now is just to periodically remove a process.
-- ``Deadpool`` tasks can have timeouts. When a task hits the timeout,
-  the underlying subprocess in the pool is killed with ``SIGKILL``.
-  The entire process tree of that subprocess is killed. Your application
-  logic needs to handle this. The ``finalizer`` will not run.
-- ``Deadpool`` tasks can have priorities. The priority is set in the
-  ``submit()`` call. See the examples later in this document for further
-  discussion on priorities.
-- The shutdown parameters ``wait`` and ``cancel_futures`` can behave
-  differently to how they work in the _ProcessPoolExecutor. This is
-  discussed in more detail later in this document.
+  going to ruin your day eventually. While this is a difference to the
+  default behaviour of the stdlib pool, it's not a difference in
+  behaviour to the stdlib pool when you use the ``forkserver`` context
+  which is the recommended context for multiprocessing.
+
+Differences in existing behaviour
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+``Deadpool`` differs from the stdlib pool in the following ways:
+
 - If a ``Deadpool`` subprocess in the pool is killed by some
   external actor, for example, the OS runs out of memory and the
   `OOM killer`_ kills a pool subprocess that is using too much memory,
   ``Deadpool`` does not care and further operation is unaffected.
   ``Deadpool`` will not, and indeed cannot raise
   `BrokenProcessPool <https://docs.python.org/3/library/concurrent.futures.html?highlight=broken%20process%20pool#concurrent.futures.process.BrokenProcessPool>`_ or
   `BrokenExecutor <https://docs.python.org/3/library/concurrent.futures.html?highlight=broken%20process%20pool#concurrent.futures.BrokenExecutor>`_.
+- ``Deadpool`` precreates all subprocesses up to the pool size on
+  creation.
+- ``Deadpool`` tasks can have priorities. When the executor chooses
+  the next pending task to schedule to a subprocess, it chooses the
+  pending task with the highest priority. This gives you a way of
+  prioritizing certain kinds of tasks. For example, you might give
+  UI-sensitive tasks a higher priority to deliver a more snappy
+  user experience to your users. The priority can be specified in
+  the ``submit`` call.
+- The shutdown parameters ``wait`` and ``cancel_futures`` can behave
+  differently to how they work in the `ProcessPoolExecutor`_. This is
+  discussed in more detail later in this document.
+- ``Deadpool`` currently only works on Linux. There isn't any specific
+  reason it can't work on other platforms. The malloc trim feature also
+  requires a glibc system, so probably won't work on Alpine.
+
+New features in Deadpool
+^^^^^^^^^^^^^^^^^^^^^^^^
+
+``Deadpool`` has the following features that are not present in the
+stdlib pool:
+
+- With ``Deadpool`` you can provider a "finalizer" callback that will
+  fire before a subprocess is shut down or killed. The finalizer callback
+  might be executed in a different thread than the main thread of the
+  subprocess, so don't rely on the callback running in the main
+  subprocess thread. There are certain circumstances where the finalizer
+  will not run at all, such as when the subprocess is killed by the OS
+  due to an out-of-memory (OOM) condition. So don't design your application
+  such that the finalizer is required to run for correct operation.
+- Even though ``Deadpool`` typically uses a hard kill to remove
+  subprocesses, it does still run any handlers registered with
+  ``atexit``.
+- ``Deadpool`` tasks can have timeouts. When a task hits the timeout,
+  the underlying subprocess in the pool is killed with ``SIGKILL``.
+  The entire process tree of that subprocess is killed. Your application
+  logic needs to handle this. The ``finalizer`` will not run.
 - ``Deadpool`` also allows a ``finalizer``, with corresponding
   ``finalargs``, that will be called after a task is executed on
   a subprocess, but before the subprocess terminates. It is
   analogous to the ``initializer`` and ``initargs`` parameters.
   Just like the ``initializer`` callable, the ``finalizer``
   callable is executed inside the subprocess. It is not guaranteed that
   the finalizer will always run. If a process is killed, e.g. due to a
   timeout or any other reason, the finalizer will not run. The finalizer
   could be used for things like flushing pending monitoring messages,
   such as traces and so on.
-- ``Deadpool`` currently only works on Linux. There isn't any specific
-  reason it can't work on other platforms. The malloc trim feature also
-  requires a glibc system, so probably won't work on Alpine.
+- ``Deadpool`` can ask the system allocator (Linux only) to return
+  unused memory back to the OS based on exceeding a max threshold RSS.
+  For long-running pools and modern
+  kernels, the system memory allocator can hold onto unused memory
+  for a surprisingly long time, and coupled with bloat due to
+  memory fragmentation, this can result in carrying very large
+  RSS values in your pool. The ``max_tasks_per_child`` helps with
+  this because a subprocess is entirely erased when the max is
+  reached, but it does mean that periodically there will be a small
+  latency penalty from constructing the replacement subprocess. In
+  my opinion, ``max_tasks_per_child`` is appropriate for when you
+  know or suspect there's a real memory leak somewhere in your code
+  (or a 3rd-party package!), and the easiest way to deal with that
+  right now is just to periodically remove a process.
 
 Show me some code
 -----------------
 
 Simple case
 ^^^^^^^^^^^
 
@@ -237,14 +271,18 @@
 
     with deadpool.Deadpool() as exe:
         fut = exe.submit(f, deadpool_timeout=1.0)
 
         with pytest.raises(deadpool.TimeoutError)
             fut.result()
 
+The parameter ``deadpool_timeout`` is special and consumed by ``Deadpool``
+in the call. You can't use a parameter with this name in your function 
+kwargs.
+
 Handling OOM killed situations
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. code-block:: python
 
     import time
     import deadpool
@@ -257,17 +295,17 @@
 
         try:
             result = fut.result()
         except deadpool.ProcessError:
             print("Oh no someone killed my task!")
 
 
-As long as the OOM killer terminates the subprocess (and not the main process),
-which is likely because it'll be your subprocess that is using too much
-memory, this will not hurt the pool, and it will be able to receive and
+As long as the OOM killer terminates merely a subprocess (and not the main
+process), which is likely because it'll be your subprocess that is using too
+much memory, this will not hurt the pool, and it will be able to receive and
 process more tasks. Note that this event will show up as a ``ProcessError``
 exception when accessing the future, so you have a way of at least tracking
 these events.
 
 Design Details
 --------------
```

