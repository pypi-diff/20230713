# Comparing `tmp/Signal8-4.6.tar.gz` & `tmp/Signal8-4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-4.6.tar", last modified: Wed Jul 12 17:50:29 2023, max compression
+gzip compressed data, was "Signal8-4.8.tar", last modified: Thu Jul 13 18:10:52 2023, max compression
```

## Comparing `Signal8-4.6.tar` & `Signal8-4.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 17:50:29.731246 Signal8-4.6/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-4.6/LICENSE
--rw-rw-rw-   0        0        0     4768 2023-07-12 17:50:29.729246 Signal8-4.6/PKG-INFO
--rw-rw-rw-   0        0        0     4270 2023-07-01 17:14:19.000000 Signal8-4.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 17:50:29.652247 Signal8-4.6/Signal8/
--rw-rw-rw-   0        0        0    12543 2023-07-12 17:48:53.000000 Signal8-4.6/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       24 2023-06-19 21:16:46.000000 Signal8-4.6/Signal8/__init__.py
--rw-rw-rw-   0        0        0      202 2023-07-09 23:27:47.000000 Signal8-4.6/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-07-12 17:50:29.724248 Signal8-4.6/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-4.6/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     5346 2023-06-14 03:28:36.000000 Signal8-4.6/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     2322 2023-06-30 20:05:49.000000 Signal8-4.6/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-4.6/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    11954 2023-06-30 18:56:28.000000 Signal8-4.6/Signal8/utils/simple_env.py
--rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-4.6/Signal8/utils/test_dynamic_obs.py
-drwxrwxrwx   0        0        0        0 2023-07-12 17:50:29.695245 Signal8-4.6/Signal8.egg-info/
--rw-rw-rw-   0        0        0     4768 2023-07-12 17:50:29.000000 Signal8-4.6/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      510 2023-07-12 17:50:29.000000 Signal8-4.6/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 17:50:29.000000 Signal8-4.6/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-12 17:50:29.000000 Signal8-4.6/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 17:50:29.732245 Signal8-4.6/setup.cfg
--rw-rw-rw-   0        0        0      645 2023-07-12 17:49:09.000000 Signal8-4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:10:52.495064 Signal8-4.8/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-4.8/LICENSE
+-rw-rw-rw-   0        0        0     4768 2023-07-13 18:10:52.488065 Signal8-4.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4270 2023-07-01 17:14:19.000000 Signal8-4.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 18:10:52.322576 Signal8-4.8/Signal8/
+-rw-rw-rw-   0        0        0    12041 2023-07-13 18:09:18.000000 Signal8-4.8/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       24 2023-06-19 21:16:46.000000 Signal8-4.8/Signal8/__init__.py
+-rw-rw-rw-   0        0        0      239 2023-07-13 18:08:55.000000 Signal8-4.8/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:10:52.481066 Signal8-4.8/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-4.8/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     5369 2023-07-13 18:05:08.000000 Signal8-4.8/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     2322 2023-06-30 20:05:49.000000 Signal8-4.8/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-4.8/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    11960 2023-07-13 18:01:37.000000 Signal8-4.8/Signal8/utils/simple_env.py
+-rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-4.8/Signal8/utils/test_dynamic_obs.py
+drwxrwxrwx   0        0        0        0 2023-07-13 18:10:52.396292 Signal8-4.8/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     4768 2023-07-13 18:10:51.000000 Signal8-4.8/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2023-07-13 18:10:52.000000 Signal8-4.8/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 18:10:51.000000 Signal8-4.8/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-13 18:10:51.000000 Signal8-4.8/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 18:10:52.496065 Signal8-4.8/setup.cfg
+-rw-rw-rw-   0        0        0      645 2023-07-13 18:10:03.000000 Signal8-4.8/setup.py
```

### Comparing `Signal8-4.6/LICENSE` & `Signal8-4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-4.6/PKG-INFO` & `Signal8-4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 4.6
+Version: 4.8
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-4.6/README.md` & `Signal8-4.8/README.md`

 * *Files identical despite different names*

### Comparing `Signal8-4.6/Signal8/Signal8.py` & `Signal8-4.8/Signal8/Signal8.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,37 +60,32 @@
             obstacle = Obstacle(size=0.1)
             obstacle.name = f"obs_{i}"
             obstacle.color = np.array([0.97, 0.801, 0.8])
             world.large_obstacles.append(obstacle)
         
         # Small obstacles can only be observed by ground agent(s)
         for i in range(num_small_obstacles):
