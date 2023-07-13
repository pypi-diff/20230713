# Comparing `tmp/amqp_mqtt_transport-0.1.8.tar.gz` & `tmp/amqp_mqtt_transport-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amqp_mqtt_transport-0.1.8.tar", last modified: Tue Jun 20 21:07:43 2023, max compression
+gzip compressed data, was "amqp_mqtt_transport-0.1.9.tar", last modified: Tue Jun 20 21:22:59 2023, max compression
```

## Comparing `amqp_mqtt_transport-0.1.8.tar` & `amqp_mqtt_transport-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-20 21:07:43.453536 amqp_mqtt_transport-0.1.8/
--rw-r--r--   0 igor      (1001) igor      (1001)       87 2023-06-19 12:04:53.000000 amqp_mqtt_transport-0.1.8/.gitattributes
--rw-r--r--   0 igor      (1001) igor      (1001)      483 2023-06-19 12:04:52.000000 amqp_mqtt_transport-0.1.8/.gitignore
--rw-rw-r--   0 igor      (1001) igor      (1001)     1072 2023-06-19 12:17:58.000000 amqp_mqtt_transport-0.1.8/LICENSE
--rw-rw-r--   0 igor      (1001) igor      (1001)     1054 2023-06-19 13:51:37.000000 amqp_mqtt_transport-0.1.8/Makefile
--rw-rw-r--   0 igor      (1001) igor      (1001)     1255 2023-06-20 21:07:43.449536 amqp_mqtt_transport-0.1.8/PKG-INFO
--rw-r--r--   0 igor      (1001) igor      (1001)      788 2023-06-19 13:04:30.000000 amqp_mqtt_transport-0.1.8/README.md
-drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-20 21:07:43.421536 amqp_mqtt_transport-0.1.8/amqp_mqtt_transport/
--rw-rw-r--   0 igor      (1001) igor      (1001)      152 2023-06-20 19:34:21.000000 amqp_mqtt_transport-0.1.8/amqp_mqtt_transport/__init__.py
--rw-rw-r--   0 igor      (1001) igor      (1001)      941 2023-06-20 20:42:25.000000 amqp_mqtt_transport-0.1.8/amqp_mqtt_transport/abc.py
-drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-20 21:07:43.445536 amqp_mqtt_transport-0.1.8/amqp_mqtt_transport/amqp/
--rw-rw-r--   0 igor      (1001) igor      (1001)       75 2023-06-19 12:15:27.000000 amqp_mqtt_transport-0.1.8/amqp_mqtt_transport/amqp/__init__.py
--rw-rw-r--   0 igor      (1001) igor      (1001)     1738 2023-06-20 19:43:16.000000 amqp_mqtt_transport-0.1.8/amqp_mqtt_transport/amqp/consumer.py
--rw-rw-r--   0 igor      (1001) igor      (1001)     5545 2023-06-20 20:56:30.000000 amqp_mqtt_transport-0.1.8/amqp_mqtt_transport/amqp/controller.py
--rw-rw-r--   0 igor      (1001) igor      (1001)     1532 2023-06-20 20:39:25.000000 amqp_mqtt_transport-0.1.8/amqp_mqtt_transport/amqp/publisher.py
--rw-rw-r--   0 igor      (1001) igor      (1001)     2146 2023-06-20 20:41:28.000000 amqp_mqtt_transport-0.1.8/amqp_mqtt_transport/message_scheduler.py
-drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-20 21:07:43.449536 amqp_mqtt_transport-0.1.8/amqp_mqtt_transport/mqtt/
--rw-rw-r--   0 igor      (1001) igor      (1001)       51 2023-06-19 12:15:30.000000 amqp_mqtt_transport-0.1.8/amqp_mqtt_transport/mqtt/__init__.py
--rw-rw-r--   0 igor      (1001) igor      (1001)     3127 2023-06-20 20:39:47.000000 amqp_mqtt_transport-0.1.8/amqp_mqtt_transport/mqtt/controller.py
--rw-rw-r--   0 igor      (1001) igor      (1001)      818 2023-06-20 20:40:10.000000 amqp_mqtt_transport-0.1.8/amqp_mqtt_transport/mqtt/publisher.py
--rw-rw-r--   0 igor      (1001) igor      (1001)     2450 2023-06-20 20:41:01.000000 amqp_mqtt_transport-0.1.8/amqp_mqtt_transport/scheduled_publisher.py
-drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-20 21:07:43.433536 amqp_mqtt_transport-0.1.8/amqp_mqtt_transport.egg-info/
--rw-rw-r--   0 igor      (1001) igor      (1001)     1255 2023-06-20 21:07:43.000000 amqp_mqtt_transport-0.1.8/amqp_mqtt_transport.egg-info/PKG-INFO
--rw-rw-r--   0 igor      (1001) igor      (1001)      698 2023-06-20 21:07:43.000000 amqp_mqtt_transport-0.1.8/amqp_mqtt_transport.egg-info/SOURCES.txt
--rw-rw-r--   0 igor      (1001) igor      (1001)        1 2023-06-20 21:07:43.000000 amqp_mqtt_transport-0.1.8/amqp_mqtt_transport.egg-info/dependency_links.txt
--rw-rw-r--   0 igor      (1001) igor      (1001)       79 2023-06-20 21:07:43.000000 amqp_mqtt_transport-0.1.8/amqp_mqtt_transport.egg-info/requires.txt
--rw-rw-r--   0 igor      (1001) igor      (1001)       20 2023-06-20 21:07:43.000000 amqp_mqtt_transport-0.1.8/amqp_mqtt_transport.egg-info/top_level.txt
--rw-rw-r--   0 igor      (1001) igor      (1001)      779 2023-06-20 21:06:45.000000 amqp_mqtt_transport-0.1.8/pyproject.toml
--rw-rw-r--   0 igor      (1001) igor      (1001)       38 2023-06-20 21:07:43.453536 amqp_mqtt_transport-0.1.8/setup.cfg
--rw-rw-r--   0 igor      (1001) igor      (1001)       37 2023-06-19 12:41:38.000000 amqp_mqtt_transport-0.1.8/setup.py
+drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-20 21:22:59.107315 amqp_mqtt_transport-0.1.9/
+-rw-r--r--   0 igor      (1001) igor      (1001)       87 2023-06-19 12:04:53.000000 amqp_mqtt_transport-0.1.9/.gitattributes
+-rw-r--r--   0 igor      (1001) igor      (1001)      483 2023-06-19 12:04:52.000000 amqp_mqtt_transport-0.1.9/.gitignore
+-rw-rw-r--   0 igor      (1001) igor      (1001)     1072 2023-06-19 12:17:58.000000 amqp_mqtt_transport-0.1.9/LICENSE
+-rw-rw-r--   0 igor      (1001) igor      (1001)     1054 2023-06-19 13:51:37.000000 amqp_mqtt_transport-0.1.9/Makefile
+-rw-rw-r--   0 igor      (1001) igor      (1001)     1255 2023-06-20 21:22:59.107315 amqp_mqtt_transport-0.1.9/PKG-INFO
+-rw-r--r--   0 igor      (1001) igor      (1001)      788 2023-06-19 13:04:30.000000 amqp_mqtt_transport-0.1.9/README.md
+drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-20 21:22:59.099315 amqp_mqtt_transport-0.1.9/amqp_mqtt_transport/
+-rw-rw-r--   0 igor      (1001) igor      (1001)      152 2023-06-20 19:34:21.000000 amqp_mqtt_transport-0.1.9/amqp_mqtt_transport/__init__.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)      941 2023-06-20 20:42:25.000000 amqp_mqtt_transport-0.1.9/amqp_mqtt_transport/abc.py
+drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-20 21:22:59.103315 amqp_mqtt_transport-0.1.9/amqp_mqtt_transport/amqp/
+-rw-rw-r--   0 igor      (1001) igor      (1001)       75 2023-06-19 12:15:27.000000 amqp_mqtt_transport-0.1.9/amqp_mqtt_transport/amqp/__init__.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     1738 2023-06-20 19:43:16.000000 amqp_mqtt_transport-0.1.9/amqp_mqtt_transport/amqp/consumer.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     5545 2023-06-20 20:56:30.000000 amqp_mqtt_transport-0.1.9/amqp_mqtt_transport/amqp/controller.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     1532 2023-06-20 20:39:25.000000 amqp_mqtt_transport-0.1.9/amqp_mqtt_transport/amqp/publisher.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     2146 2023-06-20 20:41:28.000000 amqp_mqtt_transport-0.1.9/amqp_mqtt_transport/message_scheduler.py
+drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-20 21:22:59.103315 amqp_mqtt_transport-0.1.9/amqp_mqtt_transport/mqtt/
+-rw-rw-r--   0 igor      (1001) igor      (1001)       51 2023-06-19 12:15:30.000000 amqp_mqtt_transport-0.1.9/amqp_mqtt_transport/mqtt/__init__.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     3128 2023-06-20 21:22:02.000000 amqp_mqtt_transport-0.1.9/amqp_mqtt_transport/mqtt/controller.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)      818 2023-06-20 20:40:10.000000 amqp_mqtt_transport-0.1.9/amqp_mqtt_transport/mqtt/publisher.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     2450 2023-06-20 20:41:01.000000 amqp_mqtt_transport-0.1.9/amqp_mqtt_transport/scheduled_publisher.py
+drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-20 21:22:59.103315 amqp_mqtt_transport-0.1.9/amqp_mqtt_transport.egg-info/
+-rw-rw-r--   0 igor      (1001) igor      (1001)     1255 2023-06-20 21:22:59.000000 amqp_mqtt_transport-0.1.9/amqp_mqtt_transport.egg-info/PKG-INFO
+-rw-rw-r--   0 igor      (1001) igor      (1001)      698 2023-06-20 21:22:59.000000 amqp_mqtt_transport-0.1.9/amqp_mqtt_transport.egg-info/SOURCES.txt
+-rw-rw-r--   0 igor      (1001) igor      (1001)        1 2023-06-20 21:22:59.000000 amqp_mqtt_transport-0.1.9/amqp_mqtt_transport.egg-info/dependency_links.txt
+-rw-rw-r--   0 igor      (1001) igor      (1001)       62 2023-06-20 21:22:59.000000 amqp_mqtt_transport-0.1.9/amqp_mqtt_transport.egg-info/requires.txt
+-rw-rw-r--   0 igor      (1001) igor      (1001)       20 2023-06-20 21:22:59.000000 amqp_mqtt_transport-0.1.9/amqp_mqtt_transport.egg-info/top_level.txt
+-rw-rw-r--   0 igor      (1001) igor      (1001)      755 2023-06-20 21:22:11.000000 amqp_mqtt_transport-0.1.9/pyproject.toml
+-rw-rw-r--   0 igor      (1001) igor      (1001)       38 2023-06-20 21:22:59.107315 amqp_mqtt_transport-0.1.9/setup.cfg
+-rw-rw-r--   0 igor      (1001) igor      (1001)       37 2023-06-19 12:41:38.000000 amqp_mqtt_transport-0.1.9/setup.py
```

### Comparing `amqp_mqtt_transport-0.1.8/LICENSE` & `amqp_mqtt_transport-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `amqp_mqtt_transport-0.1.8/Makefile` & `amqp_mqtt_transport-0.1.9/Makefile`

 * *Files identical despite different names*

