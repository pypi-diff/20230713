# Comparing `tmp/ufss-0.1.2.tar.gz` & `tmp/ufss-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ufss-0.1.2.tar", last modified: Fri Jan 27 20:29:19 2023, max compression
+gzip compressed data, was "dist/ufss-0.1.3.tar", last modified: Thu Jul 13 18:02:22 2023, max compression
```

## Comparing `ufss-0.1.2.tar` & `ufss-0.1.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 prose      (501) staff       (20)        0 2023-01-27 20:29:19.000000 ufss-0.1.2/
--rw-r--r--   0 prose      (501) staff       (20)     1088 2020-08-10 15:01:32.000000 ufss-0.1.2/LICENSE
--rw-r--r--   0 prose      (501) staff       (20)     3900 2023-01-27 20:29:19.000000 ufss-0.1.2/PKG-INFO
--rw-r--r--   0 prose      (501) staff       (20)     3257 2021-03-31 15:12:44.000000 ufss-0.1.2/README.md
--rw-r--r--   0 prose      (501) staff       (20)       38 2023-01-27 20:29:19.000000 ufss-0.1.2/setup.cfg
--rw-r--r--   0 prose      (501) staff       (20)     1219 2023-01-27 20:28:16.000000 ufss-0.1.2/setup.py
-drwxr-xr-x   0 prose      (501) staff       (20)        0 2023-01-27 20:29:19.000000 ufss-0.1.2/tests/
--rw-r--r--   0 prose      (501) staff       (20)        0 2022-03-29 04:03:15.000000 ufss-0.1.2/tests/__init__.py
-drwxr-xr-x   0 prose      (501) staff       (20)        0 2023-01-27 20:29:19.000000 ufss-0.1.2/tests/integration/
--rw-r--r--   0 prose      (501) staff       (20)        0 2022-03-29 04:03:15.000000 ufss-0.1.2/tests/integration/__init__.py
--rw-r--r--   0 prose      (501) staff       (20)     3799 2022-03-29 04:08:06.000000 ufss-0.1.2/tests/integration/test_UF2_vs_RKE.py
--rw-r--r--   0 prose      (501) staff       (20)     6510 2022-03-29 04:03:15.000000 ufss-0.1.2/tests/integration/test_linear_absorption.py
--rw-r--r--   0 prose      (501) staff       (20)     2369 2022-03-29 04:03:15.000000 ufss-0.1.2/tests/integration/test_uf2.py
--rw-r--r--   0 prose      (501) staff       (20)     2430 2022-03-29 04:03:15.000000 ufss-0.1.2/tests/integration/test_vs_matlab_code.py
-drwxr-xr-x   0 prose      (501) staff       (20)        0 2023-01-27 20:29:19.000000 ufss-0.1.2/tests/unit/
--rw-r--r--   0 prose      (501) staff       (20)        0 2022-03-29 04:03:15.000000 ufss-0.1.2/tests/unit/__init__.py
-drwxr-xr-x   0 prose      (501) staff       (20)        0 2023-01-27 20:29:19.000000 ufss-0.1.2/ufss/
-drwxr-xr-x   0 prose      (501) staff       (20)        0 2023-01-27 20:29:19.000000 ufss-0.1.2/ufss/HLG/
--rw-r--r--   0 prose      (501) staff       (20)    56049 2021-06-03 14:45:07.000000 ufss-0.1.2/ufss/HLG/DiabaticLindblad_Liouvillians.py
--rw-r--r--   0 prose      (501) staff       (20)    41806 2021-04-13 19:33:38.000000 ufss-0.1.2/ufss/HLG/Hamiltonians.py
--rw-r--r--   0 prose      (501) staff       (20)    44861 2022-03-08 22:12:24.000000 ufss-0.1.2/ufss/HLG/Redfield_Liouvillians.py
--rw-r--r--   0 prose      (501) staff       (20)      674 2021-04-13 19:54:56.000000 ufss-0.1.2/ufss/HLG/__init__.py
--rw-r--r--   0 prose      (501) staff       (20)      551 2020-08-03 02:16:52.000000 ufss-0.1.2/ufss/HLG/base_class.py
--rw-r--r--   0 prose      (501) staff       (20)    21560 2020-08-03 02:16:52.000000 ufss-0.1.2/ufss/HLG/dipole_operator.py
--rw-r--r--   0 prose      (501) staff       (20)    12701 2020-08-03 02:16:52.000000 ufss-0.1.2/ufss/HLG/eigen_generator.py
--rw-r--r--   0 prose      (501) staff       (20)    38460 2020-08-03 02:16:52.000000 ufss-0.1.2/ufss/HLG/eigenstates.py
--rw-r--r--   0 prose      (501) staff       (20)     1938 2021-04-13 19:36:27.000000 ufss-0.1.2/ufss/HLG/general_Liouvillian_classes.py
--rw-r--r--   0 prose      (501) staff       (20)    11205 2021-02-09 01:00:24.000000 ufss-0.1.2/ufss/HLG/manual_L_input.py
--rw-r--r--   0 prose      (501) staff       (20)     3241 2021-03-16 17:24:44.000000 ufss-0.1.2/ufss/HLG/params_converter.py
--rw-r--r--   0 prose      (501) staff       (20)     2076 2021-03-17 19:39:52.000000 ufss-0.1.2/ufss/HLG/run_HLG.py
--rw-r--r--   0 prose      (501) staff       (20)     4731 2020-08-03 02:16:52.000000 ufss-0.1.2/ufss/HLG/simple_eigen_generator.py
-drwxr-xr-x   0 prose      (501) staff       (20)        0 2023-01-27 20:29:19.000000 ufss-0.1.2/ufss/RKE/
--rw-r--r--   0 prose      (501) staff       (20)    24787 2020-12-02 16:24:03.000000 ufss-0.1.2/ufss/RKE/RKE_core.py
--rw-r--r--   0 prose      (501) staff       (20)    50051 2021-04-13 15:37:27.000000 ufss-0.1.2/ufss/RKE/RKE_open_core.py
--rw-r--r--   0 prose      (501) staff       (20)       85 2020-11-30 15:31:51.000000 ufss-0.1.2/ufss/RKE/__init__.py
-drwxr-xr-x   0 prose      (501) staff       (20)        0 2023-01-27 20:29:19.000000 ufss-0.1.2/ufss/UF2/
--rw-r--r--   0 prose      (501) staff       (20)    49901 2021-06-03 19:04:43.000000 ufss-0.1.2/ufss/UF2/UF2_core.py
--rw-r--r--   0 prose      (501) staff       (20)    71597 2022-09-02 15:45:17.000000 ufss-0.1.2/ufss/UF2/UF2_open_core.py
--rw-r--r--   0 prose      (501) staff       (20)      127 2020-11-30 15:26:38.000000 ufss-0.1.2/ufss/UF2/__init__.py
--rw-r--r--   0 prose      (501) staff       (20)     3966 2020-08-18 01:44:14.000000 ufss-0.1.2/ufss/UF2/heaviside_convolve.py
--rw-r--r--   0 prose      (501) staff       (20)      401 2021-05-04 00:32:01.000000 ufss-0.1.2/ufss/__init__.py
--rw-r--r--   0 prose      (501) staff       (20)     4837 2021-05-28 14:17:36.000000 ufss-0.1.2/ufss/convergence_tester.py
--rw-r--r--   0 prose      (501) staff       (20)    17348 2023-01-27 14:53:52.000000 ufss-0.1.2/ufss/diagram_automation.py
--rw-r--r--   0 prose      (501) staff       (20)     4969 2020-08-03 02:16:52.000000 ufss-0.1.2/ufss/dipole_pruning.py
--rw-r--r--   0 prose      (501) staff       (20)     1274 2020-11-25 15:52:42.000000 ufss-0.1.2/ufss/efield_shapes.py
-drwxr-xr-x   0 prose      (501) staff       (20)        0 2023-01-27 20:29:19.000000 ufss-0.1.2/ufss/signals/
--rw-r--r--   0 prose      (501) staff       (20)      145 2020-08-03 02:16:52.000000 ufss-0.1.2/ufss/signals/__init__.py
--rw-r--r--   0 prose      (501) staff       (20)     4684 2022-03-08 22:08:00.000000 ufss-0.1.2/ufss/signals/isotropic_averaging.py
--rw-r--r--   0 prose      (501) staff       (20)    14493 2021-06-08 17:22:29.000000 ufss-0.1.2/ufss/signals/plotting_tools.py
--rw-r--r--   0 prose      (501) staff       (20)     5251 2020-08-03 02:16:52.000000 ufss-0.1.2/ufss/signals/signal_processing.py
-drwxr-xr-x   0 prose      (501) staff       (20)        0 2023-01-27 20:29:19.000000 ufss-0.1.2/ufss.egg-info/
--rw-r--r--   0 prose      (501) staff       (20)     3900 2023-01-27 20:29:19.000000 ufss-0.1.2/ufss.egg-info/PKG-INFO
--rw-r--r--   0 prose      (501) staff       (20)     1173 2023-01-27 20:29:19.000000 ufss-0.1.2/ufss.egg-info/SOURCES.txt
--rw-r--r--   0 prose      (501) staff       (20)        1 2023-01-27 20:29:19.000000 ufss-0.1.2/ufss.egg-info/dependency_links.txt
--rw-r--r--   0 prose      (501) staff       (20)       44 2023-01-27 20:29:19.000000 ufss-0.1.2/ufss.egg-info/requires.txt
--rw-r--r--   0 prose      (501) staff       (20)       11 2023-01-27 20:29:19.000000 ufss-0.1.2/ufss.egg-info/top_level.txt
+drwxr-xr-x   0 prose      (501) staff       (20)        0 2023-07-13 18:02:22.000000 ufss-0.1.3/
+-rw-r--r--   0 prose      (501) staff       (20)     1088 2020-08-10 15:01:32.000000 ufss-0.1.3/LICENSE
+-rw-r--r--   0 prose      (501) staff       (20)     3871 2023-07-13 18:02:22.000000 ufss-0.1.3/PKG-INFO
+-rw-r--r--   0 prose      (501) staff       (20)     3257 2021-03-31 15:12:44.000000 ufss-0.1.3/README.md
+-rw-r--r--   0 prose      (501) staff       (20)       38 2023-07-13 18:02:22.000000 ufss-0.1.3/setup.cfg
+-rw-r--r--   0 prose      (501) staff       (20)     1219 2023-07-13 17:53:54.000000 ufss-0.1.3/setup.py
+drwxr-xr-x   0 prose      (501) staff       (20)        0 2023-07-13 18:02:22.000000 ufss-0.1.3/tests/
+-rw-r--r--   0 prose      (501) staff       (20)        0 2022-03-29 04:03:15.000000 ufss-0.1.3/tests/__init__.py
+drwxr-xr-x   0 prose      (501) staff       (20)        0 2023-07-13 18:02:22.000000 ufss-0.1.3/tests/integration/
+-rw-r--r--   0 prose      (501) staff       (20)        0 2022-03-29 04:03:15.000000 ufss-0.1.3/tests/integration/__init__.py
+-rw-r--r--   0 prose      (501) staff       (20)     3799 2022-03-29 04:08:06.000000 ufss-0.1.3/tests/integration/test_UF2_vs_RKE.py
+-rw-r--r--   0 prose      (501) staff       (20)     6510 2022-03-29 04:03:15.000000 ufss-0.1.3/tests/integration/test_linear_absorption.py
+-rw-r--r--   0 prose      (501) staff       (20)     2369 2022-03-29 04:03:15.000000 ufss-0.1.3/tests/integration/test_uf2.py
+-rw-r--r--   0 prose      (501) staff       (20)     2430 2022-03-29 04:03:15.000000 ufss-0.1.3/tests/integration/test_vs_matlab_code.py
+drwxr-xr-x   0 prose      (501) staff       (20)        0 2023-07-13 18:02:22.000000 ufss-0.1.3/tests/unit/
+-rw-r--r--   0 prose      (501) staff       (20)        0 2022-03-29 04:03:15.000000 ufss-0.1.3/tests/unit/__init__.py
+drwxr-xr-x   0 prose      (501) staff       (20)        0 2023-07-13 18:02:22.000000 ufss-0.1.3/ufss/
+drwxr-xr-x   0 prose      (501) staff       (20)        0 2023-07-13 18:02:22.000000 ufss-0.1.3/ufss/HLG/
+-rw-r--r--   0 prose      (501) staff       (20)    56049 2021-06-03 14:45:07.000000 ufss-0.1.3/ufss/HLG/DiabaticLindblad_Liouvillians.py
+-rw-r--r--   0 prose      (501) staff       (20)    41806 2021-04-13 19:33:38.000000 ufss-0.1.3/ufss/HLG/Hamiltonians.py
+-rw-r--r--   0 prose      (501) staff       (20)    44861 2022-03-08 22:12:24.000000 ufss-0.1.3/ufss/HLG/Redfield_Liouvillians.py
+-rw-r--r--   0 prose      (501) staff       (20)      674 2021-04-13 19:54:56.000000 ufss-0.1.3/ufss/HLG/__init__.py
+-rw-r--r--   0 prose      (501) staff       (20)      551 2020-08-03 02:16:52.000000 ufss-0.1.3/ufss/HLG/base_class.py
+-rw-r--r--   0 prose      (501) staff       (20)    21560 2020-08-03 02:16:52.000000 ufss-0.1.3/ufss/HLG/dipole_operator.py
+-rw-r--r--   0 prose      (501) staff       (20)    12701 2020-08-03 02:16:52.000000 ufss-0.1.3/ufss/HLG/eigen_generator.py
+-rw-r--r--   0 prose      (501) staff       (20)    38460 2020-08-03 02:16:52.000000 ufss-0.1.3/ufss/HLG/eigenstates.py
+-rw-r--r--   0 prose      (501) staff       (20)     1938 2021-04-13 19:36:27.000000 ufss-0.1.3/ufss/HLG/general_Liouvillian_classes.py
+-rw-r--r--   0 prose      (501) staff       (20)    11205 2021-02-09 01:00:24.000000 ufss-0.1.3/ufss/HLG/manual_L_input.py
+-rw-r--r--   0 prose      (501) staff       (20)     3241 2021-03-16 17:24:44.000000 ufss-0.1.3/ufss/HLG/params_converter.py
+-rw-r--r--   0 prose      (501) staff       (20)     2076 2021-03-17 19:39:52.000000 ufss-0.1.3/ufss/HLG/run_HLG.py
+-rw-r--r--   0 prose      (501) staff       (20)     4731 2020-08-03 02:16:52.000000 ufss-0.1.3/ufss/HLG/simple_eigen_generator.py
+drwxr-xr-x   0 prose      (501) staff       (20)        0 2023-07-13 18:02:22.000000 ufss-0.1.3/ufss/RKE/
+-rw-r--r--   0 prose      (501) staff       (20)    24787 2020-12-02 16:24:03.000000 ufss-0.1.3/ufss/RKE/RKE_core.py
+-rw-r--r--   0 prose      (501) staff       (20)    50190 2023-07-03 21:22:44.000000 ufss-0.1.3/ufss/RKE/RKE_open_core.py
+-rw-r--r--   0 prose      (501) staff       (20)       85 2020-11-30 15:31:51.000000 ufss-0.1.3/ufss/RKE/__init__.py
+drwxr-xr-x   0 prose      (501) staff       (20)        0 2023-07-13 18:02:22.000000 ufss-0.1.3/ufss/UF2/
+-rw-r--r--   0 prose      (501) staff       (20)    50040 2023-07-03 21:20:00.000000 ufss-0.1.3/ufss/UF2/UF2_core.py
+-rw-r--r--   0 prose      (501) staff       (20)    71574 2023-07-03 21:25:11.000000 ufss-0.1.3/ufss/UF2/UF2_open_core.py
+-rw-r--r--   0 prose      (501) staff       (20)      127 2020-11-30 15:26:38.000000 ufss-0.1.3/ufss/UF2/__init__.py
+-rw-r--r--   0 prose      (501) staff       (20)     3966 2020-08-18 01:44:14.000000 ufss-0.1.3/ufss/UF2/heaviside_convolve.py
+-rw-r--r--   0 prose      (501) staff       (20)      401 2021-05-04 00:32:01.000000 ufss-0.1.3/ufss/__init__.py
+-rw-r--r--   0 prose      (501) staff       (20)     4837 2021-05-28 14:17:36.000000 ufss-0.1.3/ufss/convergence_tester.py
+-rw-r--r--   0 prose      (501) staff       (20)    17348 2023-01-27 14:53:52.000000 ufss-0.1.3/ufss/diagram_automation.py
+-rw-r--r--   0 prose      (501) staff       (20)     4969 2020-08-03 02:16:52.000000 ufss-0.1.3/ufss/dipole_pruning.py
+-rw-r--r--   0 prose      (501) staff       (20)     1274 2020-11-25 15:52:42.000000 ufss-0.1.3/ufss/efield_shapes.py
+drwxr-xr-x   0 prose      (501) staff       (20)        0 2023-07-13 18:02:22.000000 ufss-0.1.3/ufss/signals/
+-rw-r--r--   0 prose      (501) staff       (20)      145 2020-08-03 02:16:52.000000 ufss-0.1.3/ufss/signals/__init__.py
+-rw-r--r--   0 prose      (501) staff       (20)     4684 2022-03-08 22:08:00.000000 ufss-0.1.3/ufss/signals/isotropic_averaging.py
+-rw-r--r--   0 prose      (501) staff       (20)    14493 2021-06-08 17:22:29.000000 ufss-0.1.3/ufss/signals/plotting_tools.py
+-rw-r--r--   0 prose      (501) staff       (20)     5251 2020-08-03 02:16:52.000000 ufss-0.1.3/ufss/signals/signal_processing.py
+drwxr-xr-x   0 prose      (501) staff       (20)        0 2023-07-13 18:02:22.000000 ufss-0.1.3/ufss.egg-info/
+-rw-r--r--   0 prose      (501) staff       (20)     3871 2023-07-13 18:02:22.000000 ufss-0.1.3/ufss.egg-info/PKG-INFO
+-rw-r--r--   0 prose      (501) staff       (20)     1173 2023-07-13 18:02:22.000000 ufss-0.1.3/ufss.egg-info/SOURCES.txt
+-rw-r--r--   0 prose      (501) staff       (20)        1 2023-07-13 18:02:22.000000 ufss-0.1.3/ufss.egg-info/dependency_links.txt
+-rw-r--r--   0 prose      (501) staff       (20)       44 2023-07-13 18:02:22.000000 ufss-0.1.3/ufss.egg-info/requires.txt
+-rw-r--r--   0 prose      (501) staff       (20)       11 2023-07-13 18:02:22.000000 ufss-0.1.3/ufss.egg-info/top_level.txt
```

### Comparing `ufss-0.1.2/LICENSE` & `ufss-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ufss-0.1.2/PKG-INFO` & `ufss-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ufss
-Version: 0.1.2
+Version: 0.1.3
 Summary: Package for simulating nonlinear optical spectra
 Home-page: https://github.com/peterarose/ufss/
 Author: Peter A. Rose and Jacob J. Krich
 Author-email: peter.rose56@gmail.com
