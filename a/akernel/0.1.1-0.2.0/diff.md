# Comparing `tmp/akernel-0.1.1.tar.gz` & `tmp/akernel-0.2.0.tar.gz`

## Comparing `akernel-0.1.1.tar` & `akernel-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 akernel-0.1.1/MANIFEST.in
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 akernel-0.1.1/.github/workflows/main.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/__init__.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/akernel.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/cache.py
--rw-r--r--   0        0        0     9111 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/code.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/connect.py
--rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/execution.py
--rw-r--r--   0        0        0    17853 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/kernel.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/kernelspec.py
--rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/message.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/traceback.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/IPython/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/IPython/core/__init__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/IPython/core/getipython.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/IPython/core/interactiveshell.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/comm/__init__.py
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/comm/comm.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/comm/manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/display/__init__.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/display/display.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/tests/conftest.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/tests/test_async_code.py
--rw-r--r--   0        0        0     5885 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/tests/test_execution.py
--rw-r--r--   0        0        0     6748 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/tests/test_kernel.py
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 akernel-0.1.1/akernel/tests/test_react_code.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 akernel-0.1.1/binder/environment.yml
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 akernel-0.1.1/binder/postBuild
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 akernel-0.1.1/examples/reactivity.ipynb
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 akernel-0.1.1/share/jupyter/kernels/akernel/kernel.json
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 akernel-0.1.1/LICENSE
--rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 akernel-0.1.1/README.md
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 akernel-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6047 2020-02-02 00:00:00.000000 akernel-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 akernel-0.2.0/MANIFEST.in
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 akernel-0.2.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 akernel-0.2.0/akernel/__init__.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 akernel-0.2.0/akernel/akernel.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 akernel-0.2.0/akernel/cache.py
+-rw-r--r--   0        0        0     9111 2020-02-02 00:00:00.000000 akernel-0.2.0/akernel/code.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 akernel-0.2.0/akernel/connect.py
+-rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 akernel-0.2.0/akernel/execution.py
+-rw-r--r--   0        0        0    18491 2020-02-02 00:00:00.000000 akernel-0.2.0/akernel/kernel.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 akernel-0.2.0/akernel/kernelspec.py
+-rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 akernel-0.2.0/akernel/message.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 akernel-0.2.0/akernel/traceback.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 akernel-0.2.0/akernel/IPython/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akernel-0.2.0/akernel/IPython/core/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 akernel-0.2.0/akernel/IPython/core/getipython.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 akernel-0.2.0/akernel/IPython/core/interactiveshell.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 akernel-0.2.0/akernel/comm/__init__.py
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 akernel-0.2.0/akernel/comm/comm.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 akernel-0.2.0/akernel/comm/manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 akernel-0.2.0/akernel/display/__init__.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 akernel-0.2.0/akernel/display/display.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 akernel-0.2.0/akernel/tests/conftest.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 akernel-0.2.0/akernel/tests/test_async_code.py
+-rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 akernel-0.2.0/akernel/tests/test_execution.py
+-rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 akernel-0.2.0/akernel/tests/test_kernel.py
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 akernel-0.2.0/akernel/tests/test_react_code.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 akernel-0.2.0/binder/environment.yml
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 akernel-0.2.0/binder/postBuild
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 akernel-0.2.0/examples/reactivity.ipynb
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 akernel-0.2.0/share/jupyter/kernels/akernel/kernel.json
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 akernel-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5519 2020-02-02 00:00:00.000000 akernel-0.2.0/README.md
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 akernel-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6999 2020-02-02 00:00:00.000000 akernel-0.2.0/PKG-INFO
```

### Comparing `akernel-0.1.1/.github/workflows/main.yml` & `akernel-0.2.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `akernel-0.1.1/akernel/akernel.py` & `akernel-0.2.0/akernel/akernel.py`

 * *Files identical despite different names*

### Comparing `akernel-0.1.1/akernel/code.py` & `akernel-0.2.0/akernel/code.py`

 * *Files identical despite different names*

### Comparing `akernel-0.1.1/akernel/connect.py` & `akernel-0.2.0/akernel/connect.py`

 * *Files identical despite different names*

### Comparing `akernel-0.1.1/akernel/execution.py` & `akernel-0.2.0/akernel/execution.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,28 +128,31 @@
 
 
 # used in tests (mimic execute_and_finish, finish_execution)
 async def execute(
     code: str,
     globals_: Dict[str, Any],
     locals_: Dict[str, Any],
+    chain: bool = False,
     react: bool = False,
     cache: Optional[Dict[str, Any]] = None,
 ) -> Tuple[Any, List[str], bool]:
     result = None
     interrupted = False
     traceback, exception, cache_info = pre_execute(
         code, globals_, locals_, react=react, cache=cache
     )
     if traceback:
         return result, traceback, interrupted
 
     if cache_info["cached"]:
         result = cache_info["result"]
     else:
