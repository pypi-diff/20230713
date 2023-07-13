# Comparing `tmp/hscan-2.6.1.tar.gz` & `tmp/hscan-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hscan-2.6.1.tar", last modified: Mon Jun 26 08:48:58 2023, max compression
+gzip compressed data, was "hscan-2.7.0.tar", last modified: Thu Jul 13 11:07:59 2023, max compression
```

## Comparing `hscan-2.6.1.tar` & `hscan-2.7.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-06-26 08:48:58.435261 hscan-2.6.1/
--rw-r--r--   0 jyanghe    (501) staff       (20)      502 2023-06-26 08:48:58.434917 hscan-2.6.1/PKG-INFO
--rw-r--r--   0 jyanghe    (501) staff       (20)       80 2021-09-07 07:20:00.000000 hscan-2.6.1/README.md
--rw-r--r--   0 jyanghe    (501) staff       (20)     1032 2023-06-26 08:48:24.000000 hscan-2.6.1/Setup.py
-drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-06-26 08:48:58.423426 hscan-2.6.1/hscan.egg-info/
--rw-r--r--   0 jyanghe    (501) staff       (20)      502 2023-06-26 08:48:58.000000 hscan-2.6.1/hscan.egg-info/PKG-INFO
--rw-r--r--   0 jyanghe    (501) staff       (20)      548 2023-06-26 08:48:58.000000 hscan-2.6.1/hscan.egg-info/SOURCES.txt
--rw-r--r--   0 jyanghe    (501) staff       (20)        1 2023-06-26 08:48:58.000000 hscan-2.6.1/hscan.egg-info/dependency_links.txt
--rw-r--r--   0 jyanghe    (501) staff       (20)      227 2023-06-26 08:48:58.000000 hscan-2.6.1/hscan.egg-info/requires.txt
--rw-r--r--   0 jyanghe    (501) staff       (20)        5 2023-06-26 08:48:58.000000 hscan-2.6.1/hscan.egg-info/top_level.txt
-drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-06-26 08:48:58.428774 hscan-2.6.1/scan/
--rw-r--r--   0 jyanghe    (501) staff       (20)      181 2023-04-03 10:06:56.000000 hscan-2.6.1/scan/__init__.py
--rw-r--r--   0 jyanghe    (501) staff       (20)      301 2021-09-04 15:30:38.000000 hscan-2.6.1/scan/common.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     1195 2022-12-24 12:34:00.000000 hscan-2.6.1/scan/config.py
--rw-r--r--   0 jyanghe    (501) staff       (20)      866 2023-06-26 06:03:50.000000 hscan-2.6.1/scan/crawl.py
-drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-06-26 08:48:58.433357 hscan-2.6.1/scan/database/
--rw-r--r--   0 jyanghe    (501) staff       (20)      235 2022-12-20 15:11:44.000000 hscan-2.6.1/scan/database/__init__.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     6325 2023-02-23 13:03:29.000000 hscan-2.6.1/scan/database/kafka.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     1112 2021-09-06 03:30:11.000000 hscan-2.6.1/scan/database/mongodb.py
--rw-r--r--   0 jyanghe    (501) staff       (20)        0 2023-01-16 12:29:44.000000 hscan-2.6.1/scan/database/mysql.py
--rw-r--r--   0 jyanghe    (501) staff       (20)      508 2021-09-06 03:30:20.000000 hscan-2.6.1/scan/database/oss.py
--rw-r--r--   0 jyanghe    (501) staff       (20)      954 2022-09-09 07:43:05.000000 hscan-2.6.1/scan/database/pg.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     6093 2023-04-27 08:36:36.000000 hscan-2.6.1/scan/database/rabbitmq.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     2098 2022-12-22 03:15:19.000000 hscan-2.6.1/scan/database/redis.py
-drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-06-26 08:48:58.434230 hscan-2.6.1/scan/downloade/
--rw-r--r--   0 jyanghe    (501) staff       (20)        0 2021-09-01 10:54:34.000000 hscan-2.6.1/scan/downloade/__init__.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     5564 2023-06-26 08:47:36.000000 hscan-2.6.1/scan/downloade/downloader.py
--rw-r--r--   0 jyanghe    (501) staff       (20)      529 2022-09-09 07:40:26.000000 hscan-2.6.1/scan/log.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     2790 2023-04-04 03:33:16.000000 hscan-2.6.1/scan/monitor.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     1945 2022-04-29 03:52:46.000000 hscan-2.6.1/scan/response.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     9784 2022-12-27 08:14:30.000000 hscan-2.6.1/scan/spider.py
--rw-r--r--   0 jyanghe    (501) staff       (20)     1022 2023-06-19 03:37:35.000000 hscan-2.6.1/scan/util.py
--rw-r--r--   0 jyanghe    (501) staff       (20)       38 2023-06-26 08:48:58.435371 hscan-2.6.1/setup.cfg
+drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-07-13 11:07:59.401598 hscan-2.7.0/
+-rw-r--r--   0 jyanghe    (501) staff       (20)      502 2023-07-13 11:07:59.401365 hscan-2.7.0/PKG-INFO
+-rw-r--r--   0 jyanghe    (501) staff       (20)       80 2021-09-07 07:20:00.000000 hscan-2.7.0/README.md
+-rw-r--r--   0 jyanghe    (501) staff       (20)     1032 2023-07-13 11:05:39.000000 hscan-2.7.0/Setup.py
+drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-07-13 11:07:59.391545 hscan-2.7.0/hscan.egg-info/
+-rw-r--r--   0 jyanghe    (501) staff       (20)      502 2023-07-13 11:07:59.000000 hscan-2.7.0/hscan.egg-info/PKG-INFO
+-rw-r--r--   0 jyanghe    (501) staff       (20)      548 2023-07-13 11:07:59.000000 hscan-2.7.0/hscan.egg-info/SOURCES.txt
+-rw-r--r--   0 jyanghe    (501) staff       (20)        1 2023-07-13 11:07:59.000000 hscan-2.7.0/hscan.egg-info/dependency_links.txt
+-rw-r--r--   0 jyanghe    (501) staff       (20)      227 2023-07-13 11:07:59.000000 hscan-2.7.0/hscan.egg-info/requires.txt
+-rw-r--r--   0 jyanghe    (501) staff       (20)        5 2023-07-13 11:07:59.000000 hscan-2.7.0/hscan.egg-info/top_level.txt
+drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-07-13 11:07:59.395934 hscan-2.7.0/scan/
+-rw-r--r--   0 jyanghe    (501) staff       (20)      181 2023-04-03 10:06:56.000000 hscan-2.7.0/scan/__init__.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)      301 2021-09-04 15:30:38.000000 hscan-2.7.0/scan/common.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     1195 2022-12-24 12:34:00.000000 hscan-2.7.0/scan/config.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)      866 2023-06-26 06:03:50.000000 hscan-2.7.0/scan/crawl.py
+drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-07-13 11:07:59.400436 hscan-2.7.0/scan/database/
+-rw-r--r--   0 jyanghe    (501) staff       (20)      235 2022-12-20 15:11:44.000000 hscan-2.7.0/scan/database/__init__.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     6325 2023-02-23 13:03:29.000000 hscan-2.7.0/scan/database/kafka.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     1112 2021-09-06 03:30:11.000000 hscan-2.7.0/scan/database/mongodb.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)        0 2023-01-16 12:29:44.000000 hscan-2.7.0/scan/database/mysql.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)      508 2021-09-06 03:30:20.000000 hscan-2.7.0/scan/database/oss.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)      954 2022-09-09 07:43:05.000000 hscan-2.7.0/scan/database/pg.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     6093 2023-04-27 08:36:36.000000 hscan-2.7.0/scan/database/rabbitmq.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     2098 2022-12-22 03:15:19.000000 hscan-2.7.0/scan/database/redis.py
+drwxr-xr-x   0 jyanghe    (501) staff       (20)        0 2023-07-13 11:07:59.401058 hscan-2.7.0/scan/downloade/
+-rw-r--r--   0 jyanghe    (501) staff       (20)        0 2021-09-01 10:54:34.000000 hscan-2.7.0/scan/downloade/__init__.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     6338 2023-07-13 11:04:06.000000 hscan-2.7.0/scan/downloade/downloader.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)      529 2022-09-09 07:40:26.000000 hscan-2.7.0/scan/log.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     2790 2023-04-04 03:33:16.000000 hscan-2.7.0/scan/monitor.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     1945 2022-04-29 03:52:46.000000 hscan-2.7.0/scan/response.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     9784 2022-12-27 08:14:30.000000 hscan-2.7.0/scan/spider.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)     1022 2023-06-19 03:37:35.000000 hscan-2.7.0/scan/util.py
+-rw-r--r--   0 jyanghe    (501) staff       (20)       38 2023-07-13 11:07:59.401674 hscan-2.7.0/setup.cfg
```

### Comparing `hscan-2.6.1/Setup.py` & `hscan-2.7.0/Setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hscan",
-    version="2.6.1",
+    version="2.7.0",
     author="jyanghe",
     author_email="jyanghe1023@gmail.com",
     description="A python framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jyangHe/hscan",
     packages=setuptools.find_packages(),