-Keywords: n,o,n,l,i,n,e,a,r, ,o,p,t,i,c,a,l, ,s,p,e,c,t,r,o,s,c,o,p,y
+Keywords: nonlinear optical spectroscopy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `ufss-0.1.2/README.md` & `ufss-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ufss-0.1.2/setup.py` & `ufss-0.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
     
 setup(
     name='ufss',
 
-    version='0.1.2',
+    version='0.1.3',
 
     description='Package for simulating nonlinear optical spectra',
 
     long_description=long_description,
 
     long_description_content_type='text/markdown',
```

### Comparing `ufss-0.1.2/tests/integration/test_UF2_vs_RKE.py` & `ufss-0.1.3/tests/integration/test_UF2_vs_RKE.py`

 * *Files identical despite different names*

### Comparing `ufss-0.1.2/tests/integration/test_linear_absorption.py` & `ufss-0.1.3/tests/integration/test_linear_absorption.py`

 * *Files identical despite different names*

### Comparing `ufss-0.1.2/tests/integration/test_uf2.py` & `ufss-0.1.3/tests/integration/test_uf2.py`

 * *Files identical despite different names*

### Comparing `ufss-0.1.2/tests/integration/test_vs_matlab_code.py` & `ufss-0.1.3/tests/integration/test_vs_matlab_code.py`

 * *Files identical despite different names*

