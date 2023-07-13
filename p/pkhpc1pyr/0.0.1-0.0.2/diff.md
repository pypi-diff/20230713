# Comparing `tmp/pkhpc1pyr-0.0.1.tar.gz` & `tmp/pkhpc1pyr-0.0.2.tar.gz`

## Comparing `pkhpc1pyr-0.0.1.tar` & `pkhpc1pyr-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,22 @@
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.1/requirements.txt
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.1/src/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.1/src/pkhpc1pyr/P2L1.py
--rw-r--r--   0        0        0     7208 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.1/src/pkhpc1pyr/P2L2.py
--rw-r--r--   0        0        0     7994 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.1/src/pkhpc1pyr/P2L3.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.1/src/pkhpc1pyr/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.1/src/pkhpc1pyr/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.1/src/pkhpc1pyr/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.1/src/pkhpc1pyr/tests/TestP2L1.py
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.1/src/pkhpc1pyr/tests/TestP2L2.py
--rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.1/src/pkhpc1pyr/tests/TestP2L3.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.1/src/pkhpc1pyr/tests/__init__.py
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.1/src/pkhpc1pyr/utils/P2L1Err.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.1/src/pkhpc1pyr/utils/P2L1Plot.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.1/src/pkhpc1pyr/utils/P2L2Err.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.1/src/pkhpc1pyr/utils/P2L2Plot.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.1/src/pkhpc1pyr/utils/P2L3Err.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.1/src/pkhpc1pyr/utils/P2L3Plot.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.1/src/pkhpc1pyr/utils/__init__.py
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.1/src/pkhpc1pyr/utils/helperFunctions.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.1/LICENSE
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.1/README.md
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/requirements.txt
+-rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/P2L1.py
+-rw-r--r--   0        0        0     7208 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/P2L2.py
+-rw-r--r--   0        0        0     7994 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/P2L3.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/__init__.py
+-rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/tests/TestP2L1.py
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/tests/TestP2L2.py
+-rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/tests/TestP2L3.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/tests/__init__.py
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/utils/P2L1Err.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/utils/P2L1Plot.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/utils/P2L2Err.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/utils/P2L2Plot.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/utils/P2L3Err.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/utils/P2L3Plot.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/utils/__init__.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/src/pkhpc1pyr/utils/helperFunctions.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/README.md
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 pkhpc1pyr-0.0.2/PKG-INFO
```

### Comparing `pkhpc1pyr-0.0.1/src/pkhpc1pyr/P2L1.py` & `pkhpc1pyr-0.0.2/src/pkhpc1pyr/P2L1.py`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.1/src/pkhpc1pyr/P2L2.py` & `pkhpc1pyr-0.0.2/src/pkhpc1pyr/P2L2.py`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.1/src/pkhpc1pyr/P2L3.py` & `pkhpc1pyr-0.0.2/src/pkhpc1pyr/P2L3.py`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.1/src/pkhpc1pyr/tests/TestP2L1.py` & `pkhpc1pyr-0.0.2/src/pkhpc1pyr/tests/TestP2L1.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
 
     # Check for user entered parameters
     if parms == None:
         parms = [.05] # This is Kpl only
     else:
         np.array(parms)
-    Mxy, Mz = P2L1.P2L1(parms, fdv)
+    Mxy, Mz = P2L1(parms, fdv)
     fdv['data'] = Mxy 
 
     ### Create a fit for the generated data ###
     guess = [.01]
     LB = 0
     UB = np.Inf
 
@@ -92,13 +92,13 @@
         bounds = (LB, UB)
     )
 
     popt = fit['x']
     resid = fit['fun']
 
     ### Plot the fits ###
-    fig = P2L1Plot.plot(resid, popt, fdv)
+    fig = P2L1Plot.P2L1Plot(resid, popt, fdv)
 
     return fig
 
 if __name__ == '__main__':
-    TestP2L1()
+    TestP2L1()
```

### Comparing `pkhpc1pyr-0.0.1/src/pkhpc1pyr/tests/TestP2L2.py` & `pkhpc1pyr-0.0.2/src/pkhpc1pyr/tests/TestP2L2.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     fdv['data'] = np.ones( (2, fdv['NFlips']) )
 
     # Generate synthetic data
     if parms == None:
         parms = np.array( [0.1, 1000] )
     else:
         parms = np.array( parms )
-    EV, IV, vb, Mzev, Mziv = P2L2.P2L2(parms, fdv) 
+    EV, IV, vb, Mzev, Mziv = P2L2(parms, fdv) 
     fdv['data'] = IV*vb + EV*(1-vb)
 
     ### Create a fit for the generated data and try to recover parameters above ###
     LB = [0, 0]
     UB = [1, np.Inf]
     guess = (parms*10) * np.random.rand(2)
 
@@ -103,15 +103,15 @@
         bounds = (LB, UB)
     )
 
     popt = fit['x']
     resid = fit['fun']
 
     ### Plot the fits ###
