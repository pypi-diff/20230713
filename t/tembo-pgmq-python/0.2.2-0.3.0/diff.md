# Comparing `tmp/tembo_pgmq_python-0.2.2.tar.gz` & `tmp/tembo_pgmq_python-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tembo_pgmq_python-0.2.2.tar", max compression
+gzip compressed data, was "tembo_pgmq_python-0.3.0.tar", max compression
```

## Comparing `tembo_pgmq_python-0.2.2.tar` & `tembo_pgmq_python-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1491 2023-06-20 16:10:14.149884 tembo_pgmq_python-0.2.2/README.md
--rw-r--r--   0        0        0     1168 2023-06-20 16:10:14.149884 tembo_pgmq_python-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      105 2023-06-20 16:10:14.149884 tembo_pgmq_python-0.2.2/tembo_pgmq_python/__init__.py
--rw-r--r--   0        0        0     4371 2023-06-20 16:10:14.149884 tembo_pgmq_python-0.2.2/tembo_pgmq_python/queue.py
--rw-r--r--   0        0        0     2278 1970-01-01 00:00:00.000000 tembo_pgmq_python-0.2.2/setup.py
--rw-r--r--   0        0        0     2389 1970-01-01 00:00:00.000000 tembo_pgmq_python-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-07-13 03:34:35.192602 tembo_pgmq_python-0.3.0/README.md
+-rw-r--r--   0        0        0     1168 2023-07-13 03:34:35.192602 tembo_pgmq_python-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      105 2023-07-13 03:34:35.192602 tembo_pgmq_python-0.3.0/tembo_pgmq_python/__init__.py
+-rw-r--r--   0        0        0     4651 2023-07-13 03:34:35.192602 tembo_pgmq_python-0.3.0/tembo_pgmq_python/queue.py
+-rw-r--r--   0        0        0     2278 1970-01-01 00:00:00.000000 tembo_pgmq_python-0.3.0/setup.py
+-rw-r--r--   0        0        0     2389 1970-01-01 00:00:00.000000 tembo_pgmq_python-0.3.0/PKG-INFO
```

### Comparing `tembo_pgmq_python-0.2.2/README.md` & `tembo_pgmq_python-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tembo_pgmq_python-0.2.2/pyproject.toml` & `tembo_pgmq_python-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tembo-pgmq-python"
-version = "0.2.2"
+version = "0.3.0"
 description = "Python client for the PGMQ Postgres extension."
 authors = ["Adam Hendel <adam@tembo.io>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "tembo_pgmq_python"}]
 
 [tool.poetry.urls]
```

### Comparing `tembo_pgmq_python-0.2.2/tembo_pgmq_python/queue.py` & `tembo_pgmq_python-0.3.0/tembo_pgmq_python/queue.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,15 +43,17 @@
         password={self.password}
         """
         self.pool = ConnectionPool(conninfo, **self.kwargs)
 
         with self.pool.connection() as conn:
             conn.execute("create extension if not exists pgmq cascade;")
 
-    def create_queue(self, queue: str, partition_interval: int = 10000, retention_interval: int = 100000) -> None:
+    def create_partitioned_queue(
+        self, queue: str, partition_interval: int = 10000, retention_interval: int = 100000
+    ) -> None:
         """Create a new queue
 
         Note: Partitions are created pg_partman which must be configured in postgresql.conf
             Set `pg_partman_bgw.interval` to set the interval for partition creation and deletion.
             A value of 10 will create new/delete partitions every 10 seconds. This value should be tuned
             according to the volume of messages being sent to the queue.
 
@@ -61,14 +63,23 @@
             retention_interval: The number of messages to retain. Messages exceeding this number will be dropped.
                 Defaults to 100,000.
         """
 
         with self.pool.connection() as conn:
             conn.execute("select pgmq_create(%s, %s::text, %s::text);", [queue, partition_interval, retention_interval])
 
+    def create_queue(self, queue: str) -> None:
+        """Create a new queue
+        Args:
+            queue: The name of the queue.
+        """
+
+        with self.pool.connection() as conn:
+            conn.execute("select pgmq_create(%s);", [queue])
+
     def send(self, queue: str, message: dict, delay: Optional[int] = None) -> int:
         """Send a message to a queue"""
 
         with self.pool.connection() as conn:
             if delay is not None:
                 # TODO(chuckend): implement send_delay in pgmq
                 raise NotImplementedError("send_delay is not implemented in pgmq")
```

### Comparing `tembo_pgmq_python-0.2.2/setup.py` & `tembo_pgmq_python-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['orjson>=3.8.10,<4.0.0',
  'psycopg[binary,pool]>=3.1.8,<4.0.0',
  'pydantic>=1.10.7,<2.0.0']
 
 setup_kwargs = {
     'name': 'tembo-pgmq-python',
-    'version': '0.2.2',
+    'version': '0.3.0',
     'description': 'Python client for the PGMQ Postgres extension.',
     'long_description': '# Tembo\'s Python Client for PGMQ\n\n## Installation\n\nInstall with `pip` from pypi.org\n\n```bash\npip install tembo-pgmq-python\n```\n\nDependencies:\n\nPostgres running the [Tembo PGMQ extension](https://github.com/tembo-io/tembo/tree/main/pgmq).\n\n## Usage\n\n## Start a Postgres Instance with the Tembo extension installed\n\n```bash\ndocker run -d --name postgres -e POSTGRES_PASSWORD=postgres -p 5432:5432 quay.io/coredb/pgmq-pg:latest\n```\n\nInitialize a connection to Postgres\n\n```python\nfrom tembo_pgmq_python import PGMQueue, Message\n\nqueue = PGMQueue(host="0.0.0.0")\n```\n\nCreate a queue (or a partitioned queue)\n\n```python\nqueue.create_queue("my_queue")\n# queue.create_partitioned_queue("my_partitioned_queue", partition_size=10000)\n```\n\n\nSend a message\n\n```python\nmsg_id: int = queue.send("my_queue", {"hello": "world"})\n```\n\nRead a message, set it invisible for 30 seconds.\n\n```python\nread_message: Message = queue.read("my_queue", vt=10)\nprint(read_message)\n```\n\nArchive the message after we\'re done with it. Archived messages are moved to an archive table.\n\n```python\narchived: bool = queue.archive("my_queue", read_message.msg_id)\n```\n\nDelete a message completely.\n\n```python\nmsg_id: int = queue.send("my_queue", {"hello": "world"})\nread_message: Message = queue.read("my_queue")\ndeleted: bool = queue.delete("my_queue", read_message.msg_id)\n```\n\nPop a message, deleting it and reading it in one transaction.\n\n```python\npopped_message: Message = queue.pop("my_queue")\nprint(popped_message)\n```\n',
     'author': 'Adam Hendel',
     'author_email': 'adam@tembo.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tembo_pgmq_python-0.2.2/PKG-INFO` & `tembo_pgmq_python-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tembo-pgmq-python
-Version: 0.2.2
+Version: 0.3.0
 Summary: Python client for the PGMQ Postgres extension.
 License: Apache 2.0
 Author: Adam Hendel
 Author-email: adam@tembo.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

