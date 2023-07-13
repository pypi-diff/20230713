# Comparing `tmp/svc_reg-23.1.0.tar.gz` & `tmp/svc_reg-23.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Wed Jul 12 17:30:52 2023, max compression
+gzip compressed data, last modified: Thu Jul 13 11:01:31 2023, max compression
```

## Comparing `svc_reg-23.1.0.tar` & `svc_reg-23.2.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0      472 2023-07-12 17:30:52.000000 svc_reg-23.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0        5 2023-07-12 17:30:52.000000 svc_reg-23.1.0/.python-version-default
--rw-r--r--   0        0        0      707 2023-07-12 17:30:52.000000 svc_reg-23.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      294 2023-07-12 17:30:52.000000 svc_reg-23.1.0/conftest.py
--rw-r--r--   0        0        0      840 2023-07-12 17:30:52.000000 svc_reg-23.1.0/tox.ini
--rw-r--r--   0        0        0     5482 2023-07-12 17:30:52.000000 svc_reg-23.1.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       18 2023-07-12 17:30:52.000000 svc_reg-23.1.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      865 2023-07-12 17:30:52.000000 svc_reg-23.1.0/.github/SECURITY.md
--rw-r--r--   0        0        0      117 2023-07-12 17:30:52.000000 svc_reg-23.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0     3925 2023-07-12 17:30:52.000000 svc_reg-23.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      749 2023-07-12 17:30:52.000000 svc_reg-23.1.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1642 2023-07-12 17:30:52.000000 svc_reg-23.1.0/.github/workflows/pypi-package.yml
--rw-r--r--   0        0        0      367 2023-07-12 17:30:52.000000 svc_reg-23.1.0/src/svc_reg/__init__.py
--rw-r--r--   0        0        0     5090 2023-07-12 17:30:52.000000 svc_reg-23.1.0/src/svc_reg/_core.py
--rw-r--r--   0        0        0     2088 2023-07-12 17:30:52.000000 svc_reg-23.1.0/src/svc_reg/flask.py
--rw-r--r--   0        0        0        0 2023-07-12 17:30:52.000000 svc_reg-23.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1105 2023-07-12 17:30:52.000000 svc_reg-23.1.0/tests/test_async.py
--rw-r--r--   0        0        0     7426 2023-07-12 17:30:52.000000 svc_reg-23.1.0/tests/test_core.py
--rw-r--r--   0        0        0     4823 2023-07-12 17:30:52.000000 svc_reg-23.1.0/tests/test_flask.py
--rw-r--r--   0        0        0      435 2023-07-12 17:30:52.000000 svc_reg-23.1.0/tests/typing/core.py
--rw-r--r--   0        0        0      511 2023-07-12 17:30:52.000000 svc_reg-23.1.0/tests/typing/flask_.py
--rw-r--r--   0        0        0      108 2023-07-12 17:30:52.000000 svc_reg-23.1.0/.gitignore
--rw-r--r--   0        0        0     1072 2023-07-12 17:30:52.000000 svc_reg-23.1.0/LICENSE
--rw-r--r--   0        0        0     8715 2023-07-12 17:30:52.000000 svc_reg-23.1.0/README.md
--rw-r--r--   0        0        0     3328 2023-07-12 17:30:52.000000 svc_reg-23.1.0/pyproject.toml
--rw-r--r--   0        0        0    10072 2023-07-12 17:30:52.000000 svc_reg-23.1.0/PKG-INFO
+-rw-r--r--   0        0        0      472 2023-07-13 11:01:31.000000 svc_reg-23.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        5 2023-07-13 11:01:31.000000 svc_reg-23.2.0/.python-version-default
+-rw-r--r--   0        0        0     1504 2023-07-13 11:01:31.000000 svc_reg-23.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0    11229 2023-07-13 11:01:31.000000 svc_reg-23.2.0/README.md
+-rw-r--r--   0        0        0      294 2023-07-13 11:01:31.000000 svc_reg-23.2.0/conftest.py
+-rw-r--r--   0        0        0      840 2023-07-13 11:01:31.000000 svc_reg-23.2.0/tox.ini
+-rw-r--r--   0        0        0     5482 2023-07-13 11:01:31.000000 svc_reg-23.2.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      291 2023-07-13 11:01:31.000000 svc_reg-23.2.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0       18 2023-07-13 11:01:31.000000 svc_reg-23.2.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      865 2023-07-13 11:01:31.000000 svc_reg-23.2.0/.github/SECURITY.md
+-rw-r--r--   0        0        0      117 2023-07-13 11:01:31.000000 svc_reg-23.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     3925 2023-07-13 11:01:31.000000 svc_reg-23.2.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      749 2023-07-13 11:01:31.000000 svc_reg-23.2.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1642 2023-07-13 11:01:31.000000 svc_reg-23.2.0/.github/workflows/pypi-package.yml
+-rw-r--r--   0        0        0      367 2023-07-13 11:01:31.000000 svc_reg-23.2.0/src/svc_reg/__init__.py
+-rw-r--r--   0        0        0     5611 2023-07-13 11:01:31.000000 svc_reg-23.2.0/src/svc_reg/_core.py
+-rw-r--r--   0        0        0     2893 2023-07-13 11:01:31.000000 svc_reg-23.2.0/src/svc_reg/flask.py
+-rw-r--r--   0        0        0        0 2023-07-13 11:01:31.000000 svc_reg-23.2.0/src/svc_reg/py.typed
+-rw-r--r--   0        0        0        0 2023-07-13 11:01:31.000000 svc_reg-23.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1103 2023-07-13 11:01:31.000000 svc_reg-23.2.0/tests/test_async.py
+-rw-r--r--   0        0        0     8819 2023-07-13 11:01:31.000000 svc_reg-23.2.0/tests/test_core.py
+-rw-r--r--   0        0        0     6182 2023-07-13 11:01:31.000000 svc_reg-23.2.0/tests/test_flask.py
+-rw-r--r--   0        0        0      684 2023-07-13 11:01:31.000000 svc_reg-23.2.0/tests/typing/core.py
+-rw-r--r--   0        0        0      947 2023-07-13 11:01:31.000000 svc_reg-23.2.0/tests/typing/flask_.py
+-rw-r--r--   0        0        0      108 2023-07-13 11:01:31.000000 svc_reg-23.2.0/.gitignore
+-rw-r--r--   0        0        0     1072 2023-07-13 11:01:31.000000 svc_reg-23.2.0/LICENSE
+-rw-r--r--   0        0        0     4143 2023-07-13 11:01:31.000000 svc_reg-23.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4658 2023-07-13 11:01:31.000000 svc_reg-23.2.0/PKG-INFO
```

### Comparing `svc_reg-23.1.0/tox.ini` & `svc_reg-23.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `svc_reg-23.1.0/.github/CODE_OF_CONDUCT.md` & `svc_reg-23.2.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `svc_reg-23.1.0/.github/SECURITY.md` & `svc_reg-23.2.0/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `svc_reg-23.1.0/.github/workflows/ci.yml` & `svc_reg-23.2.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `svc_reg-23.1.0/.github/workflows/codeql-analysis.yml` & `svc_reg-23.2.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `svc_reg-23.1.0/.github/workflows/pypi-package.yml` & `svc_reg-23.2.0/.github/workflows/pypi-package.yml`

 * *Files identical despite different names*

