# Comparing `tmp/kr8s-0.8.4.tar.gz` & `tmp/kr8s-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kr8s-0.8.4.tar", max compression
+gzip compressed data, was "kr8s-0.8.5.tar", max compression
```

## Comparing `kr8s-0.8.4.tar` & `kr8s-0.8.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1549 2023-07-11 16:29:57.052792 kr8s-0.8.4/LICENSE
--rw-r--r--   0        0        0     2587 2023-07-11 16:29:57.052792 kr8s-0.8.4/README.md
--rw-r--r--   0        0        0     1143 2023-07-11 16:30:26.706629 kr8s-0.8.4/kr8s/__init__.py
--rw-r--r--   0        0        0    14674 2023-07-11 16:29:57.072793 kr8s-0.8.4/kr8s/_api.py
--rw-r--r--   0        0        0     5879 2023-07-11 16:29:57.072793 kr8s-0.8.4/kr8s/_auth.py
--rw-r--r--   0        0        0     1920 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/_data_utils.py
--rw-r--r--   0        0        0      163 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/_exceptions.py
--rw-r--r--   0        0        0     4336 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/_io.py
--rw-r--r--   0        0        0    33161 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/_objects.py
--rw-r--r--   0        0        0     8074 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/_portforward.py
--rw-r--r--   0        0        0      680 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/_testutils.py
--rw-r--r--   0        0        0      248 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/asyncio/__init__.py
--rw-r--r--   0        0        0     1110 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/asyncio/_api.py
--rw-r--r--   0        0        0     1681 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/asyncio/_helpers.py
--rw-r--r--   0        0        0      827 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/asyncio/objects.py
--rw-r--r--   0        0        0      168 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/asyncio/portforward.py
--rw-r--r--   0        0        0     5503 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/conftest.py
--rw-r--r--   0        0        0     6001 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/objects.py
--rw-r--r--   0        0        0      152 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/portforward.py
--rw-r--r--   0        0        0       78 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/tests/resources/custom/evc.yaml
--rw-r--r--   0        0        0       61 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/tests/resources/serviceaccount.yaml
--rw-r--r--   0        0        0      369 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/tests/resources/simple/nested/nginx_ingress.yaml
--rw-r--r--   0        0        0      144 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/tests/resources/simple/nginx_pod.yaml
--rw-r--r--   0        0        0      435 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/tests/resources/simple/nginx_pod_service.yaml
--rwxr-xr-x   0        0        0      614 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/tests/scripts/envexec.py
--rw-r--r--   0        0        0     5909 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/tests/test_api.py
--rw-r--r--   0        0        0     3394 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/tests/test_auth.py
--rw-r--r--   0        0        0      824 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/tests/test_data_utils.py
--rw-r--r--   0        0        0     1710 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/tests/test_io.py
--rw-r--r--   0        0        0    17737 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/tests/test_objects.py
--rw-r--r--   0        0        0      622 2023-07-11 16:29:57.076794 kr8s-0.8.4/kr8s/tests/test_testutils.py
--rw-r--r--   0        0        0     2578 2023-07-11 16:30:26.706629 kr8s-0.8.4/pyproject.toml
--rw-r--r--   0        0        0     3366 1970-01-01 00:00:00.000000 kr8s-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1549 2023-07-13 09:34:07.417851 kr8s-0.8.5/LICENSE
+-rw-r--r--   0        0        0     2587 2023-07-13 09:34:07.417851 kr8s-0.8.5/README.md
+-rw-r--r--   0        0        0     1143 2023-07-13 09:34:35.938589 kr8s-0.8.5/kr8s/__init__.py
+-rw-r--r--   0        0        0    14674 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/_api.py
+-rw-r--r--   0        0        0     5879 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/_auth.py
+-rw-r--r--   0        0        0     1920 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/_data_utils.py
+-rw-r--r--   0        0        0      163 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/_exceptions.py
+-rw-r--r--   0        0        0     4336 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/_io.py
+-rw-r--r--   0        0        0    34939 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/_objects.py
+-rw-r--r--   0        0        0     8074 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/_portforward.py
+-rw-r--r--   0        0        0      680 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/_testutils.py
+-rw-r--r--   0        0        0      248 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/asyncio/__init__.py
+-rw-r--r--   0        0        0     1110 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/asyncio/_api.py
+-rw-r--r--   0        0        0     1681 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/asyncio/_helpers.py
+-rw-r--r--   0        0        0      827 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/asyncio/objects.py
+-rw-r--r--   0        0        0      168 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/asyncio/portforward.py
+-rw-r--r--   0        0        0     5503 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/conftest.py
+-rw-r--r--   0        0        0     6001 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/objects.py
+-rw-r--r--   0        0        0      152 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/portforward.py
+-rw-r--r--   0        0        0       78 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/tests/resources/custom/evc.yaml
+-rw-r--r--   0        0        0       61 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/tests/resources/serviceaccount.yaml
+-rw-r--r--   0        0        0      369 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/tests/resources/simple/nested/nginx_ingress.yaml
+-rw-r--r--   0        0        0      144 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/tests/resources/simple/nginx_pod.yaml
+-rw-r--r--   0        0        0      435 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/tests/resources/simple/nginx_pod_service.yaml
+-rwxr-xr-x   0        0        0      614 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/tests/scripts/envexec.py
+-rw-r--r--   0        0        0     5909 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/tests/test_api.py
+-rw-r--r--   0        0        0     3394 2023-07-13 09:34:07.437851 kr8s-0.8.5/kr8s/tests/test_auth.py
+-rw-r--r--   0        0        0      824 2023-07-13 09:34:07.441851 kr8s-0.8.5/kr8s/tests/test_data_utils.py
+-rw-r--r--   0        0        0     1710 2023-07-13 09:34:07.441851 kr8s-0.8.5/kr8s/tests/test_io.py
+-rw-r--r--   0        0        0    18224 2023-07-13 09:34:07.441851 kr8s-0.8.5/kr8s/tests/test_objects.py
+-rw-r--r--   0        0        0      622 2023-07-13 09:34:07.441851 kr8s-0.8.5/kr8s/tests/test_testutils.py
+-rw-r--r--   0        0        0     2578 2023-07-13 09:34:35.938589 kr8s-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0     3366 1970-01-01 00:00:00.000000 kr8s-0.8.5/PKG-INFO
```

### Comparing `kr8s-0.8.4/LICENSE` & `kr8s-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.4/README.md` & `kr8s-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.4/kr8s/__init__.py` & `kr8s-0.8.5/kr8s/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from .asyncio import (
     version as _version,
 )
 from .asyncio import (
     watch as _watch,
 )
 