### Comparing `ufss-0.1.2/ufss/HLG/DiabaticLindblad_Liouvillians.py` & `ufss-0.1.3/ufss/HLG/DiabaticLindblad_Liouvillians.py`

 * *Files identical despite different names*

### Comparing `ufss-0.1.2/ufss/HLG/Hamiltonians.py` & `ufss-0.1.3/ufss/HLG/Hamiltonians.py`

 * *Files identical despite different names*

### Comparing `ufss-0.1.2/ufss/HLG/Redfield_Liouvillians.py` & `ufss-0.1.3/ufss/HLG/Redfield_Liouvillians.py`

 * *Files identical despite different names*

### Comparing `ufss-0.1.2/ufss/HLG/__init__.py` & `ufss-0.1.3/ufss/HLG/__init__.py`

 * *Files identical despite different names*

### Comparing `ufss-0.1.2/ufss/HLG/base_class.py` & `ufss-0.1.3/ufss/HLG/base_class.py`

 * *Files identical despite different names*

### Comparing `ufss-0.1.2/ufss/HLG/dipole_operator.py` & `ufss-0.1.3/ufss/HLG/dipole_operator.py`

 * *Files identical despite different names*

### Comparing `ufss-0.1.2/ufss/HLG/eigen_generator.py` & `ufss-0.1.3/ufss/HLG/eigen_generator.py`

 * *Files identical despite different names*

