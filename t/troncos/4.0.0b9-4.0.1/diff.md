# Comparing `tmp/troncos-4.0.0b9.tar.gz` & `tmp/troncos-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "troncos-4.0.0b9.tar", max compression
+gzip compressed data, was "troncos-4.0.1.tar", max compression
```

## Comparing `troncos-4.0.0b9.tar` & `troncos-4.0.1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0     1077 2023-06-02 06:54:10.106833 troncos-4.0.0b9/LICENSE
--rw-r--r--   0        0        0     7753 2023-06-02 06:54:10.106833 troncos-4.0.0b9/README.md
--rw-r--r--   0        0        0     2389 2023-06-02 06:54:10.106833 troncos-4.0.0b9/pyproject.toml
--rw-r--r--   0        0        0      291 2023-06-02 06:54:10.106833 troncos-4.0.0b9/troncos/__init__.py
--rw-r--r--   0        0        0        0 2023-06-02 06:54:10.106833 troncos-4.0.0b9/troncos/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-06-02 06:54:10.106833 troncos-4.0.0b9/troncos/contrib/asgi/__init__.py
--rw-r--r--   0        0        0        0 2023-06-02 06:54:10.106833 troncos-4.0.0b9/troncos/contrib/asgi/logging/__init__.py
--rw-r--r--   0        0        0     5297 2023-06-02 06:54:10.106833 troncos-4.0.0b9/troncos/contrib/asgi/logging/middleware.py
--rw-r--r--   0        0        0        0 2023-06-02 06:54:10.106833 troncos-4.0.0b9/troncos/contrib/asgi/profiling/__init__.py
--rw-r--r--   0        0        0      576 2023-06-02 06:54:10.106833 troncos-4.0.0b9/troncos/contrib/asgi/profiling/app.py
--rw-r--r--   0        0        0        0 2023-06-02 06:54:10.106833 troncos-4.0.0b9/troncos/contrib/celery/__init__.py
--rw-r--r--   0        0        0        0 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/contrib/celery/logging/__init__.py
--rw-r--r--   0        0        0      969 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/contrib/celery/logging/signals.py
--rw-r--r--   0        0        0        0 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/contrib/django/__init__.py
--rw-r--r--   0        0        0        0 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/contrib/django/logging/__init__.py
--rw-r--r--   0        0        0     2354 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/contrib/django/logging/middleware.py
--rw-r--r--   0        0        0        0 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/contrib/django/profiling/__init__.py
--rw-r--r--   0        0        0      259 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/contrib/django/profiling/views.py
--rw-r--r--   0        0        0        0 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/contrib/logging/__init__.py
--rw-r--r--   0        0        0     3455 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/contrib/logging/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/contrib/starlette/__init__.py
--rw-r--r--   0        0        0        0 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/contrib/starlette/profiling/__init__.py
--rw-r--r--   0        0        0      291 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/contrib/starlette/profiling/views.py
--rw-r--r--   0        0        0     4148 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/contrib/structlog/__init__.py
--rw-r--r--   0        0        0      906 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/contrib/structlog/processors.py
--rw-r--r--   0        0        0        0 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/profiling/__init__.py
--rw-r--r--   0        0        0      192 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/profiling/auto.py
--rw-r--r--   0        0        0        0 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/profiling/bootstrap/__init__.py
--rw-r--r--   0        0        0      439 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/profiling/bootstrap/profile.py
--rw-r--r--   0        0        0      343 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/profiling/bootstrap/start.py
--rw-r--r--   0        0        0     1814 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/profiling/profiler.py
--rw-r--r--   0        0        0        0 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/py.typed
--rw-r--r--   0        0        0      690 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/tracing/__init__.py
--rw-r--r--   0        0        0       82 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/tracing/_enums.py
--rw-r--r--   0        0        0     2053 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/tracing/_otel.py
--rw-r--r--   0        0        0     4545 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/tracing/_span.py
--rw-r--r--   0        0        0     1884 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/tracing/_writer.py
--rw-r--r--   0        0        0     7585 2023-06-02 06:54:10.110833 troncos-4.0.0b9/troncos/tracing/decorators.py
--rw-r--r--   0        0        0     8744 1970-01-01 00:00:00.000000 troncos-4.0.0b9/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-13 09:38:03.586661 troncos-4.0.1/LICENSE
+-rw-r--r--   0        0        0     8203 2023-07-13 09:38:03.586661 troncos-4.0.1/README.md
+-rw-r--r--   0        0        0     2459 2023-07-13 09:38:03.586661 troncos-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0      291 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/asgi/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/asgi/logging/__init__.py
+-rw-r--r--   0        0        0     5297 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/asgi/logging/middleware.py
+-rw-r--r--   0        0        0        0 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/asgi/profiling/__init__.py
+-rw-r--r--   0        0        0      576 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/asgi/profiling/app.py
+-rw-r--r--   0        0        0        0 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/celery/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/celery/logging/__init__.py
+-rw-r--r--   0        0        0      969 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/celery/logging/signals.py
+-rw-r--r--   0        0        0        0 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/django/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/django/logging/__init__.py
+-rw-r--r--   0        0        0     2354 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/django/logging/middleware.py
+-rw-r--r--   0        0        0        0 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/django/profiling/__init__.py
+-rw-r--r--   0        0        0      259 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/django/profiling/views.py
+-rw-r--r--   0        0        0        0 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/logging/__init__.py
+-rw-r--r--   0        0        0     3455 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/logging/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/starlette/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/starlette/profiling/__init__.py
+-rw-r--r--   0        0        0      291 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/starlette/profiling/views.py
+-rw-r--r--   0        0        0     4300 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/structlog/__init__.py
+-rw-r--r--   0        0        0      906 2023-07-13 09:38:03.590661 troncos-4.0.1/troncos/contrib/structlog/processors.py
+-rw-r--r--   0        0        0       82 2023-07-13 09:38:03.598661 troncos-4.0.1/troncos/profiling/__init__.py
+-rw-r--r--   0        0        0      192 2023-07-13 09:38:03.598661 troncos-4.0.1/troncos/profiling/auto.py
+-rw-r--r--   0        0        0        0 2023-07-13 09:38:03.598661 troncos-4.0.1/troncos/profiling/bootstrap/__init__.py
+-rw-r--r--   0        0        0      439 2023-07-13 09:38:03.598661 troncos-4.0.1/troncos/profiling/bootstrap/profile.py
+-rw-r--r--   0        0        0      343 2023-07-13 09:38:03.598661 troncos-4.0.1/troncos/profiling/bootstrap/start.py
+-rw-r--r--   0        0        0     1814 2023-07-13 09:38:03.598661 troncos-4.0.1/troncos/profiling/profiler.py
+-rw-r--r--   0        0        0     1155 2023-07-13 09:38:03.598661 troncos-4.0.1/troncos/profiling/pyroscope.py
+-rw-r--r--   0        0        0        0 2023-07-13 09:38:03.598661 troncos-4.0.1/troncos/py.typed
+-rw-r--r--   0        0        0      690 2023-07-13 09:38:03.598661 troncos-4.0.1/troncos/tracing/__init__.py
+-rw-r--r--   0        0        0       82 2023-07-13 09:38:03.598661 troncos-4.0.1/troncos/tracing/_enums.py
+-rw-r--r--   0        0        0     2053 2023-07-13 09:38:03.598661 troncos-4.0.1/troncos/tracing/_otel.py
+-rw-r--r--   0        0        0     4582 2023-07-13 09:38:03.598661 troncos-4.0.1/troncos/tracing/_span.py
+-rw-r--r--   0        0        0     2675 2023-07-13 09:38:03.598661 troncos-4.0.1/troncos/tracing/_writer.py
+-rw-r--r--   0        0        0     7585 2023-07-13 09:38:03.598661 troncos-4.0.1/troncos/tracing/decorators.py
+-rw-r--r--   0        0        0     9237 1970-01-01 00:00:00.000000 troncos-4.0.1/PKG-INFO
```

### Comparing `troncos-4.0.0b9/LICENSE` & `troncos-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b9/README.md` & `troncos-4.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -86,17 +86,17 @@
 
 Add the following environment variables to your application.
 
 ```
 DD_ENV="{{ environment }}"
 DD_SERVICE="{{ app }}"
 DD_VERSION="{{ version }}"
-# b3 is usually used to propagate distributed traces across services.
-DD_TRACE_PROPAGATION_STYLE_EXTRACT="b3"
-DD_TRACE_PROPAGATION_STYLE_INJECT="b3"
+# tracecontext/w3c is usually used to propagate distributed traces across services.
+DD_TRACE_PROPAGATION_STYLE_EXTRACT="tracecontext"
+DD_TRACE_PROPAGATION_STYLE_INJECT="tracecontext"
 ```
 
 ### Using the GRPC span exporter
 
 Using the GRPC span exporter gives you significant performance gains.
 If you are running a critical service with high load in production,
 we recommend using GRPC.
