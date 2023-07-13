# Comparing `tmp/pymilldb-0.0.8.tar.gz` & `tmp/pymilldb-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymilldb-0.0.8.tar", last modified: Tue Jun 27 13:27:32 2023, max compression
+gzip compressed data, was "pymilldb-0.0.9.tar", last modified: Thu Jun 29 18:31:13 2023, max compression
```

## Comparing `pymilldb-0.0.8.tar` & `pymilldb-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,22 @@
-drwxr-xr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-27 13:27:32.343078 pymilldb-0.0.8/
--rw-r--r--   0 zeus      (1000) zeus      (1000)     1095 2023-05-30 21:05:16.000000 pymilldb-0.0.8/LICENSE
--rw-r--r--   0 zeus      (1000) zeus      (1000)     1031 2023-06-27 13:27:32.343078 pymilldb-0.0.8/PKG-INFO
--rw-r--r--   0 zeus      (1000) zeus      (1000)      523 2023-05-30 21:18:35.000000 pymilldb-0.0.8/README.md
--rw-r--r--   0 zeus      (1000) zeus      (1000)       89 2023-05-30 21:05:16.000000 pymilldb-0.0.8/pyproject.toml
--rw-r--r--   0 zeus      (1000) zeus      (1000)      633 2023-06-27 13:27:32.343078 pymilldb-0.0.8/setup.cfg
-drwxr-xr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-27 13:27:32.333078 pymilldb-0.0.8/src/
-drwxr-xr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-27 13:27:32.343078 pymilldb-0.0.8/src/pymilldb/
--rw-r--r--   0 zeus      (1000) zeus      (1000)      226 2023-06-27 13:06:16.000000 pymilldb-0.0.8/src/pymilldb/__init__.py
--rw-r--r--   0 zeus      (1000) zeus      (1000)     2802 2023-06-06 21:04:43.000000 pymilldb-0.0.8/src/pymilldb/mdb_client.py
--rw-r--r--   0 zeus      (1000) zeus      (1000)     1600 2023-06-27 13:20:48.000000 pymilldb-0.0.8/src/pymilldb/node_iterator.py
--rw-r--r--   0 zeus      (1000) zeus      (1000)     1655 2023-06-27 13:03:43.000000 pymilldb-0.0.8/src/pymilldb/protocol.py
--rw-r--r--   0 zeus      (1000) zeus      (1000)     1430 2023-06-06 21:04:43.000000 pymilldb-0.0.8/src/pymilldb/sampler.py
--rw-r--r--   0 zeus      (1000) zeus      (1000)    10748 2023-06-23 13:54:50.000000 pymilldb-0.0.8/src/pymilldb/tensor_store.py
-drwxr-xr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-27 13:27:32.343078 pymilldb-0.0.8/src/pymilldb/utils/
--rw-r--r--   0 zeus      (1000) zeus      (1000)        0 2023-05-30 21:05:16.000000 pymilldb-0.0.8/src/pymilldb/utils/__init__.py
--rw-r--r--   0 zeus      (1000) zeus      (1000)      353 2023-05-30 21:05:16.000000 pymilldb-0.0.8/src/pymilldb/utils/decorators.py
--rw-r--r--   0 zeus      (1000) zeus      (1000)      630 2023-05-30 21:05:16.000000 pymilldb-0.0.8/src/pymilldb/utils/graph.py
--rw-r--r--   0 zeus      (1000) zeus      (1000)     2173 2023-06-06 21:04:43.000000 pymilldb-0.0.8/src/pymilldb/utils/packer.py
-drwxr-xr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-27 13:27:32.343078 pymilldb-0.0.8/src/pymilldb.egg-info/
--rw-r--r--   0 zeus      (1000) zeus      (1000)     1031 2023-06-27 13:27:32.000000 pymilldb-0.0.8/src/pymilldb.egg-info/PKG-INFO
--rw-r--r--   0 zeus      (1000) zeus      (1000)      467 2023-06-27 13:27:32.000000 pymilldb-0.0.8/src/pymilldb.egg-info/SOURCES.txt
--rw-r--r--   0 zeus      (1000) zeus      (1000)        1 2023-06-27 13:27:32.000000 pymilldb-0.0.8/src/pymilldb.egg-info/dependency_links.txt
--rw-r--r--   0 zeus      (1000) zeus      (1000)        9 2023-06-27 13:27:32.000000 pymilldb-0.0.8/src/pymilldb.egg-info/top_level.txt
+drwxr-xr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-29 18:31:13.775826 pymilldb-0.0.9/
+-rw-r--r--   0 zeus      (1000) zeus      (1000)     1095 2023-05-30 21:05:16.000000 pymilldb-0.0.9/LICENSE
+-rw-r--r--   0 zeus      (1000) zeus      (1000)     1031 2023-06-29 18:31:13.775826 pymilldb-0.0.9/PKG-INFO
+-rw-r--r--   0 zeus      (1000) zeus      (1000)      523 2023-05-30 21:18:35.000000 pymilldb-0.0.9/README.md
+-rw-r--r--   0 zeus      (1000) zeus      (1000)       89 2023-05-30 21:05:16.000000 pymilldb-0.0.9/pyproject.toml
+-rw-r--r--   0 zeus      (1000) zeus      (1000)      633 2023-06-29 18:31:13.775826 pymilldb-0.0.9/setup.cfg
+drwxr-xr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-29 18:31:13.775826 pymilldb-0.0.9/src/
+drwxr-xr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-29 18:31:13.775826 pymilldb-0.0.9/src/pymilldb/
+-rw-r--r--   0 zeus      (1000) zeus      (1000)      329 2023-06-29 17:43:16.000000 pymilldb-0.0.9/src/pymilldb/__init__.py
+-rw-r--r--   0 zeus      (1000) zeus      (1000)      353 2023-06-29 16:25:41.000000 pymilldb-0.0.9/src/pymilldb/decorators.py
+-rw-r--r--   0 zeus      (1000) zeus      (1000)     3776 2023-06-29 18:19:33.000000 pymilldb-0.0.9/src/pymilldb/graph.py
+-rw-r--r--   0 zeus      (1000) zeus      (1000)     2784 2023-06-29 16:26:33.000000 pymilldb-0.0.9/src/pymilldb/mdb_client.py
+-rw-r--r--   0 zeus      (1000) zeus      (1000)     1595 2023-06-29 16:26:16.000000 pymilldb-0.0.9/src/pymilldb/node_iterator.py
+-rw-r--r--   0 zeus      (1000) zeus      (1000)     2195 2023-06-29 16:26:05.000000 pymilldb-0.0.9/src/pymilldb/packer.py
+-rw-r--r--   0 zeus      (1000) zeus      (1000)     1655 2023-06-27 13:03:43.000000 pymilldb-0.0.9/src/pymilldb/protocol.py
+-rw-r--r--   0 zeus      (1000) zeus      (1000)     2065 2023-06-29 16:26:01.000000 pymilldb-0.0.9/src/pymilldb/sampler.py
+-rw-r--r--   0 zeus      (1000) zeus      (1000)    10743 2023-06-29 16:26:24.000000 pymilldb-0.0.9/src/pymilldb/tensor_store.py
+drwxr-xr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-29 18:31:13.775826 pymilldb-0.0.9/src/pymilldb.egg-info/
+-rw-r--r--   0 zeus      (1000) zeus      (1000)     1031 2023-06-29 18:31:13.000000 pymilldb-0.0.9/src/pymilldb.egg-info/PKG-INFO
+-rw-r--r--   0 zeus      (1000) zeus      (1000)      418 2023-06-29 18:31:13.000000 pymilldb-0.0.9/src/pymilldb.egg-info/SOURCES.txt
+-rw-r--r--   0 zeus      (1000) zeus      (1000)        1 2023-06-29 18:31:13.000000 pymilldb-0.0.9/src/pymilldb.egg-info/dependency_links.txt
+-rw-r--r--   0 zeus      (1000) zeus      (1000)        9 2023-06-29 18:31:13.000000 pymilldb-0.0.9/src/pymilldb.egg-info/top_level.txt
```

### Comparing `pymilldb-0.0.8/LICENSE` & `pymilldb-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pymilldb-0.0.8/PKG-INFO` & `pymilldb-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymilldb
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python library for MillenniumDB
 Home-page: https://github.com/MillenniumDB/PyMillDB
 Author: Vicente Calisto
 Author-email: vecalisto@uc.cl
 Project-URL: Bug Tracker, https://github.com/MillenniumDB/PyMillDB/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymilldb-0.0.8/README.md` & `pymilldb-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pymilldb-0.0.8/setup.cfg` & `pymilldb-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pymilldb
