# Comparing `tmp/coregio-0.5.0.tar.gz` & `tmp/coregio-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coregio-0.5.0.tar", last modified: Fri Jun  9 15:23:17 2023, max compression
+gzip compressed data, was "coregio-0.5.1.tar", last modified: Thu Jul 13 08:32:32 2023, max compression
```

## Comparing `coregio-0.5.0.tar` & `coregio-0.5.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:23:17.819536 coregio-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-09 15:23:07.000000 coregio-0.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-06-09 15:23:17.819536 coregio-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-06-09 15:23:07.000000 coregio-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:23:17.819536 coregio-0.5.0/coregio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 15:23:07.000000 coregio-0.5.0/coregio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-06-09 15:23:07.000000 coregio-0.5.0/coregio/registry_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-06-09 15:23:07.000000 coregio-0.5.0/coregio/registry_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-09 15:23:07.000000 coregio-0.5.0/coregio/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:23:17.819536 coregio-0.5.0/coregio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-06-09 15:23:17.000000 coregio-0.5.0/coregio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-09 15:23:17.000000 coregio-0.5.0/coregio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 15:23:17.000000 coregio-0.5.0/coregio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-09 15:23:17.000000 coregio-0.5.0/coregio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 15:23:17.000000 coregio-0.5.0/coregio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-09 15:23:07.000000 coregio-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 15:23:17.819536 coregio-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:23:17.819536 coregio-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-06-09 15:23:07.000000 coregio-0.5.0/tests/test_registry_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-06-09 15:23:07.000000 coregio-0.5.0/tests/test_registry_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-09 15:23:07.000000 coregio-0.5.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:32:32.416153 coregio-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-13 08:32:24.000000 coregio-0.5.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-07-13 08:32:32.416153 coregio-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-07-13 08:32:24.000000 coregio-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:32:32.412153 coregio-0.5.1/coregio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:32:24.000000 coregio-0.5.1/coregio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-07-13 08:32:24.000000 coregio-0.5.1/coregio/registry_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-13 08:32:24.000000 coregio-0.5.1/coregio/registry_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-13 08:32:24.000000 coregio-0.5.1/coregio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:32:32.416153 coregio-0.5.1/coregio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-07-13 08:32:32.000000 coregio-0.5.1/coregio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-13 08:32:32.000000 coregio-0.5.1/coregio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 08:32:32.000000 coregio-0.5.1/coregio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-13 08:32:32.000000 coregio-0.5.1/coregio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 08:32:32.000000 coregio-0.5.1/coregio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-13 08:32:24.000000 coregio-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 08:32:32.416153 coregio-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:32:32.416153 coregio-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-07-13 08:32:24.000000 coregio-0.5.1/tests/test_registry_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-07-13 08:32:24.000000 coregio-0.5.1/tests/test_registry_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-13 08:32:24.000000 coregio-0.5.1/tests/test_utils.py
```

### Comparing `coregio-0.5.0/LICENSE.txt` & `coregio-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coregio-0.5.0/PKG-INFO` & `coregio-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coregio
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python container registry API library.
 Author-email: Ales Raszka <araszka@redhat.com>
 License: Copyright (c) 2023 Ales Raszka
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -90,14 +90,15 @@
     manifest_types=["oci_index"]
 )
 print(manifest)
 {'schemaVersion': 2, 'mediaType': 'application/vnd.docker.distribution.manifest.list.v2+json', 'manifests': [{'mediaType': 'application/vnd.docker.distribution.manifest.v2+json', 'size': 595, 'digest': 'sha256:1b2da31e89c8efe8d67f726f9872ca2fce95ddb1d5d97fd71468d5c48de85ddf', 'platform': {'architecture': 'amd64', 'os': 'linux'}}, {'mediaType': 'application/vnd.docker.distribution.manifest.v2+json', 'size': 595, 'digest': 'sha256:18ef5a4eb0a00e0513c8d4fb87bc31728e4c7ed6caea83c608c5048418b00185', 'platform': {'architecture': 'ppc64le', 'os': 'linux'}}, {'mediaType': 'application/vnd.docker.distribution.manifest.v2+json', 'size': 595, 'digest': 'sha256:c3e79af3edaf3b05282565c0b3e08e5b189e4200153114475256d00367da09da', 'platform': {'architecture': 's390x', 'os': 'linux'}}, {'mediaType': 'application/vnd.docker.distribution.manifest.v2+json', 'size': 595, 'digest': 'sha256:7da24517de68a4af11f098841d10c2e02f12619c662e5b812bff7959e2a477a6', 'platform': {'architecture': 'arm64', 'os': 'linux'}}]}
 
 ```
 
+
 ```python
 # Using a proxy
 registry = ContainerRegistry(
     "quay.io",
     proxy="http://proxy.example.com"
 )
