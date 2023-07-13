# Comparing `tmp/peerdid-0.5.1.tar.gz` & `tmp/peerdid-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peerdid-0.5.1.tar", last modified: Tue Aug 23 07:26:37 2022, max compression
+gzip compressed data, was "peerdid-0.5.2.tar", last modified: Thu Jul 13 09:52:00 2023, max compression
```

## Comparing `peerdid-0.5.1.tar` & `peerdid-0.5.2.tar`

### file list

```diff
@@ -1,25 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 07:26:37.012956 peerdid-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-08-23 07:26:09.000000 peerdid-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-08-23 07:26:09.000000 peerdid-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6814 2022-08-23 07:26:37.012956 peerdid-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5934 2022-08-23 07:26:09.000000 peerdid-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 07:26:37.012956 peerdid-0.5.1/peerdid/
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-08-23 07:26:09.000000 peerdid-0.5.1/peerdid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 07:26:37.012956 peerdid-0.5.1/peerdid/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-23 07:26:09.000000 peerdid-0.5.1/peerdid/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1488 2022-08-23 07:26:09.000000 peerdid-0.5.1/peerdid/core/jwk_okp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1405 2022-08-23 07:26:09.000000 peerdid-0.5.1/peerdid/core/multibase.py
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2022-08-23 07:26:09.000000 peerdid-0.5.1/peerdid/core/multicodec.py
--rw-r--r--   0 runner    (1001) docker     (121)     4990 2022-08-23 07:26:09.000000 peerdid-0.5.1/peerdid/core/peer_did_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-08-23 07:26:09.000000 peerdid-0.5.1/peerdid/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7260 2022-08-23 07:26:09.000000 peerdid-0.5.1/peerdid/dids.py
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-08-23 07:26:09.000000 peerdid-0.5.1/peerdid/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     8193 2022-08-23 07:26:09.000000 peerdid-0.5.1/peerdid/keys.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 07:26:37.012956 peerdid-0.5.1/peerdid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6814 2022-08-23 07:26:37.000000 peerdid-0.5.1/peerdid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      428 2022-08-23 07:26:37.000000 peerdid-0.5.1/peerdid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-23 07:26:37.000000 peerdid-0.5.1/peerdid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-08-23 07:26:37.000000 peerdid-0.5.1/peerdid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-23 07:26:37.000000 peerdid-0.5.1/peerdid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      981 2022-08-23 07:26:37.012956 peerdid-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      213 2022-08-23 07:26:09.000000 peerdid-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:52:00.768393 peerdid-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-13 09:51:50.000000 peerdid-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-13 09:51:50.000000 peerdid-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-07-13 09:52:00.768393 peerdid-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-07-13 09:51:50.000000 peerdid-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:52:00.764393 peerdid-0.5.2/peerdid/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-13 09:51:50.000000 peerdid-0.5.2/peerdid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:52:00.768393 peerdid-0.5.2/peerdid/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:51:50.000000 peerdid-0.5.2/peerdid/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-13 09:51:50.000000 peerdid-0.5.2/peerdid/core/jwk_okp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-13 09:51:50.000000 peerdid-0.5.2/peerdid/core/multibase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-13 09:51:50.000000 peerdid-0.5.2/peerdid/core/multicodec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-07-13 09:51:50.000000 peerdid-0.5.2/peerdid/core/peer_did_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-13 09:51:50.000000 peerdid-0.5.2/peerdid/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-07-13 09:51:50.000000 peerdid-0.5.2/peerdid/dids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-13 09:51:50.000000 peerdid-0.5.2/peerdid/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-07-13 09:51:50.000000 peerdid-0.5.2/peerdid/keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:52:00.764393 peerdid-0.5.2/peerdid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-07-13 09:52:00.000000 peerdid-0.5.2/peerdid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-13 09:52:00.000000 peerdid-0.5.2/peerdid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:52:00.000000 peerdid-0.5.2/peerdid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-13 09:52:00.000000 peerdid-0.5.2/peerdid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 09:52:00.000000 peerdid-0.5.2/peerdid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-13 09:52:00.768393 peerdid-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-13 09:51:50.000000 peerdid-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:52:00.768393 peerdid-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-13 09:51:50.000000 peerdid-0.5.2/tests/test_create_peer_did_numalgo_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14144 2023-07-13 09:51:50.000000 peerdid-0.5.2/tests/test_create_peer_did_numalgo_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-13 09:51:50.000000 peerdid-0.5.2/tests/test_peer_did_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-07-13 09:51:50.000000 peerdid-0.5.2/tests/test_resolve_peer_did_numalgo_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9269 2023-07-13 09:51:50.000000 peerdid-0.5.2/tests/test_resolve_peer_did_numalgo_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19465 2023-07-13 09:51:50.000000 peerdid-0.5.2/tests/test_vectors.py
```

### Comparing `peerdid-0.5.1/LICENSE` & `peerdid-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `peerdid-0.5.1/PKG-INFO` & `peerdid-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peerdid
-Version: 0.5.1
+Version: 0.5.2
 Summary: PeerDID for Python
 Home-page: https://github.com/sicpa-dlab/peer-did-python
 Author: SICPA
 Author-email: DLCHOpenSourceContrib@sicpa.com
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/sicpa-dlab/peer-did-python
 Project-URL: Issue Tracker, https://github.com/sicpa-dlab/peer-did-python/issues/
```