### Comparing `amqp_mqtt_transport-0.1.8/PKG-INFO` & `amqp_mqtt_transport-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amqp_mqtt_transport
-Version: 0.1.8
+Version: 0.1.9
 Summary: Small wrapper for pykka-amqp and paho-mqtt packages. Makes it easier to create consumers/publishers
 Author-email: Igor Toropov <it.cups.54@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `amqp_mqtt_transport-0.1.8/README.md` & `amqp_mqtt_transport-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `amqp_mqtt_transport-0.1.8/amqp_mqtt_transport/abc.py` & `amqp_mqtt_transport-0.1.9/amqp_mqtt_transport/abc.py`

 * *Files identical despite different names*

### Comparing `amqp_mqtt_transport-0.1.8/amqp_mqtt_transport/amqp/consumer.py` & `amqp_mqtt_transport-0.1.9/amqp_mqtt_transport/amqp/consumer.py`

 * *Files identical despite different names*

### Comparing `amqp_mqtt_transport-0.1.8/amqp_mqtt_transport/amqp/controller.py` & `amqp_mqtt_transport-0.1.9/amqp_mqtt_transport/amqp/controller.py`

 * *Files identical despite different names*

### Comparing `amqp_mqtt_transport-0.1.8/amqp_mqtt_transport/amqp/publisher.py` & `amqp_mqtt_transport-0.1.9/amqp_mqtt_transport/amqp/publisher.py`

 * *Files identical despite different names*

### Comparing `amqp_mqtt_transport-0.1.8/amqp_mqtt_transport/message_scheduler.py` & `amqp_mqtt_transport-0.1.9/amqp_mqtt_transport/message_scheduler.py`

 * *Files identical despite different names*

### Comparing `amqp_mqtt_transport-0.1.8/amqp_mqtt_transport/mqtt/controller.py` & `amqp_mqtt_transport-0.1.9/amqp_mqtt_transport/mqtt/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import mqtt
+import gmqtt
 
 import logging
 import tenacity
 import tenacity.stop
 import tenacity.wait
 import functools
 from amqp_mqtt_transport.abc import Controller
