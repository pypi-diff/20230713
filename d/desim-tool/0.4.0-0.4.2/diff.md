# Comparing `tmp/desim-tool-0.4.0.tar.gz` & `tmp/desim-tool-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desim-tool-0.4.0.tar", last modified: Sat Jul  1 14:16:39 2023, max compression
+gzip compressed data, was "desim-tool-0.4.2.tar", last modified: Thu Jul 13 10:01:23 2023, max compression
```

## Comparing `desim-tool-0.4.0.tar` & `desim-tool-0.4.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 oscarbennet   (501) staff       (20)        0 2023-07-01 14:16:39.576171 desim-tool-0.4.0/
--rw-r--r--   0 oscarbennet   (501) staff       (20)     1089 2023-05-18 16:32:34.000000 desim-tool-0.4.0/LICENSE.md
--rw-r--r--   0 oscarbennet   (501) staff       (20)      211 2023-07-01 14:16:39.576536 desim-tool-0.4.0/PKG-INFO
--rw-r--r--   0 oscarbennet   (501) staff       (20)     1561 2023-05-18 16:32:34.000000 desim-tool-0.4.0/README.md
-drwxr-xr-x   0 oscarbennet   (501) staff       (20)        0 2023-07-01 14:16:39.572118 desim-tool-0.4.0/desim/
--rw-r--r--   0 oscarbennet   (501) staff       (20)        0 2023-05-18 16:32:34.000000 desim-tool-0.4.0/desim/__init__.py
--rw-r--r--   0 oscarbennet   (501) staff       (20)     2363 2023-05-18 16:32:34.000000 desim-tool-0.4.0/desim/data.py
--rw-r--r--   0 oscarbennet   (501) staff       (20)      110 2023-07-01 12:22:15.000000 desim-tool-0.4.0/desim/helper.py
--rw-r--r--   0 oscarbennet   (501) staff       (20)     6804 2023-07-01 12:52:47.000000 desim-tool-0.4.0/desim/interface.py
--rw-r--r--   0 oscarbennet   (501) staff       (20)    10439 2023-07-01 12:22:15.000000 desim-tool-0.4.0/desim/simulation.py
-drwxr-xr-x   0 oscarbennet   (501) staff       (20)        0 2023-07-01 14:16:39.575600 desim-tool-0.4.0/desim_tool.egg-info/
--rw-r--r--   0 oscarbennet   (501) staff       (20)      211 2023-07-01 14:16:39.000000 desim-tool-0.4.0/desim_tool.egg-info/PKG-INFO
--rw-r--r--   0 oscarbennet   (501) staff       (20)      295 2023-07-01 14:16:39.000000 desim-tool-0.4.0/desim_tool.egg-info/SOURCES.txt
--rw-r--r--   0 oscarbennet   (501) staff       (20)        1 2023-07-01 14:16:39.000000 desim-tool-0.4.0/desim_tool.egg-info/dependency_links.txt
--rw-r--r--   0 oscarbennet   (501) staff       (20)       12 2023-07-01 14:16:39.000000 desim-tool-0.4.0/desim_tool.egg-info/requires.txt
--rw-r--r--   0 oscarbennet   (501) staff       (20)        6 2023-07-01 14:16:39.000000 desim-tool-0.4.0/desim_tool.egg-info/top_level.txt
--rw-r--r--   0 oscarbennet   (501) staff       (20)      106 2023-07-01 14:16:39.578268 desim-tool-0.4.0/setup.cfg
--rw-r--r--   0 oscarbennet   (501) staff       (20)      284 2023-07-01 13:03:18.000000 desim-tool-0.4.0/setup.py
+drwxr-xr-x   0 oscarbennet   (501) staff       (20)        0 2023-07-13 10:01:23.923082 desim-tool-0.4.2/
+-rw-r--r--   0 oscarbennet   (501) staff       (20)     1089 2023-05-18 16:32:34.000000 desim-tool-0.4.2/LICENSE.md
+-rw-r--r--   0 oscarbennet   (501) staff       (20)      256 2023-07-13 10:01:23.923335 desim-tool-0.4.2/PKG-INFO
+-rw-r--r--   0 oscarbennet   (501) staff       (20)     1561 2023-05-18 16:32:34.000000 desim-tool-0.4.2/README.md
+drwxr-xr-x   0 oscarbennet   (501) staff       (20)        0 2023-07-13 10:01:23.919375 desim-tool-0.4.2/desim/
+-rw-r--r--   0 oscarbennet   (501) staff       (20)        0 2023-05-18 16:32:34.000000 desim-tool-0.4.2/desim/__init__.py
+-rw-r--r--   0 oscarbennet   (501) staff       (20)     2363 2023-05-18 16:32:34.000000 desim-tool-0.4.2/desim/data.py
+-rw-r--r--   0 oscarbennet   (501) staff       (20)      110 2023-07-13 08:54:55.000000 desim-tool-0.4.2/desim/helper.py
+-rw-r--r--   0 oscarbennet   (501) staff       (20)     7624 2023-07-13 10:00:32.000000 desim-tool-0.4.2/desim/interface.py
+-rw-r--r--   0 oscarbennet   (501) staff       (20)    10439 2023-07-13 08:54:55.000000 desim-tool-0.4.2/desim/simulation.py
+drwxr-xr-x   0 oscarbennet   (501) staff       (20)        0 2023-07-13 10:01:23.922694 desim-tool-0.4.2/desim_tool.egg-info/
+-rw-r--r--   0 oscarbennet   (501) staff       (20)      256 2023-07-13 10:01:23.000000 desim-tool-0.4.2/desim_tool.egg-info/PKG-INFO
+-rw-r--r--   0 oscarbennet   (501) staff       (20)      295 2023-07-13 10:01:23.000000 desim-tool-0.4.2/desim_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 oscarbennet   (501) staff       (20)        1 2023-07-13 10:01:23.000000 desim-tool-0.4.2/desim_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 oscarbennet   (501) staff       (20)       12 2023-07-13 10:01:23.000000 desim-tool-0.4.2/desim_tool.egg-info/requires.txt
+-rw-r--r--   0 oscarbennet   (501) staff       (20)        6 2023-07-13 10:01:23.000000 desim-tool-0.4.2/desim_tool.egg-info/top_level.txt
+-rw-r--r--   0 oscarbennet   (501) staff       (20)      106 2023-07-13 10:01:23.924074 desim-tool-0.4.2/setup.cfg
+-rw-r--r--   0 oscarbennet   (501) staff       (20)      329 2023-07-13 10:00:22.000000 desim-tool-0.4.2/setup.py
```

### Comparing `desim-tool-0.4.0/LICENSE.md` & `desim-tool-0.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `desim-tool-0.4.0/README.md` & `desim-tool-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `desim-tool-0.4.0/desim/data.py` & `desim-tool-0.4.2/desim/data.py`

 * *Files identical despite different names*

### Comparing `desim-tool-0.4.0/desim/interface.py` & `desim-tool-0.4.2/desim/interface.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,150 +1,152 @@
 from typing import List
 import multiprocessing as mp
 from desim.data import SimResults, TimeFormat
 from desim.simulation import Process, Simulation, NonTechCost
 
 
 class Des(object):
