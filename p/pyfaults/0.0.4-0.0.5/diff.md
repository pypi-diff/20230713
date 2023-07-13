# Comparing `tmp/pyfaults-0.0.4.tar.gz` & `tmp/pyfaults-0.0.5.tar.gz`

## Comparing `pyfaults-0.0.4.tar` & `pyfaults-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 pyfaults-0.0.4/src/pyfaults/FLT_supercell.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 pyfaults-0.0.4/src/pyfaults/UF_supercell.py
--rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 pyfaults-0.0.4/src/pyfaults/XRD_sim.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pyfaults-0.0.4/src/pyfaults/__init__.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 pyfaults-0.0.4/src/pyfaults/child_layer.py
--rw-r--r--   0        0        0     9621 2020-02-02 00:00:00.000000 pyfaults-0.0.4/src/pyfaults/classes.py
--rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 pyfaults-0.0.4/src/pyfaults/layer.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 pyfaults-0.0.4/src/pyfaults/stack_gen.py
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 pyfaults-0.0.4/src/pyfaults/stacking_vector.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 pyfaults-0.0.4/src/pyfaults/unitcell.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 pyfaults-0.0.4/src/pyfaults/write_cif.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pyfaults-0.0.4/README.md
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 pyfaults-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 pyfaults-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 pyfaults-0.0.5/src/pyfaults/FLT_supercell.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 pyfaults-0.0.5/src/pyfaults/UF_supercell.py
+-rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 pyfaults-0.0.5/src/pyfaults/XRD_sim.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pyfaults-0.0.5/src/pyfaults/__init__.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 pyfaults-0.0.5/src/pyfaults/child_layer.py
+-rw-r--r--   0        0        0     9621 2020-02-02 00:00:00.000000 pyfaults-0.0.5/src/pyfaults/classes.py
+-rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 pyfaults-0.0.5/src/pyfaults/layer.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 pyfaults-0.0.5/src/pyfaults/stack_gen.py
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 pyfaults-0.0.5/src/pyfaults/stacking_vector.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 pyfaults-0.0.5/src/pyfaults/unitcell.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 pyfaults-0.0.5/src/pyfaults/write_cif.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pyfaults-0.0.5/README.md
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 pyfaults-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 pyfaults-0.0.5/PKG-INFO
```

### Comparing `pyfaults-0.0.4/src/pyfaults/FLT_supercell.py` & `pyfaults-0.0.5/src/pyfaults/FLT_supercell.py`

 * *Files identical despite different names*

### Comparing `pyfaults-0.0.4/src/pyfaults/UF_supercell.py` & `pyfaults-0.0.5/src/pyfaults/UF_supercell.py`

 * *Files identical despite different names*

### Comparing `pyfaults-0.0.4/src/pyfaults/XRD_sim.py` & `pyfaults-0.0.5/src/pyfaults/XRD_sim.py`

 * *Files identical despite different names*

### Comparing `pyfaults-0.0.4/src/pyfaults/child_layer.py` & `pyfaults-0.0.5/src/pyfaults/child_layer.py`

 * *Files identical despite different names*

### Comparing `pyfaults-0.0.4/src/pyfaults/classes.py` & `pyfaults-0.0.5/src/pyfaults/classes.py`

 * *Files identical despite different names*

### Comparing `pyfaults-0.0.4/src/pyfaults/layer.py` & `pyfaults-0.0.5/src/pyfaults/layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,14 @@
     
     df = pd.read_csv(path)
     
     return df
     
 # generate layer from csv data
 def get_layer(df, layer_name, latt):
-    import classes
     
     l = df[df["Layer"] == layer_name]
     
     atom_list = []
     for j in range(0, len(l.index)):
         atom = l.iloc[j]["Atom"]
         elem = l.iloc[j]["Element"]
@@ -116,15 +115,15 @@
         
         pos = [x,y,z]
         
         new_atom = Atom(atype=elem, xyz=pos, label=atom, occupancy=occ, lattice=latt)
         
         atom_list.append(new_atom)
         
-    new_layer = classes.Layer(atom_list, latt, layer_name)
+    new_layer = Layer(atom_list, latt, layer_name)
     
     return new_layer
     
 # generate child layer
 def gen_child(name, parent_layer, t_vect):
     child_layer = Child_Layer(layer_name=name, parent=parent_layer, shift=t_vect)
```

### Comparing `pyfaults-0.0.4/src/pyfaults/stack_gen.py` & `pyfaults-0.0.5/src/pyfaults/stack_gen.py`

 * *Files identical despite different names*

### Comparing `pyfaults-0.0.4/src/pyfaults/stacking_vector.py` & `pyfaults-0.0.5/src/pyfaults/stacking_vector.py`

 * *Files identical despite different names*

### Comparing `pyfaults-0.0.4/src/pyfaults/unitcell.py` & `pyfaults-0.0.5/src/pyfaults/unitcell.py`

 * *Files identical despite different names*

### Comparing `pyfaults-0.0.4/src/pyfaults/write_cif.py` & `pyfaults-0.0.5/src/pyfaults/write_cif.py`

 * *Files identical despite different names*

### Comparing `pyfaults-0.0.4/pyproject.toml` & `pyfaults-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyfaults"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
 	{name = "Sinclair Combs", email = "sinclaircombs@mines.edu"}
 ]
 description = "Python package for modelling stacking faults"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

