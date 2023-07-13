# Comparing `tmp/cbcmgr-1.4.1.tar.gz` & `tmp/cbcmgr-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbcmgr-1.4.1.tar", last modified: Wed Jul 12 14:07:12 2023, max compression
+gzip compressed data, was "cbcmgr-1.4.2.tar", last modified: Thu Jul 13 02:48:10 2023, max compression
```

## Comparing `cbcmgr-1.4.1.tar` & `cbcmgr-1.4.2.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-12 14:07:12.307904 cbcmgr-1.4.1/
--rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.4.1/LICENSE.txt
--rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-12 14:07:12.307629 cbcmgr-1.4.1/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.4.1/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-12 14:07:12.139554 cbcmgr-1.4.1/cbcmgr/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.4.1/cbcmgr/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)    10719 2023-07-12 01:28:33.000000 cbcmgr-1.4.1/cbcmgr/cb_connect.py
--rw-r--r--   0 michael    (501) staff       (20)    11149 2023-07-12 01:28:33.000000 cbcmgr-1.4.1/cbcmgr/cb_connect_lite.py
--rw-r--r--   0 michael    (501) staff       (20)    27544 2023-07-12 01:28:33.000000 cbcmgr-1.4.1/cbcmgr/cb_management.py
--rw-r--r--   0 michael    (501) staff       (20)     7249 2023-07-12 01:28:33.000000 cbcmgr-1.4.1/cbcmgr/cb_operation_s.py
--rw-r--r--   0 michael    (501) staff       (20)     3881 2023-07-12 13:52:42.000000 cbcmgr-1.4.1/cbcmgr/cb_pathmap.py
--rw-r--r--   0 michael    (501) staff       (20)    13289 2023-07-12 01:28:33.000000 cbcmgr-1.4.1/cbcmgr/cb_session.py
--rw-r--r--   0 michael    (501) staff       (20)     2021 2023-07-07 19:01:23.000000 cbcmgr-1.4.1/cbcmgr/config.py
--rw-r--r--   0 michael    (501) staff       (20)     4334 2023-07-12 01:28:33.000000 cbcmgr-1.4.1/cbcmgr/exceptions.py
--rw-r--r--   0 michael    (501) staff       (20)    11048 2023-06-12 14:40:15.000000 cbcmgr-1.4.1/cbcmgr/httpsessionmgr.py
--rw-r--r--   0 michael    (501) staff       (20)      938 2023-07-12 01:28:33.000000 cbcmgr-1.4.1/cbcmgr/id_format.py
--rw-r--r--   0 michael    (501) staff       (20)     2373 2023-07-12 01:28:33.000000 cbcmgr-1.4.1/cbcmgr/mt_pool.py
--rw-r--r--   0 michael    (501) staff       (20)     2825 2023-07-07 21:38:37.000000 cbcmgr-1.4.1/cbcmgr/retry.py
--rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.4.1/cbcmgr/schema.py
--rw-r--r--   0 michael    (501) staff       (20)     1446 2023-07-12 01:28:33.000000 cbcmgr-1.4.1/cbcmgr/util.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-12 14:07:12.307063 cbcmgr-1.4.1/cbcmgr.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-12 14:07:12.000000 cbcmgr-1.4.1/cbcmgr.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      485 2023-07-12 14:07:12.000000 cbcmgr-1.4.1/cbcmgr.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-12 14:07:12.000000 cbcmgr-1.4.1/cbcmgr.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       67 2023-07-12 14:07:12.000000 cbcmgr-1.4.1/cbcmgr.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        7 2023-07-12 14:07:12.000000 cbcmgr-1.4.1/cbcmgr.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-07-12 14:07:12.307976 cbcmgr-1.4.1/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)     1266 2023-07-12 13:52:42.000000 cbcmgr-1.4.1/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-13 02:48:10.111665 cbcmgr-1.4.2/
+-rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.4.2/LICENSE.txt
+-rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-13 02:48:10.111279 cbcmgr-1.4.2/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.4.2/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-13 02:48:10.097897 cbcmgr-1.4.2/cbcmgr/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.4.2/cbcmgr/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     2606 2023-07-13 01:40:09.000000 cbcmgr-1.4.2/cbcmgr/async_pool.py
+-rw-r--r--   0 michael    (501) staff       (20)    10719 2023-07-12 01:28:33.000000 cbcmgr-1.4.2/cbcmgr/cb_connect.py
+-rw-r--r--   0 michael    (501) staff       (20)    10466 2023-07-13 01:22:43.000000 cbcmgr-1.4.2/cbcmgr/cb_connect_lite.py
+-rw-r--r--   0 michael    (501) staff       (20)    11368 2023-07-13 02:29:07.000000 cbcmgr-1.4.2/cbcmgr/cb_connect_lite_a.py
+-rw-r--r--   0 michael    (501) staff       (20)    27544 2023-07-12 01:28:33.000000 cbcmgr-1.4.2/cbcmgr/cb_management.py
+-rw-r--r--   0 michael    (501) staff       (20)     7658 2023-07-12 21:45:43.000000 cbcmgr-1.4.2/cbcmgr/cb_operation_a.py
+-rw-r--r--   0 michael    (501) staff       (20)     7121 2023-07-12 14:35:27.000000 cbcmgr-1.4.2/cbcmgr/cb_operation_s.py
+-rw-r--r--   0 michael    (501) staff       (20)     3881 2023-07-12 13:52:42.000000 cbcmgr-1.4.2/cbcmgr/cb_pathmap.py
+-rw-r--r--   0 michael    (501) staff       (20)    12508 2023-07-12 14:35:27.000000 cbcmgr-1.4.2/cbcmgr/cb_session.py
+-rw-r--r--   0 michael    (501) staff       (20)     2021 2023-07-07 19:01:23.000000 cbcmgr-1.4.2/cbcmgr/config.py
+-rw-r--r--   0 michael    (501) staff       (20)     4334 2023-07-12 01:28:33.000000 cbcmgr-1.4.2/cbcmgr/exceptions.py
+-rw-r--r--   0 michael    (501) staff       (20)    11048 2023-06-12 14:40:15.000000 cbcmgr-1.4.2/cbcmgr/httpsessionmgr.py
+-rw-r--r--   0 michael    (501) staff       (20)      938 2023-07-12 01:28:33.000000 cbcmgr-1.4.2/cbcmgr/id_format.py
+-rw-r--r--   0 michael    (501) staff       (20)     2373 2023-07-12 01:28:33.000000 cbcmgr-1.4.2/cbcmgr/mt_pool.py
+-rw-r--r--   0 michael    (501) staff       (20)     2825 2023-07-07 21:38:37.000000 cbcmgr-1.4.2/cbcmgr/retry.py
+-rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.4.2/cbcmgr/schema.py
+-rw-r--r--   0 michael    (501) staff       (20)     1446 2023-07-12 01:28:33.000000 cbcmgr-1.4.2/cbcmgr/util.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-13 02:48:10.110567 cbcmgr-1.4.2/cbcmgr.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-13 02:48:09.000000 cbcmgr-1.4.2/cbcmgr.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      559 2023-07-13 02:48:09.000000 cbcmgr-1.4.2/cbcmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-13 02:48:09.000000 cbcmgr-1.4.2/cbcmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       82 2023-07-13 02:48:09.000000 cbcmgr-1.4.2/cbcmgr.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        7 2023-07-13 02:48:09.000000 cbcmgr-1.4.2/cbcmgr.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-07-13 02:48:10.111798 cbcmgr-1.4.2/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     1292 2023-07-12 22:19:35.000000 cbcmgr-1.4.2/setup.py
```

### Comparing `cbcmgr-1.4.1/LICENSE.txt` & `cbcmgr-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.1/PKG-INFO` & `cbcmgr-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.4.1
+Version: 1.4.2
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Keywords: couchbase,nosql,pycouchbase,database
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cbcmgr-1.4.1/README.md` & `cbcmgr-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.1/cbcmgr/cb_connect.py` & `cbcmgr-1.4.2/cbcmgr/cb_connect.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.1/cbcmgr/cb_connect_lite.py` & `cbcmgr-1.4.2/cbcmgr/cb_connect_lite.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,27 @@
 ##
 ##
 
