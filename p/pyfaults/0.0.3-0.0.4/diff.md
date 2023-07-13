# Comparing `tmp/pyfaults-0.0.3.tar.gz` & `tmp/pyfaults-0.0.4.tar.gz`

## Comparing `pyfaults-0.0.3.tar` & `pyfaults-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 pyfaults-0.0.3/src/pyfaults/FLT_supercell.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 pyfaults-0.0.3/src/pyfaults/UF_supercell.py
--rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 pyfaults-0.0.3/src/pyfaults/XRD_sim.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pyfaults-0.0.3/src/pyfaults/__init__.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 pyfaults-0.0.3/src/pyfaults/child_layer.py
--rw-r--r--   0        0        0     9621 2020-02-02 00:00:00.000000 pyfaults-0.0.3/src/pyfaults/classes.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 pyfaults-0.0.3/src/pyfaults/layer.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pyfaults-0.0.3/src/pyfaults/stack_gen.py
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 pyfaults-0.0.3/src/pyfaults/stacking_vector.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 pyfaults-0.0.3/src/pyfaults/unitcell.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 pyfaults-0.0.3/src/pyfaults/write_cif.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pyfaults-0.0.3/README.md
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 pyfaults-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 pyfaults-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 pyfaults-0.0.4/src/pyfaults/FLT_supercell.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 pyfaults-0.0.4/src/pyfaults/UF_supercell.py
+-rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 pyfaults-0.0.4/src/pyfaults/XRD_sim.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pyfaults-0.0.4/src/pyfaults/__init__.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 pyfaults-0.0.4/src/pyfaults/child_layer.py
+-rw-r--r--   0        0        0     9621 2020-02-02 00:00:00.000000 pyfaults-0.0.4/src/pyfaults/classes.py
+-rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 pyfaults-0.0.4/src/pyfaults/layer.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 pyfaults-0.0.4/src/pyfaults/stack_gen.py
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 pyfaults-0.0.4/src/pyfaults/stacking_vector.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 pyfaults-0.0.4/src/pyfaults/unitcell.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 pyfaults-0.0.4/src/pyfaults/write_cif.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pyfaults-0.0.4/README.md
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 pyfaults-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 pyfaults-0.0.4/PKG-INFO
```

### Comparing `pyfaults-0.0.3/src/pyfaults/FLT_supercell.py` & `pyfaults-0.0.4/src/pyfaults/FLT_supercell.py`

 * *Files identical despite different names*

### Comparing `pyfaults-0.0.3/src/pyfaults/UF_supercell.py` & `pyfaults-0.0.4/src/pyfaults/UF_supercell.py`

 * *Files identical despite different names*

### Comparing `pyfaults-0.0.3/src/pyfaults/XRD_sim.py` & `pyfaults-0.0.4/src/pyfaults/XRD_sim.py`

 * *Files identical despite different names*

### Comparing `pyfaults-0.0.3/src/pyfaults/child_layer.py` & `pyfaults-0.0.4/src/pyfaults/child_layer.py`

 * *Files identical despite different names*

### Comparing `pyfaults-0.0.3/src/pyfaults/classes.py` & `pyfaults-0.0.4/src/pyfaults/classes.py`

 * *Files identical despite different names*

### Comparing `pyfaults-0.0.3/src/pyfaults/stack_gen.py` & `pyfaults-0.0.4/src/pyfaults/stack_gen.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     path = os.path.join(directory, filename + ".csv")
     
     df = pd.read_csv(path)
     
     return df
 
 def get_layer(df, layer_name, latt):
-    import classes    
+    import classes
     
     l = df[df["Layer"] == layer_name]
     
     atom_list = []
     for j in range(0, len(l.index)):
         atom = l.iloc[j]["Atom"]
         elem = l.iloc[j]["Element"]
```

### Comparing `pyfaults-0.0.3/src/pyfaults/stacking_vector.py` & `pyfaults-0.0.4/src/pyfaults/stacking_vector.py`

 * *Files identical despite different names*

### Comparing `pyfaults-0.0.3/src/pyfaults/unitcell.py` & `pyfaults-0.0.4/src/pyfaults/unitcell.py`

 * *Files identical despite different names*

### Comparing `pyfaults-0.0.3/src/pyfaults/write_cif.py` & `pyfaults-0.0.4/src/pyfaults/write_cif.py`

 * *Files identical despite different names*

### Comparing `pyfaults-0.0.3/pyproject.toml` & `pyfaults-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyfaults"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
 	{name = "Sinclair Combs", email = "sinclaircombs@mines.edu"}
 ]
 description = "Python package for modelling stacking faults"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```