### Comparing `ufss-0.1.2/ufss/HLG/eigenstates.py` & `ufss-0.1.3/ufss/HLG/eigenstates.py`

 * *Files identical despite different names*

### Comparing `ufss-0.1.2/ufss/HLG/general_Liouvillian_classes.py` & `ufss-0.1.3/ufss/HLG/general_Liouvillian_classes.py`

 * *Files identical despite different names*

### Comparing `ufss-0.1.2/ufss/HLG/manual_L_input.py` & `ufss-0.1.3/ufss/HLG/manual_L_input.py`

 * *Files identical despite different names*

### Comparing `ufss-0.1.2/ufss/HLG/params_converter.py` & `ufss-0.1.3/ufss/HLG/params_converter.py`

 * *Files identical despite different names*

### Comparing `ufss-0.1.2/ufss/HLG/run_HLG.py` & `ufss-0.1.3/ufss/HLG/run_HLG.py`

 * *Files identical despite different names*

### Comparing `ufss-0.1.2/ufss/HLG/simple_eigen_generator.py` & `ufss-0.1.3/ufss/HLG/simple_eigen_generator.py`

 * *Files identical despite different names*

### Comparing `ufss-0.1.2/ufss/RKE/RKE_core.py` & `ufss-0.1.3/ufss/RKE/RKE_core.py`

 * *Files identical despite different names*

