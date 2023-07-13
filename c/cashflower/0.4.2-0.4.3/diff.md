# Comparing `tmp/cashflower-0.4.2.tar.gz` & `tmp/cashflower-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cashflower-0.4.2.tar", last modified: Wed Jul 12 19:30:35 2023, max compression
+gzip compressed data, was "cashflower-0.4.3.tar", last modified: Thu Jul 13 18:54:42 2023, max compression
```

## Comparing `cashflower-0.4.2.tar` & `cashflower-0.4.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:30:35.348088 cashflower-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-12 19:30:21.000000 cashflower-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-12 19:30:21.000000 cashflower-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-12 19:30:35.348088 cashflower-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-12 19:30:21.000000 cashflower-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:30:35.348088 cashflower-0.4.2/cashflower/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-12 19:30:21.000000 cashflower-0.4.2/cashflower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-07-12 19:30:21.000000 cashflower-0.4.2/cashflower/cashflow.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-12 19:30:21.000000 cashflower-0.4.2/cashflower/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-07-12 19:30:21.000000 cashflower-0.4.2/cashflower/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:30:35.348088 cashflower-0.4.2/cashflower/model_tpl/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-12 19:30:21.000000 cashflower-0.4.2/cashflower/model_tpl/input.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-12 19:30:21.000000 cashflower-0.4.2/cashflower/model_tpl/model.py-tpl
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-12 19:30:21.000000 cashflower-0.4.2/cashflower/model_tpl/run.py-tpl
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-12 19:30:21.000000 cashflower-0.4.2/cashflower/model_tpl/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-07-12 19:30:21.000000 cashflower-0.4.2/cashflower/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-12 19:30:21.000000 cashflower-0.4.2/cashflower/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:30:35.348088 cashflower-0.4.2/cashflower.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-12 19:30:35.000000 cashflower-0.4.2/cashflower.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-12 19:30:35.000000 cashflower-0.4.2/cashflower.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 19:30:35.000000 cashflower-0.4.2/cashflower.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-12 19:30:35.000000 cashflower-0.4.2/cashflower.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 19:30:35.000000 cashflower-0.4.2/cashflower.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 19:30:35.348088 cashflower-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-12 19:30:21.000000 cashflower-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 19:30:35.348088 cashflower-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-12 19:30:21.000000 cashflower-0.4.2/tests/test_cashflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-12 19:30:21.000000 cashflower-0.4.2/tests/test_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-12 19:30:21.000000 cashflower-0.4.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:54:42.657668 cashflower-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-13 18:54:30.000000 cashflower-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-13 18:54:30.000000 cashflower-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-13 18:54:42.657668 cashflower-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-13 18:54:30.000000 cashflower-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:54:42.653668 cashflower-0.4.3/cashflower/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-13 18:54:30.000000 cashflower-0.4.3/cashflower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14938 2023-07-13 18:54:30.000000 cashflower-0.4.3/cashflower/cashflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-13 18:54:30.000000 cashflower-0.4.3/cashflower/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-13 18:54:30.000000 cashflower-0.4.3/cashflower/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:54:42.657668 cashflower-0.4.3/cashflower/model_tpl/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-13 18:54:30.000000 cashflower-0.4.3/cashflower/model_tpl/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-13 18:54:30.000000 cashflower-0.4.3/cashflower/model_tpl/model.py-tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-13 18:54:30.000000 cashflower-0.4.3/cashflower/model_tpl/run.py-tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-13 18:54:30.000000 cashflower-0.4.3/cashflower/model_tpl/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7945 2023-07-13 18:54:30.000000 cashflower-0.4.3/cashflower/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-13 18:54:30.000000 cashflower-0.4.3/cashflower/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:54:42.657668 cashflower-0.4.3/cashflower.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-13 18:54:42.000000 cashflower-0.4.3/cashflower.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-13 18:54:42.000000 cashflower-0.4.3/cashflower.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 18:54:42.000000 cashflower-0.4.3/cashflower.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-13 18:54:42.000000 cashflower-0.4.3/cashflower.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 18:54:42.000000 cashflower-0.4.3/cashflower.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 18:54:42.657668 cashflower-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-13 18:54:30.000000 cashflower-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:54:42.657668 cashflower-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-13 18:54:30.000000 cashflower-0.4.3/tests/test_cashflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-13 18:54:30.000000 cashflower-0.4.3/tests/test_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-13 18:54:30.000000 cashflower-0.4.3/tests/test_utils.py
```

### Comparing `cashflower-0.4.2/LICENSE` & `cashflower-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.2/PKG-INFO` & `cashflower-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cashflower
-Version: 0.4.2
+Version: 0.4.3
 Summary: Framework for actuarial cash flow models
 Home-page: https://github.com/acturtle/cashflower
 Author: Zuzanna Chmielewska
 Project-URL: Source, https://github.com/acturtle/cashflower
 Project-URL: Tracker, https://github.com/acturtle/cashflower/issues
 Project-URL: Documentation, https://cashflower.acturtle.com
 Requires-Python: >=3.9
