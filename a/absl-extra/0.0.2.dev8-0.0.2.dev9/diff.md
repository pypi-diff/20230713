# Comparing `tmp/absl_extra-0.0.2.dev8.tar.gz` & `tmp/absl_extra-0.0.2.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "absl_extra-0.0.2.dev8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "absl_extra-0.0.2.dev9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `absl_extra-0.0.2.dev8.tar` & `absl_extra-0.0.2.dev9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1588 2023-07-02 12:04:55.830758 absl_extra-0.0.2.dev8/Readme.md
--rw-r--r--   0        0        0      682 2023-07-02 12:04:55.830758 absl_extra-0.0.2.dev8/absl_extra/__init__.py
--rw-r--r--   0        0        0       64 2023-07-02 12:04:55.830758 absl_extra-0.0.2.dev8/absl_extra/py.typed
--rw-r--r--   0        0        0        0 2023-07-02 12:04:55.830758 absl_extra-0.0.2.dev8/absl_extra/src/__init__.py
--rw-r--r--   0        0        0     1202 2023-07-02 12:04:55.830758 absl_extra-0.0.2.dev8/absl_extra/src/jax_utils.py
--rw-r--r--   0        0        0     2296 2023-07-02 12:04:55.830758 absl_extra-0.0.2.dev8/absl_extra/src/logging_utils.py
--rw-r--r--   0        0        0     2487 2023-07-02 12:04:55.830758 absl_extra-0.0.2.dev8/absl_extra/src/notifier.py
--rw-r--r--   0        0        0     4281 2023-07-02 12:04:55.830758 absl_extra-0.0.2.dev8/absl_extra/src/tasks.py
--rw-r--r--   0        0        0     4456 2023-07-02 12:04:55.830758 absl_extra-0.0.2.dev8/absl_extra/src/tf_utils.py
--rw-r--r--   0        0        0      914 2023-07-02 12:04:55.830758 absl_extra-0.0.2.dev8/pyproject.toml
--rw-r--r--   0        0        0     2693 1970-01-01 00:00:00.000000 absl_extra-0.0.2.dev8/PKG-INFO
+-rw-r--r--   0        0        0     1588 2023-07-02 12:24:04.092328 absl_extra-0.0.2.dev9/Readme.md
+-rw-r--r--   0        0        0      713 2023-07-02 12:24:04.092328 absl_extra-0.0.2.dev9/absl_extra/__init__.py
+-rw-r--r--   0        0        0       64 2023-07-02 12:24:04.092328 absl_extra-0.0.2.dev9/absl_extra/py.typed
+-rw-r--r--   0        0        0        0 2023-07-02 12:24:04.092328 absl_extra-0.0.2.dev9/absl_extra/src/__init__.py
+-rw-r--r--   0        0        0     1202 2023-07-02 12:24:04.092328 absl_extra-0.0.2.dev9/absl_extra/src/jax_utils.py
+-rw-r--r--   0        0        0     2297 2023-07-02 12:24:04.092328 absl_extra-0.0.2.dev9/absl_extra/src/logging_utils.py
+-rw-r--r--   0        0        0     3273 2023-07-02 12:24:04.092328 absl_extra-0.0.2.dev9/absl_extra/src/notifier.py
+-rw-r--r--   0        0        0     4299 2023-07-02 12:24:04.092328 absl_extra-0.0.2.dev9/absl_extra/src/tasks.py
+-rw-r--r--   0        0        0     4432 2023-07-02 12:24:04.092328 absl_extra-0.0.2.dev9/absl_extra/src/tf_utils.py
+-rw-r--r--   0        0        0      914 2023-07-02 12:24:04.092328 absl_extra-0.0.2.dev9/pyproject.toml
+-rw-r--r--   0        0        0     2693 1970-01-01 00:00:00.000000 absl_extra-0.0.2.dev9/PKG-INFO
```

### Comparing `absl_extra-0.0.2.dev8/Readme.md` & `absl_extra-0.0.2.dev9/Readme.md`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.2.dev8/absl_extra/__init__.py` & `absl_extra-0.0.2.dev9/absl_extra/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 def is_lib_installed(name: str) -> bool:
     return util.find_spec(name) is not None
 
 
 from absl_extra.src.tasks import run, register_task
-from absl_extra.src.notifier import BaseNotifier
+from absl_extra.src.notifier import BaseNotifier, NoOpNotifier, LoggingNotifier
 
 if is_lib_installed("slack_sdk"):
     from absl_extra.src.notifier import SlackNotifier
 from absl_extra.src.logging_utils import (
     log_before,
     log_after,
     setup_logging,
```

### Comparing `absl_extra-0.0.2.dev8/absl_extra/src/jax_utils.py` & `absl_extra-0.0.2.dev9/absl_extra/src/jax_utils.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import functools
 import logging
-from typing import Callable, TypeVar
 import platform