-from .exceptions import (IndexInternalError, CollectionGetError, CollectionCountError, NodeConnectionError, NodeConnectionFailed, ClusterHealthCheckError, KeyFormatError)
+from .exceptions import (IndexInternalError, CollectionGetError, CollectionCountError)
 from .retry import retry
-from .httpsessionmgr import APISession
-from .config import KeyStyle
 from .cb_session import CBSession, BucketMode
 import logging
-import socket
-import dns.resolver
-import uuid
 import hashlib
-from typing import Union, Dict, Any, List
-from enum import Enum
 from datetime import timedelta
-from couchbase.auth import PasswordAuthenticator
-from couchbase.options import ClusterTimeoutOptions, LockMode, ClusterOptions, TLSVerifyMode
+from typing import Union, Dict, Any, List
 from couchbase.cluster import Cluster
-from acouchbase.cluster import AsyncCluster
 from couchbase.bucket import Bucket
-from acouchbase.bucket import AsyncBucket
 from couchbase.scope import Scope
-from acouchbase.scope import AsyncScope
 from couchbase.collection import Collection
-from acouchbase.collection import AsyncCollection
-from couchbase.diagnostics import ServiceType, PingState
 from couchbase.management.buckets import CreateBucketSettings, BucketType, StorageBackend
 from couchbase.management.collections import CollectionSpec