-    fig = P2L2Plot.plot(resid, popt, fdv)
+    fig = P2L2Plot.P2L2Plot(resid, popt, fdv)
 
     return fig
 
 
 if __name__ == '__main__':
     TestP2L2()
```

### Comparing `pkhpc1pyr-0.0.1/src/pkhpc1pyr/tests/TestP2L3.py` & `pkhpc1pyr-0.0.2/src/pkhpc1pyr/tests/TestP2L3.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     fdv['data'] = np.ones( (2, fdv['ntp']) )
 
     # Generate synthetic data
     if parms == None:
         parms = np.array( [0.1, 1000] )
     else:
         parms = np.array(parms)
-    EV, IV, vols, Mzev, Mziv = P2L3.P2L3(parms, fdv)
+    EV, IV, vols, Mzev, Mziv = P2L3(parms, fdv)
     fdv['data'] = IV[0:2]*vols[0] + EV[0:2]*vols[1] + EV[2:4]*vols[2]
 
     ### Create a fit for the generated data and try to recover parameters above ###
     LB = [0,0]
     UB = [1, np.Inf]
     guess = (parms*10) * np.random.rand(2)
 
@@ -108,14 +108,14 @@
         bounds = (LB, UB)
     )
 
     popt = fit['x']
     resid = fit['fun']
 
     ### Plot the fits ###
-    fig = P2L3Plot.plot(resid, popt, fdv)
+    fig = P2L3Plot.P2L3Plot(resid, popt, fdv)
 
     return fig
 
 
 if __name__ == '__main__':
-    TestP2L3()
+    TestP2L3()
```

### Comparing `pkhpc1pyr-0.0.1/src/pkhpc1pyr/utils/P2L1Err.py` & `pkhpc1pyr-0.0.2/src/pkhpc1pyr/utils/P2L1Err.py`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.1/src/pkhpc1pyr/utils/P2L1Plot.py` & `pkhpc1pyr-0.0.2/src/pkhpc1pyr/utils/P2L1Plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import matplotlib.pyplot as plt
 import numpy as np
 
 from .. import P2L1
 
-def plot(resid, parms, fdv):
+def P2L1Plot(resid, parms, fdv):
     '''
     A function to plot the result of TestP2L1.py
 
     The customizability of this function is fairly limited without editing.
 
     L2Norm is defined as the norm of the vector residuals array.
     '''
@@ -40,8 +40,8 @@
     ax[1].set_ylabel('Mxy')
     ax[1].grid()
     ax[1].set_xlabel('Time (s)', fontsize = 'x-large')
 
     plt.subplots_adjust(hspace = .5)
     plt.show() 
 
-    return fig
+    return fig
```

### Comparing `pkhpc1pyr-0.0.1/src/pkhpc1pyr/utils/P2L2Err.py` & `pkhpc1pyr-0.0.2/src/pkhpc1pyr/utils/P2L2Err.py`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.1/src/pkhpc1pyr/utils/P2L2Plot.py` & `pkhpc1pyr-0.0.2/src/pkhpc1pyr/utils/P2L2Plot.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import matplotlib.pyplot as plt
 import numpy as np
 from .. import P2L2
 
-def plot(resid, parms, fdv):
+def P2L2Plot(resid, parms, fdv):
     '''
     A function to plot the result of TestP2L1.py
 
     The customizability of this function is fairly limited without editing.
 
     L2Norm is defined as the norm of the vector residuals array.
     '''
@@ -41,8 +41,8 @@
     ax[1].set_xlabel('Time (s)')
     ax[1].grid()
     ax[1].set_ylabel('Mxy')
 
     plt.subplots_adjust(hspace = .5)
     plt.show()
 
-    return fig
+    return fig
```

### Comparing `pkhpc1pyr-0.0.1/src/pkhpc1pyr/utils/P2L3Err.py` & `pkhpc1pyr-0.0.2/src/pkhpc1pyr/utils/P2L3Err.py`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.1/src/pkhpc1pyr/utils/P2L3Plot.py` & `pkhpc1pyr-0.0.2/src/pkhpc1pyr/utils/P2L3Plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import matplotlib.pyplot as plt
 import numpy as np
 from .. import P2L3
 
 
-def plot(resid, parms, fdv):
+def P2L3Plot(resid, parms, fdv):
     '''
     A function to plot the result of TestP2L1.py
 
     The customizability of this function is fairly limited without editing.
 
     L2Norm is defined as the norm of the vector residuals array.
     '''
@@ -46,8 +46,8 @@
     ax[1].grid()
     ax[1].legend()
     ax[1].set_ylabel('Mxy')
 
     plt.subplots_adjust(hspace = .5)
     plt.show()
 
-    return fig
+    return fig
```