-__version__ = "0.8.4"
+__version__ = "0.8.5"
 
 
 @_sync
 class Api(_AsyncApi):
     __doc__ = _AsyncApi.__doc__
```

### Comparing `kr8s-0.8.4/kr8s/_api.py` & `kr8s-0.8.5/kr8s/_api.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.4/kr8s/_auth.py` & `kr8s-0.8.5/kr8s/_auth.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.4/kr8s/_data_utils.py` & `kr8s-0.8.5/kr8s/_data_utils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.4/kr8s/_io.py` & `kr8s-0.8.5/kr8s/_io.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.4/kr8s/_objects.py` & `kr8s-0.8.5/kr8s/_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -369,14 +369,68 @@
         """Return the keys of this object."""
         return self.raw.keys()
 
     def __getitem__(self, key: str) -> Any:
         """Get an item from this object."""
         return self.raw[key]
 
+    async def set_owner(self, owner: APIObject) -> None:
+        """Set the owner reference of this object.
+
+        See https://kubernetes.io/docs/concepts/overview/working-with-objects/owners-dependents/
+
+        Args:
+            owner: The owner object to set a reference to.
+
+        Example:
+            >>> from kr8s.objects import Deployment, Pod
+            >>> deployment = Deployment.get("my-deployment")
+            >>> pod = Pod.get("my-pod")
+            >>> pod.set_owner(deployment)
+        """
+        await self._set_owner(owner)
+
+    async def _set_owner(self, owner: APIObject) -> None:
+        """Set the owner of this object."""
+        await self._patch(
+            {
+                "metadata": {
+                    "ownerReferences": [
+                        {
+                            "controller": True,
+                            "blockOwnerDeletion": True,
+                            "apiVersion": owner.version,
+                            "kind": owner.kind,
+                            "name": owner.name,
+                            "uid": owner.metadata.uid,
+                        }
+                    ],
+                }
+            }
+        )
+
+    async def adopt(self, child: APIObject) -> None:
+        """Adopt this object.
+
+        This will set the owner reference of the child object to this object.
+
+        See https://kubernetes.io/docs/concepts/overview/working-with-objects/owners-dependents/
+
+        Args:
+            child: The child object to adopt.
+
+        Example:
+            >>> from kr8s.objects import Deployment, Pod
+            >>> deployment = Deployment.get("my-deployment")
+            >>> pod = Pod.get("my-pod")
+            >>> deployment.adopt(pod)
+
+        """
+        await child._set_owner(self)
+
 
 ## v1 objects
 
 
 class Binding(APIObject):
     """A Kubernetes Binding."""
