# Comparing `tmp/Signal8-4.8.tar.gz` & `tmp/Signal8-4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-4.8.tar", last modified: Thu Jul 13 18:10:52 2023, max compression
+gzip compressed data, was "Signal8-4.9.tar", last modified: Thu Jul 13 21:23:45 2023, max compression
```

## Comparing `Signal8-4.8.tar` & `Signal8-4.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 18:10:52.495064 Signal8-4.8/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-4.8/LICENSE
--rw-rw-rw-   0        0        0     4768 2023-07-13 18:10:52.488065 Signal8-4.8/PKG-INFO
--rw-rw-rw-   0        0        0     4270 2023-07-01 17:14:19.000000 Signal8-4.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 18:10:52.322576 Signal8-4.8/Signal8/
--rw-rw-rw-   0        0        0    12041 2023-07-13 18:09:18.000000 Signal8-4.8/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       24 2023-06-19 21:16:46.000000 Signal8-4.8/Signal8/__init__.py
--rw-rw-rw-   0        0        0      239 2023-07-13 18:08:55.000000 Signal8-4.8/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-07-13 18:10:52.481066 Signal8-4.8/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-4.8/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     5369 2023-07-13 18:05:08.000000 Signal8-4.8/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     2322 2023-06-30 20:05:49.000000 Signal8-4.8/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-4.8/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    11960 2023-07-13 18:01:37.000000 Signal8-4.8/Signal8/utils/simple_env.py
--rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-4.8/Signal8/utils/test_dynamic_obs.py
-drwxrwxrwx   0        0        0        0 2023-07-13 18:10:52.396292 Signal8-4.8/Signal8.egg-info/
--rw-rw-rw-   0        0        0     4768 2023-07-13 18:10:51.000000 Signal8-4.8/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      510 2023-07-13 18:10:52.000000 Signal8-4.8/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 18:10:51.000000 Signal8-4.8/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-13 18:10:51.000000 Signal8-4.8/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 18:10:52.496065 Signal8-4.8/setup.cfg
--rw-rw-rw-   0        0        0      645 2023-07-13 18:10:03.000000 Signal8-4.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 21:23:45.087731 Signal8-4.9/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-4.9/LICENSE
+-rw-rw-rw-   0        0        0     4768 2023-07-13 21:23:45.082731 Signal8-4.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4270 2023-07-01 17:14:19.000000 Signal8-4.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 21:23:44.858733 Signal8-4.9/Signal8/
+-rw-rw-rw-   0        0        0    12074 2023-07-13 21:21:08.000000 Signal8-4.9/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       24 2023-06-19 21:16:46.000000 Signal8-4.9/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      239 2023-07-13 18:08:55.000000 Signal8-4.9/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-07-13 21:23:45.059730 Signal8-4.9/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-4.9/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     5369 2023-07-13 18:05:08.000000 Signal8-4.9/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     2322 2023-06-30 20:05:49.000000 Signal8-4.9/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-4.9/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    11960 2023-07-13 18:01:37.000000 Signal8-4.9/Signal8/utils/simple_env.py
+-rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-4.9/Signal8/utils/test_dynamic_obs.py
+drwxrwxrwx   0        0        0        0 2023-07-13 21:23:44.967729 Signal8-4.9/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     4768 2023-07-13 21:23:43.000000 Signal8-4.9/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2023-07-13 21:23:43.000000 Signal8-4.9/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 21:23:43.000000 Signal8-4.9/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-13 21:23:43.000000 Signal8-4.9/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 21:23:45.088731 Signal8-4.9/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-07-13 21:22:11.000000 Signal8-4.9/setup.py
```

### Comparing `Signal8-4.8/LICENSE` & `Signal8-4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-4.8/PKG-INFO` & `Signal8-4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 4.8
+Version: 4.9
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-4.8/README.md` & `Signal8-4.9/README.md`

 * *Files identical despite different names*

### Comparing `Signal8-4.8/Signal8/Signal8.py` & `Signal8-4.9/Signal8/Signal8.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 
 class raw_env(SimpleEnv, EzPickle):
     def __init__(
         self, 
         num_agents=1, 
         num_large_obstacles=4, 
         num_small_obstacles=10, 
-        render_mode=None
+        render_mode=None,
+        max_cycles=500,
         ):
         
         if num_agents > 2:
             raise ValueError("Signal8 currently can only support up to 2 agents.")
         
         if num_large_obstacles > 16:
             raise ValueError("Signal8 has a maximum of 10 large obstacles.")
@@ -28,15 +29,15 @@
         scenario = Scenario()
         world = scenario.make_world(num_agents, num_large_obstacles, num_small_obstacles)
         
         super().__init__(
             scenario=scenario, 
             world=world, 
             render_mode=render_mode,
-            max_cycles=500, 
+            max_cycles=max_cycles, 
         )
         
 env = make_env(raw_env)
 
 class Scenario(BaseScenario):
     def make_world(self, num_agents, num_large_obstacles, num_small_obstacles):
         world = World()
```

### Comparing `Signal8-4.8/Signal8/utils/core.py` & `Signal8-4.9/Signal8/utils/core.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.8/Signal8/utils/problems.py` & `Signal8-4.9/Signal8/utils/problems.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.8/Signal8/utils/simple_env.py` & `Signal8-4.9/Signal8/utils/simple_env.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.8/Signal8/utils/test_dynamic_obs.py` & `Signal8-4.9/Signal8/utils/test_dynamic_obs.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.8/Signal8.egg-info/PKG-INFO` & `Signal8-4.9/Signal8.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 4.8
+Version: 4.9
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-4.8/setup.py` & `Signal8-4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="4.8",
+    version="4.9",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