```

### Comparing `hscan-2.6.1/hscan.egg-info/SOURCES.txt` & `hscan-2.7.0/hscan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hscan-2.6.1/scan/config.py` & `hscan-2.7.0/scan/config.py`

 * *Files identical despite different names*

### Comparing `hscan-2.6.1/scan/crawl.py` & `hscan-2.7.0/scan/crawl.py`

 * *Files identical despite different names*

### Comparing `hscan-2.6.1/scan/database/kafka.py` & `hscan-2.7.0/scan/database/kafka.py`

 * *Files identical despite different names*

### Comparing `hscan-2.6.1/scan/database/mongodb.py` & `hscan-2.7.0/scan/database/mongodb.py`

 * *Files identical despite different names*

### Comparing `hscan-2.6.1/scan/database/pg.py` & `hscan-2.7.0/scan/database/pg.py`

 * *Files identical despite different names*

### Comparing `hscan-2.6.1/scan/database/rabbitmq.py` & `hscan-2.7.0/scan/database/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `hscan-2.6.1/scan/database/redis.py` & `hscan-2.7.0/scan/database/redis.py`

 * *Files identical despite different names*

### Comparing `hscan-2.6.1/scan/downloade/downloader.py` & `hscan-2.7.0/scan/downloade/downloader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 import random
 import httpx
 from httpx import ConnectError, ConnectTimeout, ProxyError, ReadTimeout, ReadError, UnsupportedProtocol
 from curl_cffi import requests
 from scan.response import Response
 from scan.common import logger