```

### Comparing `amqp_mqtt_transport-0.1.8/amqp_mqtt_transport/mqtt/publisher.py` & `amqp_mqtt_transport-0.1.9/amqp_mqtt_transport/mqtt/publisher.py`

 * *Files identical despite different names*

### Comparing `amqp_mqtt_transport-0.1.8/amqp_mqtt_transport/scheduled_publisher.py` & `amqp_mqtt_transport-0.1.9/amqp_mqtt_transport/scheduled_publisher.py`

 * *Files identical despite different names*

### Comparing `amqp_mqtt_transport-0.1.8/amqp_mqtt_transport.egg-info/PKG-INFO` & `amqp_mqtt_transport-0.1.9/amqp_mqtt_transport.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amqp-mqtt-transport
-Version: 0.1.8
+Version: 0.1.9
 Summary: Small wrapper for pykka-amqp and paho-mqtt packages. Makes it easier to create consumers/publishers
 Author-email: Igor Toropov <it.cups.54@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `amqp_mqtt_transport-0.1.8/amqp_mqtt_transport.egg-info/SOURCES.txt` & `amqp_mqtt_transport-0.1.9/amqp_mqtt_transport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amqp_mqtt_transport-0.1.8/pyproject.toml` & `amqp_mqtt_transport-0.1.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "amqp_mqtt_transport"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Igor Toropov", email="it.cups.54@gmail.com" },
 ]
 description = "Small wrapper for pykka-amqp and paho-mqtt packages. Makes it easier to create consumers/publishers"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
@@ -17,15 +17,14 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "tenacity<=8.2.2",
     "aio-pika<=9.0.5",
     "autopep8==2.0.2",
-    "paho-mqtt==1.5.1",
     "gmqtt<=0.6.12"
 ]
 
 [tool.autopep8]
 max_line_length = 120
 ignore = []
 recursive = true
```

