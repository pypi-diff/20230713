# Comparing `tmp/moesifdjango-2.3.2.tar.gz` & `tmp/moesifdjango-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/moesifdjango-2.3.2.tar", last modified: Sat Jul  1 00:57:44 2023, max compression
+gzip compressed data, was "moesifdjango-2.3.3.tar", last modified: Wed Jul 12 22:37:49 2023, max compression
```

## Comparing `moesifdjango-2.3.2.tar` & `moesifdjango-2.3.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-07-01 00:57:44.613497 moesifdjango-2.3.2/
--rwxr-xr-x   0 keyur      (501) staff       (20)    11918 2020-12-27 23:18:46.000000 moesifdjango-2.3.2/LICENSE
--rw-r--r--   0 keyur      (501) staff       (20)       61 2020-05-04 14:40:14.000000 moesifdjango-2.3.2/MANIFEST.in
--rw-r--r--   0 keyur      (501) staff       (20)    23072 2023-07-01 00:57:44.614194 moesifdjango-2.3.2/PKG-INFO
--rwxr-xr-x   0 keyur      (501) staff       (20)    18400 2022-07-12 17:48:38.000000 moesifdjango-2.3.2/README.md
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-07-01 00:57:44.602151 moesifdjango-2.3.2/moesifdjango/
--rw-r--r--   0 keyur      (501) staff       (20)       63 2020-05-04 14:40:14.000000 moesifdjango-2.3.2/moesifdjango/__init__.py
--rw-r--r--   0 keyur      (501) staff       (20)      666 2023-07-01 00:56:37.000000 moesifdjango-2.3.2/moesifdjango/block_response_buffer.py
--rw-r--r--   0 keyur      (501) staff       (20)     4855 2020-12-29 03:43:47.000000 moesifdjango-2.3.2/moesifdjango/client_ip.py
--rw-r--r--   0 keyur      (501) staff       (20)     1570 2023-07-01 00:56:37.000000 moesifdjango-2.3.2/moesifdjango/event_mapper.py
--rw-r--r--   0 keyur      (501) staff       (20)      555 2023-07-01 00:56:37.000000 moesifdjango-2.3.2/moesifdjango/governance_rule_response.py
--rw-r--r--   0 keyur      (501) staff       (20)     2152 2022-07-12 17:48:38.000000 moesifdjango-2.3.2/moesifdjango/governance_rules.py
--rw-r--r--   0 keyur      (501) staff       (20)      616 2020-05-04 14:40:14.000000 moesifdjango-2.3.2/moesifdjango/http_response_catcher.py
--rw-r--r--   0 keyur      (501) staff       (20)     3212 2023-06-30 20:29:59.000000 moesifdjango-2.3.2/moesifdjango/job_scheduler.py
--rw-r--r--   0 keyur      (501) staff       (20)    14517 2021-07-08 18:25:55.000000 moesifdjango-2.3.2/moesifdjango/logger_helper.py
--rw-r--r--   0 keyur      (501) staff       (20)     1403 2020-12-29 05:09:32.000000 moesifdjango-2.3.2/moesifdjango/masks.py
--rw-r--r--   0 keyur      (501) staff       (20)    17343 2023-07-01 00:56:37.000000 moesifdjango-2.3.2/moesifdjango/middleware.py
--rw-r--r--   0 keyur      (501) staff       (20)    14371 2023-06-30 20:31:52.000000 moesifdjango-2.3.2/moesifdjango/middleware_pre19.py
--rw-r--r--   0 keyur      (501) staff       (20)    25617 2023-07-01 00:56:37.000000 moesifdjango-2.3.2/moesifdjango/moesif_gov.py
--rw-r--r--   0 keyur      (501) staff       (20)     2471 2022-07-12 17:48:38.000000 moesifdjango-2.3.2/moesifdjango/parse_body.py
--rw-r--r--   0 keyur      (501) staff       (20)     6657 2020-12-29 03:47:33.000000 moesifdjango-2.3.2/moesifdjango/update_companies.py
--rw-r--r--   0 keyur      (501) staff       (20)     6381 2020-12-29 03:47:52.000000 moesifdjango-2.3.2/moesifdjango/update_users.py
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-07-01 00:57:44.609494 moesifdjango-2.3.2/moesifdjango.egg-info/
--rw-r--r--   0 keyur      (501) staff       (20)    23072 2023-07-01 00:57:44.000000 moesifdjango-2.3.2/moesifdjango.egg-info/PKG-INFO
--rw-r--r--   0 keyur      (501) staff       (20)      861 2023-07-01 00:57:44.000000 moesifdjango-2.3.2/moesifdjango.egg-info/SOURCES.txt
--rw-r--r--   0 keyur      (501) staff       (20)        1 2023-07-01 00:57:44.000000 moesifdjango-2.3.2/moesifdjango.egg-info/dependency_links.txt
--rw-r--r--   0 keyur      (501) staff       (20)      136 2023-07-01 00:57:44.000000 moesifdjango-2.3.2/moesifdjango.egg-info/requires.txt
--rw-r--r--   0 keyur      (501) staff       (20)       19 2023-07-01 00:57:44.000000 moesifdjango-2.3.2/moesifdjango.egg-info/top_level.txt
--rw-r--r--   0 keyur      (501) staff       (20)       67 2023-07-01 00:57:44.615083 moesifdjango-2.3.2/setup.cfg
--rw-r--r--   0 keyur      (501) staff       (20)     3363 2023-07-01 00:56:37.000000 moesifdjango-2.3.2/setup.py
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-07-01 00:57:44.571308 moesifdjango-2.3.2/tests/
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-07-01 00:57:44.610762 moesifdjango-2.3.2/tests/middleware_pre19_tests/
--rw-r--r--   0 keyur      (501) staff       (20)        0 2020-05-04 14:40:14.000000 moesifdjango-2.3.2/tests/middleware_pre19_tests/__init__.py
--rw-r--r--   0 keyur      (501) staff       (20)     4990 2020-12-29 19:17:16.000000 moesifdjango-2.3.2/tests/middleware_pre19_tests/tests.py
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-07-01 00:57:44.612281 moesifdjango-2.3.2/tests/middleware_tests/
--rw-r--r--   0 keyur      (501) staff       (20)        0 2020-05-04 14:40:14.000000 moesifdjango-2.3.2/tests/middleware_tests/__init__.py
--rw-r--r--   0 keyur      (501) staff       (20)     5266 2022-07-12 17:48:38.000000 moesifdjango-2.3.2/tests/middleware_tests/tests.py
+drwxr-xr-x   0 brian     (1000) brian     (1001)        0 2023-07-12 22:37:49.656316 moesifdjango-2.3.3/
+-rwxr-xr-x   0 brian     (1000) brian     (1001)    11918 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/LICENSE
+-rw-r--r--   0 brian     (1000) brian     (1001)       61 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/MANIFEST.in
+-rw-r--r--   0 brian     (1000) brian     (1001)    19503 2023-07-12 22:37:49.656316 moesifdjango-2.3.3/PKG-INFO
+-rwxr-xr-x   0 brian     (1000) brian     (1001)    18400 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/README.md
+drwxr-xr-x   0 brian     (1000) brian     (1001)        0 2023-07-12 22:37:49.656316 moesifdjango-2.3.3/moesifdjango/
+-rw-r--r--   0 brian     (1000) brian     (1001)       63 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/moesifdjango/__init__.py
+-rw-r--r--   0 brian     (1000) brian     (1001)      666 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/moesifdjango/block_response_buffer.py
+-rw-r--r--   0 brian     (1000) brian     (1001)     4855 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/moesifdjango/client_ip.py
+-rw-r--r--   0 brian     (1000) brian     (1001)     1570 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/moesifdjango/event_mapper.py
+-rw-r--r--   0 brian     (1000) brian     (1001)      555 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/moesifdjango/governance_rule_response.py
+-rw-r--r--   0 brian     (1000) brian     (1001)     2152 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/moesifdjango/governance_rules.py
+-rw-r--r--   0 brian     (1000) brian     (1001)      616 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/moesifdjango/http_response_catcher.py
+-rw-r--r--   0 brian     (1000) brian     (1001)     3699 2023-07-12 22:28:28.000000 moesifdjango-2.3.3/moesifdjango/job_scheduler.py
+-rw-r--r--   0 brian     (1000) brian     (1001)    14517 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/moesifdjango/logger_helper.py
+-rw-r--r--   0 brian     (1000) brian     (1001)     1403 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/moesifdjango/masks.py
+-rw-r--r--   0 brian     (1000) brian     (1001)    17343 2023-07-12 22:37:26.000000 moesifdjango-2.3.3/moesifdjango/middleware.py
+-rw-r--r--   0 brian     (1000) brian     (1001)    14371 2023-07-12 20:54:27.000000 moesifdjango-2.3.3/moesifdjango/middleware_pre19.py
+-rw-r--r--   0 brian     (1000) brian     (1001)    25617 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/moesifdjango/moesif_gov.py
+-rw-r--r--   0 brian     (1000) brian     (1001)     2471 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/moesifdjango/parse_body.py
+-rw-r--r--   0 brian     (1000) brian     (1001)     6657 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/moesifdjango/update_companies.py
+-rw-r--r--   0 brian     (1000) brian     (1001)     6381 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/moesifdjango/update_users.py
+drwxr-xr-x   0 brian     (1000) brian     (1001)        0 2023-07-12 22:37:49.656316 moesifdjango-2.3.3/moesifdjango.egg-info/
+-rw-r--r--   0 brian     (1000) brian     (1001)    19503 2023-07-12 22:37:49.000000 moesifdjango-2.3.3/moesifdjango.egg-info/PKG-INFO
+-rw-r--r--   0 brian     (1000) brian     (1001)      861 2023-07-12 22:37:49.000000 moesifdjango-2.3.3/moesifdjango.egg-info/SOURCES.txt
+-rw-r--r--   0 brian     (1000) brian     (1001)        1 2023-07-12 22:37:49.000000 moesifdjango-2.3.3/moesifdjango.egg-info/dependency_links.txt
+-rw-r--r--   0 brian     (1000) brian     (1001)      136 2023-07-12 22:37:49.000000 moesifdjango-2.3.3/moesifdjango.egg-info/requires.txt
+-rw-r--r--   0 brian     (1000) brian     (1001)       19 2023-07-12 22:37:49.000000 moesifdjango-2.3.3/moesifdjango.egg-info/top_level.txt
+-rw-r--r--   0 brian     (1000) brian     (1001)       67 2023-07-12 22:37:49.656316 moesifdjango-2.3.3/setup.cfg
+-rw-r--r--   0 brian     (1000) brian     (1001)     3363 2023-07-12 21:19:51.000000 moesifdjango-2.3.3/setup.py
+drwxr-xr-x   0 brian     (1000) brian     (1001)        0 2023-07-12 22:37:49.656316 moesifdjango-2.3.3/tests/
+drwxr-xr-x   0 brian     (1000) brian     (1001)        0 2023-07-12 22:37:49.656316 moesifdjango-2.3.3/tests/middleware_pre19_tests/
+-rw-r--r--   0 brian     (1000) brian     (1001)        0 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/tests/middleware_pre19_tests/__init__.py
+-rw-r--r--   0 brian     (1000) brian     (1001)     4990 2023-07-12 21:17:50.000000 moesifdjango-2.3.3/tests/middleware_pre19_tests/tests.py
+drwxr-xr-x   0 brian     (1000) brian     (1001)        0 2023-07-12 22:37:49.656316 moesifdjango-2.3.3/tests/middleware_tests/
+-rw-r--r--   0 brian     (1000) brian     (1001)        0 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/tests/middleware_tests/__init__.py
+-rw-r--r--   0 brian     (1000) brian     (1001)     5266 2023-07-12 20:42:10.000000 moesifdjango-2.3.3/tests/middleware_tests/tests.py
```

### Comparing `moesifdjango-2.3.2/LICENSE` & `moesifdjango-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.2/README.md` & `moesifdjango-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.2/moesifdjango/block_response_buffer.py` & `moesifdjango-2.3.3/moesifdjango/block_response_buffer.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.2/moesifdjango/client_ip.py` & `moesifdjango-2.3.3/moesifdjango/client_ip.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.2/moesifdjango/event_mapper.py` & `moesifdjango-2.3.3/moesifdjango/event_mapper.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.2/moesifdjango/governance_rule_response.py` & `moesifdjango-2.3.3/moesifdjango/governance_rule_response.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.2/moesifdjango/governance_rules.py` & `moesifdjango-2.3.3/moesifdjango/governance_rules.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.2/moesifdjango/http_response_catcher.py` & `moesifdjango-2.3.3/moesifdjango/http_response_catcher.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.2/moesifdjango/job_scheduler.py` & `moesifdjango-2.3.3/moesifdjango/job_scheduler.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,27 +45,33 @@
             if debug:
                 print('Error while fetching the application configuration')
                 print(str(e))
         return config, config_etag, sampling_percentage, last_updated_time
 
 
     def batch_events(self, api_client, moesif_events_queue, debug, batch_size):