### Comparing `svc_reg-23.1.0/src/svc_reg/_core.py` & `svc_reg-23.2.0/src/svc_reg/_core.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from __future__ import annotations
 
 import asyncio
+import logging
 
 from collections.abc import Callable
 from contextlib import suppress
 from typing import Any
 
 import attrs
 
 
+log = logging.getLogger(__name__)
+
+
 class ServiceNotFoundError(Exception):
     """
     Raised when a service type is not registered.
     """
 
 
 @attrs.define
@@ -84,37 +88,49 @@
     def forget_service_type(self, svc_type: type) -> None:
         """
         Remove all traces of *svc_type*.
         """
         with suppress(KeyError):
             del self.instantiated[svc_type]
 
-    def cleanup(self) -> None:
+    def close(self) -> None:
         """
         Run all synchronous registered cleanups.
         """
         while self.cleanups:
             rs, svc = self.cleanups.pop()
-            rs.cleanup(svc)  # type: ignore[misc]
+            try:
+                rs.cleanup(svc)  # type: ignore[misc]
+            except Exception:  # noqa: PERF203, BLE001
+                log.warning(
+                    "clean up failed",
+                    exc_info=True,
+                    extra={"service": rs.name},
+                )
 
-    async def acleanup(self) -> None:
+    async def aclose(self) -> None:
         """
-        Run *all* registered cleanups.
-
-        This method calls ``cleanup()`` first.
+        Run *all* registered cleanups -- synchronous **and** asynchronous.
         """