@@ -193,57 +193,69 @@
 )
 
 connect_troncos_logging_celery_signals()
 ```
 
 ## Profiling
 
-### Enabling the profiler
+### Enabling the continuous py-spy profiler
+
+Start the profiler by running the `start_py_spy_profiler` method early in your application. This is
+typically done in `settings.py` of you want to profile a Django application, or in `__init__.py`
+in the root project package.
+
+```python
+from troncos.profiling import start_py_spy_profiler
+
+start_py_spy_profiler(server_address="http://127.0.0.1:4100")
+```
+
+### Enabling the ddtrace profiler
 
 Start the profiler by importing the profiler module early in your application. This is
 typically done in `settings.py` of you want to profile a Django application, or in `__init__.py`
 in the root project package.
 
 ```python
 import troncos.profiling.auto
 ```
 
-### Setup profile endpoint
+#### Setup profile endpoint
 
 Use one of the methods bellow based on your selected framework.
 
-#### Django
+##### Django
 
 Add the profile view to the url config.
 
 ```python
 from django.urls import path
 
 from troncos.contrib.django.profiling.views import profiling_view
 
 urlpatterns = [
     path("/debug/pprof", profiling_view, name="profiling"),
 ]
 ```
 
-#### Starlette
+##### Starlette
 
 Add the profile view to your router.
 
 ```python
 from starlette.routing import Route
 
 from troncos.contrib.starlette.profiling.views import profiling_view
 
 routes = [
     Route("/debug/pprof", profiling_view),
 ]
 ```
 
-#### ASGI
+##### ASGI
 
 Mount the generic ASGI profiling application. There is no generic way to do this,
 please check the relevant ASGI framework documentation.
 
 ```python
 from troncos.contrib.asgi.profiling.app import profiling_asgi_app
 