+from httpx._config import SSLConfig, DEFAULT_CIPHERS
 
 
 class Downloader(object):
     def __init__(self):
         self.client = None
+        self.ssl_context = None
+
+    def create_ssl_context(self, verify):
+        ssl_config = SSLConfig(verify=verify)
+        ssl_context = ssl_config.load_ssl_context()
+        ssl_context.set_ciphers(DEFAULT_CIPHERS + 'HIGH:!DH')
+        self.ssl_context = ssl_context
 
     @staticmethod
     async def gen_headers():
         kit = f'{random.randint(490, 540)}.{random.randint(10, 90)}'
         return {
             'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;'
                       'q=0.8,application/signed-exchange;v=b3;q=0.9',
@@ -56,14 +64,16 @@
         except Exception as e:
             logger.error(f'tls request error: {e}')
         return response
 
     async def request(self, url, params=None, headers=None, cookies=None, auth=None, proxies=None, allow_redirects=True,
                       verify=True, http2=False,  content=None, data=None, files=None, json=None, stream=False,
                       timeout=30, cycle=3, tls=False):
+        if not self.ssl_context:
+            self.create_ssl_context(verify)
         if data or json or content:
             method = 'POST'
         else:
             method = 'GET'
         if not headers:
             headers = await self.gen_headers()
         if tls:
@@ -71,23 +81,31 @@
         response = Response()
         response.request_url = url
         for _ in range(cycle):
             try:
                 if stream:
                     client = httpx.AsyncClient(proxies=proxies, event_hooks={'response': [self.log_response]},
                                                verify=verify, http2=http2, follow_redirects=allow_redirects)
+                    try:
+                        list(client._mounts.values())[0]._pool._ssl_context = self.ssl_context
+                    except:
+                        pass
                     request = client.build_request(method=method, url=url, headers=headers, cookies=cookies,
                                                    content=content, data=data, files=files, json=json, timeout=timeout)
                     resp = await client.send(request, stream=True)
                     response.response = resp
                     response.ok = True
                     response.client = client  # need aclose
                 else:
                     async with httpx.AsyncClient(proxies=proxies, event_hooks={'response': [self.log_response]},
                                                  verify=verify, http2=http2) as client:
+                        try:
+                            list(client._mounts.values())[0]._pool._ssl_context = self.ssl_context
+                        except:
+                            pass
                         resp = await client.request(
                             method=method, url=url, content=content, data=data, files=files, json=json, params=params,
                             headers=headers, cookies=cookies, auth=auth, follow_redirects=allow_redirects,
                             timeout=timeout
                         )
                         response.response = resp
                         response.ok = True
```

### Comparing `hscan-2.6.1/scan/log.py` & `hscan-2.7.0/scan/log.py`

 * *Files identical despite different names*

### Comparing `hscan-2.6.1/scan/monitor.py` & `hscan-2.7.0/scan/monitor.py`

 * *Files identical despite different names*

### Comparing `hscan-2.6.1/scan/response.py` & `hscan-2.7.0/scan/response.py`

 * *Files identical despite different names*

### Comparing `hscan-2.6.1/scan/spider.py` & `hscan-2.7.0/scan/spider.py`

 * *Files identical despite different names*

### Comparing `hscan-2.6.1/scan/util.py` & `hscan-2.7.0/scan/util.py`

 * *Files identical despite different names*