-from couchbase.management.options import CreateQueryIndexOptions, CreatePrimaryQueryIndexOptions
+from couchbase.management.options import CreateQueryIndexOptions, CreatePrimaryQueryIndexOptions, WatchQueryIndexOptions
 from couchbase.exceptions import (BucketNotFoundException, ScopeNotFoundException, CollectionNotFoundException, BucketAlreadyExistsException, ScopeAlreadyExistsException,
-                                  CollectionAlreadyExistsException, QueryIndexAlreadyExistsException, QueryIndexNotFoundException, DocumentNotFoundException)
+                                  CollectionAlreadyExistsException, QueryIndexAlreadyExistsException, QueryIndexNotFoundException, DocumentNotFoundException,
+                                  WatchQueryIndexTimeoutException)
 
 logger = logging.getLogger('cbutil.connect.lite')
 logger.addHandler(logging.NullHandler())
 JSONType = Union[str, int, float, bool, None, Dict[str, Any], List[Any]]
 
 
 class CBConnectLite(CBSession):
@@ -71,23 +59,14 @@
                                                   bucket_type=b_type,
                                                   storage_backend=b_stor,
                                                   num_replicas=replicas,
                                                   ram_quota_mb=quota))
         except BucketAlreadyExistsException:
             pass
 
-    @retry(always_raise_list=(BucketNotFoundException,))
-    async def get_bucket_a(self, cluster: AsyncCluster, name: str) -> AsyncBucket:
-        if name is None:
-            raise TypeError("name can not be None")
-        logger.debug(f"bucket: connect {name}")
-        bucket = cluster.bucket(name)
-        await bucket.on_connect()
-        return bucket
-
     @retry(always_raise_list=(ScopeNotFoundException,))
     def get_scope(self, bucket: Bucket, name: str = "_default") -> Scope:
         if name is None:
             raise TypeError("name can not be None")
         logger.debug(f"scope: connect {name}")
         if not self.is_scope(bucket, name):
             raise ScopeNotFoundException(f"scope {name} does not exist")
@@ -101,22 +80,14 @@
         try:
             if name != "_default":
                 cm = bucket.collections()
                 cm.create_scope(name)
         except ScopeAlreadyExistsException:
             pass
 
-    @retry(always_raise_list=(ScopeNotFoundException,))
-    async def get_scope_a(self, bucket: AsyncBucket, name: str = "_default") -> AsyncScope:
-        if name is None:
-            raise TypeError("name can not be None")
-        logger.debug(f"scope: connect {name}")
-        scope = bucket.scope(name)
-        return scope
-
     @retry(always_raise_list=(CollectionNotFoundException,))
     def get_collection(self, bucket: Bucket, scope: Scope, name: str = "_default") -> Collection:
         if name is None:
             raise TypeError("name can not be None")
         logger.debug(f"collection: connect {name}")
         if not self.is_collection(bucket, scope.name, name):
             raise CollectionNotFoundException(f"collection {name} does not exist")
