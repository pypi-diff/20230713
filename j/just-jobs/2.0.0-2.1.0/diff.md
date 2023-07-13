# Comparing `tmp/just_jobs-2.0.0.tar.gz` & `tmp/just_jobs-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "just_jobs-2.0.0.tar", last modified: Sat May  6 03:01:22 2023, max compression
+gzip compressed data, was "just_jobs-2.1.0.tar", last modified: Thu Jul 13 04:10:28 2023, max compression
```

## Comparing `just_jobs-2.0.0.tar` & `just_jobs-2.1.0.tar`

### file list

```diff
@@ -1,12 +1,18 @@
--rw-r--r--   0        0        0     1683 2023-05-06 03:00:07.988141 just_jobs-2.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1462 2023-05-06 02:17:56.635972 just_jobs-2.0.0/LICENSE
--rw-r--r--   0        0        0     7262 2023-05-06 02:17:56.820059 just_jobs-2.0.0/README.md
--rw-r--r--   0        0        0        0 2021-07-24 20:17:02.002842 just_jobs-2.0.0/just_jobs/py.typed
--rw-r--r--   0        0        0     1043 2023-05-06 03:01:22.722490 just_jobs-2.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-30 18:43:21.184656 just_jobs-2.0.0/tests/__init__.py
--rw-r--r--   0        0        0     1064 2023-05-06 02:17:56.436966 just_jobs-2.0.0/tests/conftest.py
--rw-r--r--   0        0        0      848 2023-05-06 01:36:07.154826 just_jobs-2.0.0/tests/test_broker.py
--rw-r--r--   0        0        0     2197 2023-05-06 02:17:56.437970 just_jobs-2.0.0/tests/test_job.py
--rw-r--r--   0        0        0     1436 2023-05-06 01:36:07.156496 just_jobs-2.0.0/tests/test_settings.py
--rw-r--r--   0        0        0     1781 2023-05-06 01:36:07.157696 just_jobs-2.0.0/tests/test_utils.py
--rw-r--r--   0        0        0     7766 1970-01-01 00:00:00.000000 just_jobs-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1462 2023-05-06 02:17:56.635972 just_jobs-2.1.0/LICENSE
+-rw-r--r--   0        0        0     7150 2023-07-13 04:09:45.934624 just_jobs-2.1.0/README.md
+-rw-r--r--   0        0        0      205 2023-05-06 01:36:07.144803 just_jobs-2.1.0/just_jobs/__init__.py
+-rw-r--r--   0        0        0     1291 2023-05-06 01:36:07.145950 just_jobs-2.1.0/just_jobs/broker.py
+-rw-r--r--   0        0        0      729 2023-05-06 01:36:07.146500 just_jobs-2.1.0/just_jobs/job_type.py
+-rw-r--r--   0        0        0     4518 2023-07-13 04:09:45.938620 just_jobs-2.1.0/just_jobs/jobs.py
+-rw-r--r--   0        0        0        0 2021-07-24 20:17:02.002842 just_jobs-2.1.0/just_jobs/py.typed
+-rw-r--r--   0        0        0     4342 2023-05-06 01:36:07.148678 just_jobs-2.1.0/just_jobs/settings.py
+-rw-r--r--   0        0        0      323 2023-05-06 01:36:07.149245 just_jobs-2.1.0/just_jobs/typing.py
+-rw-r--r--   0        0        0     1548 2023-05-06 01:36:07.149774 just_jobs-2.1.0/just_jobs/utils.py
+-rw-r--r--   0        0        0     1094 2023-07-13 04:10:28.161795 just_jobs-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-30 18:43:21.184656 just_jobs-2.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     1064 2023-05-06 02:17:56.436966 just_jobs-2.1.0/tests/conftest.py
+-rw-r--r--   0        0        0      848 2023-05-06 01:36:07.154826 just_jobs-2.1.0/tests/test_broker.py
+-rw-r--r--   0        0        0     2584 2023-07-13 04:09:45.941622 just_jobs-2.1.0/tests/test_job.py
+-rw-r--r--   0        0        0     1436 2023-05-06 01:36:07.156496 just_jobs-2.1.0/tests/test_settings.py
+-rw-r--r--   0        0        0     1781 2023-05-06 01:36:07.157696 just_jobs-2.1.0/tests/test_utils.py
+-rw-r--r--   0        0        0     7851 1970-01-01 00:00:00.000000 just_jobs-2.1.0/PKG-INFO
```

### Comparing `just_jobs-2.0.0/LICENSE` & `just_jobs-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `just_jobs-2.0.0/README.md` & `just_jobs-2.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ## Features
 
 just-jobs doesn't aim to replace the invocations that arq provides, only wrap some of them to make job creation and execution easier and better. It lets you:
 
 - Define and run non-async jobs. Passing a non-async `@job` function to arq will run properly. Non-async jobs can also be defined as either IO-bound or CPU-bound, which changes how the job will be executed to prevent blocking the asyncio event loop.
 - The arq `Context` parameter now works a lot like [FastAPI's `Request`](https://fastapi.tiangolo.com/advanced/using-request-directly/). It's no longer a required parameter, but if it exists, it will get set. It doesn't have to be named `ctx` either, only have the type `Context`.
 - Specify a single `RedisSettings` within your `WorkerSettings` from which you can create a pool using `Settings.create_pool()`.
-- Run jobs either immediately with the `.now()` function or via normal arq enqueueing.
+- Run jobs either immediately or via normal arq enqueueing.
 - Use non-pickable job arguments and kwargs (supported by the [dill](http://dill.rtfd.io/) library).
 
 ## Usage
 
 Using just-jobs is pretty straight forward:
 
 ### Add `@job()` to any function to make it a delayable job.
@@ -43,29 +43,29 @@
 If it's a coroutine function, you don't need to specify a job type (and will get a warning if you do).
 
 ```python
 @job()
 async def poll_reddit(subr: str)
 ```
 
-### Use `.now` if you want to run the job immediately.
+### Invoke a job normally if you want to run it immediately.
 
-Using `.now` allows you to run the job as if it were a normal function. If you have logic that you only want to execute when enqueued, include a parameter with type `Context` and check if it exists at runtime (functions with a `Context` that are run immediately will have that argument set to `None`).
+Invoking a job as a regular function allows you to run a job as if it were one. If you have logic that you only want to execute when enqueued, include a parameter with type `Context` and check if it exists at runtime (functions with a `Context` that are run immediately will have that argument set to `None`).
 
 ```python
 @job()
 async def context_aware(ctx: Context, msg: str):
     if ctx:
         # enqueued then run by arq
         return f"hello {msg}"
     else:
         # invoked manually
         return f"bye {msg}"
 