```

### Comparing `cashflower-0.4.2/README.md` & `cashflower-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.2/cashflower/cashflow.py` & `cashflower-0.4.3/cashflower/cashflow.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,38 +5,67 @@
 import pandas as pd
 
 from .error import CashflowModelError
 from .utils import get_object_by_name, print_log, split_to_ranges, updt
 from .graph import get_calc_direction, get_calls, get_predecessors
 
 
-def variable():
+def variable(repeat=None):
     """Decorator"""
     def wrapper(func):
+        # Variable must have parameter 't' or no parameters at all
+        if func.__code__.co_argcount > 1:
+            msg = f"Model variable must have maximally one parameter. Please review '{func.__name__}'."
+            raise CashflowModelError(msg)
+
+        # Parameter must be named 't'
+        if func.__code__.co_argcount == 1:
+            if not func.__code__.co_varnames[0] == 't':
+                msg = f"The name of the parameter must be named 't'. Please review '{func.__name__}'."
+                raise CashflowModelError(msg)
+
+        # Create a variable
         variable = Variable(func)
+
+        # Variable is constant if it is t-independent
+        if func.__code__.co_argcount == 0:
+            variable.constant = True
+
+        # Results are repeated for all model points
+        if repeat:
+            variable.repeat = True
+
         return variable
     return wrapper
 
 
 class Variable:
     def __init__(self, func):
         self.func = func
         self.name = None
         self._settings = None
-        self.result = None
+
         self.calls = None
+        self.calc_direction = None
         self.calc_order = None
+        self.constant = False
         self.cycle = False
-        self.calc_direction = None
+        self.repeat = False
+        self.result = None
+
         self.runtime = 0
 
     def __repr__(self):
         return f"V: {self.func.__name__}"
 
-    def __call__(self, t):
+    def __call__(self, t=None):
+        # Variable is constant so all values are the same
+        if t is None and self.constant:
+            return self.result[0]
+
         if t < 0 or t > self.settings["T_MAX_CALCULATION"]:
             msg = f"Variable '{self.name}' has been called for period '{t}' which is outside of calculation range."
             raise CashflowModelError(msg)
 
         # In the cycle, we don't know exact calculation order
         if self.cycle and self.result[t] is None:
             return self.func(t)
@@ -53,27 +82,44 @@
 
     @settings.setter
     def settings(self, new_settings):
         self._settings = new_settings
         self.result = [None for _ in range(0, self.settings["T_MAX_CALCULATION"] + 1)]
 
     def calculate_t(self, t):
-        self.result[t] = self.func(t)
+        if self.repeat and self.result[t] is not None:
+            return None
+
+        # Constant variable
+        if self.constant:
+            self.result[t] = self.func()
+        # Time-dependent variable
+        else:
+            self.result[t] = self.func(t)
 
     def calculate(self):
-        if self.calc_direction == "irrelevant":
-            self.result = [*map(self.func, range(self.settings["T_MAX_CALCULATION"] + 1))]
-        elif self.calc_direction == "forward":
-            for t in range(self.settings["T_MAX_CALCULATION"] + 1):
-                self.result[t] = self.func(t)
-        elif self.calc_direction == "backward":
-            for t in range(self.settings["T_MAX_CALCULATION"], -1, -1):
-                self.result[t] = self.func(t)
+        if self.repeat and not any([_ is None for _ in self.result]):
+            return None
+
+        # Constant variable
+        if self.constant:
+            value = self.func()
+            self.result = [value for _ in range(0, self.settings["T_MAX_CALCULATION"] + 1)]
+        # Time-dependent variable
         else:
-            raise CashflowModelError(f"Incorrect calculation direction {self.calc_direction}")
+            if self.calc_direction == "irrelevant":
+                self.result = [*map(self.func, range(self.settings["T_MAX_CALCULATION"] + 1))]
+            elif self.calc_direction == "forward":
+                for t in range(self.settings["T_MAX_CALCULATION"] + 1):
+                    self.result[t] = self.func(t)
+            elif self.calc_direction == "backward":
+                for t in range(self.settings["T_MAX_CALCULATION"], -1, -1):
+                    self.result[t] = self.func(t)
+            else:
+                raise CashflowModelError(f"Incorrect calculation direction {self.calc_direction}")
 
 
 class Runplan:
     """Runplan of the cash flow model."""
     def __init__(self, data=None, version="1"):
         self.data = data
         self.set_empty_data()
@@ -282,14 +328,16 @@
         diagnostic = None
         if self.settings["SAVE_DIAGNOSTIC"]:
             diagnostic = pd.DataFrame({
                 "variable": [v.name for v in self.variables],
                 "calc_order": [v.calc_order for v in self.variables],
                 "cycle": [v.cycle for v in self.variables],
                 "calc_direction": [v.calc_direction for v in self.variables],
+                "constant": [v.constant for v in self.variables],
+                "repeat": [v.repeat for v in self.variables],
                 "runtime": [v.runtime for v in self.variables]
             })
 
         return result, diagnostic
 
     def calculate_model_point(self, row, one_core, progressbar_max):
         main = get_object_by_name(self.model_point_sets, "main")