+        if chain:
+            await locals_["__task__"]()
         try:
             result = await locals_["__async_cell__"]()
         except KeyboardInterrupt:
             interrupted = True
         except Exception as e:
             traceback = get_traceback(code, e)
         else:
```

### Comparing `akernel-0.1.1/akernel/kernel.py` & `akernel-0.2.0/akernel/kernel.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import asyncio
 import json
 from io import StringIO
 from contextvars import ContextVar
 from typing import Dict, Any, List, Optional, Union, Awaitable, cast
 
 from zmq.asyncio import Socket
-
 import comm  # type: ignore
 from akernel.comm.manager import CommManager
 from akernel.display import display
 import akernel.IPython
 from akernel.IPython import core
 from .connect import connect_channel
 from .message import receive_message, send_message, create_message, check_message
@@ -67,20 +66,22 @@
         def get_comm_manager():
             return self.comm_manager
 
         comm.get_comm_manager = get_comm_manager
         self.loop = asyncio.get_event_loop()
         self.kernel_mode = kernel_mode
         self.cache_dir = cache_dir
+        self._concurrent_kernel = None
         self._multi_kernel = None
         self._cache_kernel = None
         self._react_kernel = None
         self.kernel_initialized = []
         self.globals = {}
         self.locals = {}
+        self._chain_execution = not self.concurrent_kernel
         self.running_cells = {}
         self.task_i = 0
         self.execution_count = 1
         self.execution_state = "starting"
         with open(connection_file) as f:
             self.connection_cfg = json.load(f)
         self.key = cast(str, self.connection_cfg["key"])
@@ -111,14 +112,26 @@
             else:
                 if not self.restart:
                     break
             finally:
                 self.shell_task.cancel()
                 self.control_task.cancel()
 
+    def chain_execution(self) -> None:
+        self._chain_execution = True
+
+    def unchain_execution(self) -> None:
+        self._chain_execution = False
+
+    @property
+    def concurrent_kernel(self):
+        if self._concurrent_kernel is None:
+            self._concurrent_kernel = "concurrent" in self.kernel_mode
+        return self._concurrent_kernel
+
     @property
     def multi_kernel(self):
         if self._multi_kernel is None:
             self._multi_kernel = "multi" in self.kernel_mode
         return self._multi_kernel
 
     @property
@@ -138,14 +151,16 @@
             return
 
         self.globals[namespace] = {
             "ainput": self.ainput,
             "asyncio": asyncio,
             "print": self.print,
             "__task__": self.task,
+            "__chain_execution__": self.chain_execution,
+            "__unchain_execution__": self.unchain_execution,
             "_": None,
         }
         self.locals[namespace] = {}
         if self.react_kernel:
             code = (
                 "import ipyx, ipywidgets;"
                 "globals().update({'ipyx': ipyx, 'ipywidgets': ipywidgets})"
@@ -334,14 +349,16 @@
         idents: List[bytes],
         parent: Dict[str, Any],
         task_i: int,
         execution_count: int,
         code: str,
         cache_info: Dict[str, Any],
     ) -> None:
+        if self._chain_execution:
+            await self.task()
         PARENT_VAR.set(parent)
         IDENTS_VAR.set(idents)
         parent_header = parent["header"]
         traceback, exception = [], None
         namespace = self.get_namespace(parent_header)
         try:
             result = await self.locals[namespace]["__async_cell__"]()
```

### Comparing `akernel-0.1.1/akernel/kernelspec.py` & `akernel-0.2.0/akernel/kernelspec.py`

 * *Files identical despite different names*

### Comparing `akernel-0.1.1/akernel/message.py` & `akernel-0.2.0/akernel/message.py`

 * *Files identical despite different names*

### Comparing `akernel-0.1.1/akernel/traceback.py` & `akernel-0.2.0/akernel/traceback.py`

 * *Files identical despite different names*

### Comparing `akernel-0.1.1/akernel/comm/comm.py` & `akernel-0.2.0/akernel/comm/comm.py`

 * *Files identical despite different names*

### Comparing `akernel-0.1.1/akernel/tests/conftest.py` & `akernel-0.2.0/akernel/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `akernel-0.1.1/akernel/tests/test_async_code.py` & `akernel-0.2.0/akernel/tests/test_async_code.py`

 * *Files identical despite different names*

