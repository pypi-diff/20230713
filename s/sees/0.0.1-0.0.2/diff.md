# Comparing `tmp/sees-0.0.1.tar.gz` & `tmp/sees-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sees-0.0.1.tar", last modified: Wed Jul 12 22:49:32 2023, max compression
+gzip compressed data, was "sees-0.0.2.tar", last modified: Wed Jul 12 22:53:21 2023, max compression
```

## Comparing `sees-0.0.1.tar` & `sees-0.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-12 22:49:32.495062 sees-0.0.1/
--rw-r--r--   0 claudio   (1001) claudio   (1001)      390 2023-07-12 22:49:32.495062 sees-0.0.1/PKG-INFO
--rw-r--r--   0 claudio   (1001) claudio   (1001)        0 2023-07-12 02:36:52.000000 sees-0.0.1/README.md
--rw-r--r--   0 claudio   (1001) claudio   (1001)      726 2023-07-12 02:36:41.000000 sees-0.0.1/pyproject.toml
--rw-r--r--   0 claudio   (1001) claudio   (1001)       38 2023-07-12 22:49:32.495062 sees-0.0.1/setup.cfg
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-12 22:49:32.475062 sees-0.0.1/src/
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-12 22:49:32.475062 sees-0.0.1/src/sees/
--rwxr-xr-x   0 claudio   (1001) claudio   (1001)    25650 2023-07-12 19:58:25.000000 sees-0.0.1/src/sees/__init__.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     8200 2023-07-12 20:46:07.000000 sees-0.0.1/src/sees/__main__.py
--rwxr-xr-x   0 claudio   (1001) claudio   (1001)    46057 2023-07-12 02:10:35.000000 sees-0.0.1/src/sees/_render.py
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-12 22:49:32.485062 sees-0.0.1/src/sees/canvas/
--rw-r--r--   0 claudio   (1001) claudio   (1001)      698 2023-07-12 02:42:52.000000 sees-0.0.1/src/sees/canvas/canvas.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     2604 2023-07-12 03:36:02.000000 sees-0.0.1/src/sees/canvas/gltflib.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     1501 2023-07-12 02:42:06.000000 sees-0.0.1/src/sees/canvas/mpl.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     4873 2023-07-12 02:42:13.000000 sees-0.0.1/src/sees/canvas/ply.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     1442 2023-07-12 04:22:07.000000 sees-0.0.1/src/sees/canvas/tri.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     1376 2023-07-12 02:25:12.000000 sees-0.0.1/src/sees/config.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)        0 2023-03-27 17:30:37.000000 sees-0.0.1/src/sees/section.py
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-12 22:49:32.485062 sees-0.0.1/src/sees/solid/
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-12 22:49:32.485062 sees-0.0.1/src/sees/solid/convert/
--rw-r--r--   0 claudio   (1001) claudio   (1001)     3303 2022-12-07 20:44:36.000000 sees-0.0.1/src/sees/solid/convert/convert.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)      383 2022-12-07 20:44:36.000000 sees-0.0.1/src/sees/solid/convert/example.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)     1460 2023-03-28 16:46:02.000000 sees-0.0.1/src/sees/solid/ops.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)      265 2023-03-28 16:26:56.000000 sees-0.0.1/src/sees/solid/plt.py
--rw-r--r--   0 claudio   (1001) claudio   (1001)        0 2023-03-27 17:30:37.000000 sees-0.0.1/src/sees/structure.py
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-12 22:49:32.485062 sees-0.0.1/src/sees/utilities/
--rw-r--r--   0 claudio   (1001) claudio   (1001)     3098 2023-07-12 17:28:46.000000 sees-0.0.1/src/sees/utilities/alpha_shape.py
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-12 22:49:32.485062 sees-0.0.1/src/sees.egg-info/
--rw-r--r--   0 claudio   (1001) claudio   (1001)      390 2023-07-12 22:49:32.000000 sees-0.0.1/src/sees.egg-info/PKG-INFO
--rw-r--r--   0 claudio   (1001) claudio   (1001)      592 2023-07-12 22:49:32.000000 sees-0.0.1/src/sees.egg-info/SOURCES.txt
--rw-r--r--   0 claudio   (1001) claudio   (1001)        1 2023-07-12 22:49:32.000000 sees-0.0.1/src/sees.egg-info/dependency_links.txt
--rw-r--r--   0 claudio   (1001) claudio   (1001)       44 2023-07-12 22:49:32.000000 sees-0.0.1/src/sees.egg-info/entry_points.txt
--rw-r--r--   0 claudio   (1001) claudio   (1001)        5 2023-07-12 22:49:32.000000 sees-0.0.1/src/sees.egg-info/top_level.txt
-drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-12 22:49:32.485062 sees-0.0.1/tests/
--rw-r--r--   0 claudio   (1001) claudio   (1001)      108 2022-06-20 06:36:53.000000 sees-0.0.1/tests/test.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-12 22:53:21.055062 sees-0.0.2/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      390 2023-07-12 22:53:21.055062 sees-0.0.2/PKG-INFO
+-rw-r--r--   0 claudio   (1001) claudio   (1001)        0 2023-07-12 02:36:52.000000 sees-0.0.2/README.md
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      726 2023-07-12 22:52:34.000000 sees-0.0.2/pyproject.toml
+-rw-r--r--   0 claudio   (1001) claudio   (1001)       38 2023-07-12 22:53:21.055062 sees-0.0.2/setup.cfg
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-12 22:53:21.045062 sees-0.0.2/src/
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-12 22:53:21.055062 sees-0.0.2/src/sees/
+-rwxr-xr-x   0 claudio   (1001) claudio   (1001)    25650 2023-07-12 19:58:25.000000 sees-0.0.2/src/sees/__init__.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     8200 2023-07-12 20:46:07.000000 sees-0.0.2/src/sees/__main__.py
+-rwxr-xr-x   0 claudio   (1001) claudio   (1001)    46057 2023-07-12 02:10:35.000000 sees-0.0.2/src/sees/_render.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-12 22:53:21.055062 sees-0.0.2/src/sees/canvas/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      698 2023-07-12 02:42:52.000000 sees-0.0.2/src/sees/canvas/canvas.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     2604 2023-07-12 03:36:02.000000 sees-0.0.2/src/sees/canvas/gltflib.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     1501 2023-07-12 02:42:06.000000 sees-0.0.2/src/sees/canvas/mpl.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     4878 2023-07-12 22:52:20.000000 sees-0.0.2/src/sees/canvas/ply.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     1442 2023-07-12 04:22:07.000000 sees-0.0.2/src/sees/canvas/tri.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     1376 2023-07-12 02:25:12.000000 sees-0.0.2/src/sees/config.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)        0 2023-03-27 17:30:37.000000 sees-0.0.2/src/sees/section.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-12 22:53:21.055062 sees-0.0.2/src/sees/solid/
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-12 22:53:21.055062 sees-0.0.2/src/sees/solid/convert/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     3303 2022-12-07 20:44:36.000000 sees-0.0.2/src/sees/solid/convert/convert.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      383 2022-12-07 20:44:36.000000 sees-0.0.2/src/sees/solid/convert/example.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     1460 2023-03-28 16:46:02.000000 sees-0.0.2/src/sees/solid/ops.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      265 2023-03-28 16:26:56.000000 sees-0.0.2/src/sees/solid/plt.py
+-rw-r--r--   0 claudio   (1001) claudio   (1001)        0 2023-03-27 17:30:37.000000 sees-0.0.2/src/sees/structure.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-12 22:53:21.055062 sees-0.0.2/src/sees/utilities/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)     3098 2023-07-12 17:28:46.000000 sees-0.0.2/src/sees/utilities/alpha_shape.py
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-12 22:53:21.055062 sees-0.0.2/src/sees.egg-info/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      390 2023-07-12 22:53:20.000000 sees-0.0.2/src/sees.egg-info/PKG-INFO
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      592 2023-07-12 22:53:21.000000 sees-0.0.2/src/sees.egg-info/SOURCES.txt
+-rw-r--r--   0 claudio   (1001) claudio   (1001)        1 2023-07-12 22:53:20.000000 sees-0.0.2/src/sees.egg-info/dependency_links.txt
+-rw-r--r--   0 claudio   (1001) claudio   (1001)       44 2023-07-12 22:53:20.000000 sees-0.0.2/src/sees.egg-info/entry_points.txt
+-rw-r--r--   0 claudio   (1001) claudio   (1001)        5 2023-07-12 22:53:20.000000 sees-0.0.2/src/sees.egg-info/top_level.txt
+drwxr-xr-x   0 claudio   (1001) claudio   (1001)        0 2023-07-12 22:53:21.055062 sees-0.0.2/tests/
+-rw-r--r--   0 claudio   (1001) claudio   (1001)      108 2022-06-20 06:36:53.000000 sees-0.0.2/tests/test.py
```

### Comparing `sees-0.0.1/pyproject.toml` & `sees-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sees"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   {name="Claudio M. Perez", email="50180406+claudioperez@users.noreply.github.com"},
   {name="Chrystal Chern",   email="52893467+chrystalchern@users.noreply.github.com"}
 ]
 
 readme = "README.md"