```

### Comparing `coregio-0.5.0/README.md` & `coregio-0.5.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     manifest_types=["oci_index"]
 )
 print(manifest)
 {'schemaVersion': 2, 'mediaType': 'application/vnd.docker.distribution.manifest.list.v2+json', 'manifests': [{'mediaType': 'application/vnd.docker.distribution.manifest.v2+json', 'size': 595, 'digest': 'sha256:1b2da31e89c8efe8d67f726f9872ca2fce95ddb1d5d97fd71468d5c48de85ddf', 'platform': {'architecture': 'amd64', 'os': 'linux'}}, {'mediaType': 'application/vnd.docker.distribution.manifest.v2+json', 'size': 595, 'digest': 'sha256:18ef5a4eb0a00e0513c8d4fb87bc31728e4c7ed6caea83c608c5048418b00185', 'platform': {'architecture': 'ppc64le', 'os': 'linux'}}, {'mediaType': 'application/vnd.docker.distribution.manifest.v2+json', 'size': 595, 'digest': 'sha256:c3e79af3edaf3b05282565c0b3e08e5b189e4200153114475256d00367da09da', 'platform': {'architecture': 's390x', 'os': 'linux'}}, {'mediaType': 'application/vnd.docker.distribution.manifest.v2+json', 'size': 595, 'digest': 'sha256:7da24517de68a4af11f098841d10c2e02f12619c662e5b812bff7959e2a477a6', 'platform': {'architecture': 'arm64', 'os': 'linux'}}]}
 
 ```
 
+
 ```python
 # Using a proxy
 registry = ContainerRegistry(
     "quay.io",
     proxy="http://proxy.example.com"
 )
```

### Comparing `coregio-0.5.0/coregio/registry_api.py` & `coregio-0.5.1/coregio/registry_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -289,14 +289,38 @@
             if not next_page:
                 break
             if limit != 0 and len(data) >= limit:
                 break
 
         return data[:limit] if limit else data
 
+    def get_manifest_raw(
+        self, repository: str, reference: str, manifest_types: Any = None
+    ) -> Any:
+        """
+        Get manifest raw response in a repository by a reference
+        (manifest digest or tag).
+
+        Args:
+            repository (str): Repository name
+            reference (str): Manifest digest or tag
+            manifest_types (Optional, List[str]): What type of manifest
+                to get, i.e. index, manifest, ...
+
+        Returns:
+            Any: Manifest raw http response object
+        """
+        if not manifest_types:
+            manifest_types = ["docker_manifest_v2", "oci_manifest"]
+
+        accept_header = ", ".join([ACCEPT_HEADERS[type] for type in manifest_types])
+        headers = {"Accept": accept_header}
+        uri = f"v2/{repository}/manifests/{reference}"
+        return self.get_request(uri, headers=headers)
+
     def get_manifest(
         self,
         repository: str,
         reference: str,
         manifest_types: Any = None,
         is_headers: bool = False,
     ) -> Any:
@@ -310,21 +334,15 @@
                 to get, i.e. index, manifest, ...
             is_headers (bool): Indicates if headers need to be returned or response data
 
         Returns:
             dict: Manifest in the given repository or headers of the response
                 (depends on value of is_headers parameter)
         """
-        if not manifest_types:
-            manifest_types = ["docker_manifest_v2", "oci_manifest"]
-
-        accept_header = ", ".join([ACCEPT_HEADERS[type] for type in manifest_types])
-        headers = {"Accept": accept_header}
-        uri = f"v2/{repository}/manifests/{reference}"
-        rsp = self.get_request(uri, headers=headers)
+        rsp = self.get_manifest_raw(repository, reference, manifest_types)
         if is_headers:
             return rsp.headers
         return rsp.json()
 
     def get_manifest_headers(self, repository: str, reference: str) -> Any:
         """
         Get manifest headers in a repository by a reference (manifest digest or tag).