### Comparing `akernel-0.1.1/akernel/tests/test_execution.py` & `akernel-0.2.0/akernel/tests/test_execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,22 +9,23 @@
 
 from akernel.execution import execute
 
 
 async def run(
     code: str,
     globals_: Optional[Dict[str, Any]] = None,
+    chain: bool = False,
     react: bool = False,
     cache: Optional[Dict[str, Any]] = None,
 ) -> Tuple[Any, List[str], bool, Dict[str, Any], Dict[str, Any]]:
     if globals_ is None:
         globals_ = {}
     locals_: Dict[str, Any] = {}
     result, traceback, interrupted = await execute(
-        code, globals_, locals_, react=react, cache=cache
+        code, globals_, locals_, chain=chain, react=react, cache=cache
     )
     if "__builtins__" in globals_:
         del globals_["__builtins__"]
     return result, traceback, interrupted, globals_, locals_
 
 
 def tb_str(traceback: List[str]) -> str:
```

### Comparing `akernel-0.1.1/akernel/tests/test_kernel.py` & `akernel-0.2.0/akernel/tests/test_kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,17 @@
 
 
 @pytest.mark.asyncio
 async def test_concurrent_cells(capfd, all_modes):
     kd = KernelDriver(kernelspec_path=KERNELSPEC_PATH, log=False)
     await kd.start(startup_timeout=TIMEOUT)
     asyncio.create_task(
+        kd.execute("__unchain_execution__()", timeout=TIMEOUT)
+    )
+    asyncio.create_task(
         kd.execute("await asyncio.sleep(0.2)\nprint('done1')", timeout=TIMEOUT)
     )
     asyncio.create_task(
         kd.execute("await asyncio.sleep(0.1)\nprint('done2')", timeout=TIMEOUT)
     )
     await asyncio.sleep(0.5)
     await kd.stop()
@@ -134,14 +137,17 @@
     assert out == "done1\ndone2\n"
 
 
 @pytest.mark.asyncio
 async def test_interrupt_async(capfd, all_modes):
     kd = KernelDriver(kernelspec_path=KERNELSPEC_PATH, log=False)
     await kd.start(startup_timeout=TIMEOUT)