### Comparing `pkhpc1pyr-0.0.1/src/pkhpc1pyr/utils/helperFunctions.py` & `pkhpc1pyr-0.0.2/src/pkhpc1pyr/utils/helperFunctions.py`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.1/LICENSE` & `pkhpc1pyr-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pkhpc1pyr-0.0.1/pyproject.toml` & `pkhpc1pyr-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pkhpc1pyr"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Ryan Boyce", email="ryty.boyce@gmail.com" },
 ]
 description = "Scripts and functions for the pharmacokinetic modeling of hyperpolarized [1-13C]-pyruvate."
 readme = "README.md"
 requires-python = "~=3.10"
 classifiers = [
@@ -31,8 +31,8 @@
   "pytz~=2023.3",
   "scipy~=1.10.1",
   "six~=1.16.0",
   "tzdata~=2023.3"
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/RytyB/HP-C1Pyr-PK-Python"
+"Homepage" = "https://github.com/RytyB/HP-C1Pyr-PK-Python"
```

### Comparing `pkhpc1pyr-0.0.1/PKG-INFO` & `pkhpc1pyr-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkhpc1pyr
-Version: 0.0.1
+Version: 0.0.2
 Summary: Scripts and functions for the pharmacokinetic modeling of hyperpolarized [1-13C]-pyruvate.
 Project-URL: Homepage, https://github.com/RytyB/HP-C1Pyr-PK-Python
 Author-email: Ryan Boyce <ryty.boyce@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -22,38 +22,70 @@
 Requires-Dist: python-dateutil~=2.8.2
 Requires-Dist: pytz~=2023.3
 Requires-Dist: scipy~=1.10.1
 Requires-Dist: six~=1.16.0
 Requires-Dist: tzdata~=2023.3
 Description-Content-Type: text/markdown
 
+<h1> HP C1-Pyruvate Pharmacokinetic Modeling Package for Python </h1>
+
+<h2>
+Purpose
+</h2>
+
 <ul>
-Python code for pharmacokinetic modeling of hyperpolarized [1-13C]-pyruvate.
+This package was meant to create a more user friendly, open source version of the MATLAB developed by the MD Anderson Magnetic Resonance Engineering Laboratory.
+The original repository is available at https://github.com/mda-mrsl/HP-C1Pyr-PK
 </ul>
 
 <ul>
 These scripts calculate the relationship between [1-13C]-pyruvate and [1-13C]-lactate, but can easily be extended to include other metabolites.
 </ul>
 
 <ul>
 There are three base models, of differing complexity, which include a different number of physical compartments:
 </ul>
 
 <ul>
-The scripts titled P2L3*.m describe signal evolution between two chemical pools and three physical compartments. The three-compartment model is the most physiologically accurate among these models, but it is also the most computationally intensive, requiring the largest number of descriptive parameters.
+The scripts titled P2L3*.py describe signal evolution between two chemical pools and three physical compartments. The three-compartment model is the most physiologically accurate among these models, but it is also the most computationally intensive, requiring the largest number of descriptive parameters.
 </ul>
 
 <ul>
-The scripts titled P2L2*.m are for the PK model with two chemical pools and two physical compartments. Here, HP pyruvate and lactate in the extravascular/extracellular space is assumed to be very well mixed with HP pyruvate in the intracellular space - and separate from pyr/lac in the vascular supply.
+The scripts titled P2L2*.py are for the PK model with two chemical pools and two physical compartments. Here, HP pyruvate and lactate in the extravascular/extracellular space is assumed to be very well mixed with HP pyruvate in the intracellular space - and separate from pyr/lac in the vascular supply.
 </ul>
 
 <ul>
-The scripts titled P2L1*.m represent a simple precursor-product model, which does not consider physical compartmentalization of imaging agents. Equivalently, this assumes that all compartments (vascular; extravascular/extracellular; and cellular) are well mixed.
+The scripts titled P2L1*.py represent a simple precursor-product model, which does not consider physical compartmentalization of imaging agents. Equivalently, this assumes that all compartments (vascular; extravascular/extracellular; and cellular) are well mixed.
 </ul>
 
 <ul>
-Each of these groups of scripts are also accompanied by a test script (TestP2L#.m) that shows how to work with these models - from setup and generation of synthetic data to PK analysis by fitting.
+Each script is accompanied by utilities and a test function which runs a model and plots the results for given parameters. 
+</ul>
+
+<h2> 
+Installation
+</h2>
+
+<ul> Running requires python version 3.10 or compatible </ul>
+
+<ul>
+Can be installed from Pypi repository with pip
+<br> <i> pip install pkhpc1pyr </i>
+<br> The required dependencies can be found in the file requirements.txt and installed with the command 
+<br> <i> pip install numpy==1.24.3 </i>
 </ul>
 
 <ul>
-Please do not hesitate to contact with any questions, comments, concerns, or suggestions for improvement: Ryan Boyce ryty.boyce@gmail.com
-</ul>
+The installation can be tested by calling the TestP2L* functions without any arguments. For example:
+<br> <i> import pkhpc1pyr as pk 
+<br> pk.tests.TestP2L3() </i>
+</ul>
+
+<h2> 
+Contact
+</h2>
+
+<ul>
+For questions about code or maintenance please contact Ryan Boyce <br> rboyce@mdanderson.org
+<br> For further questions about the original MATLAB repository please contact Dr. Jim Bankson <br> jbankson@mdanderson.org
+</ul>
+
```

