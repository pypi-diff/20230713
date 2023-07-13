# Comparing `tmp/kr8s-0.8.5.tar.gz` & `tmp/kr8s-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kr8s-0.8.5.tar", max compression
+gzip compressed data, was "kr8s-0.8.6.tar", max compression
```

## Comparing `kr8s-0.8.5.tar` & `kr8s-0.8.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1549 2023-07-13 09:34:07.417851 kr8s-0.8.5/LICENSE
--rw-r--r--   0        0        0     2587 2023-07-13 09:34:07.417851 kr8s-0.8.5/README.md
--rw-r--r--   0        0        0     1143 2023-07-13 09:34:35.938589 kr8s-0.8.5/kr8s/__init__.py
--rw-r--r--   0        0        0    14674 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/_api.py
--rw-r--r--   0        0        0     5879 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/_auth.py
--rw-r--r--   0        0        0     1920 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/_data_utils.py
--rw-r--r--   0        0        0      163 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/_exceptions.py
--rw-r--r--   0        0        0     4336 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/_io.py
--rw-r--r--   0        0        0    34939 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/_objects.py
--rw-r--r--   0        0        0     8074 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/_portforward.py
--rw-r--r--   0        0        0      680 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/_testutils.py
--rw-r--r--   0        0        0      248 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/asyncio/__init__.py
--rw-r--r--   0        0        0     1110 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/asyncio/_api.py
--rw-r--r--   0        0        0     1681 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/asyncio/_helpers.py
--rw-r--r--   0        0        0      827 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/asyncio/objects.py
--rw-r--r--   0        0        0      168 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/asyncio/portforward.py
--rw-r--r--   0        0        0     5503 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/conftest.py
--rw-r--r--   0        0        0     6001 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/objects.py
--rw-r--r--   0        0        0      152 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/portforward.py
--rw-r--r--   0        0        0       78 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/tests/resources/custom/evc.yaml
--rw-r--r--   0        0        0       61 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/tests/resources/serviceaccount.yaml
--rw-r--r--   0        0        0      369 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/tests/resources/simple/nested/nginx_ingress.yaml
--rw-r--r--   0        0        0      144 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/tests/resources/simple/nginx_pod.yaml
--rw-r--r--   0        0        0      435 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/tests/resources/simple/nginx_pod_service.yaml
--rwxr-xr-x   0        0        0      614 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/tests/scripts/envexec.py
--rw-r--r--   0        0        0     5909 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/tests/test_api.py
--rw-r--r--   0        0        0     3394 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/tests/test_auth.py
--rw-r--r--   0        0        0      824 2023-07-13 09:34:07.441851 kr8s-0.8.5/kr8s/tests/test_data_utils.py
--rw-r--r--   0        0        0     1710 2023-07-13 09:34:07.441851 kr8s-0.8.5/kr8s/tests/test_io.py
--rw-r--r--   0        0        0    18224 2023-07-13 09:34:07.441851 kr8s-0.8.5/kr8s/tests/test_objects.py
--rw-r--r--   0        0        0      622 2023-07-13 09:34:07.441851 kr8s-0.8.5/kr8s/tests/test_testutils.py
--rw-r--r--   0        0        0     2578 2023-07-13 09:34:35.938589 kr8s-0.8.5/pyproject.toml
--rw-r--r--   0        0        0     3366 1970-01-01 00:00:00.000000 kr8s-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0     1549 2023-07-13 15:15:48.461707 kr8s-0.8.6/LICENSE
+-rw-r--r--   0        0        0     2587 2023-07-13 15:15:48.461707 kr8s-0.8.6/README.md
+-rw-r--r--   0        0        0     1143 2023-07-13 15:16:17.577447 kr8s-0.8.6/kr8s/__init__.py
+-rw-r--r--   0        0        0    14674 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/_api.py
+-rw-r--r--   0        0        0     5879 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/_auth.py
+-rw-r--r--   0        0        0     1920 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/_data_utils.py
+-rw-r--r--   0        0        0      163 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/_exceptions.py
+-rw-r--r--   0        0        0     4336 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/_io.py
+-rw-r--r--   0        0        0    36589 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/_objects.py
+-rw-r--r--   0        0        0     8074 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/_portforward.py
+-rw-r--r--   0        0        0      680 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/_testutils.py
+-rw-r--r--   0        0        0      248 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/asyncio/__init__.py
+-rw-r--r--   0        0        0     1110 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/asyncio/_api.py
+-rw-r--r--   0        0        0     1681 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/asyncio/_helpers.py
+-rw-r--r--   0        0        0      827 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/asyncio/objects.py
+-rw-r--r--   0        0        0      168 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/asyncio/portforward.py
+-rw-r--r--   0        0        0     5503 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/conftest.py
+-rw-r--r--   0        0        0     6001 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/objects.py
+-rw-r--r--   0        0        0      152 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/portforward.py
+-rw-r--r--   0        0        0       78 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/tests/resources/custom/evc.yaml
+-rw-r--r--   0        0        0       61 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/tests/resources/serviceaccount.yaml
+-rw-r--r--   0        0        0      369 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/tests/resources/simple/nested/nginx_ingress.yaml
+-rw-r--r--   0        0        0      144 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/tests/resources/simple/nginx_pod.yaml
+-rw-r--r--   0        0        0      435 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/tests/resources/simple/nginx_pod_service.yaml
+-rwxr-xr-x   0        0        0      614 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/tests/scripts/envexec.py
+-rw-r--r--   0        0        0     5909 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/tests/test_api.py
+-rw-r--r--   0        0        0     3394 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/tests/test_auth.py
+-rw-r--r--   0        0        0      824 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/tests/test_data_utils.py
+-rw-r--r--   0        0        0     1710 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/tests/test_io.py
+-rw-r--r--   0        0        0    21028 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/tests/test_objects.py
+-rw-r--r--   0        0        0      622 2023-07-13 15:15:48.485708 kr8s-0.8.6/kr8s/tests/test_testutils.py
+-rw-r--r--   0        0        0     2676 2023-07-13 15:16:17.577447 kr8s-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0     3366 1970-01-01 00:00:00.000000 kr8s-0.8.6/PKG-INFO
```

### Comparing `kr8s-0.8.5/LICENSE` & `kr8s-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.5/README.md` & `kr8s-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.5/kr8s/__init__.py` & `kr8s-0.8.6/kr8s/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from .asyncio import (
     version as _version,
 )
 from .asyncio import (
     watch as _watch,
 )
 
