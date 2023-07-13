# Comparing `tmp/oxalis-0.6.4.tar.gz` & `tmp/oxalis-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oxalis-0.6.4.tar", max compression
+gzip compressed data, was "oxalis-0.6.5.tar", max compression
```

## Comparing `oxalis-0.6.4.tar` & `oxalis-0.6.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1065 2022-06-07 12:05:40.532331 oxalis-0.6.4/LICENSE
--rw-r--r--   0        0        0     6896 2023-04-20 05:15:02.504528 oxalis-0.6.4/README.md
--rw-r--r--   0        0        0       22 2022-06-03 10:29:06.678568 oxalis-0.6.4/oxalis/__init__.py
--rw-r--r--   0        0        0    11619 2023-06-15 05:51:44.478143 oxalis-0.6.4/oxalis/amqp.py
--rw-r--r--   0        0        0     7314 2023-06-15 05:41:22.005127 oxalis-0.6.4/oxalis/base.py
--rw-r--r--   0        0        0     1978 2023-04-28 02:27:00.905636 oxalis-0.6.4/oxalis/beater.py
--rw-r--r--   0        0        0     7717 2023-06-20 07:00:16.938574 oxalis-0.6.4/oxalis/kafka.py
--rw-r--r--   0        0        0     3542 2023-06-15 05:41:58.004260 oxalis-0.6.4/oxalis/pool.py
--rw-r--r--   0        0        0     7448 2023-05-12 06:41:48.719578 oxalis-0.6.4/oxalis/redis.py
--rw-r--r--   0        0        0      884 2023-06-20 06:58:30.369161 oxalis-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     7653 1970-01-01 00:00:00.000000 oxalis-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-06-07 12:05:40.532331 oxalis-0.6.5/LICENSE
+-rw-r--r--   0        0        0     6896 2023-04-20 05:15:02.504528 oxalis-0.6.5/README.md
+-rw-r--r--   0        0        0       22 2022-06-03 10:29:06.678568 oxalis-0.6.5/oxalis/__init__.py
+-rw-r--r--   0        0        0    11619 2023-06-15 05:51:44.478143 oxalis-0.6.5/oxalis/amqp.py
+-rw-r--r--   0        0        0     7314 2023-06-15 05:41:22.005127 oxalis-0.6.5/oxalis/base.py
+-rw-r--r--   0        0        0     2127 2023-07-10 06:07:13.253229 oxalis-0.6.5/oxalis/beater.py
+-rw-r--r--   0        0        0     7808 2023-07-13 06:59:15.172994 oxalis-0.6.5/oxalis/kafka.py
+-rw-r--r--   0        0        0     3542 2023-06-15 05:41:58.004260 oxalis-0.6.5/oxalis/pool.py
+-rw-r--r--   0        0        0     7448 2023-05-12 06:41:48.719578 oxalis-0.6.5/oxalis/redis.py
+-rw-r--r--   0        0        0      884 2023-07-13 07:17:47.578235 oxalis-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     7653 1970-01-01 00:00:00.000000 oxalis-0.6.5/PKG-INFO
```

### Comparing `oxalis-0.6.4/LICENSE` & `oxalis-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `oxalis-0.6.4/README.md` & `oxalis-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `oxalis-0.6.4/oxalis/amqp.py` & `oxalis-0.6.5/oxalis/amqp.py`

 * *Files identical despite different names*

### Comparing `oxalis-0.6.4/oxalis/base.py` & `oxalis-0.6.5/oxalis/base.py`

 * *Files identical despite different names*

### Comparing `oxalis-0.6.4/oxalis/beater.py` & `oxalis-0.6.5/oxalis/beater.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,20 @@
         self.tasks.append(task)
         self.crons.append(cron)
         self.croniteres.append(croniter(cron))
 
     async def beat(self, i: int):
         t = self.croniteres[i].get_next() - time.time()
         await asyncio.sleep(t)
-        await self.tasks[i].delay()
-        logger.info(f"Beat task {self.tasks[i]}")
+        try:
+            await self.tasks[i].delay()
+            logger.info(f"Beat task {self.tasks[i]}")
+        except Exception as e:
+            logger.warning(f"Beat task {self.tasks[i]} failed:")
+            logger.exception(e)
         self.futures[i] = asyncio.ensure_future(self.beat(i))
 
     async def _run(self):
         with open(self.oxalis.READY_FILE_PATH, "w") as f:
             f.write(f"{time.time():.0f}\n")
         while self.running:
             with open(self.oxalis.HEARTBEAT_FILE_PATH, "w") as f:
```

### Comparing `oxalis-0.6.4/oxalis/kafka.py` & `oxalis-0.6.5/oxalis/kafka.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,16 @@
             request_timeout_ms=int(self.timeout * 1000),
             **self.producer_kwargs,
         )
         await self.producer.start()
 
     async def disconnect(self):
         await self.producer.stop()
+        for consumer in self.consumers:
+            await consumer.stop()
 
     async def send_task(self, task: Task, *task_args, **task_kwargs):
         if task.name not in self.tasks:
             raise ValueError(f"Task {task} not register")
         logger.debug(f"Send task {task} to worker...")
         await self.producer.send_and_wait(
             task.topic.name,
@@ -230,14 +232,14 @@
                         await asyncio.wait([asyncio.ensure_future(cor) for cor in cors])
         except Exception as e:
             self.health = False
             raise e from None
         finally:
             if consumer_started:
                 await asyncio.sleep(self.timeout)  # wait for committing
-                await consumer.stop()
+                consumer.pause(*consumer.assignment())
             self.consuming_count -= 1
 
     def _run_worker(self):
         for t in self.topics:
             for _ in range(t.consumer_count):
                 asyncio.ensure_future(self._start_consumer(t))
```

### Comparing `oxalis-0.6.4/oxalis/pool.py` & `oxalis-0.6.5/oxalis/pool.py`

 * *Files identical despite different names*

### Comparing `oxalis-0.6.4/oxalis/redis.py` & `oxalis-0.6.5/oxalis/redis.py`

 * *Files identical despite different names*

### Comparing `oxalis-0.6.4/pyproject.toml` & `oxalis-0.6.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oxalis"
-version = "0.6.4"
+version = "0.6.5"
 description = "Distributed async task/job queue"
 authors = ["strongbugman <strongbugman@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers=[
     "Environment :: Console",
     "Programming Language :: Python :: 3.10",
```

### Comparing `oxalis-0.6.4/PKG-INFO` & `oxalis-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxalis
-Version: 0.6.4
+Version: 0.6.5
 Summary: Distributed async task/job queue
 License: MIT
 Author: strongbugman
 Author-email: strongbugman@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
```