-await context_aware.now("world") == "bye world"
+await context_aware("world") == "bye world"
 
 j = await p.enqueue_job("context_aware", "world")
 await j.result() == "hello world"
 ```
 
 ### Define WorkerSettings using the `BaseSettings` metaclass.
 
@@ -106,15 +106,15 @@
    @job(job_type=JobType.CPU_BOUND, keep_result_forever=True, max_tries=10)
    def task(a: int, b: int):
       return a + b
    ```
 
 2. There isn't support for asynchronous CPU-bound tasks. Currently, job types only configure the execution behavior of synchronous tasks (not coroutines). However, there are some valid cases for CPU-bound tasks that also need to be run in an asyncio context.
 
-   At the moment, the best way to achieve this will be to create a synchronous CPU-bound task (so it runs in a separate process) that then invokes a coroutine via `asyncio.run`. If you intend on running the task in the current context from time to time (with `.now`), just return the coroutine instead and it will get automatically executed in the current event loop.
+   At the moment, the best way to achieve this will be to create a synchronous CPU-bound task (so it runs in a separate process) that then invokes a coroutine via `asyncio.run`. If you intend on running the task in the current context from time to time, just return the coroutine instead and it will get automatically executed in the current event loop.
 
    ```python
    async _async_task(a: int, b: int, c: int):
        ab = await add(a, b)
        return await add(ab, c)
 
    @job(job_type=JobType.CPU_BOUND)
@@ -145,16 +145,15 @@
     functions = [async_task, sync_task]
     redis_settings = RedisSettings(host="redis")
 
 async def main():
     # create a Redis pool using the Settings already defined
     pool = await Settings.create_pool()
     # run the_task right now and return the url
-    # even though this is a sync function, `.now` returns an awaitable
-    url = await sync_task.now("https://www.theglassfiles.com")
+    url = sync_task("https://www.theglassfiles.com")
 
     await pool.enqueue_job("async_task", "https://www.eliasfgabriel.com")
     await pool.enqueue_job("sync_task", "https://gianturl.net")
 
     await pool.close(close_connection_pool=True)
 ```