-__version__ = "0.8.5"
+__version__ = "0.8.6"
 
 
 @_sync
 class Api(_AsyncApi):
     __doc__ = _AsyncApi.__doc__
```

### Comparing `kr8s-0.8.5/kr8s/_api.py` & `kr8s-0.8.6/kr8s/_api.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.5/kr8s/_auth.py` & `kr8s-0.8.6/kr8s/_auth.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.5/kr8s/_data_utils.py` & `kr8s-0.8.6/kr8s/_data_utils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.5/kr8s/_io.py` & `kr8s-0.8.6/kr8s/_io.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.5/kr8s/_objects.py` & `kr8s-0.8.6/kr8s/_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023, Dask Developers, Yuvi Panda, Anaconda Inc, NVIDIA
 # SPDX-License-Identifier: BSD 3-Clause License
 from __future__ import annotations
 
 import asyncio
+import contextlib
 import json
 import pathlib
 import re
 import time
 from typing import Any, Dict, List, Optional, Type, Union
 
 import anyio
@@ -32,21 +33,28 @@
     namespaced = False
     scalable = False
     scalable_spec = "replicas"
     _asyncio = True
 
     def __init__(self, resource: dict, namespace: str = None, api: Api = None) -> None:
         """Initialize an APIObject."""
-        # TODO support passing pykube or kubernetes objects in addition to dicts
+        with contextlib.suppress(TypeError, ValueError):
+            resource = dict(resource)
         if isinstance(resource, str):
             self._raw = {"metadata": {"name": resource}}
         elif isinstance(resource, dict):
             self._raw = resource
+        elif hasattr(resource, "to_dict"):
+            self._raw = resource.to_dict()
+        elif hasattr(resource, "obj"):
+            self._raw = resource.obj
         else:
-            raise ValueError("resource must be a dict or a string")
+            raise ValueError(
+                "resource must be a dict, string, have an obj attribute or a to_dict method"
+            )
         if namespace is not None:
             self._raw["metadata"]["namespace"] = namespace
         self.api = api
         if self.api is None and not self._asyncio:
             self.api = kr8s.api()
 
     def __await__(self):
