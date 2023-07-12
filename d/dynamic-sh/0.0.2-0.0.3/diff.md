# Comparing `tmp/dynamic-sh-0.0.2.tar.gz` & `tmp/dynamic-sh-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic-sh-0.0.2.tar", last modified: Tue Jul 11 22:14:41 2023, max compression
+gzip compressed data, was "dynamic-sh-0.0.3.tar", last modified: Wed Jul 12 21:54:12 2023, max compression
```

## Comparing `dynamic-sh-0.0.2.tar` & `dynamic-sh-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:14:41.670680 dynamic-sh-0.0.2/
--rw-r--r--   0 omarwaseem   (501) staff       (20)      516 2023-07-11 22:14:41.670542 dynamic-sh-0.0.2/PKG-INFO
--rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-sh-0.0.2/README.md
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:14:41.667348 dynamic-sh-0.0.2/dynamic/
--rw-r--r--   0 omarwaseem   (501) staff       (20)     1400 2023-07-08 22:39:44.000000 dynamic-sh-0.0.2/dynamic/__init__.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:14:41.668379 dynamic-sh-0.0.2/dynamic/classes/
--rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-sh-0.0.2/dynamic/classes/__init__.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)     1280 2023-07-08 22:39:44.000000 dynamic-sh-0.0.2/dynamic/classes/agent.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)      133 2023-07-08 22:39:44.000000 dynamic-sh-0.0.2/dynamic/classes/chain.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)      245 2023-07-08 22:39:44.000000 dynamic-sh-0.0.2/dynamic/classes/logger.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)     1289 2023-07-11 18:24:11.000000 dynamic-sh-0.0.2/dynamic/classes/message.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:14:41.668954 dynamic-sh-0.0.2/dynamic/protocols/
--rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-sh-0.0.2/dynamic/protocols/__init__.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)    10102 2023-07-11 18:24:11.000000 dynamic-sh-0.0.2/dynamic/protocols/server.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)     1419 2023-07-11 18:24:11.000000 dynamic-sh-0.0.2/dynamic/protocols/ws.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:14:41.669096 dynamic-sh-0.0.2/dynamic/request/
--rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-sh-0.0.2/dynamic/request/__init__.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:14:41.669185 dynamic-sh-0.0.2/dynamic/response/
--rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-sh-0.0.2/dynamic/response/__init__.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:14:41.669559 dynamic-sh-0.0.2/dynamic/router/
--rw-r--r--   0 omarwaseem   (501) staff       (20)       47 2023-07-08 22:39:44.000000 dynamic-sh-0.0.2/dynamic/router/__init__.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)     2607 2023-07-08 22:39:44.000000 dynamic-sh-0.0.2/dynamic/router/get_file_routes.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)     2113 2023-07-08 22:39:44.000000 dynamic-sh-0.0.2/dynamic/router/router.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-11 22:14:41.670343 dynamic-sh-0.0.2/dynamic_sh.egg-info/
--rw-r--r--   0 omarwaseem   (501) staff       (20)      516 2023-07-11 22:14:41.000000 dynamic-sh-0.0.2/dynamic_sh.egg-info/PKG-INFO
--rw-r--r--   0 omarwaseem   (501) staff       (20)      545 2023-07-11 22:14:41.000000 dynamic-sh-0.0.2/dynamic_sh.egg-info/SOURCES.txt
--rw-r--r--   0 omarwaseem   (501) staff       (20)        1 2023-07-11 22:14:41.000000 dynamic-sh-0.0.2/dynamic_sh.egg-info/dependency_links.txt
--rw-r--r--   0 omarwaseem   (501) staff       (20)        8 2023-07-11 22:14:41.000000 dynamic-sh-0.0.2/dynamic_sh.egg-info/top_level.txt
--rw-r--r--   0 omarwaseem   (501) staff       (20)      553 2023-07-11 22:13:47.000000 dynamic-sh-0.0.2/pyproject.toml
--rw-r--r--   0 omarwaseem   (501) staff       (20)       38 2023-07-11 22:14:41.670727 dynamic-sh-0.0.2/setup.cfg
--rw-r--r--   0 omarwaseem   (501) staff       (20)      840 2023-07-11 22:14:34.000000 dynamic-sh-0.0.2/setup.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-12 21:54:12.667920 dynamic-sh-0.0.3/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      654 2023-07-12 21:54:12.667788 dynamic-sh-0.0.3/PKG-INFO
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-sh-0.0.3/README.md
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-12 21:54:12.664624 dynamic-sh-0.0.3/dynamic/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     1400 2023-07-08 22:39:44.000000 dynamic-sh-0.0.3/dynamic/__init__.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-12 21:54:12.665587 dynamic-sh-0.0.3/dynamic/classes/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-sh-0.0.3/dynamic/classes/__init__.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     1280 2023-07-08 22:39:44.000000 dynamic-sh-0.0.3/dynamic/classes/agent.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      133 2023-07-08 22:39:44.000000 dynamic-sh-0.0.3/dynamic/classes/chain.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      245 2023-07-08 22:39:44.000000 dynamic-sh-0.0.3/dynamic/classes/logger.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     1289 2023-07-11 18:24:11.000000 dynamic-sh-0.0.3/dynamic/classes/message.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-12 21:54:12.666224 dynamic-sh-0.0.3/dynamic/protocols/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-sh-0.0.3/dynamic/protocols/__init__.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)    10102 2023-07-11 18:24:11.000000 dynamic-sh-0.0.3/dynamic/protocols/server.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     1419 2023-07-11 18:24:11.000000 dynamic-sh-0.0.3/dynamic/protocols/ws.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-12 21:54:12.666432 dynamic-sh-0.0.3/dynamic/request/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-sh-0.0.3/dynamic/request/__init__.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-12 21:54:12.666514 dynamic-sh-0.0.3/dynamic/response/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-sh-0.0.3/dynamic/response/__init__.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-12 21:54:12.666870 dynamic-sh-0.0.3/dynamic/router/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)       47 2023-07-08 22:39:44.000000 dynamic-sh-0.0.3/dynamic/router/__init__.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     2607 2023-07-08 22:39:44.000000 dynamic-sh-0.0.3/dynamic/router/get_file_routes.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     2113 2023-07-08 22:39:44.000000 dynamic-sh-0.0.3/dynamic/router/router.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-12 21:54:12.667625 dynamic-sh-0.0.3/dynamic_sh.egg-info/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      654 2023-07-12 21:54:12.000000 dynamic-sh-0.0.3/dynamic_sh.egg-info/PKG-INFO
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      545 2023-07-12 21:54:12.000000 dynamic-sh-0.0.3/dynamic_sh.egg-info/SOURCES.txt
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        1 2023-07-12 21:54:12.000000 dynamic-sh-0.0.3/dynamic_sh.egg-info/dependency_links.txt
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        8 2023-07-12 21:54:12.000000 dynamic-sh-0.0.3/dynamic_sh.egg-info/top_level.txt
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      596 2023-07-12 21:54:06.000000 dynamic-sh-0.0.3/pyproject.toml
+-rw-r--r--   0 omarwaseem   (501) staff       (20)       38 2023-07-12 21:54:12.667955 dynamic-sh-0.0.3/setup.cfg
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     1046 2023-07-12 21:54:09.000000 dynamic-sh-0.0.3/setup.py
```

### Comparing `dynamic-sh-0.0.2/PKG-INFO` & `dynamic-sh-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dynamic-sh
-Version: 0.0.2
-Author: 
+Version: 0.0.3
+Summary: Dynamic ⚡ is a new open-source framework that streamlines the process of building production-ready applications with LLMs. Now in beta.
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dynamic-sh-0.0.2/dynamic/__init__.py` & `dynamic-sh-0.0.3/dynamic/__init__.py`

 * *Files identical despite different names*

### Comparing `dynamic-sh-0.0.2/dynamic/classes/agent.py` & `dynamic-sh-0.0.3/dynamic/classes/agent.py`

 * *Files identical despite different names*

### Comparing `dynamic-sh-0.0.2/dynamic/classes/message.py` & `dynamic-sh-0.0.3/dynamic/classes/message.py`

 * *Files identical despite different names*

### Comparing `dynamic-sh-0.0.2/dynamic/protocols/server.py` & `dynamic-sh-0.0.3/dynamic/protocols/server.py`

 * *Files identical despite different names*

### Comparing `dynamic-sh-0.0.2/dynamic/protocols/ws.py` & `dynamic-sh-0.0.3/dynamic/protocols/ws.py`

 * *Files identical despite different names*

### Comparing `dynamic-sh-0.0.2/dynamic/router/get_file_routes.py` & `dynamic-sh-0.0.3/dynamic/router/get_file_routes.py`

 * *Files identical despite different names*

### Comparing `dynamic-sh-0.0.2/dynamic/router/router.py` & `dynamic-sh-0.0.3/dynamic/router/router.py`

 * *Files identical despite different names*

### Comparing `dynamic-sh-0.0.2/dynamic_sh.egg-info/PKG-INFO` & `dynamic-sh-0.0.3/dynamic_sh.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dynamic-sh
-Version: 0.0.2
-Author: 
+Version: 0.0.3
+Summary: Dynamic ⚡ is a new open-source framework that streamlines the process of building production-ready applications with LLMs. Now in beta.
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dynamic-sh-0.0.2/dynamic_sh.egg-info/SOURCES.txt` & `dynamic-sh-0.0.3/dynamic_sh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dynamic-sh-0.0.2/pyproject.toml` & `dynamic-sh-0.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "dynamic-sh"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = [
     "Furqan Rydhan <furqan.rydhan@gmail.com>",
     "Aman Ibrahim <amanmibra@gmail.com>"
 ]
 readme = "README.md"
 keywords = ["llm", "langchain"]
 packages = [
     {include="dynamic"}
 ]
 
 [tool.poetry.dependencies]
+# TODO: figure out minimum python version 
 python = "^3.10"
 fastapi = "^0.95.1"
 uvicorn = {version = "^0.21.1", extras= ["standard"]}
 orjson = "^3.8.10"
 langchain = "^0.0.147"
 openai = "^0.27.4"
 python-dotenv = "^1.0.0"
```

### Comparing `dynamic-sh-0.0.2/setup.py` & `dynamic-sh-0.0.3/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 for name in ['dynamic-sh', 'dynamic-llm', 'dynamic-api']:
     setup(
         name=name,
-        version='0.0.2',
-        description='',
-        author='',
+        version='0.0.3',
+        description='Dynamic ⚡ is a new open-source framework that streamlines the process of building production-ready applications with LLMs. Now in beta.',
+        authors=['Furqan Rydhan <furqan@f.inc>', 'Aman Ibrahim <amanmibra@gmail.com>'],
         author_email='',
         packages=find_packages(),
         install_requires=[
             # List of package dependencies
         ],
         classifiers=[
             'Development Status :: 3 - Alpha',
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