-version = 0.0.8
+version = 0.0.9
 author = Vicente Calisto
 author_email = vecalisto@uc.cl
 description = A python library for MillenniumDB
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/MillenniumDB/PyMillDB
 project_urls =
```

### Comparing `pymilldb-0.0.8/src/pymilldb/mdb_client.py` & `pymilldb-0.0.9/src/pymilldb/mdb_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import socket
 from typing import Tuple
 
-from . import protocol
-from .utils import decorators, packer
+from . import decorators, packer, protocol
 
 
 ## Interface for stablishing a connection with the server for
 # sending and receiving data.
 #
 # Almost every class and function in this library needs a `MDBClient` instance
 # as an argument to communicate with the server.
```

### Comparing `pymilldb-0.0.8/src/pymilldb/node_iterator.py` & `pymilldb-0.0.9/src/pymilldb/node_iterator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import TYPE_CHECKING, List
 
+from . import packer
 from .protocol import RequestType, StatusCode
-from .utils import packer
 
 if TYPE_CHECKING:
     from .mdb_client import MDBClient
 
 ## Interface for iterating over nodes in MillenniumDB.
 class NodeIterator:
     ## Constructor.
```

### Comparing `pymilldb-0.0.8/src/pymilldb/protocol.py` & `pymilldb-0.0.9/src/pymilldb/protocol.py`

 * *Files identical despite different names*

### Comparing `pymilldb-0.0.8/src/pymilldb/tensor_store.py` & `pymilldb-0.0.9/src/pymilldb/tensor_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections.abc import Iterable
 from typing import TYPE_CHECKING, List, Union
 
 import torch
 