### Comparing `ufss-0.1.2/ufss/RKE/RKE_open_core.py` & `ufss-0.1.3/ufss/RKE/RKE_open_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,14 +240,15 @@
             self.rho_to_signal = self.polarization_detection_rho_to_signal
             self.return_complex_signal = True
             detection_type = 'polarization'
             
         elif detection_type == 'integrated_polarization':
             raise Exception('detection_type: Integrated polarization is not implemented for Open RKE')
             self.rho_to_signal = self.integrated_polarization_detection_rho_to_signal
+            self.return_complex_signal = False
             
         elif detection_type == 'fluorescence':
             self.rho_to_signal = self.fluorescence_detection_rho_to_signal
 
         DiagramGenerator.__init__(self,detection_type=detection_type)
         self.KB_dict = {'Bu':self.bra_up,'Ku':self.ket_up,'Kd':self.ket_down,'Bd':self.bra_down}
 
@@ -1296,27 +1297,30 @@
 
         P_of_w = fftshift(ifft(ifftshift(P_of_t)))*len(P_of_t)*dt#/np.sqrt(2*np.pi)
 
         signal = P_of_w * np.conjugate(efield)
         if not self.return_complex_signal:
             return np.imag(signal)
         else:
-            return 1j*signal
+            return -1j*signal
 
     def integrated_polarization_to_signal(self,P,*,
                                 local_oscillator_number = -1):
         """This function generates a frequency-resolved signal from a polarization field
            local_oscillator_number - usually the local oscillator will be the last pulse 
                                      in the list self.efields"""
         efield_t = self.efield_times[local_oscillator_number]
 
         efield = self.efields[local_oscillator_number]
 
         signal = np.trapz(P * np.conjugate(efield),x=efield_t)
