# Comparing `tmp/w3bstream_client_python-1.0.0.tar.gz` & `tmp/w3bstream_client_python-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "w3bstream_client_python-1.0.0.tar", last modified: Thu Jul 13 17:37:01 2023, max compression
+gzip compressed data, was "w3bstream_client_python-1.0.1.tar", last modified: Thu Jul 13 19:09:46 2023, max compression
```

## Comparing `w3bstream_client_python-1.0.0.tar` & `w3bstream_client_python-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-13 17:37:01.583950 w3bstream_client_python-1.0.0/
--rw-r--r--   0 haaai     (1000) haaai     (1000)     3078 2023-06-30 05:29:14.000000 w3bstream_client_python-1.0.0/.gitignore
--rw-r--r--   0 haaai     (1000) haaai     (1000)    11357 2023-06-30 05:29:14.000000 w3bstream_client_python-1.0.0/LICENSE
--rw-r--r--   0 haaai     (1000) haaai     (1000)      886 2023-07-13 17:37:01.573950 w3bstream_client_python-1.0.0/PKG-INFO
--rw-r--r--   0 haaai     (1000) haaai     (1000)      709 2023-07-11 18:41:55.000000 w3bstream_client_python-1.0.0/README.md
--rw-r--r--   0 haaai     (1000) haaai     (1000)      391 2023-07-13 17:36:42.000000 w3bstream_client_python-1.0.0/pyproject.toml
--rw-r--r--   0 haaai     (1000) haaai     (1000)       38 2023-07-13 17:37:01.583950 w3bstream_client_python-1.0.0/setup.cfg
-drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-13 17:37:01.573950 w3bstream_client_python-1.0.0/src/
-drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-13 17:37:01.573950 w3bstream_client_python-1.0.0/src/w3bstream_client_python/
--rw-r--r--   0 haaai     (1000) haaai     (1000)       67 2023-07-10 18:18:02.000000 w3bstream_client_python-1.0.0/src/w3bstream_client_python/__init__.py
--rw-r--r--   0 haaai     (1000) haaai     (1000)     3773 2023-07-13 17:36:42.000000 w3bstream_client_python-1.0.0/src/w3bstream_client_python/client.py
-drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-13 17:37:01.573950 w3bstream_client_python-1.0.0/src/w3bstream_client_python.egg-info/
--rw-r--r--   0 haaai     (1000) haaai     (1000)      886 2023-07-13 17:37:01.000000 w3bstream_client_python-1.0.0/src/w3bstream_client_python.egg-info/PKG-INFO
--rw-r--r--   0 haaai     (1000) haaai     (1000)      375 2023-07-13 17:37:01.000000 w3bstream_client_python-1.0.0/src/w3bstream_client_python.egg-info/SOURCES.txt
--rw-r--r--   0 haaai     (1000) haaai     (1000)        1 2023-07-13 17:37:01.000000 w3bstream_client_python-1.0.0/src/w3bstream_client_python.egg-info/dependency_links.txt
--rw-r--r--   0 haaai     (1000) haaai     (1000)       19 2023-07-13 17:37:01.000000 w3bstream_client_python-1.0.0/src/w3bstream_client_python.egg-info/requires.txt
--rw-r--r--   0 haaai     (1000) haaai     (1000)       24 2023-07-13 17:37:01.000000 w3bstream_client_python-1.0.0/src/w3bstream_client_python.egg-info/top_level.txt
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-13 19:09:46.306090 w3bstream_client_python-1.0.1/
+-rw-r--r--   0 haaai     (1000) haaai     (1000)     3078 2023-06-30 05:29:14.000000 w3bstream_client_python-1.0.1/.gitignore
+-rw-r--r--   0 haaai     (1000) haaai     (1000)    11357 2023-06-30 05:29:14.000000 w3bstream_client_python-1.0.1/LICENSE
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      886 2023-07-13 19:09:46.306090 w3bstream_client_python-1.0.1/PKG-INFO
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      709 2023-07-11 18:41:55.000000 w3bstream_client_python-1.0.1/README.md
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      391 2023-07-13 19:09:03.000000 w3bstream_client_python-1.0.1/pyproject.toml
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       38 2023-07-13 19:09:46.306090 w3bstream_client_python-1.0.1/setup.cfg
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-13 19:09:46.306090 w3bstream_client_python-1.0.1/src/
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-13 19:09:46.306090 w3bstream_client_python-1.0.1/src/w3bstream_client_python/
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       67 2023-07-10 18:18:02.000000 w3bstream_client_python-1.0.1/src/w3bstream_client_python/__init__.py
+-rw-r--r--   0 haaai     (1000) haaai     (1000)     3774 2023-07-13 18:37:45.000000 w3bstream_client_python-1.0.1/src/w3bstream_client_python/client.py
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-13 19:09:46.306090 w3bstream_client_python-1.0.1/src/w3bstream_client_python.egg-info/
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      886 2023-07-13 19:09:46.000000 w3bstream_client_python-1.0.1/src/w3bstream_client_python.egg-info/PKG-INFO
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      375 2023-07-13 19:09:46.000000 w3bstream_client_python-1.0.1/src/w3bstream_client_python.egg-info/SOURCES.txt
+-rw-r--r--   0 haaai     (1000) haaai     (1000)        1 2023-07-13 19:09:46.000000 w3bstream_client_python-1.0.1/src/w3bstream_client_python.egg-info/dependency_links.txt
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       19 2023-07-13 19:09:46.000000 w3bstream_client_python-1.0.1/src/w3bstream_client_python.egg-info/requires.txt
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       24 2023-07-13 19:09:46.000000 w3bstream_client_python-1.0.1/src/w3bstream_client_python.egg-info/top_level.txt
```

### Comparing `w3bstream_client_python-1.0.0/.gitignore` & `w3bstream_client_python-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `w3bstream_client_python-1.0.0/LICENSE` & `w3bstream_client_python-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `w3bstream_client_python-1.0.0/PKG-INFO` & `w3bstream_client_python-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: w3bstream_client_python
-Version: 1.0.0
+Version: 1.0.1
 Summary: Official W3bstream Client for Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # w3bstream-client-python
 
 The Python Client for W3bstream integration on server
```

### Comparing `w3bstream_client_python-1.0.0/README.md` & `w3bstream_client_python-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `w3bstream_client_python-1.0.0/src/w3bstream_client_python/client.py` & `w3bstream_client_python-1.0.1/src/w3bstream_client_python/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         self.event_type = event_type
         self.device_id = device_id
         self.timestamp = timestamp
 
 
 PUBLISH_INTERVAL = 5
 PUBLISH_BATCH_SIZE = 10
-_DATA_PUSH_EVENT_TYPE = "$DATA#PUSH"
+_DATA_PUSH_EVENT_TYPE = "DA-TA_PU-SH"
 
 
 @typechecked
 class Client:
     def __init__(self, url: str, api_key: str, queue_size: int = 0):
         self.url = url
         self.api_key = api_key
```

### Comparing `w3bstream_client_python-1.0.0/src/w3bstream_client_python.egg-info/PKG-INFO` & `w3bstream_client_python-1.0.1/src/w3bstream_client_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: w3bstream-client-python
-Version: 1.0.0
+Version: 1.0.1
 Summary: Official W3bstream Client for Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # w3bstream-client-python
 
 The Python Client for W3bstream integration on server
```