```

### Comparing `cashflower-0.4.2/cashflower/graph.py` & `cashflower-0.4.3/cashflower/graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,16 +67,20 @@
                 queue.put(child)
                 visited.append(child)
 
     return visited
 
 
 def raise_error_if_incorrect_argument(node):
-    if len(node.args) != 1:
-        msg = f"Model variable must have one argument. Please review the call of '{node.func.id}'."
+    # Constant variable - there are no arguments
+    if len(node.args) == 0:
+        return None
+
+    if len(node.args) > 1:
+        msg = f"Model variable must have maximally one argument. Please review the call of '{node.func.id}'."
         raise CashflowModelError(msg)
 
     # Model variable can only call t, t+/-x, and x
     arg = node.args[0]
     msg = f"\nPlease review '{node.func.id}'. The argument of a model variable can be only:\n" \
           f"- t,\n" \
           f"- t plus/minus integer (e.g. t+1 or t-12),\n" \
```

### Comparing `cashflower-0.4.2/cashflower/start.py` & `cashflower-0.4.3/cashflower/start.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
 def get_variables(model_members, settings):
     """Get model variables from model.py script."""
     variable_members = [m for m in model_members if isinstance(m[1], Variable)]
     variables = []
 
     for name, variable in variable_members:
-        if name in ["t", "r"]:
+        if name == "t":
             msg = f"\nA variable can not be named '{name}' because it is a system variable. Please rename it."
             raise CashflowModelError(msg)
         variable.name = name
         variable.settings = settings
         variables.append(variable)
     return variables
 
@@ -166,22 +166,24 @@
         model_output = functools.reduce(lambda x, y: x.add(y, fill_value=0), part_model_outputs)
 
     return model_output
 
 
 def merge_part_diagnostic(part_diagnostic):
     # Nones are returned, when number of policies < number of cpus
-    part_diagnostic = [pd for pd in part_diagnostic if pd is not None]
-    total_runtimes = sum([pd["runtime"] for pd in part_diagnostic])
+    part_diagnostic = [item for item in part_diagnostic if item is not None]
+    total_runtimes = sum([item["runtime"] for item in part_diagnostic])
     first = part_diagnostic[0]
     runtimes = pd.DataFrame({
         "variable": first["variable"],
         "calc_order": first["calc_order"],
         "cycle": first["cycle"],
         "calc_direction": first["calc_direction"],
+        "constant": first["constant"],
+        "repeat": first["repeat"],
         "runtime": total_runtimes
     })
     return runtimes
 
 
 def start(model_name, settings, argv):
     timestamp = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
@@ -196,15 +198,15 @@
             parts = pool.map(p, range(cpu_count))
 
         # Merge model outputs
         part_model_outputs = [p[0] for p in parts]
         output = merge_part_model_outputs(part_model_outputs, settings)
 
         # Merge runtimes
-        if settings["SAVE_RUNTIME"]:
+        if settings["SAVE_DIAGNOSTIC"]:
             part_runtimes = [p[1] for p in parts]
             diagnostic = merge_part_diagnostic(part_runtimes)
     else:
         output, diagnostic = start_single_core(model_name, settings, argv)
 
     # Add time column
     values = [*range(settings["T_MAX_OUTPUT"]+1)] * int(output.shape[0] / (settings["T_MAX_OUTPUT"]+1))
```

### Comparing `cashflower-0.4.2/cashflower/utils.py` & `cashflower-0.4.3/cashflower/utils.py`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.2/cashflower.egg-info/PKG-INFO` & `cashflower-0.4.3/cashflower.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cashflower
-Version: 0.4.2
+Version: 0.4.3
 Summary: Framework for actuarial cash flow models
 Home-page: https://github.com/acturtle/cashflower
 Author: Zuzanna Chmielewska
 Project-URL: Source, https://github.com/acturtle/cashflower
 Project-URL: Tracker, https://github.com/acturtle/cashflower/issues
 Project-URL: Documentation, https://cashflower.acturtle.com
 Requires-Python: >=3.9
```

### Comparing `cashflower-0.4.2/cashflower.egg-info/SOURCES.txt` & `cashflower-0.4.3/cashflower.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.2/setup.py` & `cashflower-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,9 +20,9 @@
     project_urls={
         'Source': 'https://github.com/acturtle/cashflower',
         'Tracker': 'https://github.com/acturtle/cashflower/issues',
         'Documentation': 'https://cashflower.acturtle.com',
     },
     python_requires='>=3.9',
     url="https://github.com/acturtle/cashflower",
-    version="0.4.2",
+    version="0.4.3",
 )
```

### Comparing `cashflower-0.4.2/tests/test_cashflow.py` & `cashflower-0.4.3/tests/test_cashflow.py`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.2/tests/test_start.py` & `cashflower-0.4.3/tests/test_start.py`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.2/tests/test_utils.py` & `cashflower-0.4.3/tests/test_utils.py`

 * *Files identical despite different names*