```

### Comparing `coregio-0.5.0/coregio/registry_auth.py` & `coregio-0.5.1/coregio/registry_auth.py`

 * *Files identical despite different names*

### Comparing `coregio-0.5.0/coregio/utils.py` & `coregio-0.5.1/coregio/utils.py`

 * *Files identical despite different names*

### Comparing `coregio-0.5.0/coregio.egg-info/PKG-INFO` & `coregio-0.5.1/coregio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coregio
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python container registry API library.
 Author-email: Ales Raszka <araszka@redhat.com>
 License: Copyright (c) 2023 Ales Raszka
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -90,14 +90,15 @@
     manifest_types=["oci_index"]
 )
 print(manifest)
 {'schemaVersion': 2, 'mediaType': 'application/vnd.docker.distribution.manifest.list.v2+json', 'manifests': [{'mediaType': 'application/vnd.docker.distribution.manifest.v2+json', 'size': 595, 'digest': 'sha256:1b2da31e89c8efe8d67f726f9872ca2fce95ddb1d5d97fd71468d5c48de85ddf', 'platform': {'architecture': 'amd64', 'os': 'linux'}}, {'mediaType': 'application/vnd.docker.distribution.manifest.v2+json', 'size': 595, 'digest': 'sha256:18ef5a4eb0a00e0513c8d4fb87bc31728e4c7ed6caea83c608c5048418b00185', 'platform': {'architecture': 'ppc64le', 'os': 'linux'}}, {'mediaType': 'application/vnd.docker.distribution.manifest.v2+json', 'size': 595, 'digest': 'sha256:c3e79af3edaf3b05282565c0b3e08e5b189e4200153114475256d00367da09da', 'platform': {'architecture': 's390x', 'os': 'linux'}}, {'mediaType': 'application/vnd.docker.distribution.manifest.v2+json', 'size': 595, 'digest': 'sha256:7da24517de68a4af11f098841d10c2e02f12619c662e5b812bff7959e2a477a6', 'platform': {'architecture': 'arm64', 'os': 'linux'}}]}
 
 ```
 
+
 ```python
 # Using a proxy
 registry = ContainerRegistry(
     "quay.io",
     proxy="http://proxy.example.com"
 )
```

### Comparing `coregio-0.5.0/pyproject.toml` & `coregio-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.pdm]
 
 [project]
 name = "coregio"
-version = "0.5.0"
+version = "0.5.1"
 description = "Python container registry API library."
 authors = [{ name = "Ales Raszka", email = "araszka@redhat.com" }]
 dependencies = ["requests>=2.31.0"]
 requires-python = ">=3.8"
 readme = "README.md"
 license = { file = "LICENSE.txt" }
```

### Comparing `coregio-0.5.0/tests/test_registry_api.py` & `coregio-0.5.1/tests/test_registry_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -136,96 +136,69 @@
     mock_get.reset_mock()
     result = registry.get_paginated_response("v2/foo", "foo")
     assert result == ["bar1", "bar2"]
 
 
 @patch("coregio.utils.handle_response")
 @patch("coregio.registry_api.ContainerRegistry.get_request")