@@ -149,15 +120,15 @@
             sql = 'select count(*) as count from ' + keyspace + ';'
             result = self.run_query(cluster, sql)
             count: int = int(result[0]['count'])
             return count
         except Exception as err:
             raise CollectionCountError(f"failed to get count for {keyspace}: {err}")
 
-    @retry(always_raise_list=(QueryIndexAlreadyExistsException, QueryIndexNotFoundException))
+    @retry()
     def run_query(self, cluster: Cluster, sql: str):
         contents = []
         result = cluster.query(sql)
         for item in result:
             contents.append(item)
         return contents
 
@@ -206,14 +177,15 @@
             qim = cluster.query_indexes()
             for field in fields:
                 hash_string = f"{bucket.name}_{scope.name}_{collection.name}_{field}"
                 name_part = hashlib.shake_256(hash_string.encode()).hexdigest(3)
                 index_name = f"{field}_{name_part}_ix"
                 logger.debug(f"creating index {index_name} on {field} for {collection.name}")
                 qim.create_index(bucket.name, index_name, [field], index_options)
+                self.index_wait(cluster, bucket, scope, collection, index_name)
         except QueryIndexAlreadyExistsException:
             logger.debug(f"index already exists")
             pass
 
     @retry()
     def create_primary_index(self, cluster: Cluster, bucket: Bucket, scope: Scope, collection: Collection, replica: int = 0):
         if collection.name != '_default':
@@ -224,24 +196,36 @@
         else:
             index_options = CreatePrimaryQueryIndexOptions(deferred=False,
                                                            num_replicas=replica)
         logger.debug(f"creating primary index on {collection.name}")
         try:
             qim = cluster.query_indexes()
             qim.create_primary_index(bucket.name, index_options)
+            self.index_wait_primary(cluster, bucket)
         except QueryIndexAlreadyExistsException:
             pass
 
-    @retry(always_raise_list=(CollectionNotFoundException,))
-    async def get_collection_a(self, scope: AsyncScope, name: str = "_default") -> AsyncCollection:
-        if name is None:
-            raise TypeError("name can not be None")
-        logger.debug(f"collection: connect {name}")
-        collection = scope.collection(name)
-        return collection
+    @retry(always_raise_list=(WatchQueryIndexTimeoutException,))
+    def index_wait(self, cluster: Cluster, bucket: Bucket, scope: Scope, collection: Collection, index: str):
+        watch_options = WatchQueryIndexOptions(
+            collection_name=collection.name,
+            scope_name=scope.name,
+            timeout=timedelta(seconds=10)
+        )
+        qim = cluster.query_indexes()
+        qim.watch_indexes(bucket.name, [index], watch_options)
+
+    @retry(always_raise_list=(WatchQueryIndexTimeoutException,))
+    def index_wait_primary(self, cluster: Cluster, bucket: Bucket):
+        watch_options = WatchQueryIndexOptions(
+            watch_primary=True,
+            timeout=timedelta(seconds=10)
+        )
+        qim = cluster.query_indexes()
+        qim.watch_indexes(bucket.name, [], watch_options)
 
     @staticmethod
     def is_scope(bucket: Bucket, name: str):
         if name is None:
             raise TypeError("name can not be None")
         cm = bucket.collections()
         return next((s for s in cm.get_all_scopes() if s.name == name), None)
```

### Comparing `cbcmgr-1.4.1/cbcmgr/cb_management.py` & `cbcmgr-1.4.2/cbcmgr/cb_management.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.1/cbcmgr/cb_operation_s.py` & `cbcmgr-1.4.2/cbcmgr/cb_operation_s.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 import logging
 from typing import Union, Dict, Any, List
 from enum import Enum
 from couchbase.cluster import Cluster
 from couchbase.bucket import Bucket
 from couchbase.scope import Scope
 from couchbase.collection import Collection
