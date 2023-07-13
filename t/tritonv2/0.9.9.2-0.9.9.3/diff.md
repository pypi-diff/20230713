# Comparing `tmp/tritonv2-0.9.9.2.tar.gz` & `tmp/tritonv2-0.9.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tritonv2-0.9.9.2.tar", last modified: Wed Jul  5 10:31:45 2023, max compression
+gzip compressed data, was "tritonv2-0.9.9.3.tar", last modified: Thu Jul 13 11:51:57 2023, max compression
```

## Comparing `tritonv2-0.9.9.2.tar` & `tritonv2-0.9.9.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-05 10:31:45.096394 tritonv2-0.9.9.2/
--rw-r--r--   0 jojo       (501) staff       (20)     2410 2023-07-05 10:31:45.096476 tritonv2-0.9.9.2/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)     1884 2023-07-05 10:31:44.000000 tritonv2-0.9.9.2/README.md
--rw-r--r--   0 jojo       (501) staff       (20)      772 2023-07-05 10:31:45.096882 tritonv2-0.9.9.2/setup.cfg
--rw-r--r--   0 jojo       (501) staff       (20)      180 2023-07-05 10:31:44.000000 tritonv2-0.9.9.2/setup.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-05 10:31:45.095526 tritonv2-0.9.9.2/tritonv2/
--rw-r--r--   0 jojo       (501) staff       (20)      141 2023-04-12 08:56:34.000000 tritonv2-0.9.9.2/tritonv2/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)     1008 2023-06-06 13:39:44.000000 tritonv2-0.9.9.2/tritonv2/client.py
--rw-r--r--   0 jojo       (501) staff       (20)     6421 2023-06-06 13:39:44.000000 tritonv2-0.9.9.2/tritonv2/client_factory.py
--rw-r--r--   0 jojo       (501) staff       (20)     1300 2023-07-03 18:56:19.000000 tritonv2-0.9.9.2/tritonv2/constants.py
--rw-r--r--   0 jojo       (501) staff       (20)      259 2023-04-12 08:56:34.000000 tritonv2-0.9.9.2/tritonv2/exceptions.py
--rw-r--r--   0 jojo       (501) staff       (20)    17052 2023-06-06 13:39:44.000000 tritonv2-0.9.9.2/tritonv2/grpc_aio_client.py
--rw-r--r--   0 jojo       (501) staff       (20)    14424 2023-06-06 13:39:44.000000 tritonv2-0.9.9.2/tritonv2/grpc_client.py
--rw-r--r--   0 jojo       (501) staff       (20)     1880 2023-06-06 13:39:44.000000 tritonv2-0.9.9.2/tritonv2/grpc_interceptor.py
--rw-r--r--   0 jojo       (501) staff       (20)    30819 2023-06-06 13:39:44.000000 tritonv2-0.9.9.2/tritonv2/http_aio_client.py
--rw-r--r--   0 jojo       (501) staff       (20)    29292 2023-06-06 13:39:44.000000 tritonv2-0.9.9.2/tritonv2/http_client.py
--rw-r--r--   0 jojo       (501) staff       (20)     7608 2023-07-05 10:31:37.000000 tritonv2-0.9.9.2/tritonv2/model.py
--rw-r--r--   0 jojo       (501) staff       (20)     4099 2023-07-04 11:53:35.000000 tritonv2-0.9.9.2/tritonv2/model_config.py
--rw-r--r--   0 jojo       (501) staff       (20)      903 2023-07-04 11:53:39.000000 tritonv2-0.9.9.2/tritonv2/module.py
--rw-r--r--   0 jojo       (501) staff       (20)      180 2023-04-12 08:56:34.000000 tritonv2-0.9.9.2/tritonv2/setup.py
--rw-r--r--   0 jojo       (501) staff       (20)     4893 2023-07-03 19:07:51.000000 tritonv2-0.9.9.2/tritonv2/utils.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-05 10:31:45.096280 tritonv2-0.9.9.2/tritonv2.egg-info/
--rw-r--r--   0 jojo       (501) staff       (20)     2410 2023-07-05 10:31:45.000000 tritonv2-0.9.9.2/tritonv2.egg-info/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)      561 2023-07-05 10:31:45.000000 tritonv2-0.9.9.2/tritonv2.egg-info/SOURCES.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-07-05 10:31:45.000000 tritonv2-0.9.9.2/tritonv2.egg-info/dependency_links.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-07-05 10:31:45.000000 tritonv2-0.9.9.2/tritonv2.egg-info/not-zip-safe
--rw-r--r--   0 jojo       (501) staff       (20)      127 2023-07-05 10:31:45.000000 tritonv2-0.9.9.2/tritonv2.egg-info/requires.txt
--rw-r--r--   0 jojo       (501) staff       (20)        9 2023-07-05 10:31:45.000000 tritonv2-0.9.9.2/tritonv2.egg-info/top_level.txt
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-13 11:51:57.104710 tritonv2-0.9.9.3/
+-rw-r--r--   0 jojo       (501) staff       (20)     2410 2023-07-13 11:51:57.104819 tritonv2-0.9.9.3/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)     1884 2023-07-13 11:51:56.000000 tritonv2-0.9.9.3/README.md
+-rw-r--r--   0 jojo       (501) staff       (20)      772 2023-07-13 11:51:57.105262 tritonv2-0.9.9.3/setup.cfg
+-rw-r--r--   0 jojo       (501) staff       (20)      180 2023-07-13 11:51:56.000000 tritonv2-0.9.9.3/setup.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-13 11:51:57.103516 tritonv2-0.9.9.3/tritonv2/
+-rw-r--r--   0 jojo       (501) staff       (20)      141 2023-04-12 08:56:34.000000 tritonv2-0.9.9.3/tritonv2/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1008 2023-06-06 13:39:44.000000 tritonv2-0.9.9.3/tritonv2/client.py
+-rw-r--r--   0 jojo       (501) staff       (20)     6421 2023-06-06 13:39:44.000000 tritonv2-0.9.9.3/tritonv2/client_factory.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1300 2023-07-03 18:56:19.000000 tritonv2-0.9.9.3/tritonv2/constants.py
+-rw-r--r--   0 jojo       (501) staff       (20)      259 2023-04-12 08:56:34.000000 tritonv2-0.9.9.3/tritonv2/exceptions.py
+-rw-r--r--   0 jojo       (501) staff       (20)    17052 2023-06-06 13:39:44.000000 tritonv2-0.9.9.3/tritonv2/grpc_aio_client.py
+-rw-r--r--   0 jojo       (501) staff       (20)    14424 2023-06-06 13:39:44.000000 tritonv2-0.9.9.3/tritonv2/grpc_client.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1880 2023-06-06 13:39:44.000000 tritonv2-0.9.9.3/tritonv2/grpc_interceptor.py
+-rw-r--r--   0 jojo       (501) staff       (20)    31134 2023-07-10 12:07:32.000000 tritonv2-0.9.9.3/tritonv2/http_aio_client.py
+-rw-r--r--   0 jojo       (501) staff       (20)    29615 2023-07-10 12:07:40.000000 tritonv2-0.9.9.3/tritonv2/http_client.py
+-rw-r--r--   0 jojo       (501) staff       (20)     7608 2023-07-13 07:23:55.000000 tritonv2-0.9.9.3/tritonv2/model.py
+-rw-r--r--   0 jojo       (501) staff       (20)     4162 2023-07-13 11:46:37.000000 tritonv2-0.9.9.3/tritonv2/model_config.py
+-rw-r--r--   0 jojo       (501) staff       (20)      903 2023-07-04 11:53:39.000000 tritonv2-0.9.9.3/tritonv2/module.py
+-rw-r--r--   0 jojo       (501) staff       (20)      180 2023-04-12 08:56:34.000000 tritonv2-0.9.9.3/tritonv2/setup.py
+-rw-r--r--   0 jojo       (501) staff       (20)     4969 2023-07-13 11:51:28.000000 tritonv2-0.9.9.3/tritonv2/utils.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-13 11:51:57.104563 tritonv2-0.9.9.3/tritonv2.egg-info/
+-rw-r--r--   0 jojo       (501) staff       (20)     2410 2023-07-13 11:51:57.000000 tritonv2-0.9.9.3/tritonv2.egg-info/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)      561 2023-07-13 11:51:57.000000 tritonv2-0.9.9.3/tritonv2.egg-info/SOURCES.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-07-13 11:51:57.000000 tritonv2-0.9.9.3/tritonv2.egg-info/dependency_links.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-07-13 11:51:57.000000 tritonv2-0.9.9.3/tritonv2.egg-info/not-zip-safe
+-rw-r--r--   0 jojo       (501) staff       (20)      127 2023-07-13 11:51:57.000000 tritonv2-0.9.9.3/tritonv2.egg-info/requires.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        9 2023-07-13 11:51:57.000000 tritonv2-0.9.9.3/tritonv2.egg-info/top_level.txt
```

### Comparing `tritonv2-0.9.9.2/PKG-INFO` & `tritonv2-0.9.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tritonv2
-Version: 0.9.9.2
+Version: 0.9.9.3
 Summary: project descriptions here
 Home-page: https://github.com/FlyTOmeLight
 Author: zhoubohan
 Author-email: zhoubohan.pro@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -17,15 +17,15 @@
 
 # tritonv2
 A client library for promote triton official client
 
 ## Installation
 
 ```bash
-pip install tritonv2==0.9.9.2
+pip install tritonv2==0.9.9.3
 ```
 
 ## Usage
 
 First, you need to create a client object.
 
 ```python
```