+from . import decorators, packer
 from .protocol import RequestType
-from .utils import decorators, packer
 
 if TYPE_CHECKING:
     from .mdb_client import MDBClient
 
 
 ## Interface for storing tensors in the MillenniumDB's TensorStore.
 #
```

### Comparing `pymilldb-0.0.8/src/pymilldb/utils/packer.py` & `pymilldb-0.0.9/src/pymilldb/packer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import struct
 from typing import List
 
-from .graph import Graph
+from .sampler import GraphSample
 
 
 def pack_byte(b: int) -> bytes:
     return struct.pack(">B", b)
 
 
 def pack_bool(b: bool) -> bytes:
@@ -64,15 +64,15 @@
     return [unpack_uint64(data[i : i + 8]) for i in range(0, len(data), 8)]
 
 
 def unpack_float_vector(data: bytes) -> List[float]:
     return [unpack_float(data[i : i + 4]) for i in range(0, len(data), 4)]
 
 
-def unpack_graph(data: bytes) -> Graph:
+def unpack_graph(data: bytes) -> "GraphSample":
     lo, hi = 0, 8
     num_seeds = unpack_uint64(data[lo:hi])
     lo, hi = hi, hi + 8
     num_nodes = unpack_uint64(data[lo:hi])
     lo, hi = hi, hi + 8
     num_edges = unpack_uint64(data[lo:hi])
 
@@ -83,8 +83,8 @@
     lo, hi = hi, hi + 8 * num_edges
     edge_ids = unpack_uint64_vector(data[lo:hi])
 
     edge_index = [
         unpack_uint64_vector(data[i : i + 16])
         for i in range(hi, hi + 16 * num_edges, 16)
     ]
-    return Graph(seed_ids, node_ids, edge_ids, edge_index)
+    return GraphSample(seed_ids, node_ids, edge_ids, edge_index)
```

### Comparing `pymilldb-0.0.8/src/pymilldb.egg-info/PKG-INFO` & `pymilldb-0.0.9/src/pymilldb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymilldb
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python library for MillenniumDB
 Home-page: https://github.com/MillenniumDB/PyMillDB
 Author: Vicente Calisto
 Author-email: vecalisto@uc.cl
 Project-URL: Bug Tracker, https://github.com/MillenniumDB/PyMillDB/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