### Comparing `peerdid-0.5.1/README.md` & `peerdid-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `peerdid-0.5.1/peerdid/core/jwk_okp.py` & `peerdid-0.5.2/peerdid/core/jwk_okp.py`

 * *Files identical despite different names*

### Comparing `peerdid-0.5.1/peerdid/core/multibase.py` & `peerdid-0.5.2/peerdid/core/multibase.py`

 * *Files identical despite different names*

### Comparing `peerdid-0.5.1/peerdid/core/multicodec.py` & `peerdid-0.5.2/peerdid/core/multicodec.py`

 * *Files identical despite different names*

### Comparing `peerdid-0.5.1/peerdid/core/peer_did_helper.py` & `peerdid-0.5.2/peerdid/core/peer_did_helper.py`

 * *Files identical despite different names*

### Comparing `peerdid-0.5.1/peerdid/core/utils.py` & `peerdid-0.5.2/peerdid/core/utils.py`

 * *Files identical despite different names*

### Comparing `peerdid-0.5.1/peerdid/dids.py` & `peerdid-0.5.2/peerdid/dids.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,17 +121,15 @@
     else:
         did_doc = _build_did_doc_numalgo_2(peer_did, format)
     return did_doc
 
 
 def _did_document_builder(peer_did: Union[str, DID]) -> DIDDocumentBuilder:
     try:
-        return DIDDocumentBuilder(
-            peer_did, context=DIDDocumentBuilder.DEFAULT_CONTEXT.copy()
-        )
+        return DIDDocumentBuilder(peer_did)
     except InvalidDIDError as e:
         raise MalformedPeerDIDError("Invalid peer DID") from e
 
 
 def _add_key_to_document(builder: DIDDocumentBuilder, key: BaseKey):
     ver_method_result = key.verification_method(builder.id)
     builder.verification_method.methods.append(ver_method_result.method)
```

### Comparing `peerdid-0.5.1/peerdid/keys.py` & `peerdid-0.5.2/peerdid/keys.py`

 * *Files identical despite different names*

### Comparing `peerdid-0.5.1/peerdid.egg-info/PKG-INFO` & `peerdid-0.5.2/peerdid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peerdid
-Version: 0.5.1
+Version: 0.5.2
 Summary: PeerDID for Python
 Home-page: https://github.com/sicpa-dlab/peer-did-python
 Author: SICPA
 Author-email: DLCHOpenSourceContrib@sicpa.com
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/sicpa-dlab/peer-did-python
 Project-URL: Issue Tracker, https://github.com/sicpa-dlab/peer-did-python/issues/
```

### Comparing `peerdid-0.5.1/setup.cfg` & `peerdid-0.5.2/setup.cfg`

 * *Files identical despite different names*