-from couchbase.exceptions import (QueryIndexNotFoundException, QueryIndexAlreadyExistsException, BucketDoesNotExistException, BucketNotFoundException,
-                                  ScopeNotFoundException, CollectionNotFoundException)
-from cbcmgr.retry import retry
+from couchbase.exceptions import (BucketDoesNotExistException, BucketNotFoundException, ScopeNotFoundException, CollectionNotFoundException)
 from cbcmgr.cb_session import BucketMode
 from cbcmgr.cb_connect_lite import CBConnectLite
 
 logger = logging.getLogger('cbutil.operation')
 logger.addHandler(logging.NullHandler())
 JSONType = Union[str, int, float, bool, None, Dict[str, Any], List[Any]]
```

### Comparing `cbcmgr-1.4.1/cbcmgr/cb_pathmap.py` & `cbcmgr-1.4.2/cbcmgr/cb_pathmap.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.1/cbcmgr/cb_session.py` & `cbcmgr-1.4.2/cbcmgr/cb_session.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,34 +5,22 @@
 from .retry import retry
 from .httpsessionmgr import APISession
 from .config import KeyStyle
 import logging
 import socket
 import dns.resolver
 import uuid
-import hashlib
 from typing import Union
 from enum import Enum
 from datetime import timedelta
 from couchbase.auth import PasswordAuthenticator
 from couchbase.options import ClusterTimeoutOptions, LockMode, ClusterOptions, TLSVerifyMode
 from couchbase.cluster import Cluster
 from acouchbase.cluster import AsyncCluster
-from couchbase.bucket import Bucket
-from acouchbase.bucket import AsyncBucket
-from couchbase.scope import Scope
-from acouchbase.scope import AsyncScope
-from couchbase.collection import Collection
-from acouchbase.collection import AsyncCollection
 from couchbase.diagnostics import ServiceType, PingState
-from couchbase.management.buckets import CreateBucketSettings, BucketType, StorageBackend
-from couchbase.management.collections import CollectionSpec
-from couchbase.management.options import CreateQueryIndexOptions, CreatePrimaryQueryIndexOptions
-from couchbase.exceptions import (BucketNotFoundException, ScopeNotFoundException, CollectionNotFoundException, BucketAlreadyExistsException, ScopeAlreadyExistsException,
-                                  CollectionAlreadyExistsException, QueryIndexAlreadyExistsException)
 
 logger = logging.getLogger('cbutil.session')
 logger.addHandler(logging.NullHandler())
 
 
 class BucketMode(Enum):
     DEFAULT = 0
```

### Comparing `cbcmgr-1.4.1/cbcmgr/config.py` & `cbcmgr-1.4.2/cbcmgr/config.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.1/cbcmgr/exceptions.py` & `cbcmgr-1.4.2/cbcmgr/exceptions.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.1/cbcmgr/httpsessionmgr.py` & `cbcmgr-1.4.2/cbcmgr/httpsessionmgr.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.1/cbcmgr/id_format.py` & `cbcmgr-1.4.2/cbcmgr/id_format.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.1/cbcmgr/mt_pool.py` & `cbcmgr-1.4.2/cbcmgr/mt_pool.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.1/cbcmgr/retry.py` & `cbcmgr-1.4.2/cbcmgr/retry.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.1/cbcmgr/schema.py` & `cbcmgr-1.4.2/cbcmgr/schema.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.1/cbcmgr/util.py` & `cbcmgr-1.4.2/cbcmgr/util.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.4.1/cbcmgr.egg-info/PKG-INFO` & `cbcmgr-1.4.2/cbcmgr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.4.1
+Version: 1.4.2
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Keywords: couchbase,nosql,pycouchbase,database
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cbcmgr-1.4.1/setup.py` & `cbcmgr-1.4.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='cbcmgr',
-    version='1.4.1',
+    version='1.4.2',
     packages=['cbcmgr'],
     url='https://github.com/mminichino/cb-util',
     license='MIT License',
     author='Michael Minichino',
     python_requires='>=3.9',
     install_requires=[
         'attrs',
         'couchbase',
         'dnspython',
         'docker',
         'pytest',
+        'pytest-asyncio',
         'requests',
         'urllib3',
         'xmltodict'
     ],
     author_email='info@unix.us.com',
     description='Couchbase connection manager',
     long_description=long_description,
```