-        return np.imag(signal)
+        if not self.return_complex_signal:
+            return np.imag(signal)
+        else:
+            return -1j*signal
 
     def save(self,file_name,pulse_delay_names,*,use_base_path=True):
         if use_base_path:
             file_name = os.path.join(self.base_path,file_name)
         save_dict = {}
         for name,delays in zip(pulse_delay_names,self.all_pulse_delays):
             save_dict[name] = delays
```

### Comparing `ufss-0.1.2/ufss/UF2/UF2_core.py` & `ufss-0.1.3/ufss/UF2/UF2_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,14 +162,15 @@
         elif detection_type == 'complex_polarization':
             self.psi_to_signal = self.polarization_detection_signal
             self.return_complex_signal = True
             detection_type = 'polarization'
             
         elif detection_type == 'integrated_polarization':
             self.psi_to_signal = self.integrated_polarization_detection_signal
+            self.return_complex_signal = False
             
         elif detection_type == 'fluorescence':
             self.psi_to_signal = self.fluorescence_detection_signal
             self.f_yield = f_yield #quantum yield of doubly excited manifold relative to singly excited manifold
 
         DiagramGenerator.__init__(self,detection_type=detection_type)
         self.K_dict = {'u':self.up,'d':self.down}
@@ -1157,28 +1158,31 @@
 
         P_of_w = fftshift(ifft(ifftshift(P_of_t)))*P_of_t.size*dt
 
         signal = P_of_w * np.conjugate(efield)
         if not self.return_complex_signal:
             return np.imag(signal)
         else:
-            return 1j*signal
+            return -1j*signal
 
     def integrated_polarization_to_signal(self,P,*,
                                 local_oscillator_number = -1):
         """This function generates a frequency-resolved signal from a polarization field
            local_oscillator_number - usually the local oscillator will be the last pulse 
                                      in the list self.efields"""
         efield_t = self.efield_times[local_oscillator_number]
 
         efield = self.efields[local_oscillator_number]
 
         # signal = np.trapz(P * np.conjugate(efield),x=efield_t)
         signal = np.sum(P * np.conjugate(efield))*(efield_t[1] - efield_t[0])
-        return np.imag(signal)
+        if not self.return_complex_signal:
+            return np.imag(signal)
+        else:
+            return -1j*signal
 
     def add_gaussian_linewidth(self,sigma):
         try:
             old_signal = self.old_signal
         except AttributeError:
             self.old_signal = self.signal.copy()
             old_signal = self.old_signal
```

### Comparing `ufss-0.1.2/ufss/UF2/UF2_open_core.py` & `ufss-0.1.3/ufss/UF2/UF2_open_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1178,15 +1178,14 @@
         try:
             ev1 = self.eigenvalues['all_manifolds']
             ev2 = self.eigenvalues['all_manifolds']
         except KeyError:
             ev1 = self.eigenvalues[old_manifold_key]
             ev2 = self.eigenvalues[new_manifold_key]
 
