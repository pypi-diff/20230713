# Comparing `tmp/starlette-0.9.8.tar.gz` & `tmp/starlette-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/starlette-0.9.8.tar", last modified: Mon Dec 10 14:37:49 2018, max compression
+gzip compressed data, was "dist/starlette-0.9.9.tar", last modified: Fri Dec 14 16:23:34 2018, max compression
```

## Comparing `starlette-0.9.8.tar` & `starlette-0.9.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2018-12-10 14:37:49.000000 starlette-0.9.8/
--rw-r--r--   0 tomchristie   (501) staff       (20)     7602 2018-12-10 14:37:49.000000 starlette-0.9.8/PKG-INFO
-drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2018-12-10 14:37:49.000000 starlette-0.9.8/starlette.egg-info/
--rw-r--r--   0 tomchristie   (501) staff       (20)     7602 2018-12-10 14:37:48.000000 starlette-0.9.8/starlette.egg-info/PKG-INFO
--rw-r--r--   0 tomchristie   (501) staff       (20)     1152 2018-12-10 14:37:48.000000 starlette-0.9.8/starlette.egg-info/SOURCES.txt
--rw-r--r--   0 tomchristie   (501) staff       (20)       96 2018-12-10 14:37:48.000000 starlette-0.9.8/starlette.egg-info/requires.txt
--rw-r--r--   0 tomchristie   (501) staff       (20)       50 2018-12-10 14:37:48.000000 starlette-0.9.8/starlette.egg-info/top_level.txt
--rw-r--r--   0 tomchristie   (501) staff       (20)        1 2018-12-10 14:37:48.000000 starlette-0.9.8/starlette.egg-info/dependency_links.txt
-drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2018-12-10 14:37:49.000000 starlette-0.9.8/starlette/
-drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2018-12-10 14:37:49.000000 starlette-0.9.8/starlette/middleware/
--rw-r--r--   0 tomchristie   (501) staff       (20)     3751 2018-11-23 11:50:25.000000 starlette-0.9.8/starlette/middleware/gzip.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     2740 2018-12-06 10:44:39.000000 starlette-0.9.8/starlette/middleware/sessions.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     6462 2018-11-23 11:50:25.000000 starlette-0.9.8/starlette/middleware/cors.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     2813 2018-12-06 10:43:11.000000 starlette-0.9.8/starlette/middleware/database.py
--rw-r--r--   0 tomchristie   (501) staff       (20)        0 2018-11-23 11:50:25.000000 starlette-0.9.8/starlette/middleware/__init__.py
--rw-r--r--   0 tomchristie   (501) staff       (20)      671 2018-11-23 11:50:25.000000 starlette-0.9.8/starlette/middleware/httpsredirect.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     1803 2018-11-23 11:50:25.000000 starlette-0.9.8/starlette/middleware/trustedhost.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     1282 2018-12-07 14:56:14.000000 starlette-0.9.8/starlette/middleware/authentication.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     5110 2018-11-23 11:50:25.000000 starlette-0.9.8/starlette/middleware/errors.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     2330 2018-11-23 11:50:25.000000 starlette-0.9.8/starlette/middleware/base.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     3943 2018-11-28 13:40:17.000000 starlette-0.9.8/starlette/middleware/lifespan.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     5052 2018-11-23 11:50:25.000000 starlette-0.9.8/starlette/middleware/wsgi.py
-drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2018-12-10 14:37:49.000000 starlette-0.9.8/starlette/database/
--rw-r--r--   0 tomchristie   (501) staff       (20)      260 2018-12-06 09:33:35.000000 starlette-0.9.8/starlette/database/__init__.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     2916 2018-12-10 14:37:46.000000 starlette-0.9.8/starlette/database/core.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     4823 2018-12-10 14:37:46.000000 starlette-0.9.8/starlette/database/postgres.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     9008 2018-12-06 09:33:35.000000 starlette-0.9.8/starlette/graphql.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     9612 2018-11-23 11:50:25.000000 starlette-0.9.8/starlette/responses.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     3579 2018-12-06 09:33:35.000000 starlette-0.9.8/starlette/config.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     5790 2018-11-23 11:50:25.000000 starlette-0.9.8/starlette/websockets.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     5437 2018-11-28 11:51:27.000000 starlette-0.9.8/starlette/applications.py
--rw-r--r--   0 tomchristie   (501) staff       (20)      795 2018-11-23 11:50:25.000000 starlette-0.9.8/starlette/concurrency.py
--rw-r--r--   0 tomchristie   (501) staff       (20)      561 2018-11-23 11:50:25.000000 starlette-0.9.8/starlette/background.py
--rw-r--r--   0 tomchristie   (501) staff       (20)       22 2018-12-10 14:37:46.000000 starlette-0.9.8/starlette/__init__.py
--rw-r--r--   0 tomchristie   (501) staff       (20)      349 2018-12-07 10:02:51.000000 starlette-0.9.8/starlette/types.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     1755 2018-11-23 11:50:25.000000 starlette-0.9.8/starlette/convertors.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     4072 2018-11-23 11:50:25.000000 starlette-0.9.8/starlette/staticfiles.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     3147 2018-11-23 15:20:18.000000 starlette-0.9.8/starlette/schemas.py
--rw-r--r--   0 tomchristie   (501) staff       (20)    16969 2018-11-28 11:51:27.000000 starlette-0.9.8/starlette/routing.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     2717 2018-12-07 13:05:43.000000 starlette-0.9.8/starlette/authentication.py
--rw-r--r--   0 tomchristie   (501) staff       (20)    14616 2018-11-28 15:07:41.000000 starlette-0.9.8/starlette/testclient.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     3407 2018-11-23 11:50:25.000000 starlette-0.9.8/starlette/exceptions.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     5576 2018-12-07 13:05:43.000000 starlette-0.9.8/starlette/requests.py
--rw-r--r--   0 tomchristie   (501) staff       (20)    13849 2018-12-06 09:33:35.000000 starlette-0.9.8/starlette/datastructures.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     4334 2018-11-23 11:50:25.000000 starlette-0.9.8/starlette/endpoints.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     9025 2018-11-23 11:50:25.000000 starlette-0.9.8/starlette/formparsers.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     2441 2018-11-23 11:50:25.000000 starlette-0.9.8/starlette/status.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     5492 2018-12-07 13:06:40.000000 starlette-0.9.8/README.md
--rw-r--r--   0 tomchristie   (501) staff       (20)     1894 2018-12-07 13:05:43.000000 starlette-0.9.8/setup.py
--rw-r--r--   0 tomchristie   (501) staff       (20)       38 2018-12-10 14:37:49.000000 starlette-0.9.8/setup.cfg
+drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2018-12-14 16:23:34.000000 starlette-0.9.9/
+-rw-r--r--   0 tomchristie   (501) staff       (20)     7660 2018-12-14 16:23:34.000000 starlette-0.9.9/PKG-INFO
+drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2018-12-14 16:23:34.000000 starlette-0.9.9/starlette.egg-info/
+-rw-r--r--   0 tomchristie   (501) staff       (20)     7660 2018-12-14 16:23:34.000000 starlette-0.9.9/starlette.egg-info/PKG-INFO
+-rw-r--r--   0 tomchristie   (501) staff       (20)     1152 2018-12-14 16:23:34.000000 starlette-0.9.9/starlette.egg-info/SOURCES.txt
+-rw-r--r--   0 tomchristie   (501) staff       (20)      104 2018-12-14 16:23:34.000000 starlette-0.9.9/starlette.egg-info/requires.txt
+-rw-r--r--   0 tomchristie   (501) staff       (20)       50 2018-12-14 16:23:34.000000 starlette-0.9.9/starlette.egg-info/top_level.txt
+-rw-r--r--   0 tomchristie   (501) staff       (20)        1 2018-12-14 16:23:34.000000 starlette-0.9.9/starlette.egg-info/dependency_links.txt
+drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2018-12-14 16:23:34.000000 starlette-0.9.9/starlette/
+drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2018-12-14 16:23:34.000000 starlette-0.9.9/starlette/middleware/
+-rw-r--r--   0 tomchristie   (501) staff       (20)     3751 2018-11-23 11:50:25.000000 starlette-0.9.9/starlette/middleware/gzip.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     2740 2018-12-06 10:44:39.000000 starlette-0.9.9/starlette/middleware/sessions.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     6462 2018-11-23 11:50:25.000000 starlette-0.9.9/starlette/middleware/cors.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     2813 2018-12-06 10:43:11.000000 starlette-0.9.9/starlette/middleware/database.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)        0 2018-11-23 11:50:25.000000 starlette-0.9.9/starlette/middleware/__init__.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)      671 2018-11-23 11:50:25.000000 starlette-0.9.9/starlette/middleware/httpsredirect.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     1803 2018-11-23 11:50:25.000000 starlette-0.9.9/starlette/middleware/trustedhost.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     1282 2018-12-13 14:05:04.000000 starlette-0.9.9/starlette/middleware/authentication.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     5110 2018-12-13 14:05:04.000000 starlette-0.9.9/starlette/middleware/errors.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     2330 2018-12-13 14:05:04.000000 starlette-0.9.9/starlette/middleware/base.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     2618 2018-12-14 09:39:34.000000 starlette-0.9.9/starlette/middleware/lifespan.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     5052 2018-11-23 11:50:25.000000 starlette-0.9.9/starlette/middleware/wsgi.py
+drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2018-12-14 16:23:34.000000 starlette-0.9.9/starlette/database/
+-rw-r--r--   0 tomchristie   (501) staff       (20)      260 2018-12-06 09:33:35.000000 starlette-0.9.9/starlette/database/__init__.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     2916 2018-12-10 14:37:46.000000 starlette-0.9.9/starlette/database/core.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     4823 2018-12-10 14:37:46.000000 starlette-0.9.9/starlette/database/postgres.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     9190 2018-12-14 16:16:51.000000 starlette-0.9.9/starlette/graphql.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)    10679 2018-12-14 09:28:35.000000 starlette-0.9.9/starlette/responses.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     3579 2018-12-06 09:33:35.000000 starlette-0.9.9/starlette/config.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     5938 2018-12-14 09:28:35.000000 starlette-0.9.9/starlette/websockets.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     5437 2018-11-28 11:51:27.000000 starlette-0.9.9/starlette/applications.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)      795 2018-11-23 11:50:25.000000 starlette-0.9.9/starlette/concurrency.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)      996 2018-12-14 16:16:51.000000 starlette-0.9.9/starlette/background.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)       22 2018-12-14 16:22:57.000000 starlette-0.9.9/starlette/__init__.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)      349 2018-12-07 10:02:51.000000 starlette-0.9.9/starlette/types.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     1755 2018-11-23 11:50:25.000000 starlette-0.9.9/starlette/convertors.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     4072 2018-12-13 14:05:04.000000 starlette-0.9.9/starlette/staticfiles.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     3147 2018-11-23 15:20:18.000000 starlette-0.9.9/starlette/schemas.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)    16963 2018-12-13 14:05:04.000000 starlette-0.9.9/starlette/routing.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     2717 2018-12-07 13:05:43.000000 starlette-0.9.9/starlette/authentication.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)    14773 2018-12-14 09:28:35.000000 starlette-0.9.9/starlette/testclient.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     3407 2018-12-13 14:05:04.000000 starlette-0.9.9/starlette/exceptions.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     6062 2018-12-14 14:51:18.000000 starlette-0.9.9/starlette/requests.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)    14875 2018-12-14 16:22:57.000000 starlette-0.9.9/starlette/datastructures.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     4489 2018-12-13 14:05:04.000000 starlette-0.9.9/starlette/endpoints.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     9025 2018-11-23 11:50:25.000000 starlette-0.9.9/starlette/formparsers.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     2441 2018-11-23 11:50:25.000000 starlette-0.9.9/starlette/status.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)     5526 2018-12-13 12:21:11.000000 starlette-0.9.9/README.md
+-rw-r--r--   0 tomchristie   (501) staff       (20)     1917 2018-12-13 12:21:11.000000 starlette-0.9.9/setup.py
+-rw-r--r--   0 tomchristie   (501) staff       (20)       38 2018-12-14 16:23:34.000000 starlette-0.9.9/setup.cfg
```

### Comparing `starlette-0.9.8/PKG-INFO` & `starlette-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starlette
-Version: 0.9.8
+Version: 0.9.9
 Summary: The little ASGI library that shines.
 Home-page: https://github.com/encode/starlette
 Author: Tom Christie
 Author-email: tom@tomchristie.com
 License: BSD
 Description: <p align="center">
           <a href="https://www.starlette.io/"><img width="320" height="192" src="https://raw.githubusercontent.com/encode/starlette/master/docs/starlette.png" alt='starlette'></a>