-  """
-  This is a class for running a discrete event simulation. 
+    """
+    This is a class for running a discrete event simulation.
 
-  It is an interface of the different types of simulations that can be run. 
-  Possible simulation types:
-    Normal simulation.
-    Monte Carlo simulation.
-    Parallellized simulation.
-  """
-
-  def __init__(self) -> None:
-      pass
-
-  def run_simulation(self, flow_time: float, flow_rate: float, 
-      flow_start_process: str, processes: List[Process], 
-      non_tech_processes, non_tech_costs: NonTechCost, dsm: dict, time_format: TimeFormat,
-      discount_rate=0.08, until = 100):
-      """
-      Function for running a standard discrete event simulation. Will run the simulation once. 
-
-      Parameters:
-        flow_time (float): The time that entities will flow in the simulation.
-        flow_rate (float): The rate that entities will flow in the simulation. Calculated as Product/time_unit 
-        flow_start_process (str): The process that will start the flow of entites. Takes the name of the process
-        processes (List[Process]): The list of processes of the simulation. 
-        non_tech_processes (List[NonTechProcess]): The list of non technical processes in the simulation.
-        non_tech_costs (NonTechCost): How the non technical processes will be distributed. 
-        dsm (dict): A design structure matrix showing how the processes interact with eachother. 
-        time_format (TimeFormat): The unit of time of the simulation. 
-        discount_rate (float): The discount rate. 
-        until (float): For how long the simulation will run. 
-
-      """
-      
-      sim = Simulation(flow_time, flow_rate, flow_start_process, until, discount_rate,
-                    processes, non_tech_processes, non_tech_costs, dsm, time_format)
-      sim.run_simulation()
-
-
-      return SimResults('No Design', processes, [sim.time_steps], [sim.cum_NPV], [sim.total_costs], [sim.total_revenue])
-
-  def run_monte_carlo_simulation(self, flow_time: float, flow_rate: float, 
-      flow_start_process: str, processes: List[Process], 
-      non_tech_processes, non_tech_costs: NonTechCost, dsm: dict, time_format: TimeFormat,
-      discount_rate=0.08, until = 100, runs=300):
-      """
-      Function for running a monte carlo version of the simulation. Will run the simulation @runs amount of times. 
-
-      Parameters:
-        flow_time (float): The time that entities will flow in the simulation.
-        flow_rate (float): The rate that entities will flow in the simulation. Calculated as Product/time_unit 
-        flow_start_process (str): The process that will start the flow of entites. Takes the name of the process
-        processes (List[Process]): The list of processes of the simulation. 
-        non_tech_processes (List[NonTechProcess]): The list of non technical processes in the simulation.
-        non_tech_costs (NonTechCost): How the non technical processes will be distributed. 
-        dsm (dict): A design structure matrix showing how the processes interact with eachother. 
-        time_format (TimeFormat): The unit of time of the simulation. 
-        discount_rate (float): The discount rate. 
-        until (float): For how long the simulation will run. 
-        runs (int): The amount of times the simulation will be run. 
-
-      """
-
-
-      time_steps = []
-      cumulative_NPV = []
-      total_costs = []
-      total_revenue = []
+    It is an interface of the different types of simulations that can be run.
+    Possible simulation types:
+      Normal simulation.
+      Monte Carlo simulation.
+      Parallellized simulation.
+    """
+
+    def __init__(self) -> None:
+        pass
+
+    def run_simulation(self, flow_time: float, flow_rate: float,
+                       flow_start_process: str, processes: List[Process],
+                       non_tech_processes, non_tech_costs: NonTechCost, dsm: dict, time_format: TimeFormat,
+                       discount_rate=0.08, until=100):
+        """
+        Function for running a standard discrete event simulation. Will run the simulation once.
+
+        Parameters:
+          flow_time (float): The time that entities will flow in the simulation.
+          flow_rate (float): The rate that entities will flow in the simulation. Calculated as Product/time_unit
+          flow_start_process (str): The process that will start the flow of entites. Takes the name of the process
+          processes (List[Process]): The list of processes of the simulation.
+          non_tech_processes (List[NonTechProcess]): The list of non technical processes in the simulation.
+          non_tech_costs (NonTechCost): How the non technical processes will be distributed.
+          dsm (dict): A design structure matrix showing how the processes interact with eachother.
+          time_format (TimeFormat): The unit of time of the simulation.
+          discount_rate (float): The discount rate.
+          until (float): For how long the simulation will run.
+
+        """
 