```

### Comparing `just_jobs-2.0.0/pyproject.toml` & `just_jobs-2.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "just-jobs"
 description = "A friendly and lightweight wrapper for arq."
-version = "2.0.0"
+version = "2.1.0"
 authors = [
     { name = "Elias Gabriel", email = "me@eliasfgabriel.com" },
 ]
 readme = "README.md"
 keywords = [
     "jobs",
     "arq",
@@ -20,22 +20,18 @@
     "dill>=0.3.6",
 ]
 
 [project.license]
 text = "BSD-3-Clause"
 
 [project.urls]
-repository = "https://github.com/thearchitector/just-jobs"
+homepage = "https://justjobs.thearchitector.dev"
 documentation = "https://justjobs.thearchitector.dev"
-
-[tool.pdm.build]
-includes = [
-    "just_jobs/py.typed",
-    "CHANGELOG.md",
-]
+changelog = "https://github.com/thearchitector/just-jobs/blob/main/CHANGELOG.md"
+repository = "https://github.com/thearchitector/just-jobs"
 
 [tool.pdm.scripts]
 docs = "pdoc -o docs --no-search just_jobs"
 
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest>=7.3.1",
```

### Comparing `just_jobs-2.0.0/tests/conftest.py` & `just_jobs-2.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `just_jobs-2.0.0/tests/test_broker.py` & `just_jobs-2.1.0/tests/test_broker.py`

 * *Files identical despite different names*

### Comparing `just_jobs-2.0.0/tests/test_job.py` & `just_jobs-2.1.0/tests/test_job.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,21 +35,34 @@
 
     task = f(val)
     return asyncio.run(task) if ctx else task
 
 
 @pytest.mark.parametrize("func", [async_task, cpu_task, io_task, async_cpu_task])
 async def test_invoke_now(func):
-    res = await func.now(" on ")
+    with pytest.deprecated_call():
+        res = await func.now(" on ")
+        assert res == f"{getpid()} on {get_ident()}"
+
+
+@pytest.mark.parametrize("func", [async_task, async_cpu_task])
+async def test_invoke_async_now(func):
+    res = await func(" on ")
+    assert res == f"{getpid()} on {get_ident()}"
+
+
+@pytest.mark.parametrize("func", [cpu_task, io_task])
+async def test_invoke_sync_now(func):
+    res = func(" on ")
     assert res == f"{getpid()} on {get_ident()}"
 
 
 async def test_failing_now():
     with pytest.raises(Exception, match="mock"):
-        await failing_task.now()
+        await failing_task()
 
 
 async def test_enqueue_job_async(enqueue_run_job):
     # test async is on same process and thread
     job = await enqueue_run_job(async_task, " on ")
     res = await job.result(poll_delay=0)
     assert res == f"{getpid()} on {get_ident()}"
```

### Comparing `just_jobs-2.0.0/tests/test_settings.py` & `just_jobs-2.1.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `just_jobs-2.0.0/tests/test_utils.py` & `just_jobs-2.1.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `just_jobs-2.0.0/PKG-INFO` & `just_jobs-2.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: just-jobs
-Version: 2.0.0
+Version: 2.1.0
 Summary: A friendly and lightweight wrapper for arq.
 Keywords: jobs arq tasks celery redis
+Home-page: https://justjobs.thearchitector.dev
 Author-Email: Elias Gabriel <me@eliasfgabriel.com>
 License: BSD-3-Clause
-Project-URL: Repository, https://github.com/thearchitector/just-jobs
+Project-URL: Homepage, https://justjobs.thearchitector.dev
 Project-URL: Documentation, https://justjobs.thearchitector.dev
+Project-URL: Changelog, https://github.com/thearchitector/just-jobs/blob/main/CHANGELOG.md
+Project-URL: Repository, https://github.com/thearchitector/just-jobs
 Requires-Python: <4.0,>=3.7
 Requires-Dist: arq>=0.25.0
 Requires-Dist: colorama>=0.4.6
 Requires-Dist: dill>=0.3.6
 Description-Content-Type: text/markdown
 
 # just-jobs