-        self.cleanup()
+        self.close()
 
         while self.async_cleanups:
             rs, svc = self.async_cleanups.pop()
-            await rs.cleanup(svc)  # type: ignore[misc]
+            try:
+                await rs.cleanup(svc)  # type: ignore[misc]
+            except Exception:  # noqa: PERF203, BLE001
+                log.warning(
+                    "clean up failed",
+                    exc_info=True,
+                    extra={"service": rs.name},
+                )
 
     def get_pings(self) -> list[ServicePing]:
         """
-        Get all pingable services and bind them to *container* for cleanups.
+        Get all pingable services and bind them to ourselves for cleanups.
         """
         return [
             ServicePing(self, rs)
             for rs in self.registry.services.values()
             if rs.ping is not None
         ]
```

### Comparing `svc_reg-23.1.0/src/svc_reg/flask.py` & `svc_reg-23.2.0/src/svc_reg/flask.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+import warnings
+
 from collections.abc import Callable
 from typing import Any
 
 from flask import Flask, current_app, g, has_app_context
 
 from ._core import Container, Registry, ServicePing
 
@@ -26,27 +28,53 @@
     """
     _, container = _ensure_req_data()
 
     return container.get(svc_type)
 
 
 def register_factory(
+    app: Flask,
+    svc_type: type,
+    factory: Callable,
+    *,
+    cleanup: Callable | None = None,
+    ping: Callable | None = None,
+) -> None:
+    app.config["svc_registry"].register_factory(
+        svc_type, factory, cleanup=cleanup, ping=ping
+    )
+
+
+def register_value(
+    app: Flask,
+    svc_type: type,
+    instance: object,
+    *,
+    cleanup: Callable | None = None,
+    ping: Callable | None = None,
+) -> None:
+    app.config["svc_registry"].register_value(
+        svc_type, instance, cleanup=cleanup, ping=ping
+    )
+
+
+def replace_factory(
     svc_type: type,
     factory: Callable,
     *,
     cleanup: Callable | None = None,
     ping: Callable | None = None,
 ) -> None:
     registry, container = _ensure_req_data()
 
     container.forget_service_type(svc_type)
     registry.register_factory(svc_type, factory, cleanup=cleanup, ping=ping)
 
 
-def register_value(
+def replace_value(
     svc_type: type,
     instance: object,
     *,
     cleanup: Callable | None = None,
     ping: Callable | None = None,
 ) -> None:
     registry, container = _ensure_req_data()
@@ -64,24 +92,23 @@
 def teardown(exc: BaseException | None) -> None:
     """
     To be used with Flask.teardown_appcontext that requires to take an
     exception.
 
     The app context is torn down after the response is sent.
     """
-    if has_app_context():
-        cleanup()
-
-
-def cleanup() -> None:
-    """
-    Remove container & run all registered cleanups.
-    """
-    if container := g.pop("svc_container", None):
-        container.cleanup()
+    if has_app_context() and (container := g.pop("svc_container", None)):
+        container.close()
+        if container.async_cleanups:
+            warnings.warn(
+                f"{len(container.async_cleanups)} async cleanup(s) left, but "
+                "svc-reg's Flask support does not support them automatically.",
+                # stacklevel doesn't matter here; it's coming from a framework.
+                stacklevel=1,
+            )
 
 
 def _ensure_req_data() -> tuple[Registry, Container]:
     registry: Registry = current_app.config["svc_registry"]
     if "svc_container" not in g:
         g.svc_container = Container(registry)
```

### Comparing `svc_reg-23.1.0/tests/test_async.py` & `svc_reg-23.2.0/tests/test_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,8 +46,8 @@
         reg.register_factory(Service, Service, cleanup=cleanup)
 
         svc = container.get(Service)
 
         assert 1 == len(container.async_cleanups)
         assert Service() == svc
 
-        await container.acleanup()
+        await container.aclose()
```

### Comparing `svc_reg-23.1.0/tests/test_core.py` & `svc_reg-23.2.0/tests/test_core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,26 @@
-from unittest.mock import Mock
+from unittest.mock import AsyncMock, Mock
 
 import pytest
 
 import svc_reg
 
 
 class Service:
     pass
 
 
 class AnotherService:
     pass
 
 
+class YetAnotherService:
+    pass
+
+
 @pytest.fixture(name="rs")
 def _rs(svc):
     return svc_reg.RegisteredService(Service, Service, None, None)
 
 
 @pytest.fixture(name="container")
 def _container(registry):
@@ -188,20 +192,25 @@
     def test_repr(self, container, rs, svc):
         """
         The repr counts correctly.
         """
         rs2 = svc_reg.RegisteredService(
             AnotherService, svc, Mock(spec_set=["__call__"]), None
         )
+        rs3 = svc_reg.RegisteredService(
+            AnotherService, svc, AsyncMock(spec_set=["__call__"]), None
+        )
 
         container._add_instance(rs, Service())
         container._add_instance(rs2, Service())
+        container._add_instance(rs3, Service())  # overwrites  rs2
 
         assert (
-            "<Container(instantiated=2, cleanups=1, async_cleanups=0>"
+            # rs2 has been removed, but its cleanup is still there.
+            "<Container(instantiated=2, cleanups=1, async_cleanups=1>"
             == repr(container)
         )
 
     def test_cleanup_called(self, container, rs):
         """
         Services that have a cleanup have them called on cleanup.
         """
@@ -209,18 +218,52 @@
 
         svc = AnotherService()
         rs_cleanup = svc_reg.RegisteredService(
             AnotherService, AnotherService, Mock(spec_set=["__call__"]), None
         )
         container._add_instance(rs_cleanup, svc)
 
-        container.cleanup()
+        container.close()
 
         rs_cleanup.cleanup.assert_called_once_with(svc)
 
+    @pytest.mark.asyncio()
+    async def test_clean_resilient(self, container, registry, caplog):
+        """
+        Failing cleanups are logged and ignored. They do not break the
+        cleanup process.
+        """
+        registry.register_factory(
+            Service,
+            Service,
+            cleanup=Mock(spec_set=["__call__"], side_effect=Exception),
+        )
+        registry.register_factory(
+            AnotherService,
+            AnotherService,
+            cleanup=AsyncMock(spec_set=["__call__"], side_effect=Exception),
+        )
+        last_cleanup = Mock(spec_set=["__call__"])
+        registry.register_factory(
+            YetAnotherService,
+            YetAnotherService,
+            cleanup=last_cleanup,
+        )
+
+        container.get(Service)
+        container.get(AnotherService)
+        container.get(YetAnotherService)
+
+        await container.aclose()
+
+        # Sync cleanups are run first.
+        assert "Service" == caplog.records[0].service
+        assert "AnotherService" == caplog.records[1].service
+        last_cleanup.assert_called_once()
+
 
 class TestRegisteredService:
     def test_repr(self, rs):
         """
         repr uses the fully-qualified name of a svc type.
         """
```

### Comparing `svc_reg-23.1.0/LICENSE` & `svc_reg-23.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `svc_reg-23.1.0/README.md` & `svc_reg-23.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,82 @@
+<!-- begin-pypi -->
+
 # A Service Registry for Dependency Injection
 
 > **Warning**
 > ☠️ Not ready yet! ☠️
 >
-> Feedback is welcome, but everything can and will change until proclaimed stable.
+> This project is only public to [gather feedback](https://github.com/hynek/svc-reg/discussions), and everything can and will change until the project is proclaimed stable.
+>
+> Currently only [**Flask** support](#flask) is production-ready, but API details can still change.
+>
+> At this point, it's unclear whether this project will become a "proper Hynek project".
+> I will keep using it for my work projects, but whether this will grow beyond my personal needs depends on community interest.
+
+*svc-reg* is a [service locator](https://en.wikipedia.org/wiki/Service_locator_pattern) for Python that lets you register factories for types/interfaces and then create instances of those types with unified life-cycle management and health checks.
+
+**This allows you to configure and manage resources in *one central place* and access them in a *consistent* way.**
+
+The idea is that at runtime, you say, for example, "*Give me a database connection*!", and *svc-reg* will give you one, depending on how you configured it.
+If you like the [*Dependency Inversion Principle*](https://en.wikipedia.org/wiki/Dependency_inversion_principle) (aka "*program against interfaces, not implementations*"), you would register concrete factories for abstract interfaces[^abstract].
+
+[^abstract]: In Python usually a [`Protocol`](https://docs.python.org/3/library/typing.html#typing.Protocol) or an [Abstract Base Class](https://docs.python.org/3.11/library/abc.html).
+
+That:
+
+- enables **dependency injection**,
+- simplifies **testing**,
+- unifies **cleanups**,
+- and allows for **easy health** checks across *all* resources.
+
+No global mutable state is necessary – but possible for extra comfort.
+
+The goal is to minimize your business code to:
+
+```python
+def view(request):
+    db = request.services.get(Database)
+```
 
-*svc-reg* is a service registry for Python that lets you register factories for certain types and then create instances of those types with life-cycle management and health checks.
+or even:
 
-This allows you to store resources and their factories in one central place and access them in a consistent way.
-That enables dependency injection, simplifies testing, unifies cleanups, and allows for easy health checks across *all* resources.
+```python
+def view():
+    db = services.get(Database)
+```
 
-It's up to you whether you want to use thread-local global variable magic like Flask has popularized, or not.
+The latter already works with [Flask](#flask).
+
+<!-- end-pypi -->
 
 
 ## Low-Level Core API
 
-You're unlikely to use the core API directly, but it's good to know what's going on underneath.
+You're unlikely to use the core API directly, but knowing what's happening underneath is good to dispel any concerns about magic.
 
-*svc-reg* has two important concepts:
+*svc-reg* has two essential concepts:
 
 A **`Registry`** allows to register factories for certain types.
-It's expected to live as long as you application lives.
-It's only job is to store and retrieve factories.
+It's expected to live as long as your application lives.
+Its only job is to store and retrieve factories.
 
 It is possible to register either factories or values:
 
 ```python
 >>> import svc_reg
 >>> import uuid
 
 >>> reg = svc_reg.Registry()
 
 >>> reg.register_factory(uuid.UUID, uuid.uuid4)
 >>> reg.register_value(str, "Hello World")
 
 ```
 
-The values and return values of the factories don't have to be actually instances of the type they're registered for.
+The values and return values of the factories don't have to be actual instances of the type they're registered for.
 But the types must be *hashable* because they're used as keys in a lookup dictionary.
 
 ---
 
 A **`Container`** belongs to a Registry and allows to create instances of the registered types and takes care of their life-cycle:
 
 ```python
@@ -54,50 +90,62 @@
 >>> u is container.get(uuid.UUID)
 True
 >>> container.get(str)
 'Hello World'
 
 ```
 
-A container lives as long as you want the instances to live -- e.g. as long as a request lives.
-At the end the you run `container.cleanup()` to cleanup all instances that the container has created.
+A container lives as long as you want the instances to live -- e.g., as long as a request lives.
+At the end, you run `container.close()` to clean up all instances that the container has created.
 You can use this to return database connections to a pool, et cetera.
 
-If you have async cleanup functions, use `await container.acleanup()` instead.
+If you have async cleanup functions, use `await container.aclose()` instead.
 It will run both sync and async cleanup functions.
 
+Failing cleanups are logged at `warning` level but otherwise ignored.
+
 ---
 
-Additionally, each registered service may have a `ping` callable that can be used in a health check.
-You can ask for all pingable registered services with `container.get_pings()`.
+Additionally, each registered service may have a `ping` callable that you can use for health checks.
+You can request all pingable registered services with `container.get_pings()`.
 This returns a list of `ServicePing` objects that currently have a name property to identify the ping and a `ping` method that instantiates the service, adds it to the cleanup list, and runs the ping.
 
-Importantly: It is possible to overwrite registered service factories later -- e.g. for testing -- **without monkey-patching**.
-You have to make sure to remove possibly cached instances from the container if you're using nested dependencies (`Container.forget_service_type()`).
+Importantly: It is possible to overwrite registered service factories later -- e.g., for testing -- **without monkey-patching**.
+You have to remove possibly cached instances from the container if you're using nested dependencies (`Container.forget_service_type()`).
 The Flask integration takes care of this for you.
 
+How to achieve this in other frameworks elegantly is TBD.
+
 ---
 
-Generally speaking, the `Registry` object should live on an application-scoped object like Flask's `app.config` object.
+Generally, the `Registry` object should live on an application-scoped object like Flask's `app.config` object.
 On the other hand, the `Container` object should live on a request-scoped object like Flask's `g` object or Pyramid's `request` object.
 
 
 > **Note**
-> The core APIs only use pure object without any global state but also without any comfort.
-> It gets more interesting when using framework-specific integrations where the life-cycle of the Container and thus services is handled automatically.
+> The core APIs only use vanilla objects without any global state but also without any comfort.
+> It gets more interesting when using framework-specific integrations where the life-cycle of the container and, thus, services is handled automatically.
 
 
 ## Flask
 
-*svc-reg* has grown from my frustration of the repetitiveness of using the `get_x` that creates an `x` and then stores it on the `g` object.
+*svc-reg* has grown from my frustration with the repetitiveness of using the `get_x` that creates an `x` and then stores it on the `g` object [pattern](https://flask.palletsprojects.com/en/latest/appcontext/#storing-data).
 
 Therefore it comes with Flask support out of the box in the form of the `svc_reg.flask` module.
+It:
+
+- puts the registry into `app.config["svc_registry"]`,
+- unifies the putting and caching of services on the `g` object by putting a container into `g.svc_container`,
+- transparently retrieves them from there for you,
+- and installs a [`teardown_appcontext()`](http://flask.pocoo.org/docs/latest/api#flask.Flask.teardown_appcontext) handler that calls `close()` on the container when a request is done.
+
+---
 
 You can add support for *svc-reg* by calling `svc_reg.flask.init_app(app)` in your [*application factory*](https://flask.palletsprojects.com/en/latest/patterns/appfactories/).
-For instance to create a factory that uses an SQLAlchemy Engine to create Connections, you could do this:
+For instance, to create a factory that uses a SQLAlchemy engine to produce connections, you could do this:
 
 ```python
 from flask import Flask
 from sqlalchemy import Connection
 from sqlalchemy.sql import text
 
 import svc_reg
@@ -105,37 +153,36 @@
 
 def create_app(config_filename):
     app = Flask(__name__)
     app.config.from_pyfile(config_filename)
 
     ##########################################################################
     # Set up the registry using Flask integration.
-    reg = svc_reg.Registry()
-    app = svc_reg.flask.init_app(app, reg)
-
-    # The registry lives in app.config["svc_registry"] now. If you don't pass it
-    # explicitly, init_app creates one for you.
+    app = svc_reg.flask.init_app(app)
 
     # Now, register a factory that calls `engine.connect()` if you ask for a
     # Connections and `connection.close()` on cleanup.
     # If you ask for a ping, it will run `SELECT 1` on a new connection and
-    # cleanup the connection behind itself.
+    # clean up the connection behind itself.
     engine = create_engine("postgresql://localhost")
     ping = text("SELECT 1")
-    reg.register_factory(
+    svc_reg_flask.register_factory(
+        # The app argument makes it good for custom init_app() functions.
+        app,
         Connection,
         engine.connect,
         cleanup=lambda conn: conn.close(),
         ping=lambda conn: conn.execute(ping)
     )
 
     # You also use svc_reg WITHIN factories:
-    reg.register_factory(
-        unit_of_work.UnitOfWork,
-        lambda: unit_of_work.UnitOfWork.from_connection(
+    svc_reg_flask.register_factory(
+        app, # <---
+        AbstractRepository,
+        lambda: Repository.from_connection(
             svc_reg.flask.get(Connection)
         ),
     )
     ##########################################################################
 
     from yourapplication.views.admin import admin
     from yourapplication.views.frontend import frontend
@@ -145,126 +192,138 @@
     return app
 ```
 
 Now you can request the `Connection` object in your views:
 
 ```python
 @app.route("/")
-def index():
+def index() -> flask.ResponseValue:
     conn: Connection = svc_reg.flask.get(Connection)
 ```
 
-If you have an health endpoint, it could look like this:
+If you have a health endpoint, it could look like this:
 
 ```python
-@bp.get("healthy")
+@app.get("healthy")
 def healthy() -> flask.ResponseValue:
     """
     Ping all external services.
     """
     ok: list[str] = []
     failing: list[dict[str, str]] = []
     code = 200
 
-    for svc in services.get_pings():
+    for svc in svc_reg.flask.get_pings():
         try:
             svc.ping()
             ok.append(svc.name)
         except Exception as e:
             failing.append({svc.name: repr(e)})
             code = 500
 
     return {"ok": ok, "failing": failing}, code
 ```
 
-`init_app()` also installs an `teardown_appcontext()` handler that calls `cleanup()` on the container when a request is done.
-
 
 ### Testing
 
-Now if you want the database to return a mock `Connection`, you can do this:
+Having a central place for all your services, makes it obvious where to mock them for testing.
+So, if you want the connection service to return a mock `Connection`, you can do this:
 
 ```python
 from unittest.mock import Mock
 
 def test_handles_db_failure():
     """
     If the database raises an exception, the endpoint should return a 500.
     """
     app = create_app("test.cfg")
     with app.app_context():
         conn = Mock(spec_set=Connection)
         conn.execute.side_effect = Exception("Database is down!")
 
+        #################################################
         # Overwrite the Connection factory with the Mock.
         # This is all it takes to mock the database.
-        reg_svc.flask.register_value(Connection, conn)
+        reg_svc.flask.replace_value(Connection, conn)
+        #################################################
 
         # Now, the endpoint should return a 500.
         response = app.test_client().get("/")
         assert response.status_code == 500
 ```
 
+> **Note**
+> The `replace_(factory|value)` method *requires* an application context and ensures that if a factory/value has already been created *and cached*, they're removed before the new factory/value is registered.
+>>
+> Possible situations where this can occur are Pytest fixtures where you don't control the order in which they're called.
+
 
 ### Quality of Life
 
-In practice, you can simplify / beautify the code within your views by creating a `services` module that re-exports those Flask helpers.
+In practice, you can simplify/beautify the code within your views by creating a `services` module that re-exports those Flask helpers.
 
 Say this is `app/services.py`:
 
 ```python
 from svc_reg.flask import (
     get,
     get_pings,
     init_app,
     register_factory,
     register_value,
+    replace_factory,
+    replace_value,
 )
 
 
 __all__ = [
     "get_pings",
     "get",
     "init_app",
     "register_factory",
     "register_value",
+    "replace_factory",
+    "replace_value",
 ]
 ```
 
 Now you can register services in your application factory like this:
 
 ```python
-from app import services
+from your_app import services
 
-services.register_factory(Connection, ...)
+def init_app(app):
+    services.register_factory(app, Connection, ...)
+    return app
 ```
 
-And you get them in your views like this::
+And you get them in your views like this:
 
 ```python
-from app import services
+from your_app import services
 
 @app.route("/")
 def index():
     conn: Connection = services.get(Connection)
 ```
 
 🧑‍🍳💋
 
 
 ## Caveats
 
 One would expect the the `Container.get()` method would have a type signature like `get(type: type[T]) -> T`.
-Unfortunately, that's currently impossible, because it [precludes the usage of `Protocols` as service types](https://github.com/python/mypy/issues/4717) which would make the package pointless.
+Unfortunately, that's currently impossible because it [precludes the usage of `Protocols` as service types](https://github.com/python/mypy/issues/4717), making this package pointless.
 
-Therefore it returns `Any` and until Mypy changes its stance, you have to use it like this:
+Therefore it returns `Any`, and until Mypy changes its stance, you have to use it like this:
 
 ```python
 conn: Connection = container.get(Connection)
 ```
 
 
 ## Credits
 
-*stamina* is written by [Hynek Schlawack](https://hynek.me/) and distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+*svc-reg* is written by [Hynek Schlawack](https://hynek.me/) and distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
 
 The development is kindly supported by my employer [Variomedia AG](https://www.variomedia.de/) and all my amazing [GitHub Sponsors](https://github.com/sponsors/hynek).
```

### Comparing `svc_reg-23.1.0/pyproject.toml` & `svc_reg-23.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 [build-system]
-requires = ["hatchling", "hatch-vcs"]
+requires = ["hatchling", "hatch-vcs", "hatch-fancy-pypi-readme"]
 build-backend = "hatchling.build"
 
 
 [project]
-dynamic = ["version"]
-readme = { file = "README.md", content-type = "text/markdown" }
+dynamic = ["version", "readme"]
 name = "svc-reg"
 description = "A Service Registry for Dependency Injection"
 requires-python = ">=3.8"
 license = "MIT"
 keywords = ["dependency injection"]
 authors = [{ name = "Hynek Schlawack", email = "hs@ox.cx" }]
 classifiers = [
@@ -36,14 +35,52 @@
 Funding = "https://github.com/sponsors/hynek"
 
 
 [tool.hatch.version]
 source = "vcs"
 raw-options = { local_scheme = "no-local-version" }
 
+[tool.hatch.metadata.hooks.fancy-pypi-readme]
+content-type = "text/markdown"
+
+[[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
+path = "README.md"
+start-after = "<!-- begin-pypi -->\n"
+end-before = "\n<!-- end-pypi -->"
+
+[[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
+text = """
+
+---
+
+For now, please refer to the [GitHub README](https://github.com/hynek/svc-reg/blob/main/README.md) for latest documentation.
+
+
+## Release Information
+
+"""
+
+[[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
+path = "CHANGELOG.md"
+start-after = "<!-- changelog follows -->"
+pattern = "\n(###.+?\n)## "
+
+[[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
+text = """
+---
+
+[→ Full Changelog](https://github.com/hynek/svc-reg/blob/main/CHANGELOG.md)
+
+
+"""
+
+[[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
+path = "README.md"
+start-at = "## Credits"
+
 
 [tool.pytest.ini_options]
 addopts = ["-ra", "--strict-markers", "--strict-config"]
 xfail_strict = true
 filterwarnings = ["once::Warning"]
 
 
@@ -69,18 +106,16 @@
 
 [tool.mypy]
 strict = true
 
 show_error_codes = true
 enable_error_code = ["ignore-without-code"]
 
-ignore_missing_imports = true
 allow_any_generics = true
 
-
 [[tool.mypy.overrides]]
 module = "tests.*"
 ignore_errors = true
 
 [[tool.mypy.overrides]]
 module = "tests.typing.*"
 ignore_errors = false
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

