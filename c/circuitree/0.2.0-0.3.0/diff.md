# Comparing `tmp/circuitree-0.2.0.tar.gz` & `tmp/circuitree-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitree-0.2.0.tar", max compression
+gzip compressed data, was "circuitree-0.3.0.tar", max compression
```

## Comparing `circuitree-0.2.0.tar` & `circuitree-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-04-06 18:32:42.965443 circuitree-0.2.0/LICENSE
--rw-r--r--   0        0        0     1011 2023-06-09 16:36:39.964761 circuitree-0.2.0/README.md
--rwxr-xr-x   0        0        0      117 2023-06-23 05:39:39.142840 circuitree-0.2.0/circuitree/__init__.py
--rwxr-xr-x   0        0        0    15843 2023-06-23 06:25:24.652892 circuitree-0.2.0/circuitree/circuitree.py
--rwxr-xr-x   0        0        0     5381 2023-06-23 20:46:19.095399 circuitree-0.2.0/circuitree/models.py
--rw-r--r--   0        0        0     3991 2023-05-26 18:27:42.279204 circuitree-0.2.0/circuitree/modularity.py
--rw-r--r--   0        0        0     9417 2023-06-28 00:46:06.604507 circuitree-0.2.0/circuitree/parallel.py
--rw-r--r--   0        0        0      267 2023-05-26 18:24:06.289207 circuitree-0.2.0/circuitree/regret.py
--rw-r--r--   0        0        0      750 2023-05-13 02:24:31.319175 circuitree-0.2.0/circuitree/rewards.py
--rw-r--r--   0        0        0     1442 2023-06-23 05:30:14.382829 circuitree-0.2.0/circuitree/utils.py
--rw-r--r--   0        0        0    10132 2023-06-27 21:29:15.594283 circuitree-0.2.0/circuitree/viz.py
--rw-r--r--   0        0        0     1813 2023-06-28 03:58:26.084726 circuitree-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2525 1970-01-01 00:00:00.000000 circuitree-0.2.0/setup.py
--rw-r--r--   0        0        0     2530 1970-01-01 00:00:00.000000 circuitree-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-06 18:32:42.965443 circuitree-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1011 2023-06-09 16:36:39.964761 circuitree-0.3.0/README.md
+-rwxr-xr-x   0        0        0      117 2023-06-23 05:39:39.142840 circuitree-0.3.0/circuitree/__init__.py
+-rwxr-xr-x   0        0        0    15843 2023-06-23 06:25:24.652892 circuitree-0.3.0/circuitree/circuitree.py
+-rwxr-xr-x   0        0        0    17012 2023-07-13 01:44:13.327169 circuitree-0.3.0/circuitree/models.py
+-rw-r--r--   0        0        0     3991 2023-05-26 18:27:42.279204 circuitree-0.3.0/circuitree/modularity.py
+-rw-r--r--   0        0        0     9417 2023-06-28 00:46:06.604507 circuitree-0.3.0/circuitree/parallel.py
+-rw-r--r--   0        0        0      267 2023-05-26 18:24:06.289207 circuitree-0.3.0/circuitree/regret.py
+-rw-r--r--   0        0        0      750 2023-05-13 02:24:31.319175 circuitree-0.3.0/circuitree/rewards.py
+-rw-r--r--   0        0        0     1442 2023-06-23 05:30:14.382829 circuitree-0.3.0/circuitree/utils.py
+-rw-r--r--   0        0        0    10391 2023-06-28 20:54:12.669759 circuitree-0.3.0/circuitree/viz.py
+-rw-r--r--   0        0        0     1813 2023-07-13 01:45:02.237170 circuitree-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2525 1970-01-01 00:00:00.000000 circuitree-0.3.0/setup.py
+-rw-r--r--   0        0        0     2530 1970-01-01 00:00:00.000000 circuitree-0.3.0/PKG-INFO
```

### Comparing `circuitree-0.2.0/LICENSE` & `circuitree-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitree-0.2.0/README.md` & `circuitree-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `circuitree-0.2.0/circuitree/circuitree.py` & `circuitree-0.3.0/circuitree/circuitree.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.2.0/circuitree/modularity.py` & `circuitree-0.3.0/circuitree/modularity.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.2.0/circuitree/parallel.py` & `circuitree-0.3.0/circuitree/parallel.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.2.0/circuitree/rewards.py` & `circuitree-0.3.0/circuitree/rewards.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.2.0/circuitree/utils.py` & `circuitree-0.3.0/circuitree/utils.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.2.0/circuitree/viz.py` & `circuitree-0.3.0/circuitree/viz.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,20 +75,26 @@
     from matplotlib.patches import Circle
 
     if ax is None:
         ax = plt.gca()
 
     n_components = len(names)
 
-    angle0 = (0.0, np.pi / 2)[n_components % 2]
-    theta = np.linspace(angle0, angle0 + 2 * np.pi, n_components, endpoint=False)
-    theta = theta % (2 * np.pi)
+    if n_components == 1:
+        # Special case
+        theta = np.array([np.pi / 2])
+        x = np.array([0.0]) + center[0]
+        y = np.array([0.0]) + center[1]
+    elif n_components > 1:
+        angle0 = np.pi / 2
+        theta = np.linspace(angle0, angle0 + 2 * np.pi, n_components, endpoint=False)
+        x = np.cos(theta) + center[0]
+        y = np.sin(theta) + center[1]
 
-    x = np.cos(theta) + center[0]
-    y = np.sin(theta) + center[1]
+    theta = theta % (2 * np.pi)
     xy = np.column_stack([x, y])
 
     colormap = plt.get_cmap(cmap)
     colors = colormap(range(n_components))
 
     radius = node_shrink * _compute_radius(n_components)
     molecules = []
@@ -408,8 +414,11 @@
         head_length=0,
     )
 
     return arc, head
 
 
 def _compute_radius(n_components: int):
-    return 0.25 * np.sqrt(2 * (1 - np.cos(2 * np.pi / n_components)))
+    if n_components == 1:
+        return _compute_radius(2)
+    else:
+        return 0.25 * np.sqrt(2 * (1 - np.cos(2 * np.pi / n_components)))
```