-      for _ in range(runs):
         sim = Simulation(flow_time, flow_rate, flow_start_process, until, discount_rate,
-                    processes, non_tech_processes, non_tech_costs, dsm, time_format)
+                         processes, non_tech_processes, non_tech_costs, dsm, time_format)
         sim.run_simulation()
-         
 
-        time_steps.append(sim.time_steps)
-        cumulative_NPV.append(sim.cum_NPV)
-        total_costs.append(sim.total_costs)
-        total_revenue.append(sim.total_revenue)
-      
-      
-      
-      return SimResults('No Design', processes, time_steps, cumulative_NPV, total_costs, total_revenue)
-
-  def run_parallell_simulations(self, flow_time: float, flow_rate: float, 
-      flow_start_process: str, processes: List[Process], 
-      non_tech_processes, non_tech_costs: NonTechCost, dsm: dict, time_format: TimeFormat,
-      discount_rate=0.08, until = 100, runs=300):
-      """
-      Function for running a parallelized monte carlo version of the simulation. 
-      Will run the simulation @runs amount of times. 
-
-      Parameters:
-        flow_time (float): The time that entities will flow in the simulation.
-        flow_rate (float): The rate that entities will flow in the simulation. Calculated as Product/time_unit 
-        flow_start_process (str): The process that will start the flow of entites. Takes the name of the process.
-        processes (List[Process]): The list of processes of the simulation. 
-        non_tech_processes (List[NonTechProcess]): The list of non technical processes in the simulation.
-        non_tech_costs (NonTechCost): How the non technical processes will be distributed. 
-        dsm (dict): A design structure matrix showing how the processes interact with eachother. 
-        time_format (TimeFormat): The unit of time of the simulation. 
-        discount_rate (float): The discount rate. 
-        until (float): For how long the simulation will run. 
-        runs (int): The amount of times the simulation will be run. 
-      
-      """
-
-      time_steps = []
-      cumulative_NPV = []
-      total_costs = []
-      total_revenue = []
-
-
-      pool = mp.Pool(mp.cpu_count())
-
-      mp_processes = [pool.apply_async(func=self.help_run_simulation, args=(flow_time, flow_rate, flow_start_process, processes, 
-        non_tech_processes, non_tech_costs, dsm, time_format, discount_rate, until)) for _ in range(runs)]
-
-      res = [f.get() for f in mp_processes]
-
-      for time, npv, cost, revenue in res:
-          time_steps.append(time)
-          cumulative_NPV.append(npv)
-          total_costs.append(cost)
-          total_revenue.append(revenue)
-
-
-      return SimResults('No Design', processes, time_steps, cumulative_NPV, total_costs, total_revenue)
-
-  def help_run_simulation(self, flow_time: float, flow_rate: float, 
-      flow_start_process: str, processes: List[Process], 
-      non_tech_processes, non_tech_costs: NonTechCost, dsm: dict, time_format: TimeFormat,
-      discount_rate=0.08, until = 100):
-      """
-      Helper function for the parallelization module in this class. 
-      
-      """
-
-      sim = Simulation(flow_time, flow_rate, flow_start_process, until, discount_rate,
-                    processes, non_tech_processes, non_tech_costs, dsm, time_format)
-      sim.run_simulation()
+        return SimResults('No Design', processes, [sim.time_steps], [sim.cum_NPV], [sim.total_costs],
+                          [sim.total_revenue])
+
+    def run_monte_carlo_simulation(self, flow_time: float, flow_rate: float,
+                                   flow_start_process: str, processes: List[Process],
+                                   non_tech_processes, non_tech_costs: NonTechCost, dsm: dict, time_format: TimeFormat,
+                                   discount_rate=0.08, until=100, runs=300):
+        """
+        Function for running a monte carlo version of the simulation. Will run the simulation @runs amount of times.
+
+        Parameters:
+          flow_time (float): The time that entities will flow in the simulation.
+          flow_rate (float): The rate that entities will flow in the simulation. Calculated as Product/time_unit
+          flow_start_process (str): The process that will start the flow of entites. Takes the name of the process
+          processes (List[Process]): The list of processes of the simulation.
+          non_tech_processes (List[NonTechProcess]): The list of non technical processes in the simulation.
+          non_tech_costs (NonTechCost): How the non technical processes will be distributed.
+          dsm (dict): A design structure matrix showing how the processes interact with eachother.
+          time_format (TimeFormat): The unit of time of the simulation.
+          discount_rate (float): The discount rate.
+          until (float): For how long the simulation will run.
+          runs (int): The amount of times the simulation will be run.
+
+        """
+
+        time_steps = []
+        cumulative_NPV = []
+        total_costs = []
+        total_revenue = []
+
+        for _ in range(runs):
+            sim = Simulation(flow_time, flow_rate, flow_start_process, until, discount_rate,
+                             processes, non_tech_processes, non_tech_costs, dsm, time_format)
+            sim.run_simulation()
+
+            time_steps.append(sim.time_steps)
+            cumulative_NPV.append(sim.cum_NPV)
+            total_costs.append(sim.total_costs)
+            total_revenue.append(sim.total_revenue)
+
+        return SimResults('No Design', processes, time_steps, cumulative_NPV, total_costs, total_revenue)
+
+    def run_parallell_simulations(self, flow_time: float, flow_rate: float,
+                                  flow_start_process: str, processes: List[Process],
+                                  non_tech_processes, non_tech_costs: NonTechCost, dsm: dict, time_format: TimeFormat,
+                                  discount_rate=0.08, until=100, runs=300):
+        """
+        Function for running a parallelized monte carlo version of the simulation.
+        Will run the simulation @runs amount of times.
+
+        Parameters:
+          flow_time (float): The time that entities will flow in the simulation.
+          flow_rate (float): The rate that entities will flow in the simulation. Calculated as Product/time_unit
+          flow_start_process (str): The process that will start the flow of entites. Takes the name of the process.
+          processes (List[Process]): The list of processes of the simulation.
+          non_tech_processes (List[NonTechProcess]): The list of non technical processes in the simulation.
+          non_tech_costs (NonTechCost): How the non technical processes will be distributed.
+          dsm (dict): A design structure matrix showing how the processes interact with eachother.
+          time_format (TimeFormat): The unit of time of the simulation.
+          discount_rate (float): The discount rate.
+          until (float): For how long the simulation will run.
+          runs (int): The amount of times the simulation will be run.
+
+        """
+
+        time_steps = []
+        cumulative_NPV = []
+        total_costs = []
+        total_revenue = []
+
+        # Try/Catch because it can only be set once.
+        try:
+            # Important! If not set, the server will be terminated after simulation is complete.
+            mp.set_start_method('spawn')
+        except RuntimeError:
+            pass
+        pool = mp.Pool(mp.cpu_count())
+
+        mp_processes = [
+            pool.apply_async(func=self.help_run_simulation, args=(flow_time, flow_rate, flow_start_process, processes,
+                                                                  non_tech_processes, non_tech_costs, dsm, time_format,
+                                                                  discount_rate, until)) for _ in range(runs)]
+
+        res = [f.get() for f in mp_processes]
+
+        for time, npv, cost, revenue in res:
+            time_steps.append(time)
+            cumulative_NPV.append(npv)
+            total_costs.append(cost)
+            total_revenue.append(revenue)
+
+        return SimResults('No Design', processes, time_steps, cumulative_NPV, total_costs, total_revenue)
+
+    def help_run_simulation(self, flow_time: float, flow_rate: float,
+                            flow_start_process: str, processes: List[Process],
+                            non_tech_processes, non_tech_costs: NonTechCost, dsm: dict, time_format: TimeFormat,
+                            discount_rate=0.08, until=100):
+        """
+        Helper function for the parallelization module in this class.
+
+        """
+
+        sim = Simulation(flow_time, flow_rate, flow_start_process, until, discount_rate,
+                         processes, non_tech_processes, non_tech_costs, dsm, time_format)
+        sim.run_simulation()
 
-      return sim.time_steps, sim.cum_NPV, sim.total_costs, sim.total_revenue
+        return sim.time_steps, sim.cum_NPV, sim.total_costs, sim.total_revenue
```

### Comparing `desim-tool-0.4.0/desim/simulation.py` & `desim-tool-0.4.2/desim/simulation.py`

 * *Files identical despite different names*