-            obstacle = Obstacle(size=0.01)
+            obstacle = Obstacle(size=0.02)
             obstacle.name = f"obs_{i}"
             obstacle.color = np.array([0.97, 0.801, 0.8])
             world.small_obstacles.append(obstacle)    
         
         world.buffer_dist = world.agents[0].size + world.large_obstacles[0].size
         return world
     
     # Get constraints on entities given problem instance name
     def _set_problem_instance(self, world, instance_name):
         instance_constr = get_problem_instance(instance_name)
         world.problem_instance = instance_name
         world.instance_constr = instance_constr
     
     # Generate valid points according to some condition
-    def _generate_position(self, np_random, condition, circle=False, bounds=(-1, 1)):
+    def _generate_position(self, np_random, condition):
         while True:
-            if circle:
-                theta = np_random.uniform(0, 2*np.pi)
-                r = 0.5 * np.sqrt(np_random.uniform(0, 1))
-                point = np.array([r * np.cos(theta), r * np.sin(theta)])
-            else:
-                point = np_random.uniform(bounds[0], bounds[1], 2)  # use the bounds here
+            point = np_random.uniform(-1, +1, 2)
             if condition(point):
                 break
         return point
 
     # Check if point is outside of triangular obstacle regions
     def _outside_triangle(self, point, paths, epsilon):
         enlarged_paths = []
@@ -146,39 +141,37 @@
                     y_constraints=y_constraints,
                     epsilon=epsilon, 
                     )
 
             agent.state.p_pos = self._generate_position(np_random, condition)
             agent.goal.state.p_pos = self._generate_position(np_random, condition)
     
-    # Reset all large obstacles to a position that does not intersect with the agents and is within its shape                
+    # Reset all large obstacles to a position that does not intersect with the agents and is within its shape
     def _reset_large_obstacles(self, world, np_random, paths):
         def inside_shape_condition(point):
             return any(path.contains_points(point[None, :]) for path in paths)    
-
+        
         occupied = set()
         num_shapes = len(world.instance_constr)
-        circle = True if world.problem_instance in ['circle', 'solar_system'] else False    
-        radius = world.large_obstacles[0].size  # get the radius of the obstacle
-
+        
         for i, large_obstacle in enumerate(world.large_obstacles):            
             large_obstacle.state.p_vel = np.zeros(world.dim_p)
-
+            
             while True:
-                pos = self._generate_position(np_random, inside_shape_condition, circle=circle, bounds=(-1+radius, 1-radius))  # adjust the bounds here
+                pos = self._generate_position(np_random, inside_shape_condition)
                 shape_idx = next((i for i, path in enumerate(paths) if path.contains_points(pos[None, :])), None)
-
+                
                 if i % num_shapes == 0:
                     occupied.clear()
-
+                
                 if shape_idx not in occupied:
                     large_obstacle.state.p_pos = pos
                     occupied.add(shape_idx)
                     break
-
+    
     def _reset_small_obstacles(self, world, np_random, paths):
         epsilon = world.small_obstacles[0].size + world.large_obstacles[0].size
 
         agent_positions = [agent.state.p_pos for agent in world.agents]
         goal_positions = [goal.state.p_pos for goal in world.goals]
         large_obstacle_positions = [obstacle.state.p_pos for obstacle in world.large_obstacles]
```

### Comparing `Signal8-4.6/Signal8/utils/core.py` & `Signal8-4.8/Signal8/utils/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         # problem instance
         self.problem_instance = None
         self.instance_constr = None
         
     # return all entities in the world
     @property
     def entities(self):
-        return self.agents + self.goals + self.large_obstacles
+        return self.agents + self.goals + self.large_obstacles + self.small_obstacles
 
     # update state of the world
     def step(self):
         # gather forces applied to entities
         p_force = [None] * len(self.entities)
         # apply agent physical controls
         p_force = self.apply_action_force(p_force)
```

### Comparing `Signal8-4.6/Signal8/utils/problems.py` & `Signal8-4.8/Signal8/utils/problems.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.6/Signal8/utils/simple_env.py` & `Signal8-4.8/Signal8/utils/simple_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from gymnasium.utils import seeding
 
 from pettingzoo import AECEnv
 from pettingzoo.utils import wrappers
 from pettingzoo.utils.agent_selector import agent_selector
 
 def make_env(raw_env):
-    def env(*args):
-        env = raw_env(*args)
+    def env(**kwargs):
+        env = raw_env(**kwargs)
         env = wrappers.AssertOutOfBoundsWrapper(env)
         env = wrappers.OrderEnforcingWrapper(env)
         return env
     return env
 
 
 class SimpleEnv(AECEnv):
```

### Comparing `Signal8-4.6/Signal8/utils/test_dynamic_obs.py` & `Signal8-4.8/Signal8/utils/test_dynamic_obs.py`

 * *Files identical despite different names*

### Comparing `Signal8-4.6/Signal8.egg-info/PKG-INFO` & `Signal8-4.8/Signal8.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 4.6
+Version: 4.8
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-4.6/setup.py` & `Signal8-4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="4.6",
+    version="4.8",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