### Comparing `tritonv2-0.9.9.2/README.md` & `tritonv2-0.9.9.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # tritonv2
 A client library for promote triton official client
 
 ## Installation
 
 ```bash
-pip install tritonv2==0.9.9.2
+pip install tritonv2==0.9.9.3
 ```
 
 ## Usage
 
 First, you need to create a client object.
 
 ```python
```

### Comparing `tritonv2-0.9.9.2/setup.cfg` & `tritonv2-0.9.9.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = tritonv2
 author = zhoubohan
 author_email = zhoubohan.pro@gmail.com
-version = 0.9.9.2
+version = 0.9.9.3
 description = project descriptions here
 long_description = file: README.md
 long_description_content_type = text/markdown
 home_page = https://github.com/FlyTOmeLight
 license = MIT
 classifier = 
 	Programming Language :: Python
```

### Comparing `tritonv2-0.9.9.2/tritonv2/client.py` & `tritonv2-0.9.9.3/tritonv2/client.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.9.2/tritonv2/client_factory.py` & `tritonv2-0.9.9.3/tritonv2/client_factory.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.9.2/tritonv2/constants.py` & `tritonv2-0.9.9.3/tritonv2/constants.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.9.2/tritonv2/grpc_aio_client.py` & `tritonv2-0.9.9.3/tritonv2/grpc_aio_client.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.9.2/tritonv2/grpc_client.py` & `tritonv2-0.9.9.3/tritonv2/grpc_client.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.9.2/tritonv2/grpc_interceptor.py` & `tritonv2-0.9.9.3/tritonv2/grpc_interceptor.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.9.2/tritonv2/http_aio_client.py` & `tritonv2-0.9.9.3/tritonv2/http_aio_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,16 @@
                 # wait for the limiter
                 async with self._limiter.ratelimit(self._identifier,
                                                    delay=self._limiter_delay,
                                                    max_delay=self._limiter_max_delay):
                     return await self._client.is_server_live(headers=headers, query_params=query_params)
             return await self._client.is_server_live(headers=headers, query_params=query_params)
         except Exception as e:
-            raise TritonClientException('Failed to check server live: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to check server live: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     async def server_meta(self, headers=None, query_params=None):
         """
         get server metadata
         Returns
@@ -131,15 +132,16 @@
                 # wait for the limiter
                 async with self._limiter.ratelimit(self._identifier,
                                                    delay=self._limiter_delay,
                                                    max_delay=self._limiter_max_delay):
                     return await self._client.get_server_metadata(headers=headers, query_params=query_params)
             return await self._client.get_server_metadata(headers=headers, query_params=query_params)
         except Exception as e:
-            raise TritonClientException('Failed to get server meta: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to get server meta: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     async def model_ready(self, model_name, model_version="", headers=None, query_params=None):
         """
         check if model is ready
         :param model_name:
@@ -155,15 +157,16 @@
                                                    delay=self._limiter_delay,
                                                    max_delay=self._limiter_max_delay):
                     return await self._client.is_model_ready(model_name, model_version, headers=headers,
                                                              query_params=query_params)
             return await self._client.is_model_ready(model_name, model_version, headers=headers,
                                                      query_params=query_params)
         except Exception as e:
-            raise TritonClientException('Failed to get model ready: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to get model ready: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     async def model_meta(self, model_name, model_version="", headers=None, query_params=None):
         """
         get model meta
         Parameters
@@ -180,15 +183,16 @@
                                                    delay=self._limiter_delay,
                                                    max_delay=self._limiter_max_delay):
                     return await self._client.get_model_metadata(model_name, model_version, headers=headers,
                                                                  query_params=query_params)
             return await self._client.get_model_metadata(model_name, model_version, headers=headers,
                                                          query_params=query_params)
         except Exception as e:
-            raise TritonClientException('Failed to get model meta: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to get model meta: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     async def model_config(self, model_name, model_version="", headers=None, query_params=None):
         """
         get model config
         Parameters
@@ -203,17 +207,18 @@
                 # wait for the limiter
                 async with self._limiter.ratelimit(self._identifier,
                                                    delay=self._limiter_delay,
                                                    max_delay=self._limiter_max_delay):
                     return await self._client.get_model_config(model_name, model_version, headers=headers,
                                                                query_params=query_params)
             return await self._client.get_model_config(model_name, model_version, headers=headers,
-                                                               query_params=query_params)
+                                                       query_params=query_params)
         except Exception as e:
-            raise TritonClientException('Failed to get model config: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to get model config: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     async def model_infer(self,
                           model_name,
                           inputs,
                           model_version="",
@@ -280,15 +285,16 @@
                 priority=priority,
                 timeout=timeout,
                 headers=headers,
                 query_params=query_params,
                 request_compression_algorithm=request_compression_algorithm,
                 response_compression_algorithm=response_compression_algorithm)
         except Exception as e:
-            raise TritonClientException('Failed to model infer: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to model infer: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     async def model_statistics(self, model_name, model_version="", headers=None, query_params=None):
         """
         get model statistics
         :param model_name:
@@ -304,15 +310,16 @@
                                                    delay=self._limiter_delay,
                                                    max_delay=self._limiter_max_delay):
                     return await self._client.get_inference_statistics(model_name, model_version, headers=headers,
                                                                        query_params=query_params)
             return await self._client.get_inference_statistics(model_name, model_version, headers=headers,
                                                                query_params=query_params)
         except Exception as e:
-            raise TritonClientException('Failed to get model statistics: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to get model statistics: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     async def repository_index(self, headers=None, query_params=None):
         """
         get repository index
         :param headers:
@@ -324,15 +331,16 @@
                 # wait for the limiter
                 async with self._limiter.ratelimit(self._identifier,
                                                    delay=self._limiter_delay,
                                                    max_delay=self._limiter_max_delay):
                     return await self._client.get_model_repository_index(headers=headers, query_params=query_params)
             return await self._client.get_model_repository_index(headers=headers, query_params=query_params)
         except Exception as e:
-            raise TritonClientException('Failed to get repository index: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to get repository index: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     async def repository_model_load(self, model_name, headers=None, query_params=None, config="", files=None):
         """
         load model
         :param model_name:
@@ -355,15 +363,16 @@
                                                          files=files)
             return await self._client.load_model(model_name=model_name,
                                                  headers=headers,
                                                  query_params=query_params,
                                                  config=config,
                                                  files=files)
         except Exception as e:
-            raise TritonClientException('Failed to load model: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to load model: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     async def repository_model_unload(self, model_name, headers=None, query_params=None, unload_dependents=False):
         """
         unload model
         :param model_name:
@@ -383,15 +392,16 @@
                                                            query_params=query_params,
                                                            unload_dependents=unload_dependents)
             return await self._client.unload_model(model_name=model_name,
                                                    headers=headers,
                                                    query_params=query_params,
                                                    unload_dependents=unload_dependents)
         except Exception as e:
-            raise TritonClientException('Failed to unload model: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to unload model: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     async def system_shared_memory_status(self, region_name="", headers=None, query_params=None):
         """
         get system shared memory status
         :param region_name:
@@ -406,15 +416,16 @@
                                                    delay=self._limiter_delay,
                                                    max_delay=self._limiter_max_delay):
                     return await self._client.get_system_shared_memory_status(region_name=region_name, headers=headers,
                                                                               query_params=query_params)
             return await self._client.get_system_shared_memory_status(region_name=region_name, headers=headers,
                                                                       query_params=query_params)
         except Exception as e:
-            raise TritonClientException('Failed to get system shared memory status: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to get system shared memory status: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     async def system_shared_memory_register(self, name, key, byte_size, offset=0, headers=None, query_params=None):
         """
         register system shared memory
         :param name:
@@ -440,15 +451,16 @@
             return await self._client.register_system_shared_memory(name=name,
                                                                     key=key,
                                                                     byte_size=byte_size,
                                                                     offset=offset,
                                                                     headers=headers,
                                                                     query_params=query_params)
         except Exception as e:
-            raise TritonClientException('Failed to register system shared memory: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to register system shared memory: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     async def system_shared_memory_unregister(self, name, headers=None, query_params=None):
         """
         unregister system shared memory
         :param name:
@@ -465,15 +477,16 @@
                     return await self._client.unregister_system_shared_memory(name=name,
                                                                               headers=headers,
                                                                               query_params=query_params)
             return await self._client.unregister_system_shared_memory(name=name,
                                                                       headers=headers,
                                                                       query_params=query_params)
         except Exception as e:
-            raise TritonClientException('Failed to unregister system shared memory: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to unregister system shared memory: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     async def cuda_shared_memory_status(self, region_name="", headers=None, query_params=None):
         """
         get cuda shared memory status
         :param region_name:
@@ -490,15 +503,16 @@
                     return await self._client.get_cuda_shared_memory_status(region_name=region_name,
                                                                             headers=headers,
                                                                             query_params=query_params)
             return await self._client.get_cuda_shared_memory_status(region_name=region_name,
                                                                     headers=headers,
                                                                     query_params=query_params)
         except Exception as e:
-            raise TritonClientException('Failed to get cuda shared memory status: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to get cuda shared memory status: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     async def cuda_shared_memory_register(self, name, raw_handle, byte_size, device_id, headers=None,
                                           query_params=None):
         """
         register cuda shared memory
@@ -525,15 +539,16 @@
             return await self._client.register_cuda_shared_memory(name=name,
                                                                   raw_handle=raw_handle,
                                                                   device_id=device_id,
                                                                   byte_size=byte_size,
                                                                   headers=headers,
                                                                   query_params=query_params)
         except Exception as e:
-            raise TritonClientException('Failed to register cuda shared memory: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to register cuda shared memory: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     async def cuda_shared_memory_unregister(self, name, headers=None, query_params=None):
         """
         unregister cuda shared memory
         :param name:
@@ -550,15 +565,16 @@
                     return await self._client.unregister_cuda_shared_memory(name=name,
                                                                             headers=headers,
                                                                             query_params=query_params)
             return await self._client.unregister_cuda_shared_memory(name=name,
                                                                     headers=headers,
                                                                     query_params=query_params)
         except Exception as e:
-            raise TritonClientException('Failed to  unregister cuda shared memory: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to  unregister cuda shared memory: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     async def trace_setting(self, model_name="", settings=None, headers=None, query_params=None):
         """
         update trace setting
         :param model_name:
@@ -580,15 +596,16 @@
                                                                     headers=headers,
                                                                     query_params=query_params)
             return await self._client.update_trace_settings(model_name=model_name,
                                                             settings=settings,
                                                             headers=headers,
                                                             query_params=query_params)
         except Exception as e:
-            raise TritonClientException('Failed to update trace setting: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to update trace setting: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     async def get_trace_settings(self, model_name="", headers=None, query_params=None):
         """
         get_trace_settings
         :param model_name:
@@ -605,22 +622,24 @@
                     return await self._client.get_trace_settings(model_name=model_name,
                                                                  headers=headers,
                                                                  query_params=query_params)
             return await self._client.get_trace_settings(model_name=model_name,
                                                          headers=headers,
                                                          query_params=query_params)
         except Exception as e:
-            raise TritonClientException('Failed to get trace settings: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to get trace settings: {}'.format(e)) from None
 
     async def get_inputs_and_outputs_detail(self, model_name, model_version):
         """
         get inputs and outputs detail
         :param model_name:
         :param model_version:
         :return:
         """
         try:
             model_meta = await self.model_meta(model_name, model_version)
             model_config = await self.model_config(model_name, model_version)
             return parse_model(model_meta, model_config)
         except Exception as e:
-            raise TritonClientException('Failed to get inputs and outputs detail: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to get inputs and outputs detail: {}'.format(e)) from None
```

### Comparing `tritonv2-0.9.9.2/tritonv2/http_client.py` & `tritonv2-0.9.9.3/tritonv2/http_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,16 @@
                 with self._limiter.ratelimit(self._identifier,
                                              delay=self._limiter_delay,
                                              max_delay=self._limiter_max_delay):
                     return self._client.is_server_live(headers=headers, query_params=query_params)
             else:
                 return self._client.is_server_live(headers=headers, query_params=query_params)
         except Exception as e:
-            raise TritonClientException('Failed to check server live: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to check server live: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def server_meta(self, headers=None, query_params=None):
         """
         get server metadata
         Returns
@@ -118,15 +119,16 @@
                 with self._limiter.ratelimit(self._identifier,
                                              delay=self._limiter_delay,
                                              max_delay=self._limiter_max_delay):
                     return self._client.get_server_metadata(headers=headers, query_params=query_params)
             else:
                 return self._client.get_server_metadata(headers=headers, query_params=query_params)
         except Exception as e:
-            raise TritonClientException('Failed to get server meta: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to get server meta: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def model_ready(self, model_name, model_version="", headers=None, query_params=None):
         """
         check if model is ready
         :param model_name:
@@ -142,15 +144,16 @@
                                              max_delay=self._limiter_max_delay):
                     return self._client.is_model_ready(model_name, model_version, headers=headers,
                                                        query_params=query_params)
             else:
                 return self._client.is_model_ready(model_name, model_version, headers=headers,
                                                    query_params=query_params)
         except Exception as e:
-            raise TritonClientException('Failed to get model ready: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to get model ready: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def model_meta(self, model_name, model_version="", headers=None, query_params=None):
         """
         get model meta
         Parameters
@@ -167,15 +170,16 @@
                                              max_delay=self._limiter_max_delay):
                     return self._client.get_model_metadata(model_name, model_version, headers=headers,
                                                            query_params=query_params)
             else:
                 return self._client.get_model_metadata(model_name, model_version, headers=headers,
                                                        query_params=query_params)
         except Exception as e:
-            raise TritonClientException('Failed to get model meta: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to get model meta: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def model_config(self, model_name, model_version="", headers=None, query_params=None):
         """
         get model config
         Parameters
@@ -192,15 +196,16 @@
                                              max_delay=self._limiter_max_delay):
                     return self._client.get_model_config(model_name, model_version, headers=headers,
                                                          query_params=query_params)
             else:
                 return self._client.get_model_config(model_name, model_version, headers=headers,
                                                      query_params=query_params)
         except Exception as e:
-            raise TritonClientException('Failed to get model config: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to get model config: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def model_infer(self,
                     model_name,
                     inputs,
                     model_version="",
@@ -267,15 +272,16 @@
                     priority=priority,
                     timeout=timeout,
                     headers=headers,
                     query_params=query_params,
                     request_compression_algorithm=request_compression_algorithm,
                     response_compression_algorithm=response_compression_algorithm)
         except Exception as e:
-            raise TritonClientException('Failed to model infer: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to model infer: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def model_statistics(self, model_name, model_version="", headers=None, query_params=None):
         """
         get model statistics
         :param model_name:
@@ -291,15 +297,16 @@
                                              max_delay=self._limiter_max_delay):
                     return self._client.get_inference_statistics(model_name, model_version, headers=headers,
                                                                  query_params=query_params)
             else:
                 return self._client.get_inference_statistics(model_name, model_version, headers=headers,
                                                              query_params=query_params)
         except Exception as e:
-            raise TritonClientException('Failed to get model statistics: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to get model statistics: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def repository_index(self, headers=None, query_params=None):
         """
         get repository index
         :param headers:
@@ -311,15 +318,16 @@
                 with self._limiter.ratelimit(self._identifier,
                                              delay=self._limiter_delay,
                                              max_delay=self._limiter_max_delay):
                     return self._client.get_model_repository_index(headers=headers, query_params=query_params)
             else:
                 return self._client.get_model_repository_index(headers=headers, query_params=query_params)
         except Exception as e:
-            raise TritonClientException('Failed to get repository index: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to get repository index: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def repository_model_load(self, model_name, headers=None, query_params=None, config="", files=None):
         """
         load model
         :param model_name:
@@ -343,15 +351,16 @@
             else:
                 return self._client.load_model(model_name=model_name,
                                                headers=headers,
                                                query_params=query_params,
                                                config=config,
                                                files=files)
         except Exception as e:
-            raise TritonClientException('Failed to load model: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to load model: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def repository_model_unload(self, model_name, headers=None, query_params=None, unload_dependents=False):
         """
         unload model
         :param model_name:
@@ -371,15 +380,16 @@
                                                      unload_dependents=unload_dependents)
             else:
                 return self._client.unload_model(model_name=model_name,
                                                  headers=headers,
                                                  query_params=query_params,
                                                  unload_dependents=unload_dependents)
         except Exception as e:
-            raise TritonClientException('Failed to unload model: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to unload model: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def system_shared_memory_status(self, region_name="", headers=None, query_params=None):
         """
         get system shared memory status
         :param region_name:
@@ -394,15 +404,16 @@
                                              max_delay=self._limiter_max_delay):
                     return self._client.get_system_shared_memory_status(region_name=region_name, headers=headers,
                                                                         query_params=query_params)
             else:
                 return self._client.get_system_shared_memory_status(region_name=region_name, headers=headers,
                                                                     query_params=query_params)
         except Exception as e:
-            raise TritonClientException('Failed to get system shared memory status: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to get system shared memory status: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def system_shared_memory_register(self, name, key, byte_size, offset=0, headers=None, query_params=None):
         """
         register system shared memory
         :param name:
@@ -428,15 +439,16 @@
                 return self._client.register_system_shared_memory(name=name,
                                                                   key=key,
                                                                   byte_size=byte_size,
                                                                   offset=offset,
                                                                   headers=headers,
                                                                   query_params=query_params)
         except Exception as e:
-            raise TritonClientException('Failed to register system shared memory: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to register system shared memory: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def system_shared_memory_unregister(self, name, headers=None, query_params=None):
         """
         unregister system shared memory
         :param name:
@@ -453,15 +465,16 @@
                                                                         headers=headers,
                                                                         query_params=query_params)
             else:
                 return self._client.unregister_system_shared_memory(name=name,
                                                                     headers=headers,
                                                                     query_params=query_params)
         except Exception as e:
-            raise TritonClientException('Failed to unregister system shared memory: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to unregister system shared memory: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def cuda_shared_memory_status(self, region_name="", headers=None, query_params=None):
         """
         get cuda shared memory status
         :param region_name:
@@ -478,15 +491,16 @@
                                                                       headers=headers,
                                                                       query_params=query_params)
             else:
                 return self._client.get_cuda_shared_memory_status(region_name=region_name,
                                                                   headers=headers,
                                                                   query_params=query_params)
         except Exception as e:
-            raise TritonClientException('Failed to get cuda shared memory status: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to get cuda shared memory status: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def cuda_shared_memory_register(self, name, raw_handle, byte_size, device_id, headers=None, query_params=None):
         """
         register cuda shared memory
         :param name:
@@ -512,15 +526,16 @@
                 return self._client.register_cuda_shared_memory(name=name,
                                                                 raw_handle=raw_handle,
                                                                 device_id=device_id,
                                                                 byte_size=byte_size,
                                                                 headers=headers,
                                                                 query_params=query_params)
         except Exception as e:
-            raise TritonClientException('Failed to register cuda shared memory: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to register cuda shared memory: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def cuda_shared_memory_unregister(self, name, headers=None, query_params=None):
         """
         unregister cuda shared memory
         :param name:
@@ -537,15 +552,16 @@
                                                                       headers=headers,
                                                                       query_params=query_params)
             else:
                 return self._client.unregister_cuda_shared_memory(name=name,
                                                                   headers=headers,
                                                                   query_params=query_params)
         except Exception as e:
-            raise TritonClientException('Failed to  unregister cuda shared memory: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to  unregister cuda shared memory: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def trace_setting(self, model_name="", settings=None, headers=None, query_params=None):
         """
         update trace setting
         :param model_name:
@@ -567,15 +583,16 @@
                                                               query_params=query_params)
             else:
                 return self._client.update_trace_settings(model_name=model_name,
                                                           settings=settings,
                                                           headers=headers,
                                                           query_params=query_params)
         except Exception as e:
-            raise TritonClientException('Failed to update trace setting: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to update trace setting: {}'.format(e)) from None
 
     @retry(stop=(stop_after_attempt(NUMBER_RETRIES + 1) | stop_after_delay(MAX_INTERVAL_SECS)),
            wait=wait_fixed(BASE_INTERVAL_SECS), reraise=True)
     def get_trace_settings(self, model_name="", headers=None, query_params=None):
         """
         get_trace_settings
         :param model_name:
@@ -592,22 +609,24 @@
                                                            headers=headers,
                                                            query_params=query_params)
             else:
                 return self._client.get_trace_settings(model_name=model_name,
                                                        headers=headers,
                                                        query_params=query_params)
         except Exception as e:
-            raise TritonClientException('Failed to get trace settings: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to get trace settings: {}'.format(e)) from None
 
     def get_inputs_and_outputs_detail(self, model_name, model_version):
         """
         get inputs and outputs detail
         :param model_name:
         :param model_version:
         :return:
         """
         try:
             model_meta = self.model_meta(model_name, model_version)
             model_config = self.model_config(model_name, model_version)
             return parse_model(model_meta, model_config)
         except Exception as e:
-            raise TritonClientException('Failed to get inputs and outputs detail: {}'.format(e)) from None
+            raise TritonClientException(
+                'Failed to get inputs and outputs detail: {}'.format(e)) from None
```

### Comparing `tritonv2-0.9.9.2/tritonv2/model.py` & `tritonv2-0.9.9.3/tritonv2/model.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.9.2/tritonv2/model_config.py` & `tritonv2-0.9.9.3/tritonv2/model_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 # Copyright (c) 2023 Baidu.com, Inc. All Rights Reserved
 
 import os
 from typing import Dict
 from tritonclient.grpc import model_config_pb2
 from google.protobuf import text_format, json_format
 
+
 class ModelConfig:
     """
     ModelConfig For Triton Model
     """
+
     def __init__(self, model_config):
         self._model_config = model_config
 
     def is_ensemble(self) -> bool:
         """
         return if model is ensemble
         Returns:
@@ -66,24 +68,27 @@
         try:
             for step in model_config_dict["ensembleScheduling"]["step"]:
                 if step["modelName"] == model_name:
                     step["modelVersion"] = model_version
         except Exception as e:
             raise ValueError("Set model version failed {}".format(e))
 
-        self._model_config = ModelConfig.create_from_dict(model_config_dict)._model_config
+        self._model_config = ModelConfig.create_from_dict(
+            model_config_dict)._model_config
 
     def write_to_file(self, model_path, variant_model_source_version, bs):
         """
         write model config to file
         """
         model_config_path = os.path.join(model_path, "config.pbtxt")
         if not bs.exist(model_config_path):
-            raise FileNotFoundError("Model config path: {} not found".format(model_config_path))
-        model_source_config_path = os.path.join(model_path, "{}/config.pbtxt".format(variant_model_source_version))
+            raise FileNotFoundError(
+                "Model config path: {} not found".format(model_config_path))
+        model_source_config_path = os.path.join(
+            model_path, "{}/config.pbtxt".format(variant_model_source_version))
         try:
             bs.copy(model_config_path, model_source_config_path)
             model_config_bytes = text_format.MessageToBytes(self._model_config)
             bs.write_file(model_config_path, model_config_bytes)
         except Exception as e:
             raise ValueError("Model config write to file error:{}".format(e))
 
@@ -104,10 +109,11 @@
     @staticmethod
     def create_from_file(model_path, bs):
         """
         create model config from file
         """
         model_config_path = os.path.join(model_path, "config.pbtxt")
         if not bs.exist(model_config_path):
-            raise FileNotFoundError("Model config path: {} not found".format(model_config_path))
+            raise FileNotFoundError(
+                "Model config path: {} not found".format(model_config_path))
         raw_str = bs.read_file(model_config_path)
-        return ModelConfig.create_from_text(raw_str)
+        return ModelConfig.create_from_text(raw_str)
```

### Comparing `tritonv2-0.9.9.2/tritonv2/module.py` & `tritonv2-0.9.9.3/tritonv2/module.py`

 * *Files identical despite different names*

### Comparing `tritonv2-0.9.9.2/tritonv2/utils.py` & `tritonv2-0.9.9.3/tritonv2/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,16 @@
     """
     Convert list of ndarrays to single ndarray with ndims+=1
     """
     lengths = list(
         map(lambda x, a=arrays: a[x].shape[0], [x for x in range(len(arrays))])
     )
     max_len = max(lengths)
-    arrays = list(map(lambda a, ml=max_len: np.pad(a, (0, ml - a.shape[0])), arrays))
+    arrays = list(map(lambda a, ml=max_len: np.pad(
+        a, (0, ml - a.shape[0])), arrays))
     for arr in arrays:
         assert arr.shape == arrays[0].shape, "arrays must have the same shape"
     return np.stack(arrays, axis=0)
 
 
 def parse_model(model_metadata, model_config):
     """
@@ -49,27 +50,30 @@
     return input_metadata, output_metadata, max_batch_size
 
 
 class BlobStoreFactory:
     """
     BlobStoreFactory
     """
+
     def create(self, kind, bucket, endpoint_url, aws_access_key_id='', aws_secret_access_key='', region='bj'):
         if kind == "s3":
             return S3BlobStore(bucket, endpoint_url, aws_access_key_id, aws_secret_access_key, region)
         if kind == "local":
             return LocalBlobStore(endpoint_url)
 
+
 class LocalBlobStore:
     """
     LocalBlobStore
     """
+
     def __init__(self, prefix_path) -> None:
         self._prefix = prefix_path+"/"
-    
+
     def exist(self, path):
         """
         file exist
         Args:
             path (_type_): _description_
 
         Returns:
@@ -77,15 +81,15 @@
         """
         try:
             path = self._prefix+path
             return os.path.exists(path)
         except Exception as e:
             print(f"File {path} not exist: {e}")
             return False
-        
+
     def read_file(self, path):
         """
         read file
         Args:
             path (_type_): _description_
 
         Returns:
@@ -95,39 +99,43 @@
             path = self._prefix+path
             with open(path, "r") as f:
                 data = f.read()
             return data
         except Exception as e:
             print(f"File {path} read error: {e}")
             return None
-    
+
     def write_file(self, path, data):
         """
         write file
         Args:
             path (_type_): _description_
             data (_type_): _description_
         """
+        if isinstance(data, bytes):
+            data = data.decode("utf-8")
+
         with open(self._prefix+path, "w") as f:
             f.write(data)
-    
+
     def copy(self, source_key, destination_key):
         """
         copy file
         Args:
             source_key (_type_): _description_
             destination_key (_type_): _description_
         """
         shutil.copy(self._prefix+source_key, self._prefix+destination_key)
-        
+
 
 class S3BlobStore:
     """
     S3BlobStore
     """
+
     def __init__(self, bucket, endpoint_url, aws_access_key_id, aws_secret_access_key, region):
         self._bucket = bucket
         self._client = boto3.client(
             "s3", aws_access_key_id=aws_access_key_id,
             aws_secret_access_key=aws_secret_access_key, endpoint_url=f"http://{endpoint_url}", region_name=region)
 
     def exist(self, path):
@@ -172,8 +180,9 @@
         """
         copy file
         Args:
             source_key (_type_): _description_
             destination_key (_type_): _description_
         """
         copy_source = {"Bucket": self._bucket, "Key": source_key}
-        self._client.copy_object(CopySource=copy_source, Bucket=self._bucket, Key=destination_key)
+        self._client.copy_object(
+            CopySource=copy_source, Bucket=self._bucket, Key=destination_key)
```

### Comparing `tritonv2-0.9.9.2/tritonv2.egg-info/PKG-INFO` & `tritonv2-0.9.9.3/tritonv2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tritonv2
-Version: 0.9.9.2
+Version: 0.9.9.3
 Summary: project descriptions here
 Home-page: https://github.com/FlyTOmeLight
 Author: zhoubohan
 Author-email: zhoubohan.pro@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -17,15 +17,15 @@
 
 # tritonv2
 A client library for promote triton official client
 
 ## Installation
 
 ```bash
-pip install tritonv2==0.9.9.2
+pip install tritonv2==0.9.9.3
 ```
 
 ## Usage
 
 First, you need to create a client object.
 
 ```python
```

### Comparing `tritonv2-0.9.9.2/tritonv2.egg-info/SOURCES.txt` & `tritonv2-0.9.9.3/tritonv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