@@ -251,23 +263,23 @@
 from fastapi import FastAPI
 
 app = FastAPI()
 
 app.mount("/debug/pprof", profiling_asgi_app)
 ```
 
-### Verify setup
+#### Verify setup
 
 You can verify that your setup works with the [pprof](https://github.com/google/pprof) cli:
 
 ```console
 $ pprof -http :6060 "http://localhost:8080/debug/pprof"
 ```
 
-### Enable scraping
+#### Enable scraping
 
 When you deploy your application, be sure to use the custom oda annotation for scraping:
 
 ```yaml
 annotations:
   phlare.oda.com/port: "8080"
   phlare.oda.com/scrape: "true"
```

#### html2text {}

```diff
@@ -23,24 +23,25 @@
 ddtrace.patch_all() # Configure the ddtrace tracer to send traces to Tempo.
 TRACE_HOST = "127.0.0.1" # Usually obtained from env variables. TRACE_PORT =
 "4318" configure_tracer( enabled=False, # Set to True when TRACE_HOST is
 configured. service_name='SERVICE_NAME', endpoint=f"http://{TRACE_HOST}:
 {TRACE_PORT}/v1/traces", ) ``` ddtrace also uses env variables to configure the
 service name, environment and version etc. Add the following environment
 variables to your application. ``` DD_ENV="{{ environment }}" DD_SERVICE="{
-{ app }}" DD_VERSION="{{ version }}" # b3 is usually used to propagate
-distributed traces across services. DD_TRACE_PROPAGATION_STYLE_EXTRACT="b3"
-DD_TRACE_PROPAGATION_STYLE_INJECT="b3" ``` ### Using the GRPC span exporter
-Using the GRPC span exporter gives you significant performance gains. If you
-are running a critical service with high load in production, we recommend using
-GRPC. `TRACE_PORT` is usually 4317 when the Grafana agent is used to collect
-spans using GRPC. ```console poetry add troncos -E grpc ``` or ```toml
-[tool.poetry.dependencies] troncos = {version="?", extras = ["grpc"]} ```
-```python from troncos.tracing import configure_tracer, Exporter TRACE_HOST =
-"127.0.0.1" # Usually obtained from env variables. TRACE_PORT = "4317"
+{ app }}" DD_VERSION="{{ version }}" # tracecontext/w3c is usually used to
+propagate distributed traces across services.
+DD_TRACE_PROPAGATION_STYLE_EXTRACT="tracecontext"
+DD_TRACE_PROPAGATION_STYLE_INJECT="tracecontext" ``` ### Using the GRPC span
+exporter Using the GRPC span exporter gives you significant performance gains.
+If you are running a critical service with high load in production, we
+recommend using GRPC. `TRACE_PORT` is usually 4317 when the Grafana agent is
+used to collect spans using GRPC. ```console poetry add troncos -E grpc ``` or
+```toml [tool.poetry.dependencies] troncos = {version="?", extras = ["grpc"]}
+``` ```python from troncos.tracing import configure_tracer, Exporter TRACE_HOST
+= "127.0.0.1" # Usually obtained from env variables. TRACE_PORT = "4317"
 configure_tracer( enabled=False, # Set to True when TRACE_HOST is configured.
 service_name='SERVICE_NAME', endpoint=f"http://{TRACE_HOST}:{TRACE_PORT}",
 exporter=Exporter.GRPC ) ``` ### Instrument your code Manual instrumentation of
 your code is described in the [ddtrace docs](https://ddtrace.readthedocs.io/en/
 stable/basic_usage.html#manual-instrumentation). ### Add tracing context to
 your log Adding the tracing context to your log makes it easier to find
 relevant traces in Grafana. Troncos include a Structlog processor designed to
@@ -58,32 +59,38 @@
 Django middleware Log Django requests. This is not needed if you run Django
 with ASGI and use the ASGI middleware. ```python MIDDLEWARE =
 [ "troncos.contrib.django.logging.middleware.DjangoLoggingMiddleware", ... ]
 ``` #### Celery signals ` Log Celery tasks. Run the code bellow when you
 configure Celery. ```python from troncos.contrib.celery.logging.signals import
 ( connect_troncos_logging_celery_signals, )
 connect_troncos_logging_celery_signals() ``` ## Profiling ### Enabling the
-profiler Start the profiler by importing the profiler module early in your
-application. This is typically done in `settings.py` of you want to profile a
-Django application, or in `__init__.py` in the root project package. ```python
-import troncos.profiling.auto ``` ### Setup profile endpoint Use one of the
-methods bellow based on your selected framework. #### Django Add the profile
-view to the url config. ```python from django.urls import path from
+continuous py-spy profiler Start the profiler by running the
+`start_py_spy_profiler` method early in your application. This is typically
+done in `settings.py` of you want to profile a Django application, or in
+`__init__.py` in the root project package. ```python from troncos.profiling
+import start_py_spy_profiler start_py_spy_profiler(server_address="http://
+127.0.0.1:4100") ``` ### Enabling the ddtrace profiler Start the profiler by
+importing the profiler module early in your application. This is typically done
+in `settings.py` of you want to profile a Django application, or in
+`__init__.py` in the root project package. ```python import
+troncos.profiling.auto ``` #### Setup profile endpoint Use one of the methods
+bellow based on your selected framework. ##### Django Add the profile view to
+the url config. ```python from django.urls import path from
 troncos.contrib.django.profiling.views import profiling_view urlpatterns =
-[ path("/debug/pprof", profiling_view, name="profiling"), ] ``` #### Starlette
+[ path("/debug/pprof", profiling_view, name="profiling"), ] ``` ##### Starlette
 Add the profile view to your router. ```python from starlette.routing import
 Route from troncos.contrib.starlette.profiling.views import profiling_view
-routes = [ Route("/debug/pprof", profiling_view), ] ``` #### ASGI Mount the
+routes = [ Route("/debug/pprof", profiling_view), ] ``` ##### ASGI Mount the
 generic ASGI profiling application. There is no generic way to do this, please
 check the relevant ASGI framework documentation. ```python from
 troncos.contrib.asgi.profiling.app import profiling_asgi_app # FastAPI example
 from fastapi import FastAPI app = FastAPI() app.mount("/debug/pprof",
-profiling_asgi_app) ``` ### Verify setup You can verify that your setup works
+profiling_asgi_app) ``` #### Verify setup You can verify that your setup works
 with the [pprof](https://github.com/google/pprof) cli: ```console $ pprof -http
-:6060 "http://localhost:8080/debug/pprof" ``` ### Enable scraping When you
+:6060 "http://localhost:8080/debug/pprof" ``` #### Enable scraping When you
 deploy your application, be sure to use the custom oda annotation for scraping:
 ```yaml annotations: phlare.oda.com/port: "8080" phlare.oda.com/scrape: "true"
 ``` ## Logging Troncos is not designed to take control over your logger. But,
 we do include logging related tools to make instrumenting your code easer. ###
 Configure Structlog Troncos contains a helper method that lets you configure
 Structlog. First, run `poetry add structlog` to install structlog in your
 project. You can now replace your existing logger config with ```python from
```

### Comparing `troncos-4.0.0b9/pyproject.toml` & `troncos-4.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "troncos"
-version = "4.0.0b9"
+version = "4.0.1"
 description = "Collection of Python logging, tracing and profiling tools"
 authors = [
     "Guðmundur Björn Birkisson <gudmundur.birkisson@oda.com>",
     "Karl Fredrik Haugland <karlfredrik.haugland@oda.com>",
     "Eirik Martiniussen Sylliaas <eirik.sylliaas@oda.com>",
 ]
 license = "MIT"
@@ -12,19 +12,20 @@
 homepage = "https://github.com/kolonialno/troncos"
 repository = "https://github.com/kolonialno/troncos"
 documentation = "https://github.com/kolonialno/troncos"
 keywords = ["logs", "traces", "opentelemetry"]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
-ddtrace = "1.13.3"
+ddtrace = "1.15.0"
 opentelemetry-sdk = "1.18.0"
 opentelemetry-exporter-otlp-proto-http = "1.18.0"
 opentelemetry-exporter-otlp-proto-grpc = {version = "1.18.0", optional = true}
 python-ipware = "^0.9.0"
+pyroscope-io = "^0.8.3"
 
 [tool.poetry.extras]
 grpc = ["opentelemetry-exporter-otlp-proto-grpc"]
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.12.0"
 black = "^23.1.0"
@@ -40,14 +41,16 @@
 django-environ = "^0.9.0"
 pytest-benchmark = "^4.0.0"
 snakeviz = "^2.2.0"
 django = "^4.2.1"
 starlette = "^0.27.0"
 structlog = "^23.1.0"
 celery = "^5.2.7"
+structlog-sentry = "^2.0.3"
+ipython = "^8.14.0"
 
 
 [tool.black]
 target-version = ['py311']
 line-length = 88
 include = '\.pyi?$'
 safe = true
```

### Comparing `troncos-4.0.0b9/troncos/contrib/asgi/logging/middleware.py` & `troncos-4.0.1/troncos/contrib/asgi/logging/middleware.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b9/troncos/contrib/asgi/profiling/app.py` & `troncos-4.0.1/troncos/contrib/asgi/profiling/app.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b9/troncos/contrib/celery/logging/signals.py` & `troncos-4.0.1/troncos/contrib/celery/logging/signals.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b9/troncos/contrib/django/logging/middleware.py` & `troncos-4.0.1/troncos/contrib/django/logging/middleware.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b9/troncos/contrib/logging/tools/__init__.py` & `troncos-4.0.1/troncos/contrib/logging/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b9/troncos/contrib/structlog/__init__.py` & `troncos-4.0.1/troncos/contrib/structlog/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     LogfmtRenderer,
     trace_injection_processor,
 )
 
 try:
     from structlog_sentry import SentryProcessor
 except ImportError:
-    SentryProcessor = None
+    SentryProcessor = None  # type: ignore
 
 shared_processors: list[structlog.types.Processor] = [
     # Add the name of the logger to event dict.
     structlog.stdlib.add_logger_name,
     # Add log level to event dict.
     structlog.stdlib.add_log_level,
     # Add a timestamp in ISO 8601 format.
@@ -24,16 +24,20 @@
     # sys.exc_info() tuple, remove "exc_info" and render the exception
     # with traceback into the "exception" key.
     structlog.processors.format_exc_info,
     trace_injection_processor,
 ]
 
 if SentryProcessor is not None:
-    shared_processors.append(
-        SentryProcessor(level=logging.INFO, event_level=logging.ERROR)
+    format_exc_info_index = shared_processors.index(
+        structlog.processors.format_exc_info
+    )
+    shared_processors.insert(
+        format_exc_info_index,
+        SentryProcessor(level=logging.INFO, event_level=logging.ERROR),
     )
 
 
 def configure_structlog(
     *, configure_logging: bool = True, format: str = "text", level: str = "INFO"
 ) -> None:
     """
```

### Comparing `troncos-4.0.0b9/troncos/contrib/structlog/processors.py` & `troncos-4.0.1/troncos/contrib/structlog/processors.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b9/troncos/profiling/profiler.py` & `troncos-4.0.1/troncos/profiling/profiler.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any
 
 from ddtrace.profiling import exporter
-from ddtrace.profiling.exporter import pprof  # type: ignore
+from ddtrace.profiling.exporter import pprof
 from ddtrace.profiling.profiler import (
     Profiler as DDProfiler,
     _ProfilerInstance as DDProfilerInstance,
 )
 
 
 class _PprofExporter(pprof.PprofExporter):  # type: ignore[misc]
@@ -32,23 +32,23 @@
         pprof_profile, _ = super(_PprofExporter, self).export(
             events, start_time_ns, end_time_ns
         )
 
         self.pprof = pprof_profile.SerializeToString()
 
 
-class _ProfilerInstance(DDProfilerInstance):
+class _ProfilerInstance(DDProfilerInstance):  # type: ignore
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         self.exporter = _PprofExporter()
 
         super().__init__(*args, **kwargs)
 
     def _build_default_exporters(self) -> list[exporter.Exporter]:
         return [self.exporter]
 
 
-class Profiler(DDProfiler):
+class Profiler(DDProfiler):  # type: ignore
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         self._profiler = _ProfilerInstance(*args, **kwargs)
 
     def get_profile(self) -> str:
-        return self._profiler.exporter.pprof  # type: ignore
+        return self._profiler.exporter.pprof
```

### Comparing `troncos-4.0.0b9/troncos/tracing/__init__.py` & `troncos-4.0.1/troncos/tracing/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b9/troncos/tracing/_otel.py` & `troncos-4.0.1/troncos/tracing/_otel.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b9/troncos/tracing/_span.py` & `troncos-4.0.1/troncos/tracing/_span.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,29 +11,31 @@
     Event,
     ReadableSpan,
 )
 from opentelemetry.sdk.util import BoundedList
 from opentelemetry.trace import SpanContext, SpanKind, Status, StatusCode
 from opentelemetry.trace.span import TraceFlags
 
-_dd_span_ignore_attr = [
+_dd_span_ignore_attr = {
     "runtime-id",
     "_sampling_priority_v1",
     "env",
     "version",
     "span.kind",
-]
+}
+
+_trace_flags_sampled = TraceFlags(1)
 
 
 def _span_context(span: DDSpan) -> SpanContext:
     return SpanContext(
         trace_id=span.trace_id,
         span_id=span.span_id,
         is_remote=False,
-        trace_flags=TraceFlags(1),
+        trace_flags=_trace_flags_sampled,
     )
 
 
 def _parent_span_context(dd_span: DDSpan) -> SpanContext | None:
     if dd_span.parent_id:
         if not dd_span._parent:
             # External trace parent
@@ -53,40 +55,41 @@
 
 
 def _span_kind(dd_span: DDSpan) -> SpanKind:
     dd_kind = dd_span._meta.get(constants.SPAN_KIND, "none")
     return _span_kind_map.get(dd_kind, SpanKind.INTERNAL)
 
 
+_dd_span_err_attr_mapping = {
+    "error.msg": "exception.message",
+    "error.type": "exception.type",
+    "error.stack": "exception.stacktrace",
+}
+
+
 def _span_status_and_attributes(
-    dd_span: DDSpan, ignore_attrs: list[str]
+    dd_span: DDSpan, ignore_attrs: set[str]
 ) -> tuple[Status, list[Event], dict[str, Any]]:
-    dd_span_err_attr_mapping = {
-        "error.msg": "exception.message",
-        "error.type": "exception.type",
-        "error.stack": "exception.stacktrace",
-    }
-
     # Collect all "attributes" from the dd span
     dd_span_attr: dict[str, Any] = {
-        **dd_span._meta,  # type: ignore
-        **dd_span._metrics,  # type: ignore
+        **dd_span._meta,
+        **dd_span._metrics,
         "resource": dd_span.resource,
     }
 
     otel_attrs = {}
     events: list[Event] = []
     otel_error_attrs = {}
 
     # Map set OTEL attributes based on DD attributes
     for k, v in dd_span_attr.items():
-        otel_err_attr = dd_span_err_attr_mapping.get(k)
         if k.startswith("_dd"):
             continue
-        elif otel_err_attr:
+        otel_err_attr = _dd_span_err_attr_mapping.get(k)
+        if otel_err_attr:
             otel_error_attrs[otel_err_attr] = v
         elif k not in ignore_attrs:
             otel_attrs[k] = v
 
     if otel_error_attrs:
         events.append(
             Event(
@@ -120,21 +123,26 @@
 
     base_attributes = dict(default_resource.attributes)
     base_attributes[SERVICE_NAME] = dd_span.service
 
     return Resource(base_attributes)
 
 
-def translate_span(dd_span: DDSpan, default_resource: Resource) -> ReadableSpan:
+def default_ignore_attrs() -> set[str]:
+    return _dd_span_ignore_attr
+
+
+def translate_span(
+    dd_span: DDSpan, default_resource: Resource, ignore_attrs: set[str]
+) -> ReadableSpan:
     """Transelate a ddtrace span to an OTEL span."""
     assert dd_span.duration_ns, "Span not finished."
 
     status, events, attributes = _span_status_and_attributes(
-        dd_span,
-        ignore_attrs=_dd_span_ignore_attr + list(default_resource.attributes.keys()),
+        dd_span, ignore_attrs=ignore_attrs
     )
 
     otel_span = ReadableSpan(
         name=dd_span.name,
         context=_span_context(dd_span),
         parent=_parent_span_context(dd_span),
         resource=_span_resource(dd_span, default_resource),
```

### Comparing `troncos-4.0.0b9/troncos/tracing/decorators.py` & `troncos-4.0.1/troncos/tracing/decorators.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b9/PKG-INFO` & `troncos-4.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: troncos
-Version: 4.0.0b9
+Version: 4.0.1
 Summary: Collection of Python logging, tracing and profiling tools
 Home-page: https://github.com/kolonialno/troncos
 License: MIT
 Keywords: logs,traces,opentelemetry
 Author: Guðmundur Björn Birkisson
 Author-email: gudmundur.birkisson@oda.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: grpc
-Requires-Dist: ddtrace (==1.13.3)
+Requires-Dist: ddtrace (==1.15.0)
 Requires-Dist: opentelemetry-exporter-otlp-proto-grpc (==1.18.0) ; extra == "grpc"
 Requires-Dist: opentelemetry-exporter-otlp-proto-http (==1.18.0)
 Requires-Dist: opentelemetry-sdk (==1.18.0)
+Requires-Dist: pyroscope-io (>=0.8.3,<0.9.0)
 Requires-Dist: python-ipware (>=0.9.0,<0.10.0)
 Project-URL: Documentation, https://github.com/kolonialno/troncos
 Project-URL: Repository, https://github.com/kolonialno/troncos
 Description-Content-Type: text/markdown
 
 <h1 align="center" style="border-bottom: 0">
   🪵<br>
@@ -110,17 +111,17 @@
 
 Add the following environment variables to your application.
 
 ```
 DD_ENV="{{ environment }}"
 DD_SERVICE="{{ app }}"
 DD_VERSION="{{ version }}"
-# b3 is usually used to propagate distributed traces across services.
-DD_TRACE_PROPAGATION_STYLE_EXTRACT="b3"
-DD_TRACE_PROPAGATION_STYLE_INJECT="b3"
+# tracecontext/w3c is usually used to propagate distributed traces across services.
+DD_TRACE_PROPAGATION_STYLE_EXTRACT="tracecontext"
+DD_TRACE_PROPAGATION_STYLE_INJECT="tracecontext"
 ```
 
 ### Using the GRPC span exporter
 
 Using the GRPC span exporter gives you significant performance gains.
 If you are running a critical service with high load in production,
 we recommend using GRPC.
@@ -217,57 +218,69 @@
 )
 
 connect_troncos_logging_celery_signals()
 ```
 
 ## Profiling
 
-### Enabling the profiler
+### Enabling the continuous py-spy profiler
+
+Start the profiler by running the `start_py_spy_profiler` method early in your application. This is
+typically done in `settings.py` of you want to profile a Django application, or in `__init__.py`
+in the root project package.
+
+```python
+from troncos.profiling import start_py_spy_profiler
+
+start_py_spy_profiler(server_address="http://127.0.0.1:4100")
+```
+
+### Enabling the ddtrace profiler
 
 Start the profiler by importing the profiler module early in your application. This is
 typically done in `settings.py` of you want to profile a Django application, or in `__init__.py`
 in the root project package.
 
 ```python
 import troncos.profiling.auto
 ```
 
-### Setup profile endpoint
+#### Setup profile endpoint
 
 Use one of the methods bellow based on your selected framework.
 
-#### Django
+##### Django
 
 Add the profile view to the url config.
 
 ```python
 from django.urls import path
 
 from troncos.contrib.django.profiling.views import profiling_view
 
 urlpatterns = [
     path("/debug/pprof", profiling_view, name="profiling"),
 ]
 ```
 
-#### Starlette
+##### Starlette
 
 Add the profile view to your router.
 
 ```python
 from starlette.routing import Route
 
 from troncos.contrib.starlette.profiling.views import profiling_view
 
 routes = [
     Route("/debug/pprof", profiling_view),
 ]
 ```
 
-#### ASGI
+##### ASGI
 
 Mount the generic ASGI profiling application. There is no generic way to do this,
 please check the relevant ASGI framework documentation.
 
 ```python
 from troncos.contrib.asgi.profiling.app import profiling_asgi_app
 
@@ -275,23 +288,23 @@
 from fastapi import FastAPI
 
 app = FastAPI()
 
 app.mount("/debug/pprof", profiling_asgi_app)
 ```
 
-### Verify setup
+#### Verify setup
 
 You can verify that your setup works with the [pprof](https://github.com/google/pprof) cli:
 
 ```console
 $ pprof -http :6060 "http://localhost:8080/debug/pprof"
 ```
 
-### Enable scraping
+#### Enable scraping
 
 When you deploy your application, be sure to use the custom oda annotation for scraping:
 
 ```yaml
 annotations:
   phlare.oda.com/port: "8080"
   phlare.oda.com/scrape: "true"
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: troncos Version: 4.0.0b9 Summary: Collection of
+Metadata-Version: 2.1 Name: troncos Version: 4.0.1 Summary: Collection of
 Python logging, tracing and profiling tools Home-page: https://github.com/
 kolonialno/troncos License: MIT Keywords: logs,traces,opentelemetry Author:
 GuÃ°mundur BjÃ¶rn Birkisson Author-email: gudmundur.birkisson@oda.com Requires-
 Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: grpc Requires-Dist: ddtrace (==1.13.3) Requires-Dist:
+Provides-Extra: grpc Requires-Dist: ddtrace (==1.15.0) Requires-Dist:
 opentelemetry-exporter-otlp-proto-grpc (==1.18.0) ; extra == "grpc" Requires-
 Dist: opentelemetry-exporter-otlp-proto-http (==1.18.0) Requires-Dist:
-opentelemetry-sdk (==1.18.0) Requires-Dist: python-ipware (>=0.9.0,<0.10.0)
-Project-URL: Documentation, https://github.com/kolonialno/troncos Project-URL:
-Repository, https://github.com/kolonialno/troncos Description-Content-Type:
-text/markdown
+opentelemetry-sdk (==1.18.0) Requires-Dist: pyroscope-io (>=0.8.3,<0.9.0)
+Requires-Dist: python-ipware (>=0.9.0,<0.10.0) Project-URL: Documentation,
+https://github.com/kolonialno/troncos Project-URL: Repository, https://
+github.com/kolonialno/troncos Description-Content-Type: text/markdown
                                   ****** ðªµ
                                    Troncos
                                      ******
           Collection of Python logging, tracing and profiling tools
        [CI_status] [https://img.shields.io/pypi/v/troncos.svg] [https://
 img.shields.io/pypi/pyversions/troncos] [https://img.shields.io/github/license/
                             kolonialno/troncos.svg]
@@ -37,24 +37,25 @@
 ddtrace.patch_all() # Configure the ddtrace tracer to send traces to Tempo.
 TRACE_HOST = "127.0.0.1" # Usually obtained from env variables. TRACE_PORT =
 "4318" configure_tracer( enabled=False, # Set to True when TRACE_HOST is
 configured. service_name='SERVICE_NAME', endpoint=f"http://{TRACE_HOST}:
 {TRACE_PORT}/v1/traces", ) ``` ddtrace also uses env variables to configure the
 service name, environment and version etc. Add the following environment
 variables to your application. ``` DD_ENV="{{ environment }}" DD_SERVICE="{
-{ app }}" DD_VERSION="{{ version }}" # b3 is usually used to propagate
-distributed traces across services. DD_TRACE_PROPAGATION_STYLE_EXTRACT="b3"
-DD_TRACE_PROPAGATION_STYLE_INJECT="b3" ``` ### Using the GRPC span exporter
-Using the GRPC span exporter gives you significant performance gains. If you
-are running a critical service with high load in production, we recommend using
-GRPC. `TRACE_PORT` is usually 4317 when the Grafana agent is used to collect
-spans using GRPC. ```console poetry add troncos -E grpc ``` or ```toml
-[tool.poetry.dependencies] troncos = {version="?", extras = ["grpc"]} ```
-```python from troncos.tracing import configure_tracer, Exporter TRACE_HOST =
-"127.0.0.1" # Usually obtained from env variables. TRACE_PORT = "4317"
+{ app }}" DD_VERSION="{{ version }}" # tracecontext/w3c is usually used to
+propagate distributed traces across services.
+DD_TRACE_PROPAGATION_STYLE_EXTRACT="tracecontext"
+DD_TRACE_PROPAGATION_STYLE_INJECT="tracecontext" ``` ### Using the GRPC span
+exporter Using the GRPC span exporter gives you significant performance gains.
+If you are running a critical service with high load in production, we
+recommend using GRPC. `TRACE_PORT` is usually 4317 when the Grafana agent is
+used to collect spans using GRPC. ```console poetry add troncos -E grpc ``` or
+```toml [tool.poetry.dependencies] troncos = {version="?", extras = ["grpc"]}
+``` ```python from troncos.tracing import configure_tracer, Exporter TRACE_HOST
+= "127.0.0.1" # Usually obtained from env variables. TRACE_PORT = "4317"
 configure_tracer( enabled=False, # Set to True when TRACE_HOST is configured.
 service_name='SERVICE_NAME', endpoint=f"http://{TRACE_HOST}:{TRACE_PORT}",
 exporter=Exporter.GRPC ) ``` ### Instrument your code Manual instrumentation of
 your code is described in the [ddtrace docs](https://ddtrace.readthedocs.io/en/
 stable/basic_usage.html#manual-instrumentation). ### Add tracing context to
 your log Adding the tracing context to your log makes it easier to find
 relevant traces in Grafana. Troncos include a Structlog processor designed to
@@ -72,32 +73,38 @@
 Django middleware Log Django requests. This is not needed if you run Django
 with ASGI and use the ASGI middleware. ```python MIDDLEWARE =
 [ "troncos.contrib.django.logging.middleware.DjangoLoggingMiddleware", ... ]
 ``` #### Celery signals ` Log Celery tasks. Run the code bellow when you
 configure Celery. ```python from troncos.contrib.celery.logging.signals import
 ( connect_troncos_logging_celery_signals, )
 connect_troncos_logging_celery_signals() ``` ## Profiling ### Enabling the
-profiler Start the profiler by importing the profiler module early in your
-application. This is typically done in `settings.py` of you want to profile a
-Django application, or in `__init__.py` in the root project package. ```python
-import troncos.profiling.auto ``` ### Setup profile endpoint Use one of the
-methods bellow based on your selected framework. #### Django Add the profile
-view to the url config. ```python from django.urls import path from
+continuous py-spy profiler Start the profiler by running the
+`start_py_spy_profiler` method early in your application. This is typically
+done in `settings.py` of you want to profile a Django application, or in
+`__init__.py` in the root project package. ```python from troncos.profiling
+import start_py_spy_profiler start_py_spy_profiler(server_address="http://
+127.0.0.1:4100") ``` ### Enabling the ddtrace profiler Start the profiler by
+importing the profiler module early in your application. This is typically done
+in `settings.py` of you want to profile a Django application, or in
+`__init__.py` in the root project package. ```python import
+troncos.profiling.auto ``` #### Setup profile endpoint Use one of the methods
+bellow based on your selected framework. ##### Django Add the profile view to
+the url config. ```python from django.urls import path from
 troncos.contrib.django.profiling.views import profiling_view urlpatterns =
-[ path("/debug/pprof", profiling_view, name="profiling"), ] ``` #### Starlette
+[ path("/debug/pprof", profiling_view, name="profiling"), ] ``` ##### Starlette
 Add the profile view to your router. ```python from starlette.routing import
 Route from troncos.contrib.starlette.profiling.views import profiling_view
-routes = [ Route("/debug/pprof", profiling_view), ] ``` #### ASGI Mount the
+routes = [ Route("/debug/pprof", profiling_view), ] ``` ##### ASGI Mount the
 generic ASGI profiling application. There is no generic way to do this, please
 check the relevant ASGI framework documentation. ```python from
 troncos.contrib.asgi.profiling.app import profiling_asgi_app # FastAPI example
 from fastapi import FastAPI app = FastAPI() app.mount("/debug/pprof",
-profiling_asgi_app) ``` ### Verify setup You can verify that your setup works
+profiling_asgi_app) ``` #### Verify setup You can verify that your setup works
 with the [pprof](https://github.com/google/pprof) cli: ```console $ pprof -http
-:6060 "http://localhost:8080/debug/pprof" ``` ### Enable scraping When you
+:6060 "http://localhost:8080/debug/pprof" ``` #### Enable scraping When you
 deploy your application, be sure to use the custom oda annotation for scraping:
 ```yaml annotations: phlare.oda.com/port: "8080" phlare.oda.com/scrape: "true"
 ``` ## Logging Troncos is not designed to take control over your logger. But,
 we do include logging related tools to make instrumenting your code easer. ###
 Configure Structlog Troncos contains a helper method that lets you configure
 Structlog. First, run `poetry add structlog` to install structlog in your
 project. You can now replace your existing logger config with ```python from
```