-
+        print("Starting batch events job")
         batch_events = []
         try:
             while not moesif_events_queue.empty():
                 batch_events.append(moesif_events_queue.get_nowait())
                 if len(batch_events) == batch_size:
                     break
 
             if batch_events:
+                req_time = batch_events[0].request.time
+                req_time = datetime.strptime(req_time, '%Y-%m-%dT%H:%M:%S.%f')
                 batch_response_config_etag, batch_response_rules_etag = self.send_events(api_client, batch_events, debug)
                 batch_events[:] = []
                 # Set the last time event job ran after sending events
-                return batch_response_config_etag, batch_response_rules_etag, datetime.utcnow()
+                batch_send_time = datetime.utcnow()
+                delta = batch_send_time - req_time
+                if debug and delta.total_seconds() > 0:
+                    print("Warning: It took %s seconds to send events to Moesif. req.time=%s now=%s"%(delta.total_seconds(), req_time, batch_send_time))
+                return batch_response_config_etag, batch_response_rules_etag, batch_send_time
             else:
                 if debug:
                     print("No events to send")
                 # Set the last time event job ran but no message to read from the queue
                 return None, None, datetime.utcnow()
         except Exception as e:
             if debug:
```

### Comparing `moesifdjango-2.3.2/moesifdjango/logger_helper.py` & `moesifdjango-2.3.3/moesifdjango/logger_helper.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.2/moesifdjango/masks.py` & `moesifdjango-2.3.3/moesifdjango/masks.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.2/moesifdjango/middleware.py` & `moesifdjango-2.3.3/moesifdjango/middleware.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.2/moesifdjango/middleware_pre19.py` & `moesifdjango-2.3.3/moesifdjango/middleware_pre19.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.2/moesifdjango/moesif_gov.py` & `moesifdjango-2.3.3/moesifdjango/moesif_gov.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.2/moesifdjango/parse_body.py` & `moesifdjango-2.3.3/moesifdjango/parse_body.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.2/moesifdjango/update_companies.py` & `moesifdjango-2.3.3/moesifdjango/update_companies.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.2/moesifdjango/update_users.py` & `moesifdjango-2.3.3/moesifdjango/update_users.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.2/moesifdjango.egg-info/SOURCES.txt` & `moesifdjango-2.3.3/moesifdjango.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.2/setup.py` & `moesifdjango-2.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 setup(
     name='moesifdjango',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='2.3.2',
+    version='2.3.3',
 
     description='Moesif Middleware for Python Django',
     long_description=long_description,
     long_description_content_type="text/markdown",
     
     # The project's main homepage.
     url='https://www.moesif.com/docs/server-integration/django/',
```

### Comparing `moesifdjango-2.3.2/tests/middleware_pre19_tests/tests.py` & `moesifdjango-2.3.3/tests/middleware_pre19_tests/tests.py`

 * *Files identical despite different names*

### Comparing `moesifdjango-2.3.2/tests/middleware_tests/tests.py` & `moesifdjango-2.3.3/tests/middleware_tests/tests.py`

 * *Files identical despite different names*