-        print(m_nonzero)
         exp_factor1 = np.exp( (ev1[m_nonzero,np.newaxis] - 1j*center)*t[np.newaxis,:])
         
         rho = rho_in(t) * exp_factor1
 
         if self.conserve_memory:
             # move back to the basis the Liouvillian was written in
             if 'all_manifolds' in self.manifolds:
@@ -1754,30 +1753,30 @@
 
         P_of_w = fftshift(ifft(ifftshift(P_of_t)))*P_of_t.size*dt
 
         signal = P_of_w * np.conjugate(efield)
         if not self.return_complex_signal:
             return np.imag(signal)
         else:
-            return 1j*signal
+            return -1j*signal
 
     def integrated_polarization_to_signal(self,P,*,
                                 local_oscillator_number = -1):
         """This function generates a frequency-resolved signal from a polarization field
            local_oscillator_number - usually the local oscillator will be the last pulse 
                                      in the list self.efields"""
         efield_t = self.efield_times[local_oscillator_number]
 
         efield = self.efields[local_oscillator_number]
 
         signal = np.trapz(P * np.conjugate(efield),x=efield_t)
         if not self.return_complex_signal:
             return np.imag(signal)
         else:
-            return 1j*signal
+            return -1j*signal
 
     def add_gaussian_linewidth(self,sigma):
         self.old_signal = self.signal.copy()
 
         sig_tau_t = fftshift(fft(ifftshift(self.old_signal,axes=(-1)),axis=-1),axes=(-1))
         sig_tau_t = sig_tau_t * (np.exp(-self.t**2/(2*sigma**2))[np.newaxis,np.newaxis,:]
                                  *np.exp(-self.t21_array**2/(2*sigma**2))[:,np.newaxis,np.newaxis])
```

### Comparing `ufss-0.1.2/ufss/UF2/heaviside_convolve.py` & `ufss-0.1.3/ufss/UF2/heaviside_convolve.py`

 * *Files identical despite different names*

### Comparing `ufss-0.1.2/ufss/convergence_tester.py` & `ufss-0.1.3/ufss/convergence_tester.py`

 * *Files identical despite different names*

### Comparing `ufss-0.1.2/ufss/diagram_automation.py` & `ufss-0.1.3/ufss/diagram_automation.py`

 * *Files identical despite different names*

### Comparing `ufss-0.1.2/ufss/dipole_pruning.py` & `ufss-0.1.3/ufss/dipole_pruning.py`

 * *Files identical despite different names*

### Comparing `ufss-0.1.2/ufss/efield_shapes.py` & `ufss-0.1.3/ufss/efield_shapes.py`

 * *Files identical despite different names*

### Comparing `ufss-0.1.2/ufss/signals/isotropic_averaging.py` & `ufss-0.1.3/ufss/signals/isotropic_averaging.py`

 * *Files identical despite different names*

### Comparing `ufss-0.1.2/ufss/signals/plotting_tools.py` & `ufss-0.1.3/ufss/signals/plotting_tools.py`

 * *Files identical despite different names*

### Comparing `ufss-0.1.2/ufss/signals/signal_processing.py` & `ufss-0.1.3/ufss/signals/signal_processing.py`

 * *Files identical despite different names*

### Comparing `ufss-0.1.2/ufss.egg-info/PKG-INFO` & `ufss-0.1.3/ufss.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ufss
-Version: 0.1.2
+Version: 0.1.3
 Summary: Package for simulating nonlinear optical spectra
 Home-page: https://github.com/peterarose/ufss/
 Author: Peter A. Rose and Jacob J. Krich
 Author-email: peter.rose56@gmail.com
-Keywords: n,o,n,l,i,n,e,a,r, ,o,p,t,i,c,a,l, ,s,p,e,c,t,r,o,s,c,o,p,y
+Keywords: nonlinear optical spectroscopy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `ufss-0.1.2/ufss.egg-info/SOURCES.txt` & `ufss-0.1.3/ufss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