@@ -26,14 +26,16 @@
         
         ---
         
         **Documentation**: [https://www.starlette.io/](https://www.starlette.io/)
         
         ---
         
+        # Starlette
+        
         Starlette is a lightweight [ASGI](https://asgi.readthedocs.io/en/latest/) framework/toolkit,
         which is ideal for building high performance asyncio services.
         
         It is production-ready, and gives you the following:
         
         * Seriously impressive performance.
         * WebSocket support.
@@ -68,23 +70,24 @@
         ```python
         from starlette.applications import Starlette
         from starlette.responses import JSONResponse
         import uvicorn
         
         app = Starlette()
         
+        
         @app.route('/')
         async def homepage(request):
             return JSONResponse({'hello': 'world'})
         
         if __name__ == '__main__':
             uvicorn.run(app, host='0.0.0.0', port=8000)
         ```
         
-        For a more complete example, [see here](https://github.com/encode/starlette-example).
+        For a more complete example, see [encode/starlette-example](https://github.com/encode/starlette-example).
         
         ## Dependencies
         
         Starlette does not have any hard dependencies, but the following are optional:
         
         * [`requests`][requests] - Required if you want to use the `TestClient`.
         * [`aiofiles`][aiofiles] - Required if you want to use `FileResponse` or `StaticFiles`.
```

### Comparing `starlette-0.9.8/starlette.egg-info/PKG-INFO` & `starlette-0.9.9/starlette.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starlette
-Version: 0.9.8
+Version: 0.9.9
 Summary: The little ASGI library that shines.
 Home-page: https://github.com/encode/starlette
 Author: Tom Christie
 Author-email: tom@tomchristie.com
 License: BSD
 Description: <p align="center">
           <a href="https://www.starlette.io/"><img width="320" height="192" src="https://raw.githubusercontent.com/encode/starlette/master/docs/starlette.png" alt='starlette'></a>
@@ -26,14 +26,16 @@
         
         ---
         
         **Documentation**: [https://www.starlette.io/](https://www.starlette.io/)
         
         ---
         
+        # Starlette
+        
         Starlette is a lightweight [ASGI](https://asgi.readthedocs.io/en/latest/) framework/toolkit,
         which is ideal for building high performance asyncio services.
         
         It is production-ready, and gives you the following:
         
         * Seriously impressive performance.
         * WebSocket support.
@@ -68,23 +70,24 @@
         ```python
         from starlette.applications import Starlette
         from starlette.responses import JSONResponse
         import uvicorn
         
         app = Starlette()
         
+        
         @app.route('/')
         async def homepage(request):
             return JSONResponse({'hello': 'world'})
         
         if __name__ == '__main__':
             uvicorn.run(app, host='0.0.0.0', port=8000)
         ```
         
-        For a more complete example, [see here](https://github.com/encode/starlette-example).
+        For a more complete example, see [encode/starlette-example](https://github.com/encode/starlette-example).
         
         ## Dependencies
         
         Starlette does not have any hard dependencies, but the following are optional:
         
         * [`requests`][requests] - Required if you want to use the `TestClient`.
         * [`aiofiles`][aiofiles] - Required if you want to use `FileResponse` or `StaticFiles`.
```

### Comparing `starlette-0.9.8/starlette.egg-info/SOURCES.txt` & `starlette-0.9.9/starlette.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `starlette-0.9.8/starlette/middleware/gzip.py` & `starlette-0.9.9/starlette/middleware/gzip.py`

 * *Files identical despite different names*

### Comparing `starlette-0.9.8/starlette/middleware/sessions.py` & `starlette-0.9.9/starlette/middleware/sessions.py`

 * *Files identical despite different names*

### Comparing `starlette-0.9.8/starlette/middleware/cors.py` & `starlette-0.9.9/starlette/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `starlette-0.9.8/starlette/middleware/database.py` & `starlette-0.9.9/starlette/middleware/database.py`

 * *Files identical despite different names*

### Comparing `starlette-0.9.8/starlette/middleware/httpsredirect.py` & `starlette-0.9.9/starlette/middleware/httpsredirect.py`

 * *Files identical despite different names*

### Comparing `starlette-0.9.8/starlette/middleware/trustedhost.py` & `starlette-0.9.9/starlette/middleware/trustedhost.py`

 * *Files identical despite different names*

### Comparing `starlette-0.9.8/starlette/middleware/authentication.py` & `starlette-0.9.9/starlette/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `starlette-0.9.8/starlette/middleware/errors.py` & `starlette-0.9.9/starlette/middleware/errors.py`

 * *Files identical despite different names*

### Comparing `starlette-0.9.8/starlette/middleware/base.py` & `starlette-0.9.9/starlette/middleware/base.py`

 * *Files identical despite different names*

### Comparing `starlette-0.9.8/starlette/middleware/wsgi.py` & `starlette-0.9.9/starlette/middleware/wsgi.py`

 * *Files identical despite different names*

### Comparing `starlette-0.9.8/starlette/database/core.py` & `starlette-0.9.9/starlette/database/core.py`

 * *Files identical despite different names*

### Comparing `starlette-0.9.8/starlette/database/postgres.py` & `starlette-0.9.9/starlette/database/postgres.py`

 * *Files identical despite different names*

### Comparing `starlette-0.9.8/starlette/graphql.py` & `starlette-0.9.9/starlette/graphql.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import functools
 import json
 import typing
 
 from starlette import status
+from starlette.background import BackgroundTasks
 from starlette.concurrency import run_in_threadpool
 from starlette.requests import Request
 from starlette.responses import HTMLResponse, JSONResponse, PlainTextResponse, Response
 from starlette.types import ASGIInstance, Receive, Scope, Send
 
 try:
     import graphene
@@ -69,31 +70,35 @@
             operation_name = data.get("operationName")
         except KeyError:
             return PlainTextResponse(
                 "No GraphQL query found in the request",
                 status_code=status.HTTP_400_BAD_REQUEST,
             )
 
-        result = await self.execute(request, query, variables)
+        background = BackgroundTasks()
+        context = {"request": request, "background": background}
+
+        result = await self.execute(query, variables=variables, context=context)
         error_data = (
             [format_graphql_error(err) for err in result.errors]
             if result.errors
             else None
         )
         response_data = {"data": result.data, "errors": error_data}
         status_code = (
             status.HTTP_400_BAD_REQUEST if result.errors else status.HTTP_200_OK
         )
-        return JSONResponse(response_data, status_code=status_code)
+
+        return JSONResponse(
+            response_data, status_code=status_code, background=background
+        )
 
     async def execute(  # type: ignore
-        self, request, query, variables=None, operation_name=None
+        self, query, variables=None, context=None, operation_name=None
     ):
-        context = dict(request=request)
-
         if self.is_async:
             return await self.schema.execute(
                 query,
                 variables=variables,
                 operation_name=operation_name,
                 executor=self.executor,
                 return_promise=True,
```

### Comparing `starlette-0.9.8/starlette/responses.py` & `starlette-0.9.9/starlette/responses.py`

 * *Files 4% similar despite different names*

```diff
@@ -134,14 +134,47 @@
     media_type = "text/html"
 
 
 class PlainTextResponse(Response):
     media_type = "text/plain"
 
 
+class TemplateResponse(Response):
+    media_type = "text/html"
+
+    def __init__(
+        self,
+        template: typing.Any,
+        context: dict,
+        status_code: int = 200,
+        headers: dict = None,
+        media_type: str = None,
+        background: BackgroundTask = None,
+    ):
+        if "request" not in context:
+            raise ValueError('context must include a "request" key')
+        self.template = template
+        self.context = context
+        content = template.render(context)
+        super().__init__(content, status_code, headers, media_type, background)
+
+    async def __call__(self, receive: Receive, send: Send) -> None:
+        request = self.context["request"]
+        extensions = request.get("extensions", {})
+        if "http.response.template" in extensions:
+            await send(
+                {
+                    "type": "http.response.template",
+                    "template": self.template,
+                    "context": self.context,
+                }
+            )
+        await super().__call__(receive, send)
+
+
 class JSONResponse(Response):
     media_type = "application/json"
 
     def render(self, content: typing.Any) -> bytes:
         return json.dumps(
             content,
             ensure_ascii=False,
```

### Comparing `starlette-0.9.8/starlette/config.py` & `starlette-0.9.9/starlette/config.py`

 * *Files identical despite different names*

### Comparing `starlette-0.9.8/starlette/websockets.py` & `starlette-0.9.9/starlette/websockets.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,71 +1,72 @@
 import enum
 import json
 import typing
 from collections.abc import Mapping
 
 from starlette.datastructures import URL, Headers, QueryParams
+from starlette.requests import HTTPConnection
 from starlette.types import Message, Receive, Scope, Send
 
 
 class WebSocketState(enum.Enum):
     CONNECTING = 0
     CONNECTED = 1
     DISCONNECTED = 2
 
 
 class WebSocketDisconnect(Exception):
     def __init__(self, code: int = 1000) -> None:
         self.code = code
 
 
-class WebSocket(Mapping):
+class WebSocket(HTTPConnection):
     def __init__(self, scope: Scope, receive: Receive, send: Send) -> None:
+        super().__init__(scope)
         assert scope["type"] == "websocket"
-        self._scope = scope
         self._receive = receive
         self._send = send
         self.client_state = WebSocketState.CONNECTING
         self.application_state = WebSocketState.CONNECTING
 
-    def __getitem__(self, key: str) -> str:
-        return self._scope[key]
-
-    def __iter__(self) -> typing.Iterator:
-        return iter(self._scope)
-
-    def __len__(self) -> int:
-        return len(self._scope)
-
-    @property
-    def url(self) -> URL:
-        if not hasattr(self, "_url"):
-            self._url = URL(scope=self._scope)
-        return self._url
-
-    @property
-    def headers(self) -> Headers:
-        if not hasattr(self, "_headers"):
-            self._headers = Headers(scope=self._scope)
-        return self._headers
-
-    @property
-    def query_params(self) -> QueryParams:
-        if not hasattr(self, "_query_params"):
-            self._query_params = QueryParams(scope=self._scope)
-        return self._query_params
-
-    @property
-    def path_params(self) -> dict:
-        return self._scope.get("path_params", {})
-
-    def url_for(self, name: str, **path_params: typing.Any) -> str:
-        router = self._scope["router"]
-        url_path = router.url_path_for(name, **path_params)
-        return url_path.make_absolute_url(base_url=self.url)
+    # def __getitem__(self, key: str) -> str:
+    #     return self._scope[key]
+    #
+    # def __iter__(self) -> typing.Iterator:
+    #     return iter(self._scope)
+    #
+    # def __len__(self) -> int:
+    #     return len(self._scope)
+    #
+    # @property
+    # def url(self) -> URL:
+    #     if not hasattr(self, "_url"):
+    #         self._url = URL(scope=self._scope)
+    #     return self._url
+    #
+    # @property
+    # def headers(self) -> Headers:
+    #     if not hasattr(self, "_headers"):
+    #         self._headers = Headers(scope=self._scope)
+    #     return self._headers
+    #
+    # @property
+    # def query_params(self) -> QueryParams:
+    #     if not hasattr(self, "_query_params"):
+    #         self._query_params = QueryParams(scope=self._scope)
+    #     return self._query_params
+    #
+    # @property
+    # def path_params(self) -> dict:
+    #     return self._scope.get("path_params", {})
+    #
+    # def url_for(self, name: str, **path_params: typing.Any) -> str:
+    #     router = self._scope["router"]
+    #     url_path = router.url_path_for(name, **path_params)
+    #     return url_path.make_absolute_url(base_url=self.url)
 
     async def receive(self) -> Message:
         """
         Receive ASGI websocket messages, ensuring valid state transitions.
         """
         if self.client_state == WebSocketState.CONNECTING:
             message = await self._receive()
```

### Comparing `starlette-0.9.8/starlette/applications.py` & `starlette-0.9.9/starlette/applications.py`

 * *Files identical despite different names*

### Comparing `starlette-0.9.8/starlette/concurrency.py` & `starlette-0.9.9/starlette/concurrency.py`

 * *Files identical despite different names*

### Comparing `starlette-0.9.8/starlette/convertors.py` & `starlette-0.9.9/starlette/convertors.py`

 * *Files identical despite different names*

### Comparing `starlette-0.9.8/starlette/staticfiles.py` & `starlette-0.9.9/starlette/staticfiles.py`

 * *Files identical despite different names*

### Comparing `starlette-0.9.8/starlette/schemas.py` & `starlette-0.9.9/starlette/schemas.py`

 * *Files identical despite different names*

### Comparing `starlette-0.9.8/starlette/routing.py` & `starlette-0.9.9/starlette/routing.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         path: str,
         endpoint: typing.Callable,
         *,
         methods: typing.List[str] = None,
         name: str = None,
         include_in_schema: bool = True
     ) -> None:
-        assert path.startswith("/"), "Routed paths must always start '/'"
+        assert path.startswith("/"), "Routed paths must start with '/'"
         self.path = path
         self.endpoint = endpoint
         self.name = get_name(endpoint) if name is None else name
         self.include_in_schema = include_in_schema
 
         if inspect.isfunction(endpoint) or inspect.ismethod(endpoint):
             # Endpoint is function or method. Treat it as `func(request) -> response`.
@@ -214,15 +214,15 @@
         )
 
 
 class WebSocketRoute(BaseRoute):
     def __init__(
         self, path: str, endpoint: typing.Callable, *, name: str = None
     ) -> None:
-        assert path.startswith("/"), "Routed paths must always start '/'"
+        assert path.startswith("/"), "Routed paths must start with '/'"
         self.path = path
         self.endpoint = endpoint
         self.name = get_name(endpoint) if name is None else name
 
         if inspect.isfunction(endpoint) or inspect.ismethod(endpoint):
             # Endpoint is function or method. Treat it as `func(websocket)`.
             self.app = websocket_session(endpoint)
@@ -271,15 +271,15 @@
             and self.path == other.path
             and self.endpoint == other.endpoint
         )
 
 
 class Mount(BaseRoute):
     def __init__(self, path: str, app: ASGIApp, name: str = None) -> None:
-        assert path == "" or path.startswith("/"), "Routed paths must always start '/'"
+        assert path == "" or path.startswith("/"), "Routed paths must start with '/'"
         self.path = path.rstrip("/")
         self.app = app
         self.name = name
         self.path_regex, self.path_format, self.param_convertors = self.compile_path(
             path + "/{path:path}"
         )
```

### Comparing `starlette-0.9.8/starlette/authentication.py` & `starlette-0.9.9/starlette/authentication.py`

 * *Files identical despite different names*

### Comparing `starlette-0.9.8/starlette/testclient.py` & `starlette-0.9.9/starlette/testclient.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,14 +122,15 @@
             "path": unquote(path),
             "root_path": "",
             "scheme": scheme,
             "query_string": query.encode(),
             "headers": headers,
             "client": ["testclient", 50000],
             "server": [host, port],
+            "extensions": {"http.response.template": {}},
         }
 
         async def receive() -> Message:
             body = request.body
             if isinstance(body, str):
                 body_bytes = body.encode("utf-8")  # type: bytes
             elif body is None:
@@ -143,15 +144,15 @@
                 except StopIteration:
                     return {"type": "http.request", "body": b""}
             else:
                 body_bytes = body
             return {"type": "http.request", "body": body_bytes}
 
         async def send(message: Message) -> None:
-            nonlocal raw_kwargs, response_started, response_complete
+            nonlocal raw_kwargs, response_started, response_complete, template, context
 
             if message["type"] == "http.response.start":
                 assert (
                     not response_started
                 ), 'Received multiple "http.response.start" messages.'
                 raw_kwargs["version"] = 11
                 raw_kwargs["status"] = message["status"]
@@ -173,18 +174,23 @@
                 ), 'Received "http.response.body" after response completed.'
                 body = message.get("body", b"")
                 more_body = message.get("more_body", False)
                 raw_kwargs["body"].write(body)
                 if not more_body:
                     raw_kwargs["body"].seek(0)
                     response_complete = True
+            elif message["type"] == "http.response.template":
+                template = message["template"]
+                context = message["context"]
 
         response_started = False
         response_complete = False
         raw_kwargs = {"body": io.BytesIO()}  # type: typing.Dict[str, typing.Any]
+        template = None
+        context = None
 
         try:
             loop = asyncio.get_event_loop()
         except RuntimeError:
             loop = asyncio.new_event_loop()
             asyncio.set_event_loop(loop)
 
@@ -205,15 +211,19 @@
                 "headers": [],
                 "preload_content": False,
                 "original_response": _MockOriginalResponse([]),
                 "body": io.BytesIO(),
             }
 
         raw = requests.packages.urllib3.HTTPResponse(**raw_kwargs)
-        return self.build_response(request, raw)
+        response = self.build_response(request, raw)
+        if template is not None:
+            response.template = template
+            response.context = context
+        return response
 
 
 class WebSocketTestSession:
     def __init__(self, app: ASGIApp, scope: Scope) -> None:
         self.accepted_subprotocol = None
         self._loop = asyncio.new_event_loop()
         self._instance = app(scope)
@@ -293,19 +303,24 @@
     def receive_json(self) -> typing.Any:
         message = self.receive()
         self._raise_on_close(message)
         encoded = message["bytes"]
         return json.loads(encoded.decode("utf-8"))
 
 
-class _TestClient(requests.Session):
+class TestClient(requests.Session):
+    __test__ = False  # For pytest to not discover this up.
+
     def __init__(
-        self, app: ASGIApp, base_url: str, raise_server_exceptions: bool = True
+        self,
+        app: ASGIApp,
+        base_url: str = "http://testserver",
+        raise_server_exceptions: bool = True,
     ) -> None:
-        super(_TestClient, self).__init__()
+        super(TestClient, self).__init__()
         adapter = _ASGIAdapter(app, raise_server_exceptions=raise_server_exceptions)
         self.mount("http://", adapter)
         self.mount("https://", adapter)
         self.mount("ws://", adapter)
         self.mount("wss://", adapter)
         self.headers.update({"user-agent": "testclient"})
         self.app = app
@@ -399,19 +414,7 @@
     async def wait_shutdown(self) -> None:
         await self.receive_queue.put({"type": "lifespan.shutdown"})
         message = await self.send_queue.get()
         if message is None:
             self.task.result()
         assert message["type"] == "lifespan.shutdown.complete"
         await self.task
-
-
-def TestClient(
-    app: ASGIApp,
-    base_url: str = "http://testserver",
-    raise_server_exceptions: bool = True,
-) -> _TestClient:
-    """
-    We have to work around py.test discovery attempting to pick up
-    the `TestClient` class, by declaring this as a function.
-    """
-    return _TestClient(app, base_url, raise_server_exceptions=raise_server_exceptions)
```

### Comparing `starlette-0.9.8/starlette/exceptions.py` & `starlette-0.9.9/starlette/exceptions.py`

 * *Files identical despite different names*

### Comparing `starlette-0.9.8/starlette/requests.py` & `starlette-0.9.9/starlette/requests.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,51 +1,46 @@
 import http.cookies
 import json
 import typing
 from collections.abc import Mapping
 
-from starlette.datastructures import URL, Headers, QueryParams
+from starlette.datastructures import URL, Address, Headers, QueryParams
 from starlette.formparsers import FormParser, MultiPartParser
 from starlette.types import Message, Receive, Scope
 
 try:
     from multipart.multipart import parse_options_header
 except ImportError:  # pragma: nocover
     parse_options_header = None  # type: ignore
 
 
 class ClientDisconnect(Exception):
     pass
 
 
-async def empty_receive() -> Message:
-    raise RuntimeError("Receive channel has not been made available")
+class HTTPConnection(Mapping):
+    """
+    A base class for incoming HTTP connections, that is used to provide
+    any functionality that is common to both `Request` and `WebSocket`.
+    """
 
-
-class Request(Mapping):
     def __init__(self, scope: Scope, receive: Receive = None) -> None:
-        assert scope["type"] == "http"
+        assert scope["type"] in ("http", "websocket")
         self._scope = scope
-        self._receive = empty_receive if receive is None else receive
-        self._stream_consumed = False
 
     def __getitem__(self, key: str) -> str:
         return self._scope[key]
 
     def __iter__(self) -> typing.Iterator[str]:
         return iter(self._scope)
 
     def __len__(self) -> int:
         return len(self._scope)
 
     @property
-    def method(self) -> str:
-        return self._scope["method"]
-
-    @property
     def url(self) -> URL:
         if not hasattr(self, "_url"):
             self._url = URL(scope=self._scope)
         return self._url
 
     @property
     def headers(self) -> Headers:
@@ -73,14 +68,19 @@
                 cookie.load(cookie_header)
                 for key, morsel in cookie.items():
                     cookies[key] = morsel.value
             self._cookies = cookies
         return self._cookies
 
     @property
+    def client(self) -> Address:
+        host, port = self._scope.get("client") or (None, None)
+        return Address(host=host, port=port)
+
+    @property
     def session(self) -> dict:
         assert (
             "session" in self._scope
         ), "SessionMiddleware must be installed to access request.session"
         return self._scope["session"]
 
     @property
@@ -100,23 +100,39 @@
     @property
     def user(self) -> typing.Any:
         assert (
             "user" in self._scope
         ), "AuthenticationMiddleware must be installed to access request.user"
         return self._scope["user"]
 
-    @property
-    def receive(self) -> Receive:
-        return self._receive
-
     def url_for(self, name: str, **path_params: typing.Any) -> str:
         router = self._scope["router"]
         url_path = router.url_path_for(name, **path_params)
         return url_path.make_absolute_url(base_url=self.url)
 
+
+async def empty_receive() -> Message:
+    raise RuntimeError("Receive channel has not been made available")
+
+
+class Request(HTTPConnection):
+    def __init__(self, scope: Scope, receive: Receive = empty_receive):
+        super().__init__(scope)
+        assert scope["type"] == "http"
+        self._receive = receive
+        self._stream_consumed = False
+
+    @property
+    def method(self) -> str:
+        return self._scope["method"]
+
+    @property
+    def receive(self) -> Receive:
+        return self._receive
+
     async def stream(self) -> typing.AsyncGenerator[bytes, None]:
         if hasattr(self, "_body"):
             yield self._body
             return
 
         if self._stream_consumed:
             raise RuntimeError("Stream consumed")
```

### Comparing `starlette-0.9.8/starlette/datastructures.py` & `starlette-0.9.9/starlette/datastructures.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import typing
+from collections import namedtuple
+from collections.abc import Sequence
+from shlex import shlex
 from urllib.parse import ParseResult, parse_qsl, urlencode, urlparse
 
 from starlette.types import Scope
 
+Address = namedtuple("Address", ["host", "port"])
+
 
 class URL:
     def __init__(
         self, url: str = "", scope: Scope = None, **components: typing.Any
     ) -> None:
         if scope is not None:
             assert not url, 'Cannot set both "url" and "scope".'
@@ -188,14 +193,41 @@
     def __repr__(self) -> str:
         return "%s('**********')" % self.__class__.__name__
 
     def __str__(self) -> str:
         return self._value
 
 
+class CommaSeparatedStrings(Sequence):
+    def __init__(self, value: typing.Union[str, typing.Sequence[str]]):
+        if isinstance(value, str):
+            splitter = shlex(value, posix=True)
+            splitter.whitespace = ","
+            splitter.whitespace_split = True
+            self._items = [item.strip() for item in splitter]
+        else:
+            self._items = list(value)
+
+    def __len__(self) -> int:
+        return len(self._items)
+
+    def __getitem__(self, index: typing.Union[int, slice]) -> typing.Any:
+        return self._items[index]
+
+    def __iter__(self) -> typing.Iterator[str]:
+        return iter(self._items)
+
+    def __repr__(self) -> str:
+        list_repr = repr([item for item in self])
+        return "%s(%s)" % (self.__class__.__name__, list_repr)
+
+    def __str__(self) -> str:
+        return ", ".join([repr(item) for item in self])
+
+
 class QueryParams(typing.Mapping[str, str]):
     """
     An immutable multidict.
     """
 
     def __init__(
         self,
```

### Comparing `starlette-0.9.8/starlette/endpoints.py` & `starlette-0.9.9/starlette/endpoints.py`

 * *Files 7% similar despite different names*

```diff
@@ -80,20 +80,24 @@
         elif self.encoding == "bytes":
             if "bytes" not in message:
                 await websocket.close(code=status.WS_1003_UNSUPPORTED_DATA)
                 raise RuntimeError("Expected bytes websocket messages, but got text")
             return message["bytes"]
 
         elif self.encoding == "json":
-            if "bytes" not in message:
+            try:
+                if "text" in message:
+                    message_json = json.loads(message["text"])
+                elif message["bytes"]:
+                    message_json = json.loads(message["bytes"].decode("utf-8"))
+            except json.decoder.JSONDecodeError:
                 await websocket.close(code=status.WS_1003_UNSUPPORTED_DATA)
-                raise RuntimeError(
-                    "Expected JSON to be transferred as bytes websocket messages, but got text"
-                )
-            return json.loads(message["bytes"].decode("utf-8"))
+                raise RuntimeError("Malformed JSON data received.")
+            else:
+                return message_json
 
         assert (
             self.encoding is None
         ), f"Unsupported 'encoding' attribute {self.encoding}"
         return message["text"] if "text" in message else message["bytes"]
 
     async def on_connect(self, websocket: WebSocket) -> None:
```

### Comparing `starlette-0.9.8/starlette/formparsers.py` & `starlette-0.9.9/starlette/formparsers.py`

 * *Files identical despite different names*

### Comparing `starlette-0.9.8/starlette/status.py` & `starlette-0.9.9/starlette/status.py`

 * *Files identical despite different names*

### Comparing `starlette-0.9.8/README.md` & `starlette-0.9.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 
 ---
 
 **Documentation**: [https://www.starlette.io/](https://www.starlette.io/)
 
 ---
 
+# Starlette
+
 Starlette is a lightweight [ASGI](https://asgi.readthedocs.io/en/latest/) framework/toolkit,
 which is ideal for building high performance asyncio services.
 
 It is production-ready, and gives you the following:
 
 * Seriously impressive performance.
 * WebSocket support.
@@ -60,23 +62,24 @@
 ```python
 from starlette.applications import Starlette
 from starlette.responses import JSONResponse
 import uvicorn
 
 app = Starlette()
 
+
 @app.route('/')
 async def homepage(request):
     return JSONResponse({'hello': 'world'})
 
 if __name__ == '__main__':
     uvicorn.run(app, host='0.0.0.0', port=8000)
 ```
 
-For a more complete example, [see here](https://github.com/encode/starlette-example).
+For a more complete example, see [encode/starlette-example](https://github.com/encode/starlette-example).
 
 ## Dependencies
 
 Starlette does not have any hard dependencies, but the following are optional:
 
 * [`requests`][requests] - Required if you want to use the `TestClient`.
 * [`aiofiles`][aiofiles] - Required if you want to use `FileResponse` or `StaticFiles`.
```

### Comparing `starlette-0.9.8/setup.py` & `starlette-0.9.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     packages=get_packages('starlette'),
     package_data = {
         'starlette': ['py.typed'],
     },
     extras_require={
         'full': [
             'aiofiles',
+            'asyncpg',
             'graphene',
             'itsdangerous',
             'jinja2',
             'python-multipart',
             'pyyaml',
             'requests',
             'sqlalchemy',
```