@@ -423,14 +431,56 @@
             >>> deployment = Deployment.get("my-deployment")
             >>> pod = Pod.get("my-pod")
             >>> deployment.adopt(pod)
 
         """
         await child._set_owner(self)
 
+    def to_lightkube(self) -> Any:
+        """Return a lightkube representation of this object."""
+        try:
+            from lightkube import codecs
+        except ImportError:
+            raise ImportError("lightkube is not installed")
+        return codecs.from_dict(self.raw)
+
+    def to_pykube(self, api) -> Any:
+        """Return a pykube representation of this object.
+
+        Args:
+            api: A pykube API object.
+
+        Example:
+            >>> from kr8s.objects import Deployment
+            >>> deployment = Deployment.get("my-deployment")
+            >>> # Create a pykube API object
+            >>> from pykube import HTTPClient
+            >>> api = HTTPClient()
+            >>> pykube_deployment = deployment.to_pykube(api)
+
+        """
+        try:
+            import pykube
+        except ImportError:
+            raise ImportError("pykube is not installed")
+        try:
+            pykube_cls = getattr(pykube.objects, self.kind)
+        except AttributeError:
+            base = (
+                pykube.objects.NamespacedAPIObject
+                if self.namespaced
+                else pykube.objects.APIObject
+            )
+            pykube_cls = type(
+                self.kind,
+                (base,),
+                {"version": self.version, "endpoint": self.endpoint, "kind": self.kind},
+            )
+        return pykube_cls(api, self.raw)
+
 
 ## v1 objects
 
 
 class Binding(APIObject):
     """A Kubernetes Binding."""
```

### Comparing `kr8s-0.8.5/kr8s/_portforward.py` & `kr8s-0.8.6/kr8s/_portforward.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.5/kr8s/_testutils.py` & `kr8s-0.8.6/kr8s/_testutils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.5/kr8s/asyncio/_api.py` & `kr8s-0.8.6/kr8s/asyncio/_api.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.5/kr8s/asyncio/_helpers.py` & `kr8s-0.8.6/kr8s/asyncio/_helpers.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.5/kr8s/asyncio/objects.py` & `kr8s-0.8.6/kr8s/asyncio/objects.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.5/kr8s/conftest.py` & `kr8s-0.8.6/kr8s/conftest.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.5/kr8s/objects.py` & `kr8s-0.8.6/kr8s/objects.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.5/kr8s/tests/scripts/envexec.py` & `kr8s-0.8.6/kr8s/tests/scripts/envexec.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.5/kr8s/tests/test_api.py` & `kr8s-0.8.6/kr8s/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.5/kr8s/tests/test_auth.py` & `kr8s-0.8.6/kr8s/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.5/kr8s/tests/test_data_utils.py` & `kr8s-0.8.6/kr8s/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.5/kr8s/tests/test_io.py` & `kr8s-0.8.6/kr8s/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.5/kr8s/tests/test_objects.py` & `kr8s-0.8.6/kr8s/tests/test_objects.py`

 * *Files 5% similar despite different names*

```diff
@@ -586,7 +586,81 @@
     [nginx_pod, *_] = await nginx_service.ready_pods()
     await nginx_service.adopt(nginx_pod)
     assert "ownerReferences" in nginx_pod.metadata
     assert nginx_pod.metadata["ownerReferences"][0]["name"] == nginx_service.name
     await nginx_service.delete()
     while await nginx_pod.exists():
         await asyncio.sleep(0.1)
+
+
+async def test_cast_to_from_lightkube(example_pod_spec):
+    pytest.importorskip("lightkube")
+    from lightkube import codecs
+    from lightkube.resources.core_v1 import Pod as LightkubePod
+
+    starting_pod = codecs.from_dict(example_pod_spec)
+
+    kr8s_pod = await Pod(starting_pod)
+    assert isinstance(kr8s_pod, Pod)
+    assert kr8s_pod.name == example_pod_spec["metadata"]["name"]
+    assert kr8s_pod.namespace == example_pod_spec["metadata"]["namespace"]
+    assert kr8s_pod.kind == "Pod"
+    assert kr8s_pod.version == "v1"
+
+    lightkube_pod = kr8s_pod.to_lightkube()
+    assert isinstance(lightkube_pod, LightkubePod)
+    assert lightkube_pod.metadata.name == example_pod_spec["metadata"]["name"]
+    assert lightkube_pod.metadata.namespace == example_pod_spec["metadata"]["namespace"]
+
+
+async def test_cast_to_from_kubernetes(example_pod_spec):
+    kubernetes = pytest.importorskip("kubernetes")
+
+    starting_pod = kubernetes.client.models.v1_pod.V1Pod(
+        api_version=example_pod_spec["apiVersion"],
+        kind=example_pod_spec["kind"],
+        metadata=example_pod_spec["metadata"],
+        spec=example_pod_spec["spec"],
+    )
+
+    kr8s_pod = await Pod(starting_pod)
+    assert isinstance(kr8s_pod, Pod)
+    assert kr8s_pod.name == example_pod_spec["metadata"]["name"]
+    assert kr8s_pod.namespace == example_pod_spec["metadata"]["namespace"]
+    assert kr8s_pod.kind == "Pod"
+    assert kr8s_pod.version == "v1"
+
+
+async def test_cast_to_from_kubernetes_asyncio(example_pod_spec):
+    kubernetes_asyncio = pytest.importorskip("kubernetes_asyncio")
+
+    starting_pod = kubernetes_asyncio.client.models.v1_pod.V1Pod(
+        api_version=example_pod_spec["apiVersion"],
+        kind=example_pod_spec["kind"],
+        metadata=example_pod_spec["metadata"],
+        spec=example_pod_spec["spec"],
+    )
+
+    kr8s_pod = await Pod(starting_pod)
+    assert isinstance(kr8s_pod, Pod)
+    assert kr8s_pod.name == example_pod_spec["metadata"]["name"]
+    assert kr8s_pod.namespace == example_pod_spec["metadata"]["namespace"]
+    assert kr8s_pod.kind == "Pod"
+    assert kr8s_pod.version == "v1"
+
+
+async def test_cast_to_from_pykube_ng(example_pod_spec):
+    pykube = pytest.importorskip("pykube")
+
+    starting_pod = pykube.objects.Pod(None, example_pod_spec)
+
+    kr8s_pod = await Pod(starting_pod)
+    assert isinstance(kr8s_pod, Pod)
+    assert kr8s_pod.name == example_pod_spec["metadata"]["name"]
+    assert kr8s_pod.namespace == example_pod_spec["metadata"]["namespace"]
+    assert kr8s_pod.kind == "Pod"
+    assert kr8s_pod.version == "v1"
+
+    pykube_pod = kr8s_pod.to_pykube(None)
+    assert isinstance(pykube_pod, pykube.objects.Pod)
+    assert pykube_pod.name == example_pod_spec["metadata"]["name"]
+    assert pykube_pod.namespace == example_pod_spec["metadata"]["namespace"]
```

### Comparing `kr8s-0.8.5/kr8s/tests/test_testutils.py` & `kr8s-0.8.6/kr8s/tests/test_testutils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.5/pyproject.toml` & `kr8s-0.8.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "aiohttp",
     'importlib-metadata; python_version<"3.8"',
 ]
 dynamic = ["version"]
 
 [tool.poetry]
 name = "kr8s"
-version = "0.8.5"  # This will be populated at build time by poetry-dynamic-versioning
+version = "0.8.6"  # This will be populated at build time by poetry-dynamic-versioning
 description = "A Kubernetes API library"
 authors = ["Jacob Tomlinson <jacob@tomlinson.email>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 
 [tool.poetry-dynamic-versioning]
 enable = true
@@ -46,14 +46,18 @@
 pytest = "^7.2.2"
 pytest-asyncio = "^0.20.3"
 pytest-kind = {git = "https://codeberg.org/hjacobs/pytest-kind.git"}
 pytest-timeout = "^2.1.0"
 pytest-rerunfailures = "^11.1.2"
 pytest-cov = "^4.0.0"
 trio = "^0.22.0"
+lightkube = "^0.13.0"
+kubernetes = "^26.1.0"
+pykube-ng = "^23.6.0"
+kubernetes-asyncio = "^24.2.3"
 
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^5.3.0"
 sphinx-autobuild = "^2021.3.14"
 myst-parser = "^1.0.0"
 furo = "^2023.3.27"
```

### Comparing `kr8s-0.8.5/PKG-INFO` & `kr8s-0.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kr8s
-Version: 0.8.5
+Version: 0.8.6
 Summary: A Kubernetes API library
 License: BSD-3-Clause
 Author: Jacob Tomlinson
 Author-email: jacob@tomlinson.email
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

