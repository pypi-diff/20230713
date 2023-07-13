# Comparing `tmp/jupyverse_api-0.1.9.tar.gz` & `tmp/jupyverse_api-0.2.0.tar.gz`

## Comparing `jupyverse_api-0.1.9.tar` & `jupyverse_api-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/__init__.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/cli.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/py.typed
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/app/__init__.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/auth/__init__.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/auth/models.py
--rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/contents/__init__.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/contents/models.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/frontend/__init__.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/jupyterlab/__init__.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/kernels/__init__.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/kernels/models.py
--rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/lab/__init__.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/login/__init__.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/main/__init__.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/nbconvert/__init__.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/resource_usage/__init__.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/retrolab/__init__.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/terminals/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/terminals/models.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/yjs/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/jupyverse_api/yjs/models.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/COPYING.md
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/README.md
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 jupyverse_api-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/__init__.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/cli.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/py.typed
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/app/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/auth/__init__.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/auth/models.py
+-rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/contents/__init__.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/contents/models.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/frontend/__init__.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/jupyterlab/__init__.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/kernels/__init__.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/kernels/models.py
+-rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/lab/__init__.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/login/__init__.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/main/__init__.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/nbconvert/__init__.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/resource_usage/__init__.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/retrolab/__init__.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/terminals/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/terminals/models.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/yjs/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/yjs/models.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/COPYING.md
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/README.md
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/PKG-INFO
```

### Comparing `jupyverse_api-0.1.9/jupyverse_api/__init__.py` & `jupyverse_api-0.2.0/jupyverse_api/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from typing import Dict
 
-from pydantic import BaseModel, Extra
+from pydantic import BaseModel
 
 from .app import App
 
 
-__version__ = "0.1.9"
+__version__ = "0.2.0"
 
 
 class Singleton(type):
     _instances: Dict = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
             cls._instances[cls] = super(Singleton, cls).__call__(*args, **kwargs)
         return cls._instances[cls]
 
 
 class Config(BaseModel):
-    class Config:
-        extra = Extra.forbid
+    model_config = {"extra": "forbid"}
 
 
 class Router:
     _app: App
 
     def __init__(
         self,
```

### Comparing `jupyverse_api-0.1.9/jupyverse_api/cli.py` & `jupyverse_api-0.2.0/jupyverse_api/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pkg_resources
 from typing import List
 
 import rich_click as click
 from asphalt.core.cli import run
 
 
-@click.command()
+@click.command()  # type: ignore
 @click.option(
     "--open-browser",
     is_flag=True,
     show_default=True,
     default=False,
     help="Open a browser window.",
 )
```

### Comparing `jupyverse_api-0.1.9/jupyverse_api/app/__init__.py` & `jupyverse_api-0.2.0/jupyverse_api/app/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.9/jupyverse_api/auth/__init__.py` & `jupyverse_api-0.2.0/jupyverse_api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.9/jupyverse_api/contents/__init__.py` & `jupyverse_api-0.2.0/jupyverse_api/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.9/jupyverse_api/contents/models.py` & `jupyverse_api-0.2.0/jupyverse_api/contents/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.9/jupyverse_api/jupyterlab/__init__.py` & `jupyverse_api-0.2.0/jupyverse_api/jupyterlab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.9/jupyverse_api/kernels/__init__.py` & `jupyverse_api-0.2.0/jupyverse_api/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.9/jupyverse_api/kernels/models.py` & `jupyverse_api-0.2.0/jupyverse_api/kernels/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.9/jupyverse_api/lab/__init__.py` & `jupyverse_api-0.2.0/jupyverse_api/lab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.9/jupyverse_api/main/__init__.py` & `jupyverse_api-0.2.0/jupyverse_api/main/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.9/jupyverse_api/nbconvert/__init__.py` & `jupyverse_api-0.2.0/jupyverse_api/nbconvert/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.9/jupyverse_api/resource_usage/__init__.py` & `jupyverse_api-0.2.0/jupyverse_api/resource_usage/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.9/jupyverse_api/retrolab/__init__.py` & `jupyverse_api-0.2.0/jupyverse_api/retrolab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.9/jupyverse_api/terminals/__init__.py` & `jupyverse_api-0.2.0/jupyverse_api/terminals/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.9/jupyverse_api/yjs/__init__.py` & `jupyverse_api-0.2.0/jupyverse_api/yjs/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.9/.gitignore` & `jupyverse_api-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.9/COPYING.md` & `jupyverse_api-0.2.0/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.9/pyproject.toml` & `jupyverse_api-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "pydantic >=1.10.6,<2",
+  "pydantic >=2,<3",
   "fastapi >=0.95.0,<1",
   "rich-click >=1.6.1,<2",
   "asphalt >=4.11.0,<5",
   "asphalt-web[fastapi] >=1.1.0,<2",
 ]
 dynamic = ["version"]
```

### Comparing `jupyverse_api-0.1.9/PKG-INFO` & `jupyverse_api-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyverse_api
-Version: 0.1.9
+Version: 0.2.0
 Summary: The public API for Jupyverse
 Project-URL: Source, https://github.com/jupyter-server/jupyverse/jupyverse_api
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: api,jupyverse
 Classifier: Development Status :: 4 - Beta
@@ -15,14 +15,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: asphalt-web[fastapi]<2,>=1.1.0
 Requires-Dist: asphalt<5,>=4.11.0
 Requires-Dist: fastapi<1,>=0.95.0
-Requires-Dist: pydantic<2,>=1.10.6
+Requires-Dist: pydantic<3,>=2
 Requires-Dist: rich-click<2,>=1.6.1
 Description-Content-Type: text/markdown
 
 # Jupyverse API
 
 The public API for Jupyverse.
```

