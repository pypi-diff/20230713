# Comparing `tmp/modelw_docker-2023.7.0.tar.gz` & `tmp/modelw_docker-2023.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelw_docker-2023.7.0.tar", max compression
+gzip compressed data, was "modelw_docker-2023.7.1.tar", max compression
```

## Comparing `modelw_docker-2023.7.0.tar` & `modelw_docker-2023.7.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      484 2023-07-03 17:29:48.345161 modelw_docker-2023.7.0/LICENSE
--rw-r--r--   0        0        0     4666 2023-07-03 17:29:48.345161 modelw_docker-2023.7.0/README.md
--rw-r--r--   0        0        0     1199 2023-07-03 17:29:48.345161 modelw_docker-2023.7.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-03 17:29:48.345161 modelw_docker-2023.7.0/src/model_w/docker/__init__.py
--rw-r--r--   0        0        0     2753 2023-07-03 17:29:48.349161 modelw_docker-2023.7.0/src/model_w/docker/__main__.py
--rw-r--r--   0        0        0     1494 2023-07-03 17:29:48.349161 modelw_docker-2023.7.0/src/model_w/docker/build.py
--rw-r--r--   0        0        0     7307 2023-07-03 17:29:48.349161 modelw_docker-2023.7.0/src/model_w/docker/config.py
--rw-r--r--   0        0        0      209 2023-07-03 17:29:48.349161 modelw_docker-2023.7.0/src/model_w/docker/exceptions.py
--rw-r--r--   0        0        0     5229 2023-07-03 17:29:48.349161 modelw_docker-2023.7.0/src/model_w/docker/install.py
--rw-r--r--   0        0        0     7755 2023-07-03 17:29:48.349161 modelw_docker-2023.7.0/src/model_w/docker/output.py
--rw-r--r--   0        0        0     1662 2023-07-03 17:29:48.349161 modelw_docker-2023.7.0/src/model_w/docker/platform.py
--rw-r--r--   0        0        0        0 2023-07-03 17:29:48.349161 modelw_docker-2023.7.0/src/model_w/docker/py.typed
--rw-r--r--   0        0        0     2580 2023-07-03 17:29:48.349161 modelw_docker-2023.7.0/src/model_w/docker/run.py
--rw-r--r--   0        0        0     5865 2023-07-03 17:29:48.349161 modelw_docker-2023.7.0/src/model_w/docker/serve.py
--rw-r--r--   0        0        0     5808 1970-01-01 00:00:00.000000 modelw_docker-2023.7.0/PKG-INFO
+-rw-r--r--   0        0        0      484 2023-07-13 07:57:58.042105 modelw_docker-2023.7.1/LICENSE
+-rw-r--r--   0        0        0     4666 2023-07-13 07:57:58.042105 modelw_docker-2023.7.1/README.md
+-rw-r--r--   0        0        0     1199 2023-07-13 07:57:58.046105 modelw_docker-2023.7.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-13 07:57:58.046105 modelw_docker-2023.7.1/src/model_w/docker/__init__.py
+-rw-r--r--   0        0        0     2753 2023-07-13 07:57:58.046105 modelw_docker-2023.7.1/src/model_w/docker/__main__.py
+-rw-r--r--   0        0        0     1494 2023-07-13 07:57:58.046105 modelw_docker-2023.7.1/src/model_w/docker/build.py
+-rw-r--r--   0        0        0     7307 2023-07-13 07:57:58.046105 modelw_docker-2023.7.1/src/model_w/docker/config.py
+-rw-r--r--   0        0        0      209 2023-07-13 07:57:58.046105 modelw_docker-2023.7.1/src/model_w/docker/exceptions.py
+-rw-r--r--   0        0        0     5229 2023-07-13 07:57:58.046105 modelw_docker-2023.7.1/src/model_w/docker/install.py
+-rw-r--r--   0        0        0     7755 2023-07-13 07:57:58.046105 modelw_docker-2023.7.1/src/model_w/docker/output.py
+-rw-r--r--   0        0        0     1662 2023-07-13 07:57:58.046105 modelw_docker-2023.7.1/src/model_w/docker/platform.py
+-rw-r--r--   0        0        0        0 2023-07-13 07:57:58.046105 modelw_docker-2023.7.1/src/model_w/docker/py.typed
+-rw-r--r--   0        0        0     2580 2023-07-13 07:57:58.046105 modelw_docker-2023.7.1/src/model_w/docker/run.py
+-rw-r--r--   0        0        0     5865 2023-07-13 07:57:58.046105 modelw_docker-2023.7.1/src/model_w/docker/serve.py
+-rw-r--r--   0        0        0     5808 1970-01-01 00:00:00.000000 modelw_docker-2023.7.1/PKG-INFO
```

### Comparing `modelw_docker-2023.7.0/README.md` & `modelw_docker-2023.7.1/README.md`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.7.0/pyproject.toml` & `modelw_docker-2023.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modelw-docker"
-version = "2023.7.0"
+version = "2023.7.1"
 description = "Utility to simplify Dockerfiles"
 authors = ["Rémy Sanchez <remy.sanchez@hyperthese.net>"]
 license = "WTFPL"
 readme = "README.md"
 packages = [{include = "model_w/docker", from = "src"}]
 repository = "https://github.com/ModelW/docker/"
 documentation = "https://github.com/ModelW/docker/"
```

### Comparing `modelw_docker-2023.7.0/src/model_w/docker/__main__.py` & `modelw_docker-2023.7.1/src/model_w/docker/__main__.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.7.0/src/model_w/docker/build.py` & `modelw_docker-2023.7.1/src/model_w/docker/build.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.7.0/src/model_w/docker/config.py` & `modelw_docker-2023.7.1/src/model_w/docker/config.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.7.0/src/model_w/docker/install.py` & `modelw_docker-2023.7.1/src/model_w/docker/install.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.7.0/src/model_w/docker/output.py` & `modelw_docker-2023.7.1/src/model_w/docker/output.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.7.0/src/model_w/docker/platform.py` & `modelw_docker-2023.7.1/src/model_w/docker/platform.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.7.0/src/model_w/docker/run.py` & `modelw_docker-2023.7.1/src/model_w/docker/run.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.7.0/src/model_w/docker/serve.py` & `modelw_docker-2023.7.1/src/model_w/docker/serve.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.7.0/PKG-INFO` & `modelw_docker-2023.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelw-docker
-Version: 2023.7.0
+Version: 2023.7.1
 Summary: Utility to simplify Dockerfiles
 Home-page: https://github.com/ModelW/docker/
 License: WTFPL
 Keywords: docker,django,nuxt,dockerfile
 Author: Rémy Sanchez
 Author-email: remy.sanchez@hyperthese.net
 Requires-Python: >=3.10,<4.0
```