+from typing import Callable, TypeVar
 
 import jax
 
 R = TypeVar("R")
 
 
 def requires_gpu(
```

### Comparing `absl_extra-0.0.2.dev8/absl_extra/src/logging_utils.py` & `absl_extra-0.0.2.dev9/absl_extra/src/logging_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import functools
 import inspect
 from importlib import util
-from typing import Callable, TypeVar, Literal
+from typing import Callable, Literal, TypeVar
 
 from absl import logging
 
 C = TypeVar("C", bound=Callable)
 
 
 def log_exception(func: C, logger: Callable[[str], None] = logging.error) -> C:
@@ -61,14 +61,15 @@
 
 def setup_logging(
     *,
     log_format: str = "%(asctime)s:[%(filename)s:%(lineno)s->%(funcName)s()]:%(levelname)s: %(message)s",
     log_level: Literal["CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG"] = "DEBUG",
 ):
     import logging
+
     import absl.logging
 
     logging.basicConfig(
         level=logging.getLevelName(log_level),
         format=log_format,
     )
```

### Comparing `absl_extra-0.0.2.dev8/absl_extra/src/notifier.py` & `absl_extra-0.0.2.dev9/absl_extra/src/notifier.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,45 @@
 from __future__ import annotations
-from absl import logging
+
+from abc import ABC, abstractmethod
 from importlib import util
+from typing import Callable
+
+from absl import logging
+
+
+class BaseNotifier(ABC):
+    @abstractmethod
+    def notify_job_started(self, name: str):
+        raise NotImplementedError
+
+    @abstractmethod
+    def notify_job_finished(self, name: str):
+        raise NotImplementedError
+
+    @abstractmethod
+    def notify_job_failed(self, name: str, exception: Exception):
+        raise NotImplementedError
+
+
+class NoOpNotifier(BaseNotifier):
+    def notify_job_started(self, name: str):
+        pass
+
+    def notify_job_finished(self, name: str):
+        pass
+
+    def notify_job_failed(self, name: str, exception: Exception):
+        raise NotImplementedError
+
 
+class LoggingNotifier(BaseNotifier):
+    def __init__(self, logger: Callable[[str], None] = logging.info):
+        self.logger = logger
 
-class BaseNotifier:
     def notify_job_started(self, name: str):
         logging.info(f"Job {name} started.")
 
     def notify_job_finished(self, name: str):
         logging.info(f"Job {name} finished.")
 
     def notify_job_failed(self, name: str, exception: Exception):
```

### Comparing `absl_extra-0.0.2.dev8/absl_extra/src/tasks.py` & `absl_extra-0.0.2.dev9/absl_extra/src/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 import json
 from functools import wraps
 from importlib import util
-from typing import Callable, NamedTuple, TypeVar, Mapping, List
+from typing import Callable, List, Mapping, NamedTuple, TypeVar
 
 from absl import app, flags, logging
 
-from absl_extra.src.notifier import BaseNotifier
+from absl_extra.src.notifier import BaseNotifier, LoggingNotifier
 
 T = TypeVar("T", bound=Callable, covariant=True)
 FLAGS = flags.FLAGS
 
 if util.find_spec("pymongo"):
     from pymongo import MongoClient
     from pymongo.collection import Collection
@@ -135,15 +135,15 @@
     Returns
     -------
 
     """
     if isinstance(notifier, Callable):
         notifier = notifier()
     if notifier is None:
-        notifier = BaseNotifier()
+        notifier = LoggingNotifier
 
     if util.find_spec("pymongo") and mongo_config is not None:
         if isinstance(mongo_config, Mapping):
             mongo_config = MongoConfig(**mongo_config)
         db = (
             MongoClient(mongo_config.uri)
             .get_database(mongo_config.db_name)
```

### Comparing `absl_extra-0.0.2.dev8/absl_extra/src/tf_utils.py` & `absl_extra-0.0.2.dev9/absl_extra/src/tf_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 from __future__ import annotations
+
 import functools
 import logging
-from typing import (
-    Callable,
-    TypeVar,
-    Protocol,
-    ContextManager,
-    Type,
-)
-from contextlib import contextmanager
-import tensorflow as tf
 import platform
+from contextlib import contextmanager
+from typing import Callable, ContextManager, Protocol, Type, TypeVar
 
+import tensorflow as tf
 
 C = TypeVar("C", bound=Callable)
 
 
 def requires_gpu(func: C, linux_only: bool = False) -> C:
     """
     Fail if function is executing on host without access to GPU(s).
```

### Comparing `absl_extra-0.0.2.dev8/pyproject.toml` & `absl_extra-0.0.2.dev9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "absl_extra"
-version = "0.0.2dev8"
+version = "0.0.2dev9"
 description = "A wrapper to run and monitor absl app."
 readme = "Readme.md"
 requires-python = ">=3.8"
 authors = [
     { name = "Artem Sereda", email = "artem.sereda.tub@gmail.com" }
 ]
 maintainers = [
```

### Comparing `absl_extra-0.0.2.dev8/PKG-INFO` & `absl_extra-0.0.2.dev9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absl_extra
-Version: 0.0.2.dev8
+Version: 0.0.2.dev9
 Summary: A wrapper to run and monitor absl app.
 Author-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Maintainer-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Requires-Dist: absl_py
```

