# Comparing `tmp/scgraph-0.1.0.tar.gz` & `tmp/scgraph-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scgraph-0.1.0.tar", last modified: Tue Jul 11 15:07:24 2023, max compression
+gzip compressed data, was "scgraph-0.2.0.tar", last modified: Thu Jul 13 19:57:49 2023, max compression
```

## Comparing `scgraph-0.1.0.tar` & `scgraph-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-11 15:07:24.930092 scgraph-0.1.0/
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)     1072 2023-04-14 17:06:21.000000 scgraph-0.1.0/LICENSE
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     4053 2023-07-11 15:07:24.930092 scgraph-0.1.0/PKG-INFO
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)     3392 2023-07-11 14:55:17.000000 scgraph-0.1.0/README.md
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      104 2023-07-11 14:07:00.000000 scgraph-0.1.0/pyproject.toml
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-11 15:07:24.930092 scgraph-0.1.0/scgraph/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       81 2023-07-11 14:58:32.000000 scgraph-0.1.0/scgraph/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    13627 2023-07-11 14:38:50.000000 scgraph-0.1.0/scgraph/core.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-11 15:07:24.930092 scgraph-0.1.0/scgraph/data/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      100 2023-07-11 12:57:30.000000 scgraph-0.1.0/scgraph/data/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      403 2023-07-11 12:57:30.000000 scgraph-0.1.0/scgraph/data/example.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)  1257473 2023-07-11 14:04:45.000000 scgraph-0.1.0/scgraph/data/marnet.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     2204 2023-07-11 14:07:20.000000 scgraph-0.1.0/scgraph/utils.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-11 15:07:24.930092 scgraph-0.1.0/scgraph.egg-info/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     4053 2023-07-11 15:07:24.000000 scgraph-0.1.0/scgraph.egg-info/PKG-INFO
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      300 2023-07-11 15:07:24.000000 scgraph-0.1.0/scgraph.egg-info/SOURCES.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2023-07-11 15:07:24.000000 scgraph-0.1.0/scgraph.egg-info/dependency_links.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        8 2023-07-11 15:07:24.000000 scgraph-0.1.0/scgraph.egg-info/top_level.txt
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)       79 2023-07-11 15:07:24.930092 scgraph-0.1.0/setup.cfg
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      969 2023-07-11 15:05:19.000000 scgraph-0.1.0/setup.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-13 19:57:49.529768 scgraph-0.2.0/
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)     1072 2023-04-14 17:06:21.000000 scgraph-0.2.0/LICENSE
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     4057 2023-07-13 19:57:49.529768 scgraph-0.2.0/PKG-INFO
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)     3396 2023-07-13 13:09:33.000000 scgraph-0.2.0/README.md
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      104 2023-07-11 14:07:00.000000 scgraph-0.2.0/pyproject.toml
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-13 19:57:49.529768 scgraph-0.2.0/scgraph/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       81 2023-07-11 14:58:32.000000 scgraph-0.2.0/scgraph/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    20483 2023-07-13 19:56:17.000000 scgraph-0.2.0/scgraph/core.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-13 19:57:49.529768 scgraph-0.2.0/scgraph/data/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      100 2023-07-11 12:57:30.000000 scgraph-0.2.0/scgraph/data/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      403 2023-07-11 12:57:30.000000 scgraph-0.2.0/scgraph/data/example.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)  1257473 2023-07-11 14:04:45.000000 scgraph-0.2.0/scgraph/data/marnet.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     2420 2023-07-11 15:18:13.000000 scgraph-0.2.0/scgraph/utils.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-13 19:57:49.529768 scgraph-0.2.0/scgraph.egg-info/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     4057 2023-07-13 19:57:49.000000 scgraph-0.2.0/scgraph.egg-info/PKG-INFO
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      300 2023-07-13 19:57:49.000000 scgraph-0.2.0/scgraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2023-07-13 19:57:49.000000 scgraph-0.2.0/scgraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        8 2023-07-13 19:57:49.000000 scgraph-0.2.0/scgraph.egg-info/top_level.txt
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)       79 2023-07-13 19:57:49.529768 scgraph-0.2.0/setup.cfg
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      969 2023-07-13 19:55:59.000000 scgraph-0.2.0/setup.py
```

### Comparing `scgraph-0.1.0/LICENSE` & `scgraph-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scgraph-0.1.0/PKG-INFO` & `scgraph-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: scgraph
-Version: 0.1.0
+Version: 0.2.0
 Summary: Determine an approximate route between two points on earth
 Home-page: https://github.com/connor-makowski/scgraph