```

### Comparing `kr8s-0.8.4/kr8s/_portforward.py` & `kr8s-0.8.5/kr8s/_portforward.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.4/kr8s/_testutils.py` & `kr8s-0.8.5/kr8s/_testutils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.4/kr8s/asyncio/_api.py` & `kr8s-0.8.5/kr8s/asyncio/_api.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.4/kr8s/asyncio/_helpers.py` & `kr8s-0.8.5/kr8s/asyncio/_helpers.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.4/kr8s/asyncio/objects.py` & `kr8s-0.8.5/kr8s/asyncio/objects.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.4/kr8s/conftest.py` & `kr8s-0.8.5/kr8s/conftest.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.4/kr8s/objects.py` & `kr8s-0.8.5/kr8s/objects.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.4/kr8s/tests/scripts/envexec.py` & `kr8s-0.8.5/kr8s/tests/scripts/envexec.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.4/kr8s/tests/test_api.py` & `kr8s-0.8.5/kr8s/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.4/kr8s/tests/test_auth.py` & `kr8s-0.8.5/kr8s/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.4/kr8s/tests/test_data_utils.py` & `kr8s-0.8.5/kr8s/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.4/kr8s/tests/test_io.py` & `kr8s-0.8.5/kr8s/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.4/kr8s/tests/test_objects.py` & `kr8s-0.8.5/kr8s/tests/test_objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,27 +55,33 @@
         "dd",
         "if=/dev/random",
         "of=/usr/share/nginx/html/foo.dat",
         "bs=4M",
         "count=10",
     )
     yield pod
-    await pod.delete()
+    try:
+        await pod.delete()
+    except kr8s.NotFoundError:
+        pass
 
 
 @pytest.fixture
 async def nginx_service(example_service_spec, nginx_pod):
     example_service_spec["metadata"]["name"] = nginx_pod.name
     example_service_spec["spec"]["selector"] = nginx_pod.labels
     service = await Service(example_service_spec)
     await service.create()
     while not await service.ready():
         await asyncio.sleep(0.1)  # pragma: no cover
     yield service
-    await service.delete()
+    try:
+        await service.delete()
+    except kr8s.NotFoundError:
+        pass
 
 
 async def test_pod_create_and_delete(example_pod_spec):
     pod = await Pod(example_pod_spec)
     await pod.create()
     with pytest.raises(NotImplementedError):
         pod.replicas
@@ -570,7 +576,17 @@
     assert len(objects) == 1
 
 
 async def test_pod_to_dict(example_pod_spec):
     pod = Pod(example_pod_spec)
     assert dict(pod) == example_pod_spec
     assert dict(pod) == pod.raw
+
+
+async def test_adoption(nginx_service):
+    [nginx_pod, *_] = await nginx_service.ready_pods()
+    await nginx_service.adopt(nginx_pod)
+    assert "ownerReferences" in nginx_pod.metadata
+    assert nginx_pod.metadata["ownerReferences"][0]["name"] == nginx_service.name
+    await nginx_service.delete()
+    while await nginx_pod.exists():
+        await asyncio.sleep(0.1)
```

### Comparing `kr8s-0.8.4/kr8s/tests/test_testutils.py` & `kr8s-0.8.5/kr8s/tests/test_testutils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.8.4/pyproject.toml` & `kr8s-0.8.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "aiohttp",
     'importlib-metadata; python_version<"3.8"',
 ]
 dynamic = ["version"]
 
 [tool.poetry]
 name = "kr8s"
-version = "0.8.4"  # This will be populated at build time by poetry-dynamic-versioning
+version = "0.8.5"  # This will be populated at build time by poetry-dynamic-versioning
 description = "A Kubernetes API library"
 authors = ["Jacob Tomlinson <jacob@tomlinson.email>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 
 [tool.poetry-dynamic-versioning]
 enable = true
```

### Comparing `kr8s-0.8.4/PKG-INFO` & `kr8s-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kr8s
-Version: 0.8.4
+Version: 0.8.5
 Summary: A Kubernetes API library
 License: BSD-3-Clause
 Author: Jacob Tomlinson
 Author-email: jacob@tomlinson.email
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