-def test_get_manifest(
+def test_get_manifest_raw(
     mock_get: MagicMock,
     mock_handle: MagicMock,
 ) -> None:
-    get = MagicMock()
-    get.json.return_value = {"foo": "bar"}
-    mock_get.return_value = get
+    mock_response = MagicMock()
+    mock_get.return_value = mock_response
     mock_handle.return_value = None
     registry = ContainerRegistry("registry", "docker_cfg")
-    result = registry.get_manifest("repo", "ref")
-
-    assert result == {"foo": "bar"}
-    mock_get.assert_called_once_with(
-        "v2/repo/manifests/ref",
-        headers={
-            "Accept": "application/vnd.docker.distribution.manifest.v2+json, application/vnd.oci.image.manifest.v1+json"
-        },
-    )
-
-    mock_get.reset_mock()
-    response = requests.Response()
-    response.status_code = 200
-    response.headers = {"Docker-Content-Digest": "demo_manifest_1"}  # type: ignore
-    mock_get.return_value = response
-    result = registry.get_manifest("repo", "ref", is_headers=True)
-    assert result == {"Docker-Content-Digest": "demo_manifest_1"}
+    result = registry.get_manifest_raw("repo", "ref")
 
+    assert result == mock_response
     mock_get.assert_called_once_with(
         "v2/repo/manifests/ref",
         headers={
             "Accept": "application/vnd.docker.distribution.manifest.v2+json, application/vnd.oci.image.manifest.v1+json"
         },
     )
 
     mock_resp = MagicMock()
     mock_resp.status_code = 400
     mock_get.side_effect = requests.HTTPError(response=mock_resp)
     with pytest.raises(requests.HTTPError):
         registry.get_manifest("repo", "ref")
 
 
-@patch("coregio.utils.handle_response")
-@patch("coregio.registry_api.ContainerRegistry.get_request")
-def test_get_manifest_headers(
-    mock_get: MagicMock,
-    mock_handle: MagicMock,
+@patch("coregio.registry_api.ContainerRegistry.get_manifest_raw")
+def test_get_manifest(
+    mock_get_manifest_raw: MagicMock,
 ) -> None:
-    get = MagicMock()
-    get.headers = {"foo": "bar"}
-    mock_get.return_value = get
-    mock_handle.return_value = None
+    manifest_rsp = MagicMock()
+    mock_get_manifest_raw.return_value = manifest_rsp
     registry_api = ContainerRegistry(url="registry")
-    result = registry_api.get_manifest_headers("repo", "ref")
+    result = registry_api.get_manifest("repo", "ref")
 
-    assert result == {"foo": "bar"}
-    mock_get.assert_called_once_with(
-        "v2/repo/manifests/ref",
-        headers={
-            "Accept": "application/vnd.docker.distribution.manifest.v2+json, application/vnd.oci.image.manifest.v1+json"
-        },
-    )
+    assert result == manifest_rsp.json()
+    mock_get_manifest_raw.assert_called_once_with("repo", "ref", None)
 
-    mock_get.reset_mock()
-    response = requests.Response()
-    response.status_code = 200
-    response.headers = {"Docker-Content-Digest": "demo_manifest_1"}  # type: ignore
-    mock_get.return_value = response
-    result = registry_api.get_manifest_headers("repo", "ref")
-    assert result == {"Docker-Content-Digest": "demo_manifest_1"}
+    mock_get_manifest_raw.reset_mock()
+    result = registry_api.get_manifest("repo", "ref", is_headers=True)
 
-    mock_get.assert_called_once_with(
-        "v2/repo/manifests/ref",
-        headers={
-            "Accept": "application/vnd.docker.distribution.manifest.v2+json, application/vnd.oci.image.manifest.v1+json"
-        },
-    )
+    assert result == manifest_rsp.headers
+    mock_get_manifest_raw.assert_called_once_with("repo", "ref", None)
 
-    mock_resp = MagicMock()
-    mock_resp.status_code = 400
-    mock_get.side_effect = requests.HTTPError(response=mock_resp)
-    with pytest.raises(requests.HTTPError):
-        registry_api.get_manifest_headers("repo", "ref")
+
+@patch("coregio.registry_api.ContainerRegistry.get_manifest")
+def test_get_manifest_headers(
+    mock_get_manifest: MagicMock,
+) -> None:
+    manifest = MagicMock()
+    mock_get_manifest.return_value = manifest
+    registry_api = ContainerRegistry(url="registry")
+    result = registry_api.get_manifest_headers("repo", "ref")
+
+    assert result == manifest
+    mock_get_manifest.assert_called_once_with("repo", "ref", is_headers=True)
 
 
 @patch("coregio.registry_api.ContainerRegistry.get_paginated_response")
 def test_get_tags(mock_get: MagicMock) -> None:
     mock_get.return_value = ["foo", "bar"]
 
     registry = ContainerRegistry("registry", "docker_cfg")
```

### Comparing `coregio-0.5.0/tests/test_registry_auth.py` & `coregio-0.5.1/tests/test_registry_auth.py`

 * *Files identical despite different names*

