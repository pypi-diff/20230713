# Comparing `tmp/opentelemetry_instrumentation_celery-0.39b0.tar.gz` & `tmp/opentelemetry_instrumentation_celery-0.40b0.tar.gz`

## Comparing `opentelemetry_instrumentation_celery-0.39b0.tar` & `opentelemetry_instrumentation_celery-0.40b0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     9372 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.39b0/src/opentelemetry/instrumentation/celery/__init__.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.39b0/src/opentelemetry/instrumentation/celery/package.py
--rw-r--r--   0        0        0     7421 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.39b0/src/opentelemetry/instrumentation/celery/utils.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.39b0/src/opentelemetry/instrumentation/celery/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.39b0/tests/__init__.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.39b0/tests/celery_test_tasks.py
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.39b0/tests/test_getter.py
--rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.39b0/tests/test_tasks.py
--rw-r--r--   0        0        0    10421 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.39b0/tests/test_utils.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.39b0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.39b0/LICENSE
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.39b0/README.rst
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.39b0/pyproject.toml
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.39b0/PKG-INFO
+-rw-r--r--   0        0        0    10879 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.40b0/src/opentelemetry/instrumentation/celery/__init__.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.40b0/src/opentelemetry/instrumentation/celery/package.py
+-rw-r--r--   0        0        0     7421 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.40b0/src/opentelemetry/instrumentation/celery/utils.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.40b0/src/opentelemetry/instrumentation/celery/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.40b0/tests/__init__.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.40b0/tests/celery_test_tasks.py
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.40b0/tests/test_getter.py
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.40b0/tests/test_metrics.py
+-rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.40b0/tests/test_tasks.py
+-rw-r--r--   0        0        0    10421 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.40b0/tests/test_utils.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.40b0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.40b0/LICENSE
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.40b0/README.rst
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.40b0/pyproject.toml
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 opentelemetry_instrumentation_celery-0.40b0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_celery-0.39b0/src/opentelemetry/instrumentation/celery/__init__.py` & `opentelemetry_instrumentation_celery-0.40b0/src/opentelemetry/instrumentation/celery/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,23 +56,25 @@
 accomplish this as shown in the example above.
 
 API
 ---
 """
 
 import logging
+from timeit import default_timer
 from typing import Collection, Iterable
 
 from celery import signals  # pylint: disable=no-name-in-module
 
 from opentelemetry import trace
 from opentelemetry.instrumentation.celery import utils
 from opentelemetry.instrumentation.celery.package import _instruments
 from opentelemetry.instrumentation.celery.version import __version__
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
+from opentelemetry.metrics import get_meter
 from opentelemetry.propagate import extract, inject
 from opentelemetry.propagators.textmap import Getter
 from opentelemetry.semconv.trace import SpanAttributes
 from opentelemetry.trace.status import Status, StatusCode
 
 logger = logging.getLogger(__name__)
 
@@ -100,23 +102,33 @@
         return []
 
 
 celery_getter = CeleryGetter()
 
 
 class CeleryInstrumentor(BaseInstrumentor):
+    def __init__(self):
+        super().__init__()
+        self.metrics = None
+        self.task_id_to_start_time = {}
+
     def instrumentation_dependencies(self) -> Collection[str]:
         return _instruments
 
     def _instrument(self, **kwargs):
         tracer_provider = kwargs.get("tracer_provider")
 
         # pylint: disable=attribute-defined-outside-init
         self._tracer = trace.get_tracer(__name__, __version__, tracer_provider)
 
+        meter_provider = kwargs.get("meter_provider")
+        meter = get_meter(__name__, __version__, meter_provider)
+
+        self.create_celery_metrics(meter)
+
         signals.task_prerun.connect(self._trace_prerun, weak=False)
         signals.task_postrun.connect(self._trace_postrun, weak=False)
         signals.before_task_publish.connect(
             self._trace_before_publish, weak=False
         )
         signals.after_task_publish.connect(
             self._trace_after_publish, weak=False
@@ -135,30 +147,30 @@
     def _trace_prerun(self, *args, **kwargs):
         task = utils.retrieve_task(kwargs)
         task_id = utils.retrieve_task_id(kwargs)
 
         if task is None or task_id is None:
             return
 
+        self.update_task_duration_time(task_id)
         request = task.request
         tracectx = extract(request, getter=celery_getter) or None
 
         logger.debug("prerun signal start task_id=%s", task_id)
 
         operation_name = f"{_TASK_RUN}/{task.name}"
         span = self._tracer.start_span(
             operation_name, context=tracectx, kind=trace.SpanKind.CONSUMER
         )
 
         activation = trace.use_span(span, end_on_exit=True)
         activation.__enter__()  # pylint: disable=E1101
         utils.attach_span(task, task_id, (span, activation))
 
-    @staticmethod
-    def _trace_postrun(*args, **kwargs):
+    def _trace_postrun(self, *args, **kwargs):
         task = utils.retrieve_task(kwargs)
         task_id = utils.retrieve_task_id(kwargs)
 
         if task is None or task_id is None:
             return
 
         logger.debug("postrun signal task_id=%s", task_id)
@@ -174,14 +186,17 @@
             span.set_attribute(_TASK_TAG_KEY, _TASK_RUN)
             utils.set_attributes_from_context(span, kwargs)
             utils.set_attributes_from_context(span, task.request)
             span.set_attribute(_TASK_NAME_KEY, task.name)
 
         activation.__exit__(None, None, None)
         utils.detach_span(task, task_id)
+        self.update_task_duration_time(task_id)
+        labels = {"task": task.name, "worker": task.request.hostname}
+        self._record_histograms(task_id, labels)
 
     def _trace_before_publish(self, *args, **kwargs):
         task = utils.retrieve_task_from_sender(kwargs)
         task_id = utils.retrieve_task_id_from_message(kwargs)
 
         if task_id is None:
             return
@@ -273,7 +288,34 @@
         if span is None or not span.is_recording():
             return
 
         # Add retry reason metadata to span
         # Use `str(reason)` instead of `reason.message` in case we get
         # something that isn't an `Exception`
         span.set_attribute(_TASK_RETRY_REASON_KEY, str(reason))
+
+    def update_task_duration_time(self, task_id):
+        cur_time = default_timer()
+        task_duration_time_until_now = (
+            cur_time - self.task_id_to_start_time[task_id]
+            if task_id in self.task_id_to_start_time
+            else cur_time
+        )
+        self.task_id_to_start_time[task_id] = task_duration_time_until_now
+
+    def _record_histograms(self, task_id, metric_attributes):
+        if task_id is None:
+            return
+
+        self.metrics["flower.task.runtime.seconds"].record(
+            self.task_id_to_start_time.get(task_id),
+            attributes=metric_attributes,
+        )
+
+    def create_celery_metrics(self, meter) -> None:
+        self.metrics = {
+            "flower.task.runtime.seconds": meter.create_histogram(
+                name="flower.task.runtime.seconds",
+                unit="seconds",
+                description="The time it took to run the task.",
+            )
+        }
```

### Comparing `opentelemetry_instrumentation_celery-0.39b0/src/opentelemetry/instrumentation/celery/package.py` & `opentelemetry_instrumentation_celery-0.40b0/src/opentelemetry/instrumentation/celery/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_celery-0.39b0/src/opentelemetry/instrumentation/celery/utils.py` & `opentelemetry_instrumentation_celery-0.40b0/src/opentelemetry/instrumentation/celery/utils.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_celery-0.39b0/src/opentelemetry/instrumentation/celery/version.py` & `opentelemetry_instrumentation_celery-0.40b0/src/opentelemetry/instrumentation/celery/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.39b0"
+__version__ = "0.40b0"
```

### Comparing `opentelemetry_instrumentation_celery-0.39b0/tests/celery_test_tasks.py` & `opentelemetry_instrumentation_celery-0.40b0/tests/celery_test_tasks.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_celery-0.39b0/tests/test_getter.py` & `opentelemetry_instrumentation_celery-0.40b0/tests/test_getter.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_celery-0.39b0/tests/test_tasks.py` & `opentelemetry_instrumentation_celery-0.40b0/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_celery-0.39b0/tests/test_utils.py` & `opentelemetry_instrumentation_celery-0.40b0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_celery-0.39b0/LICENSE` & `opentelemetry_instrumentation_celery-0.40b0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_celery-0.39b0/README.rst` & `opentelemetry_instrumentation_celery-0.40b0/README.rst`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_celery-0.39b0/pyproject.toml` & `opentelemetry_instrumentation_celery-0.40b0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -22,25 +22,25 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
   "opentelemetry-api ~= 1.12",
-  "opentelemetry-instrumentation == 0.39b0",
-  "opentelemetry-semantic-conventions == 0.39b0",
+  "opentelemetry-instrumentation == 0.40b0",
+  "opentelemetry-semantic-conventions == 0.40b0",
 ]
 
 [project.optional-dependencies]
 instruments = [
   "celery >= 4.0, < 6.0",
 ]
 test = [
   "opentelemetry-instrumentation-celery[instruments]",
-  "opentelemetry-test-utils == 0.39b0",
+  "opentelemetry-test-utils == 0.40b0",
   "pytest",
 ]
 
 [project.entry-points.opentelemetry_instrumentor]
 celery = "opentelemetry.instrumentation.celery:CeleryInstrumentor"
 
 [project.urls]
```

### Comparing `opentelemetry_instrumentation_celery-0.39b0/PKG-INFO` & `opentelemetry_instrumentation_celery-0.40b0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-celery
-Version: 0.39b0
+Version: 0.40b0
 Summary: OpenTelemetry Celery Instrumentation
 Project-URL: Homepage, https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-celery
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -14,21 +14,21 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Requires-Dist: opentelemetry-api~=1.12
-Requires-Dist: opentelemetry-instrumentation==0.39b0
-Requires-Dist: opentelemetry-semantic-conventions==0.39b0
+Requires-Dist: opentelemetry-instrumentation==0.40b0
+Requires-Dist: opentelemetry-semantic-conventions==0.40b0
 Provides-Extra: instruments
 Requires-Dist: celery<6.0,>=4.0; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: opentelemetry-instrumentation-celery[instruments]; extra == 'test'
-Requires-Dist: opentelemetry-test-utils==0.39b0; extra == 'test'
+Requires-Dist: opentelemetry-test-utils==0.40b0; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/x-rst
 
 OpenTelemetry Celery Instrumentation
 ====================================
 
 |pypi|
```