+    asyncio.create_task(
+        kd.execute("__unchain_execution__()", timeout=TIMEOUT)
+    )
     expected = []
     n0, n1 = 2, 3
     for i0 in range(n0):
         for i1 in range(n1):
             asyncio.create_task(
                 kd.execute(
                     f"print('{i0} {i1} before')\nawait asyncio.sleep(1)\nprint('{i0} {i1} after')",
```

### Comparing `akernel-0.1.1/akernel/tests/test_react_code.py` & `akernel-0.2.0/akernel/tests/test_react_code.py`

 * *Files identical despite different names*

### Comparing `akernel-0.1.1/examples/reactivity.ipynb` & `akernel-0.2.0/examples/reactivity.ipynb`

 * *Files identical despite different names*

### Comparing `akernel-0.1.1/LICENSE` & `akernel-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `akernel-0.1.1/README.md` & `akernel-0.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [![Build Status](https://github.com/davidbrochart/akernel/workflows/CI/badge.svg)](https://github.com/davidbrochart/akernel/actions)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/davidbrochart/akernel/HEAD?urlpath=lab%2Ftree%2Fexamples%2Freactivity.ipynb)
 
 # akernel
 
-An asynchronous Python Jupyter kernel, with different flavors:
+A Python Jupyter kernel, with different flavors:
+- concurrent cell execution,
 - reactive programming,
 - cell execution caching,
 - multi-kernel emulation.
 
 ## Install
 
 ```bash
@@ -16,36 +17,52 @@
 # pip install akernel[react]  # if you want to be able to use reactive programming
 # pip install akernel[cache]  # if you want to be able to use cell execution caching
 ```
 
 You can parameterize akernel's execution mode:
 
 ```bash
-akernel install  # default (async)
+akernel install  # default (chained cell execution mode)
+akernel install concurrent  # concurrent cell execution mode
 akernel install react  # reactive programming mode
 akernel install cache  # cell execution caching  mode
 akernel install multi  # multi-kernel emulation mode
-akernel install cache-multi-react  # you can combine several modes
+akernel install cache-multi-react-concurrent  # you can combine several modes
 ```
 
 ## Motivation
 
 [ipykernel](https://github.com/ipython/ipykernel) offers the ability to
 [run asynchronous code from the REPL](https://ipython.readthedocs.io/en/stable/interactive/autoawait.html).
 This means you can `await` at the top-level, outside of an async function. Unfortunately, this will still
 block the kernel.
 
-akernel changes this behavior by launching each cell in a task.
+akernel changes this behavior by launching each cell in a task. By default, cell tasks are chained, which
+means that a cell will start executing after the previous one is done. You might wonder, is it not the same
+as ipykernel then? Well, not quite. In ipykernel, when an async cell is executing, it also blocks the
+processing of
+[Comm messages](https://jupyter-client.readthedocs.io/en/stable/messaging.html#custom-messages), which
+prevents the kernel from interacting with e.g. JupyterLab widgets (see
+[here](https://github.com/ipython/ipykernel/issues/646) and
+[there](https://github.com/ipython/ipykernel/issues/696)). In akernel, it will not be the case.
 
-akernel now also supports reactive programming, although it is still experimental!
+If you want to go all the way and have cells execute concurrently, you can also do so (see below).
 
 ## Features
 
 ### Asynchronous execution
 
+First, set the concurrent execution mode in order to have async cells execute concurrently
+(you could also do that at install-time with `akernel install concurrent`):
+
+```python
+__unchain_execution__()
+# __chain_execution__()
+```
+
 akernel allows for asynchronous code execution. What this means is that when used in a Jupyter
 notebook, you can run cells concurrently if the code is cooperative. For instance, you can run a
 cell with the following code:
 
 ```python
 # cell 1
 for i in range(10):
```

### Comparing `akernel-0.1.1/pyproject.toml` & `akernel-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `akernel-0.1.1/PKG-INFO` & `akernel-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akernel
-Version: 0.1.1
+Version: 0.2.0
 Summary: An asynchronous Python Jupyter kernel
 Project-URL: Homepage, https://github.com/davidbrochart/akernel
 Author-email: David Brochart <david.brochart@gmail.com>
 License: MIT
 License-File: LICENSE
 Keywords: jupyter
 Classifier: Development Status :: 4 - Beta
@@ -41,15 +41,16 @@
 
 [![Build Status](https://github.com/davidbrochart/akernel/workflows/CI/badge.svg)](https://github.com/davidbrochart/akernel/actions)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/davidbrochart/akernel/HEAD?urlpath=lab%2Ftree%2Fexamples%2Freactivity.ipynb)
 
 # akernel
 
-An asynchronous Python Jupyter kernel, with different flavors:
+A Python Jupyter kernel, with different flavors:
+- concurrent cell execution,
 - reactive programming,
 - cell execution caching,
 - multi-kernel emulation.
 
 ## Install
 
 ```bash
@@ -57,36 +58,52 @@
 # pip install akernel[react]  # if you want to be able to use reactive programming
 # pip install akernel[cache]  # if you want to be able to use cell execution caching
 ```
 
 You can parameterize akernel's execution mode:
 
 ```bash
-akernel install  # default (async)
+akernel install  # default (chained cell execution mode)
+akernel install concurrent  # concurrent cell execution mode
 akernel install react  # reactive programming mode
 akernel install cache  # cell execution caching  mode
 akernel install multi  # multi-kernel emulation mode
-akernel install cache-multi-react  # you can combine several modes
+akernel install cache-multi-react-concurrent  # you can combine several modes
 ```
 
 ## Motivation
 
 [ipykernel](https://github.com/ipython/ipykernel) offers the ability to
 [run asynchronous code from the REPL](https://ipython.readthedocs.io/en/stable/interactive/autoawait.html).
 This means you can `await` at the top-level, outside of an async function. Unfortunately, this will still
 block the kernel.
 
-akernel changes this behavior by launching each cell in a task.
+akernel changes this behavior by launching each cell in a task. By default, cell tasks are chained, which
+means that a cell will start executing after the previous one is done. You might wonder, is it not the same
+as ipykernel then? Well, not quite. In ipykernel, when an async cell is executing, it also blocks the
+processing of
+[Comm messages](https://jupyter-client.readthedocs.io/en/stable/messaging.html#custom-messages), which
+prevents the kernel from interacting with e.g. JupyterLab widgets (see
+[here](https://github.com/ipython/ipykernel/issues/646) and
+[there](https://github.com/ipython/ipykernel/issues/696)). In akernel, it will not be the case.
 
-akernel now also supports reactive programming, although it is still experimental!
+If you want to go all the way and have cells execute concurrently, you can also do so (see below).
 
 ## Features
 
 ### Asynchronous execution
 
+First, set the concurrent execution mode in order to have async cells execute concurrently
+(you could also do that at install-time with `akernel install concurrent`):
+
+```python
+__unchain_execution__()
+# __chain_execution__()
+```
+
 akernel allows for asynchronous code execution. What this means is that when used in a Jupyter
 notebook, you can run cells concurrently if the code is cooperative. For instance, you can run a
 cell with the following code:
 
 ```python
 # cell 1
 for i in range(10):
```

