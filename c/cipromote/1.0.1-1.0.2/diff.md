# Comparing `tmp/cipromote-1.0.1.tar.gz` & `tmp/cipromote-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cipromote-1.0.1.tar", max compression
+gzip compressed data, was "cipromote-1.0.2.tar", max compression
```

## Comparing `cipromote-1.0.1.tar` & `cipromote-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       68 2023-03-13 15:43:49.230739 cipromote-1.0.1/README.md
--rw-r--r--   0        0        0      548 2023-06-20 21:26:30.105404 cipromote-1.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-01 21:23:03.887994 cipromote-1.0.1/src/cipromote/__init__.py
--rw-r--r--   0        0        0    25204 2023-03-01 22:01:52.712793 cipromote-1.0.1/src/cipromote/ci-cli.py
--rw-r--r--   0        0        0     7585 2023-06-20 20:25:28.071576 cipromote-1.0.1/src/cipromote/cli.py
--rw-r--r--   0        0        0      114 2023-03-01 22:01:52.717793 cipromote-1.0.1/src/cipromote/constants.py
--rw-r--r--   0        0        0     1680 2023-03-02 20:06:52.453096 cipromote-1.0.1/src/cipromote/instances.py
--rw-r--r--   0        0        0     5708 2023-03-02 21:27:59.317150 cipromote-1.0.1/src/cipromote/label_versions.py
--rw-r--r--   0        0        0     3889 2023-03-02 20:55:55.574572 cipromote-1.0.1/src/cipromote/labels.py
--rw-r--r--   0        0        0      387 2023-03-02 15:58:17.336622 cipromote-1.0.1/src/cipromote/login.py
--rw-r--r--   0        0        0     3510 2023-03-02 15:12:46.158566 cipromote-1.0.1/src/cipromote/loginInput.py
--rw-r--r--   0        0        0     2981 2023-03-02 19:49:52.016215 cipromote-1.0.1/src/cipromote/projects.py
--rw-r--r--   0        0        0    11691 2023-03-01 22:01:52.726793 cipromote-1.0.1/src/cipromote/queries.py
--rw-r--r--   0        0        0     2158 2023-03-01 22:01:52.728793 cipromote-1.0.1/src/cipromote/versioned_items.py
--rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 cipromote-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       68 2023-03-13 15:43:49.230739 cipromote-1.0.2/README.md
+-rw-r--r--   0        0        0      548 2023-07-13 18:41:07.535298 cipromote-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-01 21:23:03.887994 cipromote-1.0.2/src/cipromote/__init__.py
+-rw-r--r--   0        0        0    25204 2023-03-01 22:01:52.712793 cipromote-1.0.2/src/cipromote/ci-cli.py
+-rw-r--r--   0        0        0     8334 2023-07-13 18:40:33.202353 cipromote-1.0.2/src/cipromote/cli.py
+-rw-r--r--   0        0        0      114 2023-03-01 22:01:52.717793 cipromote-1.0.2/src/cipromote/constants.py
+-rw-r--r--   0        0        0     1680 2023-03-02 20:06:52.453096 cipromote-1.0.2/src/cipromote/instances.py
+-rw-r--r--   0        0        0     5708 2023-03-02 21:27:59.317150 cipromote-1.0.2/src/cipromote/label_versions.py
+-rw-r--r--   0        0        0     3889 2023-03-02 20:55:55.574572 cipromote-1.0.2/src/cipromote/labels.py
+-rw-r--r--   0        0        0      387 2023-03-02 15:58:17.336622 cipromote-1.0.2/src/cipromote/login.py
+-rw-r--r--   0        0        0     3510 2023-03-02 15:12:46.158566 cipromote-1.0.2/src/cipromote/loginInput.py
+-rw-r--r--   0        0        0     2981 2023-03-02 19:49:52.016215 cipromote-1.0.2/src/cipromote/projects.py
+-rw-r--r--   0        0        0    11691 2023-03-01 22:01:52.726793 cipromote-1.0.2/src/cipromote/queries.py
+-rw-r--r--   0        0        0     2158 2023-03-01 22:01:52.728793 cipromote-1.0.2/src/cipromote/versioned_items.py
+-rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 cipromote-1.0.2/PKG-INFO
```

### Comparing `cipromote-1.0.1/pyproject.toml` & `cipromote-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cipromote"
-version = "1.0.1"
+version = "1.0.2"
 description = "Promote MotionCI Labels"
 authors = ["Michael MacKenna <mmackenna@ufginsurance.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.1.3"
```

### Comparing `cipromote-1.0.1/src/cipromote/ci-cli.py` & `cipromote-1.0.2/src/cipromote/ci-cli.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.0.1/src/cipromote/cli.py` & `cipromote-1.0.2/src/cipromote/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,17 +61,33 @@
     server_url = os.getenv("MOTIOCI_SERVERURL")
     constants.CI_URL = server_url
     constants.GRAPH_URL = constants.CI_URL + constants.GRAPH_URL
     print('Sending query to the following url')
     print(constants.GRAPH_URL)
     instance_object = instances.get_instances_default()
     pprint(instance_object)
-    #print(f"Instance 0 has these namespaces {instance_object[0]['node']['namespaces']}")
+    print(f"Instance 0 has these namespaces {instance_object[0]['node']['namespaces']}")
     return instance_object
 
+@main.command("get-instance", short_help="Get an instance by name")
+@click.argument("instance-name")
+def get_instance(instance_name):
+    """ Get a particular instance by name """
+    server_url = os.getenv("MOTIOCI_SERVERURL")
+    constants.CI_URL = server_url
+    constants.GRAPH_URL = constants.CI_URL + constants.GRAPH_URL
+    print('Sending query to the following url')
+    print(constants.GRAPH_URL)
+    instance_object = instances.get_instances_default()
+    for instance in instance_object:
+        if instance['node']['name'].lower() == instance_name.lower():
+            target_instance = instance
+            print(f"The target instance is {target_instance['node']['name']}")
+            pprint(target_instance)
+    return target_instance
 
 @main.command("get-labels", short_help="Get a list of available labels")
 def get_labels():
     """Gets a lit of available labels"""
     server_url = os.getenv("MOTIOCI_SERVERURL")
     constants.CI_URL = server_url
     constants.GRAPH_URL = constants.CI_URL + constants.GRAPH_URL
```

### Comparing `cipromote-1.0.1/src/cipromote/instances.py` & `cipromote-1.0.2/src/cipromote/instances.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.0.1/src/cipromote/label_versions.py` & `cipromote-1.0.2/src/cipromote/label_versions.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.0.1/src/cipromote/labels.py` & `cipromote-1.0.2/src/cipromote/labels.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.0.1/src/cipromote/loginInput.py` & `cipromote-1.0.2/src/cipromote/loginInput.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.0.1/src/cipromote/projects.py` & `cipromote-1.0.2/src/cipromote/projects.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.0.1/src/cipromote/queries.py` & `cipromote-1.0.2/src/cipromote/queries.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.0.1/src/cipromote/versioned_items.py` & `cipromote-1.0.2/src/cipromote/versioned_items.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.0.1/PKG-INFO` & `cipromote-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cipromote
-Version: 1.0.1
+Version: 1.0.2
 Summary: Promote MotionCI Labels
 Author: Michael MacKenna
 Author-email: mmackenna@ufginsurance.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

