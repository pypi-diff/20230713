# Comparing `tmp/aiohttp-ratelimiter-4.1.1.tar.gz` & `tmp/aiohttp-ratelimiter-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohttp-ratelimiter-4.1.1.tar", last modified: Mon Nov 28 01:18:06 2022, max compression
+gzip compressed data, was "aiohttp-ratelimiter-4.1.2.tar", last modified: Thu Jul 13 13:54:26 2023, max compression
```

## Comparing `aiohttp-ratelimiter-4.1.1.tar` & `aiohttp-ratelimiter-4.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-11-28 01:18:06.030070 aiohttp-ratelimiter-4.1.1/
--rw-rw-rw-   0        0        0     1094 2022-02-18 00:25:08.000000 aiohttp-ratelimiter-4.1.1/LICENSE
--rw-rw-rw-   0        0        0     3921 2022-11-28 01:18:06.030070 aiohttp-ratelimiter-4.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3342 2022-11-28 01:18:00.000000 aiohttp-ratelimiter-4.1.1/README.md
-drwxrwxrwx   0        0        0        0 2022-11-28 01:18:06.024070 aiohttp-ratelimiter-4.1.1/aiohttp_ratelimiter.egg-info/
--rw-rw-rw-   0        0        0     3921 2022-11-28 01:18:05.000000 aiohttp-ratelimiter-4.1.1/aiohttp_ratelimiter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2022-11-28 01:18:05.000000 aiohttp-ratelimiter-4.1.1/aiohttp_ratelimiter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-28 01:18:05.000000 aiohttp-ratelimiter-4.1.1/aiohttp_ratelimiter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2022-11-28 01:18:05.000000 aiohttp-ratelimiter-4.1.1/aiohttp_ratelimiter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2022-11-28 01:18:05.000000 aiohttp-ratelimiter-4.1.1/aiohttp_ratelimiter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-11-28 01:18:06.029059 aiohttp-ratelimiter-4.1.1/aiohttplimiter/
--rw-rw-rw-   0        0        0      101 2022-11-28 01:16:48.000000 aiohttp-ratelimiter-4.1.1/aiohttplimiter/__init__.py
--rw-rw-rw-   0        0        0     4021 2022-11-28 00:56:36.000000 aiohttp-ratelimiter-4.1.1/aiohttplimiter/limiter.py
--rw-rw-rw-   0        0        0     1826 2022-11-28 00:56:36.000000 aiohttp-ratelimiter-4.1.1/aiohttplimiter/memcached_limiter.py
--rw-rw-rw-   0        0        0     1734 2022-11-28 00:56:36.000000 aiohttp-ratelimiter-4.1.1/aiohttplimiter/memory_limiter.py
--rw-rw-rw-   0        0        0     1888 2022-11-28 00:56:36.000000 aiohttp-ratelimiter-4.1.1/aiohttplimiter/redis_limiter.py
--rw-rw-rw-   0        0        0       42 2022-11-28 01:18:06.030070 aiohttp-ratelimiter-4.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1069 2022-11-28 01:18:00.000000 aiohttp-ratelimiter-4.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 13:54:26.612323 aiohttp-ratelimiter-4.1.2/
+-rw-rw-rw-   0        0        0     1094 2022-07-17 09:01:58.000000 aiohttp-ratelimiter-4.1.2/LICENSE
+-rw-rw-rw-   0        0        0     3908 2023-07-13 13:54:26.612323 aiohttp-ratelimiter-4.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3329 2023-07-13 13:49:42.000000 aiohttp-ratelimiter-4.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 13:54:26.596701 aiohttp-ratelimiter-4.1.2/aiohttp_ratelimiter.egg-info/
+-rw-rw-rw-   0        0        0     3908 2023-07-13 13:54:26.000000 aiohttp-ratelimiter-4.1.2/aiohttp_ratelimiter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-07-13 13:54:26.000000 aiohttp-ratelimiter-4.1.2/aiohttp_ratelimiter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 13:54:26.000000 aiohttp-ratelimiter-4.1.2/aiohttp_ratelimiter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-07-13 13:54:26.000000 aiohttp-ratelimiter-4.1.2/aiohttp_ratelimiter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-13 13:54:26.000000 aiohttp-ratelimiter-4.1.2/aiohttp_ratelimiter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-13 13:54:26.612323 aiohttp-ratelimiter-4.1.2/aiohttplimiter/
+-rw-rw-rw-   0        0        0      101 2023-07-13 13:49:42.000000 aiohttp-ratelimiter-4.1.2/aiohttplimiter/__init__.py
+-rw-rw-rw-   0        0        0     4073 2023-07-13 13:52:56.000000 aiohttp-ratelimiter-4.1.2/aiohttplimiter/limiter.py
+-rw-rw-rw-   0        0        0     1826 2023-07-13 13:49:42.000000 aiohttp-ratelimiter-4.1.2/aiohttplimiter/memcached_limiter.py
+-rw-rw-rw-   0        0        0     1734 2023-07-13 13:49:42.000000 aiohttp-ratelimiter-4.1.2/aiohttplimiter/memory_limiter.py
+-rw-rw-rw-   0        0        0     1888 2023-07-13 13:49:42.000000 aiohttp-ratelimiter-4.1.2/aiohttplimiter/redis_limiter.py
+-rw-rw-rw-   0        0        0       42 2023-07-13 13:54:26.612323 aiohttp-ratelimiter-4.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1069 2023-07-13 13:53:57.000000 aiohttp-ratelimiter-4.1.2/setup.py
```

### Comparing `aiohttp-ratelimiter-4.1.1/LICENSE` & `aiohttp-ratelimiter-4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiohttp-ratelimiter-4.1.1/PKG-INFO` & `aiohttp-ratelimiter-4.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohttp-ratelimiter
-Version: 4.1.1
+Version: 4.1.2
 Summary: A simple rate limiter for aiohttp.web
 Home-page: https://jgltechnologies.com/aiohttplimiter
 Author: George Luca
 Author-email: fixingg@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -140,15 +140,15 @@
 
 Views Example 
 
 ```python
 @routes.view("/")
 class Home(View):
     @limiter.limit("1/second")
-    def get(self: web.Request):
+    def get(self):
         return web.Response(text="hello")
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aiohttp-ratelimiter Version: 4.1.1 Summary: A
+Metadata-Version: 2.1 Name: aiohttp-ratelimiter Version: 4.1.2 Summary: A
 simple rate limiter for aiohttp.web Home-page: https://jgltechnologies.com/
 aiohttplimiter Author: George Luca Author-email: fixingg@gmail.com License: MIT
 Platform: UNKNOWN Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Description-
 Content-Type: text/markdown Provides-Extra: memcached Provides-Extra: redis
 License-File: LICENSE [https://discord.com/api/guilds/844418702430175272/
@@ -43,8 +43,8 @@
 @routes.get("/home") @limiter.limit("5/hour") def home(request): return
 web.Response(text="Hello") ```
 Then they will have separate rate limits. To prevent this use the path_id
 kwarg. ```python @routes.get("/") @routes.get("/home") @limiter.limit("2/
 3days", path_id="home") def home(request): return web.Response(text="Hello")
 ```
 Views Example ```python @routes.view("/") class Home(View): @limiter.limit("1/
-second") def get(self: web.Request): return web.Response(text="hello") ```
+second") def get(self): return web.Response(text="hello") ```
```

### Comparing `aiohttp-ratelimiter-4.1.1/README.md` & `aiohttp-ratelimiter-4.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -122,13 +122,13 @@
 
 Views Example 
 
 ```python
 @routes.view("/")
 class Home(View):
     @limiter.limit("1/second")
-    def get(self: web.Request):
+    def get(self):
         return web.Response(text="hello")
 ```