-Download-URL: https://github.com/connor-makowski/scgraph/dist/scgraph-0.1.0.tar.gz
+Download-URL: https://github.com/connor-makowski/scgraph/dist/scgraph-0.2.0.tar.gz
 Author: Connor Makowski
 Author-email: connor.m.makowski@gmail.com
 License: MIT
 Keywords: scgraph
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # scgraph
-Supply chain graph package for Python
-
 [![PyPI version](https://badge.fury.io/py/scgraph.svg)](https://badge.fury.io/py/scgraph)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
+Supply chain graph package for Python
+
+
 ![scgraph](https://raw.githubusercontent.com/connor-makowski/scgraph/main/static/scgraph.png)
 
 ## Documentation
 
-Getting Started: https://connor-makowski.github.io/scgraph/
+Getting Started: https://github.com/connor-makowski/scgraph
+
 Low Level: https://connor-makowski.github.io/scgraph/core.html
 
 
 ## Key Features
 
 - Calculate the shortest path between two points on earth using a latitude / longitude pair
     - Inputs:
@@ -80,15 +82,15 @@
 output = my_graph.get_shortest_path(
     origin={"latitude": 31.23,"longitude": 121.47}, 
     destination={"latitude": 32.08,"longitude": -81.09}
 )
 print('Length: ',output['length']) #=> Length:  19596.735
 ```
 
-In the above example, the `path` variable is a dictionary with two keys: `length` and `path`. The `length` key contains the distance in kilometers between the two points. The `path` key contains a list of dictionaries (containing `latitude` and `longitude`) that make up the shortest path between the two points.
+In the above example, the `output` variable is a dictionary with two keys: `length` and `path`. The `length` key contains the distance in kilometers between the two points. The `path` key contains a list of dictionaries (containing `latitude` and `longitude`) that make up the shortest path between the two points.
 
 To get the latitude / longitude pairs that make up the shortest path, as a list of lists, you could do something like the following:
 
 ```py
 from scgraph import Graph
 from scgraph.data import marnet_data
```

### Comparing `scgraph-0.1.0/README.md` & `scgraph-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # scgraph
-Supply chain graph package for Python
-
 [![PyPI version](https://badge.fury.io/py/scgraph.svg)](https://badge.fury.io/py/scgraph)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
+Supply chain graph package for Python
+
+
 ![scgraph](https://raw.githubusercontent.com/connor-makowski/scgraph/main/static/scgraph.png)
 
 ## Documentation
 
-Getting Started: https://connor-makowski.github.io/scgraph/
+Getting Started: https://github.com/connor-makowski/scgraph
+
 Low Level: https://connor-makowski.github.io/scgraph/core.html
 
 
 ## Key Features
 
 - Calculate the shortest path between two points on earth using a latitude / longitude pair
     - Inputs:
@@ -62,15 +64,15 @@
 output = my_graph.get_shortest_path(
     origin={"latitude": 31.23,"longitude": 121.47}, 
     destination={"latitude": 32.08,"longitude": -81.09}
 )
 print('Length: ',output['length']) #=> Length:  19596.735
 ```
 
-In the above example, the `path` variable is a dictionary with two keys: `length` and `path`. The `length` key contains the distance in kilometers between the two points. The `path` key contains a list of dictionaries (containing `latitude` and `longitude`) that make up the shortest path between the two points.
+In the above example, the `output` variable is a dictionary with two keys: `length` and `path`. The `length` key contains the distance in kilometers between the two points. The `path` key contains a list of dictionaries (containing `latitude` and `longitude`) that make up the shortest path between the two points.
 
 To get the latitude / longitude pairs that make up the shortest path, as a list of lists, you could do something like the following:
 
 ```py
 from scgraph import Graph
 from scgraph.data import marnet_data
```

### Comparing `scgraph-0.1.0/scgraph/data/marnet.py` & `scgraph-0.2.0/scgraph/data/marnet.py`

 * *Files identical despite different names*

### Comparing `scgraph-0.1.0/scgraph/utils.py` & `scgraph-0.2.0/scgraph/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,36 +9,35 @@
         destination: dict,
         units: str = "km",
         circuity: [float, int] = 1,
     ):
         """
         Function:
 
-            Calculate the great circle distance in kilometers between two points
-            on the earth (specified in decimal degrees)
+        - Calculate the great circle distance in kilometers between two points on the earth (specified in decimal degrees)
 
         Required Arguments:
 
-            - `origin`:
-                - Type: dict
-                - What: is the origin point? (dict with keys "longitude" and "latitude")
-            - `destination`:
-                - Type: dict
-                - What: is the destination point? (dict with keys "longitude" and "latitude")
+        - `origin`:
+            - Type: dict
+            - What: is the origin point? (dict with keys "longitude" and "latitude")
+        - `destination`:
+            - Type: dict
+            - What: is the destination point? (dict with keys "longitude" and "latitude")
 
         Optional Arguments:
 
-            - `units`:
-                - Type: str
-                - What: units to return the distance in? (one of "km", "m", "mi", or "ft")
-                - Default: "km"
-            - `circuity`:
-                - Type: float | int
-                - What: Multiplier to increase the calculated distance (to account for circuity)
-                - Default: 1
+        - `units`:
+            - Type: str
+            - What: units to return the distance in? (one of "km", "m", "mi", or "ft")
+            - Default: "km"
+        - `circuity`:
+            - Type: float | int
+            - What: Multiplier to increase the calculated distance (to account for circuity)
+            - Default: 1
 
         """
         # convert decimal degrees to radians
         lon1, lat1, lon2, lat2 = map(
             math.radians,
             [
                 origin["longitude"],
@@ -66,10 +65,24 @@
             radius = 3959 * 5280
         else:
             raise ValueError('Units must be one of "km", "m", "mi", or "ft"')
         return c * radius * circuity
 
 
 def hardRound(decimal_places, a):
+    """
+    Function:
+
+    - Round a number to a specified number of decimal places
+
+    Required Arguments:
+
+    - `decimal_places`:
+        - Type: int
+        - What: number of decimal places to round to
+    - `a`:
+        - Type: float | int
+        - What: number to round
+    """
     return int(a * (10**decimal_places) + (0.5 if a > 0 else -0.5)) / (
         10**decimal_places
     )
```

### Comparing `scgraph-0.1.0/scgraph.egg-info/PKG-INFO` & `scgraph-0.2.0/scgraph.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: scgraph
-Version: 0.1.0
+Version: 0.2.0
 Summary: Determine an approximate route between two points on earth
 Home-page: https://github.com/connor-makowski/scgraph
-Download-URL: https://github.com/connor-makowski/scgraph/dist/scgraph-0.1.0.tar.gz
+Download-URL: https://github.com/connor-makowski/scgraph/dist/scgraph-0.2.0.tar.gz
 Author: Connor Makowski
 Author-email: connor.m.makowski@gmail.com
 License: MIT
 Keywords: scgraph
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # scgraph
-Supply chain graph package for Python
-
 [![PyPI version](https://badge.fury.io/py/scgraph.svg)](https://badge.fury.io/py/scgraph)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
+Supply chain graph package for Python
+
+
 ![scgraph](https://raw.githubusercontent.com/connor-makowski/scgraph/main/static/scgraph.png)
 
 ## Documentation
 
-Getting Started: https://connor-makowski.github.io/scgraph/
+Getting Started: https://github.com/connor-makowski/scgraph
+
 Low Level: https://connor-makowski.github.io/scgraph/core.html
 
 
 ## Key Features
 
 - Calculate the shortest path between two points on earth using a latitude / longitude pair
     - Inputs:
@@ -80,15 +82,15 @@
 output = my_graph.get_shortest_path(
     origin={"latitude": 31.23,"longitude": 121.47}, 
     destination={"latitude": 32.08,"longitude": -81.09}
 )
 print('Length: ',output['length']) #=> Length:  19596.735
 ```
 
-In the above example, the `path` variable is a dictionary with two keys: `length` and `path`. The `length` key contains the distance in kilometers between the two points. The `path` key contains a list of dictionaries (containing `latitude` and `longitude`) that make up the shortest path between the two points.
+In the above example, the `output` variable is a dictionary with two keys: `length` and `path`. The `length` key contains the distance in kilometers between the two points. The `path` key contains a list of dictionaries (containing `latitude` and `longitude`) that make up the shortest path between the two points.
 
 To get the latitude / longitude pairs that make up the shortest path, as a list of lists, you could do something like the following:
 
 ```py
 from scgraph import Graph
 from scgraph.data import marnet_data
```

### Comparing `scgraph-0.1.0/setup.py` & `scgraph-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'scgraph',
   packages = find_packages(),
-  version = '0.1.0',
+  version = '0.2.0',
   license='MIT',
   description = 'Determine an approximate route between two points on earth',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Connor Makowski',
   author_email = 'connor.m.makowski@gmail.com',
   url = 'https://github.com/connor-makowski/scgraph',
-  download_url = 'https://github.com/connor-makowski/scgraph/dist/scgraph-0.1.0.tar.gz',
+  download_url = 'https://github.com/connor-makowski/scgraph/dist/scgraph-0.2.0.tar.gz',
   keywords = ['scgraph'],
   install_requires=[],
   classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',
```