@@ -35,15 +38,15 @@
 ## Features
 
 just-jobs doesn't aim to replace the invocations that arq provides, only wrap some of them to make job creation and execution easier and better. It lets you:
 
 - Define and run non-async jobs. Passing a non-async `@job` function to arq will run properly. Non-async jobs can also be defined as either IO-bound or CPU-bound, which changes how the job will be executed to prevent blocking the asyncio event loop.
 - The arq `Context` parameter now works a lot like [FastAPI's `Request`](https://fastapi.tiangolo.com/advanced/using-request-directly/). It's no longer a required parameter, but if it exists, it will get set. It doesn't have to be named `ctx` either, only have the type `Context`.
 - Specify a single `RedisSettings` within your `WorkerSettings` from which you can create a pool using `Settings.create_pool()`.
-- Run jobs either immediately with the `.now()` function or via normal arq enqueueing.
+- Run jobs either immediately or via normal arq enqueueing.
 - Use non-pickable job arguments and kwargs (supported by the [dill](http://dill.rtfd.io/) library).
 
 ## Usage
 
 Using just-jobs is pretty straight forward:
 
 ### Add `@job()` to any function to make it a delayable job.
@@ -58,29 +61,29 @@
 If it's a coroutine function, you don't need to specify a job type (and will get a warning if you do).
 
 ```python
 @job()
 async def poll_reddit(subr: str)
 ```
 
-### Use `.now` if you want to run the job immediately.
+### Invoke a job normally if you want to run it immediately.
 
-Using `.now` allows you to run the job as if it were a normal function. If you have logic that you only want to execute when enqueued, include a parameter with type `Context` and check if it exists at runtime (functions with a `Context` that are run immediately will have that argument set to `None`).
+Invoking a job as a regular function allows you to run a job as if it were one. If you have logic that you only want to execute when enqueued, include a parameter with type `Context` and check if it exists at runtime (functions with a `Context` that are run immediately will have that argument set to `None`).
 
 ```python
 @job()
 async def context_aware(ctx: Context, msg: str):
     if ctx:
         # enqueued then run by arq
         return f"hello {msg}"
     else:
         # invoked manually
         return f"bye {msg}"
 
-await context_aware.now("world") == "bye world"
+await context_aware("world") == "bye world"
 
 j = await p.enqueue_job("context_aware", "world")
 await j.result() == "hello world"
 ```
 
 ### Define WorkerSettings using the `BaseSettings` metaclass.
 
@@ -121,15 +124,15 @@
    @job(job_type=JobType.CPU_BOUND, keep_result_forever=True, max_tries=10)
    def task(a: int, b: int):
       return a + b
    ```
 
 2. There isn't support for asynchronous CPU-bound tasks. Currently, job types only configure the execution behavior of synchronous tasks (not coroutines). However, there are some valid cases for CPU-bound tasks that also need to be run in an asyncio context.
 
-   At the moment, the best way to achieve this will be to create a synchronous CPU-bound task (so it runs in a separate process) that then invokes a coroutine via `asyncio.run`. If you intend on running the task in the current context from time to time (with `.now`), just return the coroutine instead and it will get automatically executed in the current event loop.
+   At the moment, the best way to achieve this will be to create a synchronous CPU-bound task (so it runs in a separate process) that then invokes a coroutine via `asyncio.run`. If you intend on running the task in the current context from time to time, just return the coroutine instead and it will get automatically executed in the current event loop.
 
    ```python
    async _async_task(a: int, b: int, c: int):
        ab = await add(a, b)
        return await add(ab, c)
 
    @job(job_type=JobType.CPU_BOUND)
@@ -160,16 +163,15 @@
     functions = [async_task, sync_task]
     redis_settings = RedisSettings(host="redis")
 
 async def main():
     # create a Redis pool using the Settings already defined
     pool = await Settings.create_pool()
     # run the_task right now and return the url
-    # even though this is a sync function, `.now` returns an awaitable
-    url = await sync_task.now("https://www.theglassfiles.com")
+    url = sync_task("https://www.theglassfiles.com")
 
     await pool.enqueue_job("async_task", "https://www.eliasfgabriel.com")
     await pool.enqueue_job("sync_task", "https://gianturl.net")
 
     await pool.close(close_connection_pool=True)
 ```
```