### Comparing `circuitree-0.2.0/pyproject.toml` & `circuitree-0.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "circuitree"
-version = "0.2.0"
+version = "0.3.0"
 description = "Genetic circuit design using Monte Carlo tree search"
 authors = ["pranav-bhamidipati <pbhamidi@usc.edu>"]
 license = "GPLv3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `circuitree-0.2.0/setup.py` & `circuitree-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
               'pandas>=2.0.0,<3.0.0',
               'tables>=3.8.0,<4.0.0',
               'pyarrow>=12.0.0,<13.0.0',
               'h5py>=3.8.0,<4.0.0']}
 
 setup_kwargs = {
     'name': 'circuitree',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'Genetic circuit design using Monte Carlo tree search',
     'long_description': '# CircuiTree\nGenetic circuit design using Monte Carlo tree search\n\n## Installation\n\n### From a package repository\nTo install using `pip`:\n\n```pip install circuitree```\n\n### From the GitHub repository\n\nTo install and use `circuitree` from the GitHub source code, first clone the repo into a directory.\n\n```git clone https://github.com/pranav-bhamidipati/circuitree.git[ dir_name]```\n\nThen, you can build the environment using the command-line tool `poetry`. Instructions for installation can be [found here](https://python-poetry.org/). \n\nFrom the main project directory, run `poetry install` to install a virtual environment with `circuitree` installed. The easiest way to use this environment is to run it interactively with `poetry shell`. Alternatively, you can run a command in the virtual environment with `poetry run <command>`. For instance, to launch a Jupyter notebook with `circuitree` pre-loaded, run `poetry run jupyter notebook`. \n\n## Usage\n\nSee the [quick-start demo](examples/quick_start.ipynb).\n',
     'author': 'pranav-bhamidipati',
     'author_email': 'pbhamidi@usc.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `circuitree-0.2.0/PKG-INFO` & `circuitree-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitree
-Version: 0.2.0
+Version: 0.3.0
 Summary: Genetic circuit design using Monte Carlo tree search
 License: GPLv3
 Author: pranav-bhamidipati
 Author-email: pbhamidi@usc.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