```

### Comparing `sees-0.0.1/src/sees/__init__.py` & `sees-0.0.2/src/sees/__init__.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.1/src/sees/__main__.py` & `sees-0.0.2/src/sees/__main__.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.1/src/sees/_render.py` & `sees-0.0.2/src/sees/_render.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.1/src/sees/canvas/canvas.py` & `sees-0.0.2/src/sees/canvas/canvas.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.1/src/sees/canvas/gltflib.py` & `sees-0.0.2/src/sees/canvas/gltflib.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.1/src/sees/canvas/mpl.py` & `sees-0.0.2/src/sees/canvas/mpl.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.1/src/sees/canvas/ply.py` & `sees-0.0.2/src/sees/canvas/ply.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             "customdata": list(items),
         }
 
 
     def plot_nodes(self, coords, label = None, props=None, data=None):
         name = label or "nodes"
         x,y,z = coords.T
-        keys  = ["tag",]
+        keys  = ["tag","crd"]
 
         data = {
                 "name": name,
                 "x": x, "y": y, "z": z,
                 "type": "scatter3d","mode": "markers",
                 "hovertemplate": "<br>".join(f"{k}: %{{customdata[{v}]}}" for v,k in enumerate(keys)),
                 "customdata": data,
```

### Comparing `sees-0.0.1/src/sees/canvas/tri.py` & `sees-0.0.2/src/sees/canvas/tri.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.1/src/sees/config.py` & `sees-0.0.2/src/sees/config.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.1/src/sees/solid/convert/convert.py` & `sees-0.0.2/src/sees/solid/convert/convert.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.1/src/sees/solid/ops.py` & `sees-0.0.2/src/sees/solid/ops.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.1/src/sees/utilities/alpha_shape.py` & `sees-0.0.2/src/sees/utilities/alpha_shape.py`

 * *Files identical despite different names*

### Comparing `sees-0.0.1/src/sees.egg-info/SOURCES.txt` & `sees-0.0.2/src/sees.egg-info/SOURCES.txt`

 * *Files identical despite different names*