```

#### html2text {}

```diff
@@ -35,8 +35,8 @@
 @routes.get("/home") @limiter.limit("5/hour") def home(request): return
 web.Response(text="Hello") ```
 Then they will have separate rate limits. To prevent this use the path_id
 kwarg. ```python @routes.get("/") @routes.get("/home") @limiter.limit("2/
 3days", path_id="home") def home(request): return web.Response(text="Hello")
 ```
 Views Example ```python @routes.view("/") class Home(View): @limiter.limit("1/
-second") def get(self: web.Request): return web.Response(text="hello") ```
+second") def get(self): return web.Response(text="hello") ```
```

### Comparing `aiohttp-ratelimiter-4.1.1/aiohttp_ratelimiter.egg-info/PKG-INFO` & `aiohttp-ratelimiter-4.1.2/aiohttp_ratelimiter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohttp-ratelimiter
-Version: 4.1.1
+Version: 4.1.2
 Summary: A simple rate limiter for aiohttp.web
 Home-page: https://jgltechnologies.com/aiohttplimiter
 Author: George Luca
 Author-email: fixingg@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -140,15 +140,15 @@
 
 Views Example 
 
 ```python
 @routes.view("/")
 class Home(View):
     @limiter.limit("1/second")
-    def get(self: web.Request):
+    def get(self):
         return web.Response(text="hello")
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aiohttp-ratelimiter Version: 4.1.1 Summary: A
+Metadata-Version: 2.1 Name: aiohttp-ratelimiter Version: 4.1.2 Summary: A
 simple rate limiter for aiohttp.web Home-page: https://jgltechnologies.com/
 aiohttplimiter Author: George Luca Author-email: fixingg@gmail.com License: MIT
 Platform: UNKNOWN Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Description-
 Content-Type: text/markdown Provides-Extra: memcached Provides-Extra: redis
 License-File: LICENSE [https://discord.com/api/guilds/844418702430175272/
@@ -43,8 +43,8 @@
 @routes.get("/home") @limiter.limit("5/hour") def home(request): return
 web.Response(text="Hello") ```
 Then they will have separate rate limits. To prevent this use the path_id
 kwarg. ```python @routes.get("/") @routes.get("/home") @limiter.limit("2/
 3days", path_id="home") def home(request): return web.Response(text="Hello")
 ```
 Views Example ```python @routes.view("/") class Home(View): @limiter.limit("1/
-second") def get(self: web.Request): return web.Response(text="hello") ```
+second") def get(self): return web.Response(text="hello") ```
```

### Comparing `aiohttp-ratelimiter-4.1.1/aiohttplimiter/limiter.py` & `aiohttp-ratelimiter-4.1.2/aiohttplimiter/limiter.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 import asyncio
 from aiohttp.web import Request, Response, View
 from limits.aio.storage import Storage, MemoryStorage
 from limits.aio.strategies import MovingWindowRateLimiter
 from limits import parse
 
 
-def default_keyfunc(request: Union[Request, View]) -> str:
+def default_keyfunc(ctx: Union[Request, View]) -> str:
     """
     Returns the user's IP
     """
-    if isinstance(request, View):
-        request = request.request
+    if isinstance(ctx, View):
+        request = ctx.request
+    else:
+        request = ctx
     ip = request.headers.get(
         "X-Forwarded-For") or request.remote or "127.0.0.1"
     ip = ip.split(",")[0]
     return ip
 
 
 class Allow:
@@ -51,17 +53,19 @@
         self.db = db
         self.error_handler = error_handler
         self.path_id = path_id
         self.moving_window = moving_window
 
     def __call__(self, func: Union[Callable, Awaitable]) -> Callable[[Union[Request, View]], Coroutine[Any, Any, Response]]:
         @wraps(func)
-        async def wrapper(request: Union[Request, View]) -> Response:
-            if isinstance(request, View):
-                request = request.request
+        async def wrapper(ctx: Union[Request, View]) -> Response:
+            if isinstance(ctx, View):
+                request = ctx.request
+            else:
+                request = ctx
             key = self.keyfunc(request)
             db_key = f"{key}:{self.path_id or request.path}"
 
             if isinstance(self.db, MemoryStorage):
                 if not await self.db.check():
                     await self.db.reset()
 
@@ -90,12 +94,12 @@
                     "error", f"Rate limit exceeded: {self.amount}")
                 return response
 
             # Increments the number of calls by 1
             await self.moving_window.hit(self.item, db_key)
             # Returns normal response if the user did not go over the rate limit
             if asyncio.iscoroutinefunction(func):
-                return await func(request)
+                return await func(ctx)
             else:
-                return func(request)
+                return func(ctx)
 
         return wrapper
```

### Comparing `aiohttp-ratelimiter-4.1.1/aiohttplimiter/memcached_limiter.py` & `aiohttp-ratelimiter-4.1.2/aiohttplimiter/memcached_limiter.py`

 * *Files identical despite different names*

### Comparing `aiohttp-ratelimiter-4.1.1/aiohttplimiter/memory_limiter.py` & `aiohttp-ratelimiter-4.1.2/aiohttplimiter/memory_limiter.py`

 * *Files identical despite different names*

### Comparing `aiohttp-ratelimiter-4.1.1/aiohttplimiter/redis_limiter.py` & `aiohttp-ratelimiter-4.1.2/aiohttplimiter/redis_limiter.py`

 * *Files identical despite different names*

### Comparing `aiohttp-ratelimiter-4.1.1/setup.py` & `aiohttp-ratelimiter-4.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 def get_long_description():
     with open("README.md", encoding="utf-8") as file:
         return file.read()
 
 
-VERSION = "4.1.1"
+VERSION = "4.1.2"
 
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
```

