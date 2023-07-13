# Comparing `tmp/dLuxToliman-0.1.2.tar.gz` & `tmp/dLuxToliman-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dLuxToliman-0.1.2.tar", last modified: Mon May 29 09:10:40 2023, max compression
+gzip compressed data, was "dLuxToliman-0.1.3.tar", last modified: Thu Jul 13 04:50:18 2023, max compression
```

## Comparing `dLuxToliman-0.1.2.tar` & `dLuxToliman-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 mcha5804   (501) staff       (20)        0 2023-05-29 09:10:40.348376 dLuxToliman-0.1.2/
--rw-r--r--   0 mcha5804   (501) staff       (20)       93 2023-05-29 04:35:46.000000 dLuxToliman-0.1.2/.gitignore
--rw-r--r--   0 mcha5804   (501) staff       (20)     1498 2023-05-29 03:55:35.000000 dLuxToliman-0.1.2/LICENSE
--rw-r--r--   0 mcha5804   (501) staff       (20)     3110 2023-05-29 09:10:40.348238 dLuxToliman-0.1.2/PKG-INFO
--rw-r--r--   0 mcha5804   (501) staff       (20)     2620 2023-05-29 08:56:27.000000 dLuxToliman-0.1.2/README.md
-drwxr-xr-x   0 mcha5804   (501) staff       (20)        0 2023-05-29 09:10:40.347185 dLuxToliman-0.1.2/dLuxToliman/
--rw-r--r--   0 mcha5804   (501) staff       (20)      516 2023-05-29 09:03:03.000000 dLuxToliman-0.1.2/dLuxToliman/__init__.py
--rw-r--r--   0 mcha5804   (501) staff       (20) 16777344 2023-05-29 04:35:46.000000 dLuxToliman-0.1.2/dLuxToliman/diffractive_pupil.npy
--rw-r--r--   0 mcha5804   (501) staff       (20)     2636 2023-05-29 04:35:46.000000 dLuxToliman-0.1.2/dLuxToliman/gradient_energy.py
--rw-r--r--   0 mcha5804   (501) staff       (20)     1134 2023-05-29 04:35:46.000000 dLuxToliman-0.1.2/dLuxToliman/instruments.py
--rw-r--r--   0 mcha5804   (501) staff       (20)     6731 2023-05-29 04:35:46.000000 dLuxToliman-0.1.2/dLuxToliman/optical_layers.py
--rw-r--r--   0 mcha5804   (501) staff       (20)     8094 2023-05-29 06:12:39.000000 dLuxToliman-0.1.2/dLuxToliman/optics.py
--rw-r--r--   0 mcha5804   (501) staff       (20)     8140 2023-05-29 04:35:46.000000 dLuxToliman-0.1.2/dLuxToliman/sources.py
-drwxr-xr-x   0 mcha5804   (501) staff       (20)        0 2023-05-29 09:10:40.348066 dLuxToliman-0.1.2/dLuxToliman.egg-info/
--rw-r--r--   0 mcha5804   (501) staff       (20)     3110 2023-05-29 09:10:40.000000 dLuxToliman-0.1.2/dLuxToliman.egg-info/PKG-INFO
--rw-r--r--   0 mcha5804   (501) staff       (20)      434 2023-05-29 09:10:40.000000 dLuxToliman-0.1.2/dLuxToliman.egg-info/SOURCES.txt
--rw-r--r--   0 mcha5804   (501) staff       (20)        1 2023-05-29 09:10:40.000000 dLuxToliman-0.1.2/dLuxToliman.egg-info/dependency_links.txt
--rw-r--r--   0 mcha5804   (501) staff       (20)       11 2023-05-29 09:10:40.000000 dLuxToliman-0.1.2/dLuxToliman.egg-info/requires.txt
--rw-r--r--   0 mcha5804   (501) staff       (20)       12 2023-05-29 09:10:40.000000 dLuxToliman-0.1.2/dLuxToliman.egg-info/top_level.txt
--rw-r--r--   0 mcha5804   (501) staff       (20)      361 2023-05-29 09:03:03.000000 dLuxToliman-0.1.2/pyproject.toml
--rw-r--r--   0 mcha5804   (501) staff       (20)       11 2023-05-29 04:35:46.000000 dLuxToliman-0.1.2/requirements.txt
--rw-r--r--   0 mcha5804   (501) staff       (20)       38 2023-05-29 09:10:40.348438 dLuxToliman-0.1.2/setup.cfg
--rw-r--r--   0 mcha5804   (501) staff       (20)     1472 2023-05-29 04:35:46.000000 dLuxToliman-0.1.2/setup.py
+drwxr-xr-x   0 mcha5804   (501) staff       (20)        0 2023-07-13 04:50:18.024553 dLuxToliman-0.1.3/
+-rw-r--r--   0 mcha5804   (501) staff       (20)       93 2023-05-29 04:35:46.000000 dLuxToliman-0.1.3/.gitignore
+-rw-r--r--   0 mcha5804   (501) staff       (20)     1498 2023-05-29 03:55:35.000000 dLuxToliman-0.1.3/LICENSE
+-rw-r--r--   0 mcha5804   (501) staff       (20)     3232 2023-07-13 04:50:18.024396 dLuxToliman-0.1.3/PKG-INFO
+-rw-r--r--   0 mcha5804   (501) staff       (20)     2742 2023-07-13 04:26:03.000000 dLuxToliman-0.1.3/README.md
+drwxr-xr-x   0 mcha5804   (501) staff       (20)        0 2023-07-13 04:50:18.011849 dLuxToliman-0.1.3/assets/
+-rw-r--r--   0 mcha5804   (501) staff       (20)    20565 2023-05-29 23:40:33.000000 dLuxToliman-0.1.3/assets/basic_toliman_psf.jpg
+drwxr-xr-x   0 mcha5804   (501) staff       (20)        0 2023-07-13 04:50:18.023488 dLuxToliman-0.1.3/dLuxToliman/
+-rw-r--r--   0 mcha5804   (501) staff       (20)      515 2023-07-13 04:49:41.000000 dLuxToliman-0.1.3/dLuxToliman/__init__.py
+-rw-r--r--   0 mcha5804   (501) staff       (20) 16777344 2023-05-29 04:35:46.000000 dLuxToliman-0.1.3/dLuxToliman/diffractive_pupil.npy
+-rw-r--r--   0 mcha5804   (501) staff       (20)     2598 2023-07-13 04:26:03.000000 dLuxToliman-0.1.3/dLuxToliman/gradient_energy.py
+-rw-r--r--   0 mcha5804   (501) staff       (20)     1044 2023-07-13 04:26:03.000000 dLuxToliman-0.1.3/dLuxToliman/instruments.py
+-rw-r--r--   0 mcha5804   (501) staff       (20)     6751 2023-07-13 04:26:03.000000 dLuxToliman-0.1.3/dLuxToliman/optical_layers.py
+-rw-r--r--   0 mcha5804   (501) staff       (20)     8198 2023-07-13 04:26:03.000000 dLuxToliman-0.1.3/dLuxToliman/optics.py
+-rw-r--r--   0 mcha5804   (501) staff       (20)     9556 2023-07-13 04:42:31.000000 dLuxToliman-0.1.3/dLuxToliman/sources.py
+drwxr-xr-x   0 mcha5804   (501) staff       (20)        0 2023-07-13 04:50:18.024176 dLuxToliman-0.1.3/dLuxToliman.egg-info/
+-rw-r--r--   0 mcha5804   (501) staff       (20)     3232 2023-07-13 04:50:17.000000 dLuxToliman-0.1.3/dLuxToliman.egg-info/PKG-INFO
+-rw-r--r--   0 mcha5804   (501) staff       (20)      463 2023-07-13 04:50:17.000000 dLuxToliman-0.1.3/dLuxToliman.egg-info/SOURCES.txt
+-rw-r--r--   0 mcha5804   (501) staff       (20)        1 2023-07-13 04:50:17.000000 dLuxToliman-0.1.3/dLuxToliman.egg-info/dependency_links.txt
+-rw-r--r--   0 mcha5804   (501) staff       (20)       13 2023-07-13 04:50:17.000000 dLuxToliman-0.1.3/dLuxToliman.egg-info/requires.txt
+-rw-r--r--   0 mcha5804   (501) staff       (20)       12 2023-07-13 04:50:17.000000 dLuxToliman-0.1.3/dLuxToliman.egg-info/top_level.txt
+-rw-r--r--   0 mcha5804   (501) staff       (20)      361 2023-07-13 04:49:41.000000 dLuxToliman-0.1.3/pyproject.toml
+-rw-r--r--   0 mcha5804   (501) staff       (20)       13 2023-06-16 01:08:49.000000 dLuxToliman-0.1.3/requirements.txt
+-rw-r--r--   0 mcha5804   (501) staff       (20)       38 2023-07-13 04:50:18.024604 dLuxToliman-0.1.3/setup.cfg
+-rw-r--r--   0 mcha5804   (501) staff       (20)     2603 2023-06-06 00:49:10.000000 dLuxToliman-0.1.3/setup.py
```

### Comparing `dLuxToliman-0.1.2/LICENSE` & `dLuxToliman-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dLuxToliman-0.1.2/PKG-INFO` & `dLuxToliman-0.1.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,23 @@
-Metadata-Version: 2.1
-Name: dLuxToliman
-Version: 0.1.2
-Summary: A repo to hold the canonical dLux Toliman models.
-Home-page: https://github.com/maxecharles/dLuxToliman
-Author: Max Charles
-Author-email: max.charles@sydney.edu.au
-Project-URL: Bug Tracker, https://github.com/maxecharles/dLuxToliman/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7,<4.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # dLuxToliman
 
 [![PyPI version](https://badge.fury.io/py/dLuxToliman.svg)](https://badge.fury.io/py/dLuxToliman)
 [![License](https://img.shields.io/badge/license-BSD%203--Clause-blue.svg)](LICENSE)
 
 ## Description
+This repository/package contains pre-built ∂Lux models of the Toliman optical system, and pre-built parametrised ∂Lux source objects for Alpha Centauri.
 
 [∂Lux](https://louisdesdoigts.github.io/dLux/) is an open-source differentiable optical modelling framework harnessing the structural isomorphism between optical systems and neural networks, giving forwards models of optical system as a _parametric neural network_.
 ∂Lux is built in [Zodiax](https://github.com/LouisDesdoigts/zodiax) which is an open-source object-oriented [Jax](https://github.com/google/jax) framework built as an extension of [Equinox](https://github.com/patrick-kidger/equinox) for scientific programming.
 
 The primary goal of the Toliman mission is to discover Earth-sized exoplanets orbiting in Alpha Centauri, the closest star system to our own.
 To achieve this, the mission will employ a novel telescope design that will be able to detect subtle changes in the positions of the Alpha Centauri binary pair.
 These changes are caused by the gravitational reflex motion induced by an Earth-sized companion, and this cutting-edge technology will enable scientists to identify exoplanets too small to be detected by conventional telescopes.
 Toliman utilises a binary phase diffraction pupil to grasp the expected microarcsecond-scale astrometric signal.
 
-**This repository/package contains pre-built ∂Lux models of the Toliman optical system**, and pre-built parametrised ∂Lux source objects for Alpha Centauri.
-
 ## Installation
 
 `dLuxToliman` is pip-installable. To install the latest release, simply run:
 
 ```bash
 pip install dLuxToliman
 ```
@@ -43,24 +28,27 @@
 
 ```python
 # imports
 import dLuxToliman as dlT
 from matplotlib import pyplot as plt
 
 osys = dlT.TolimanOptics(psf_npixels=128, psf_oversample=1)  # creating Toliman optical system
-source = dlT.AlphaCen(nwavels=3, separation=8, position_angle=30)  # creating Alpha Centauri source
+source = dlT.AlphaCen(n_wavels=3, separation=8, position_angle=30)  # creating Alpha Centauri source
 psf = osys.model(source)  # running optical simulation
 
 # plotting
-plt.imshow(psf**.5, cmap = 'inferno')
+plt.imshow(psf ** .5, cmap='inferno')
 plt.title('Toliman $\sqrt{PSF}$')
 plt.show()
 ```
 
-The above code generates the PSF for the Toliman optical system, with the Alpha Centauri source, and plots the PSF on a square root stretch.
+![Example Image](./assets/basic_toliman_psf.jpg)
+
+## Contributors
+[Max Charles](https://github.com/maxecharles), [Louis Desdoigts](https://github.com/LouisDesdoigts), [Benjamin Pope](https://github.com/benjaminpope), and [Peter Tuthill](https://github.com/ptuthill).
 
 ## License
 
 This package is released under the BSD 3-Clause License. See the [LICENSE](LICENSE) file for more information.
 
 ## Support
```

### Comparing `dLuxToliman-0.1.2/README.md` & `dLuxToliman-0.1.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,37 @@
+Metadata-Version: 2.1
+Name: dLuxToliman
+Version: 0.1.3
+Summary: A repo to hold the canonical dLux Toliman models.
+Home-page: https://github.com/maxecharles/dLuxToliman
+Author: Max Charles
+Author-email: max.charles@sydney.edu.au
+Project-URL: Bug Tracker, https://github.com/maxecharles/dLuxToliman/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7,<4.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # dLuxToliman
 
 [![PyPI version](https://badge.fury.io/py/dLuxToliman.svg)](https://badge.fury.io/py/dLuxToliman)
 [![License](https://img.shields.io/badge/license-BSD%203--Clause-blue.svg)](LICENSE)
 
 ## Description
+This repository/package contains pre-built ∂Lux models of the Toliman optical system, and pre-built parametrised ∂Lux source objects for Alpha Centauri.
 
 [∂Lux](https://louisdesdoigts.github.io/dLux/) is an open-source differentiable optical modelling framework harnessing the structural isomorphism between optical systems and neural networks, giving forwards models of optical system as a _parametric neural network_.
 ∂Lux is built in [Zodiax](https://github.com/LouisDesdoigts/zodiax) which is an open-source object-oriented [Jax](https://github.com/google/jax) framework built as an extension of [Equinox](https://github.com/patrick-kidger/equinox) for scientific programming.
 
 The primary goal of the Toliman mission is to discover Earth-sized exoplanets orbiting in Alpha Centauri, the closest star system to our own.
 To achieve this, the mission will employ a novel telescope design that will be able to detect subtle changes in the positions of the Alpha Centauri binary pair.
 These changes are caused by the gravitational reflex motion induced by an Earth-sized companion, and this cutting-edge technology will enable scientists to identify exoplanets too small to be detected by conventional telescopes.
 Toliman utilises a binary phase diffraction pupil to grasp the expected microarcsecond-scale astrometric signal.
 
-**This repository/package contains pre-built ∂Lux models of the Toliman optical system**, and pre-built parametrised ∂Lux source objects for Alpha Centauri.
-
 ## Installation
 
 `dLuxToliman` is pip-installable. To install the latest release, simply run:
 
 ```bash
 pip install dLuxToliman
 ```
@@ -29,24 +42,27 @@
 
 ```python
 # imports
 import dLuxToliman as dlT
 from matplotlib import pyplot as plt
 
 osys = dlT.TolimanOptics(psf_npixels=128, psf_oversample=1)  # creating Toliman optical system
-source = dlT.AlphaCen(nwavels=3, separation=8, position_angle=30)  # creating Alpha Centauri source
+source = dlT.AlphaCen(n_wavels=3, separation=8, position_angle=30)  # creating Alpha Centauri source
 psf = osys.model(source)  # running optical simulation
 
 # plotting
-plt.imshow(psf**.5, cmap = 'inferno')
+plt.imshow(psf ** .5, cmap='inferno')
 plt.title('Toliman $\sqrt{PSF}$')
 plt.show()
 ```
 
-The above code generates the PSF for the Toliman optical system, with the Alpha Centauri source, and plots the PSF on a square root stretch.
+![Example Image](./assets/basic_toliman_psf.jpg)
+
+## Contributors
+[Max Charles](https://github.com/maxecharles), [Louis Desdoigts](https://github.com/LouisDesdoigts), [Benjamin Pope](https://github.com/benjaminpope), and [Peter Tuthill](https://github.com/ptuthill).
 
 ## License
 
 This package is released under the BSD 3-Clause License. See the [LICENSE](LICENSE) file for more information.
 
 ## Support
```

### Comparing `dLuxToliman-0.1.2/dLuxToliman/__init__.py` & `dLuxToliman-0.1.3/dLuxToliman/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 name = "dLuxToliman"
-__version__ = "0.1.2"
-
+__version__ = "0.1.3"
 
 # Import as modules
 from . import optics
 from . import optical_layers
 from . import gradient_energy
 from . import instruments
 from . import sources
```

### Comparing `dLuxToliman-0.1.2/dLuxToliman/diffractive_pupil.npy` & `dLuxToliman-0.1.3/dLuxToliman/diffractive_pupil.npy`

 * *Files identical despite different names*

### Comparing `dLuxToliman-0.1.2/dLuxToliman/gradient_energy.py` & `dLuxToliman-0.1.3/dLuxToliman/gradient_energy.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,66 @@
 import jax.numpy as np
 from jax import Array
-import dLux
 import dLux.utils as dlu
 
 __all__ = ["get_GE", "get_RGE", "get_RWGE", "get_radial_mask"]
 
 
-def get_GE(array : Array) -> Array:
+def get_GE(array: Array) -> Array:
     """
-    Calcuates the spatial gradient energy of the array.
+    Calculates the spatial gradient energy of the array.
 
     Parameters
     ----------
     array : Array
-        The array to calcuate the gradient energy for.
+        The array to calculate the gradient energy for.
 
     Returns
     -------
     array : Array
         The array of gradient energies.
     """
     grads_vec = np.gradient(array)
     return np.hypot(grads_vec[0], grads_vec[1])
 
 
-def get_RGE(array : Array, epsilon : float = 1e-8) -> Array:
+def get_RGE(array: Array, epsilon: float = 1e-8) -> Array:  # TODO : Add epsilon
     """
-    Calcuates the spatial radial gradient energy of the array.
+    Calculates the spatial radial gradient energy of the array.
 
     Parameters
     ----------
     array : Array
-        The array to calcuate the radial gradient energy for.
+        The array to calculate the radial gradient energy for.
     epsilon : float
         A small value added to the radial values to help with gradient
         stability.
 
     Returns
     -------
     array : Array
         The array of radial gradient energies.
     """
     positions = dlu.pixel_coords(array.shape[0])
     grads_vec = np.gradient(array)
 
     xnorm = positions[1]*grads_vec[0]
     ynorm = positions[0]*grads_vec[1]
+
     return np.square(xnorm + ynorm)
 
 
-def get_RWGE(array : Array, epsilon : float = 1e-8) -> Array:
+def get_RWGE(array: Array, epsilon: float = 1e-8) -> Array:
     """
-    Calcuates the spatial radially weighted gradient energy of the array.
+    Calculates the spatial radially weighted gradient energy of the array.
 
     Parameters
     ----------
     array : Array
-        The array to calcuate the radially weighted gradient energy for.
+        The array to calculate the radially weighted gradient energy for.
     epsilon : float
         A small value added to the radially weighted values to help with
         gradient stability.
 
     Returns
     -------
     array : Array
@@ -70,33 +70,32 @@
     positions = dlu.pixel_coords(npix)
     radii = dlu.pixel_coords(npix, polar=True)[0]
     radii_norm = positions/(radii + epsilon)
     grads_vec = np.gradient(array)
 
     xnorm = radii_norm[1]*grads_vec[0]
     ynorm = radii_norm[0]*grads_vec[1]
+
     return np.square(xnorm + ynorm)
 
 
-def get_radial_mask(npixels : int,
-                    rmin    : Array,
-                    rmax    : Array) -> Array:
+def get_radial_mask(npixels: int, rmin: Array, rmax: Array) -> Array:
     """
-    Calcautes a binary radial mask, masking out radii below rmin, and above
+    Calculates a binary radial mask, masking out radii below rmin, and above
     rmax.
 
     Parameters
     ----------
     npixels : int
         The linear size of the array.
     rmin : Array
         The inner radius to mask out.
     rmax : Array
         The outer radius to mask out.
 
     Returns
     -------
     mask: Array
-        A mask with the the values below rmin and above rmax masked out.
+        A mask with the values below rmin and above rmax masked out.
     """
     radii = dlu.pixel_coords(npixels, polar=True)[0]
-    return np.asarray((radii < rmax) & (radii > rmin), dtype=float)
+    return np.asarray((radii < rmax) & (radii > rmin), dtype=float)
```

### Comparing `dLuxToliman-0.1.2/dLuxToliman/instruments.py` & `dLuxToliman-0.1.3/dLuxToliman/instruments.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 from __future__ import annotations
-import jax.numpy as np
-import dLux.utils as dlu
-from jax import Array, vmap
-import matplotlib.pyplot as plt
 import dLux
 
-
 __all__ = ["Toliman"]
 
 
 class Toliman(dLux.instruments.BaseInstrument):
-    source : None
-    optics : None
-    
+    source: None
+    optics: None
+
     def __init__(self, optics, source):
         self.optics = optics
         self.source = source
         super().__init__()
-    
+
     def __getattr__(self, key):
         for attribute in self.__dict__.values():
             if hasattr(attribute, key):
                 return getattr(attribute, key)
         # if key in self.sources.keys():
         #     return self.sources[key]
         raise AttributeError(f"{self.__class__.__name__} has no attribute "
-        f"{key}.")
-    
+                             f"{key}.")
+
     def normalise(self):
         return self.set('source', self.source.normalise())
-    
+
     def model(self):
         return self.optics.model(self.source)
 
     def full_model(self):
         return self.optics.full_model(self.source)
-    
-    def perturb(self, X, parameters):
+
+    def perturb(self, X, parameters):  # TODO : fix this
         for parameter, x in zip(parameters, X):
             self = self.add(parameter, x)
-        return self
+        return self
```

### Comparing `dLuxToliman-0.1.2/dLuxToliman/optical_layers.py` & `dLuxToliman-0.1.3/dLuxToliman/optical_layers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,55 +1,50 @@
 from __future__ import annotations
 import jax.numpy as np
-import dLux.utils as dlu
 from jax import Array, vmap
-import matplotlib.pyplot as plt
 import dLux
 
-
 __all__ = ["ApplyBasisCLIMB"]
 
+OpticalLayer = lambda: dLux.optical_layers.OpticalLayer
+BasisLayer = lambda: dLux.optical_layers.BasisLayer
 
-OpticalLayer = lambda : dLux.optical_layers.OpticalLayer
-BasisLayer = lambda : dLux.optical_layers.BasisLayer
-
-
+# TODO write this class
 class ApplyBasisCLIMB(BasisLayer()):
     """
     Adds an array of binary phase values to the input wavefront from a set of
     continuous basis vectors. This uses the CLIMB algorithm in order to
-    generate the binary values in a continous manner as described in the
+    generate the binary values in a continuous manner as described in the
     paper Wong et al. 2021. The basis vectors are taken as an Optical Path
     Difference (OPD), and applied to the phase of the wavefront. The ideal
     wavelength parameter described the wavelength that will have a perfect
     anti-phase relationship given by the Optical Path Difference.
 
-    Note: Many of the methods in the class still need doccumentation.
-    Note: This currently only outputs 256 pixel arrays and uses a 3x oversample,
+    TODO: Many of the methods in the class still need doccumentation.
+    TODO: This currently only outputs 256 pixel arrays and uses a 3x oversample,
     therefore requiring a 768 pixel basis array.
 
     Attributes
     ----------
     basis: Array
         Arrays holding the continous pre-calculated basis vectors.
     coefficients: Array
         The Array of coefficients to be applied to each basis vector.
     ideal_wavelength : Array
         The target wavelength at which a perfect anti-phase relationship is
         applied via the OPD.
     """
     # basis            : Array
     # coefficients     : Array
-    ideal_wavelength : Array
+    ideal_wavelength: Array
 
-
-    def __init__(self             : OpticalLayer(),
-                 basis            : Array,
-                 ideal_wavelength : Array,
-                 coefficients     : Array = None) -> OpticalLayer():
+    def __init__(self: OpticalLayer(),
+                 basis: Array,
+                 ideal_wavelength: Array,
+                 coefficients: Array = None) -> OpticalLayer():
         """
         Constructor for the ApplyBasisCLIMB class.
 
         Parameters
         ----------
         basis : Array
             Arrays holding the continous pre-calculated basis vectors. This must
@@ -80,16 +75,15 @@
         # assert self.coefficients.ndim == 1 and \
         # self.coefficients.shape[0] == self.basis.shape[0], \
         # ("coefficients must be a 1 dimensional array with length equal to the "
         # "First dimension of the basis array.")
         # assert self.ideal_wavelength.ndim == 0, ("ideal_wavelength must be a "
         #                                          "scalar array.")
 
-
-    def __call__(self : OpticalLayer(), wavefront : Wavefront) -> Wavefront:
+    def __call__(self: OpticalLayer(), wavefront: Wavefront) -> Wavefront:
         """
         Generates and applies the binary OPD array to the wavefront in a
         differentiable manner.
 
         Parameters
         ----------
         wavefront : Wavefront
@@ -97,94 +91,85 @@
 
         Returns
         -------
         wavefront : Wavefront
             The wavefront with the binary OPD applied.
         """
         latent = self.get_opd(self.basis, self.coefficients)
-        binary_phase = np.pi*self.CLIMB(latent, ppsz=wavefront.npixels)
+        binary_phase = np.pi * self.CLIMB(latent, ppsz=wavefront.npixels)
         opd = self.phase_to_opd(binary_phase, self.ideal_wavelength)
         return wavefront.add_opd(opd)
 
-
     @property
     def applied_shape(self):
-        return tuple(np.array(self.basis.shape[-2:])//3)
-
+        return tuple(np.array(self.basis.shape[-2:]) // 3)
 
     def opd_to_phase(self, opd, wavel):
-        return 2*np.pi*opd/wavel
-
+        return 2 * np.pi * opd / wavel
 
     def phase_to_opd(self, phase, wavel):
-        return phase*wavel/(2*np.pi)
-
+        return phase * wavel / (2 * np.pi)
 
     def get_opd(self, basis, coefficients):
         return np.dot(basis.T, coefficients)
 
-
     def get_total_opd(self):
         return self.get_opd(self.basis, self.coefficients)
 
-
     def get_binary_phase(self):
         latent = self.get_opd(self.basis, self.coefficients)
-        binary_phase = np.pi*self.CLIMB(latent)
+        binary_phase = np.pi * self.CLIMB(latent)
         return binary_phase
 
-
     def lsq_params(self, img):
-        xx, yy = np.meshgrid(np.linspace(0,1,img.shape[0]),
-                             np.linspace(0,1,img.shape[1]))
+        xx, yy = np.meshgrid(np.linspace(0, 1, img.shape[0]),
+                             np.linspace(0, 1, img.shape[1]))
         A = np.vstack([xx.ravel(), yy.ravel(), np.ones_like(xx).ravel()]).T
-        matrix = np.linalg.inv(np.dot(A.T,A)).dot(A.T)
+        matrix = np.linalg.inv(np.dot(A.T, A)).dot(A.T)
         return matrix, xx, yy, A
 
-
     def lsq(self, img):
         matrix, _, _, _ = self.lsq_params(img)
-        return np.dot(matrix,img.ravel())
-
+        return np.dot(matrix, img.ravel())
 
-    def area(self, img, epsilon = 1e-15):
-        a,b,c = self.lsq(img)
-        a = np.where(a==0,epsilon,a)
-        b = np.where(b==0,epsilon,b)
-        c = np.where(c==0,epsilon,c)
-        x1 = (-b-c)/(a) # don't divide by zero
-        x2 = -c/(a) # don't divide by zero
-        x1, x2 = np.min(np.array([x1,x2])), np.max(np.array([x1,x2]))
-        x1, x2 = np.max(np.array([x1,0])), np.min(np.array([x2,1]))
+    def area(self, img, epsilon=1e-15):
+        a, b, c = self.lsq(img)
+        a = np.where(a == 0, epsilon, a)
+        b = np.where(b == 0, epsilon, b)
+        c = np.where(c == 0, epsilon, c)
+        x1 = (-b - c) / (a)  # don't divide by zero
+        x2 = -c / (a)  # don't divide by zero
+        x1, x2 = np.min(np.array([x1, x2])), np.max(np.array([x1, x2]))
+        x1, x2 = np.max(np.array([x1, 0])), np.min(np.array([x2, 1]))
 
-        dummy = x1 + (-c/b)*x2-(0.5*a/b)*x2**2 - (-c/b)*x1+(0.5*a/b)*x1**2
+        dummy = x1 + (-c / b) * x2 - (0.5 * a / b) * x2 ** 2 - (-c / b) * x1 + (0.5 * a / b) * x1 ** 2
 
         # Set the regions where there is a defined gradient
-        dummy = np.where(dummy>=0.5,dummy,1-dummy)
+        dummy = np.where(dummy >= 0.5, dummy, 1 - dummy)
 
         # Colour in regions
-        dummy = np.where(np.mean(img)>=0,dummy,1-dummy)
+        dummy = np.where(np.mean(img) >= 0, dummy, 1 - dummy)
 
         # rescale between 0 and 1?
-        dummy = np.where(np.all(img>0),1,dummy)
-        dummy = np.where(np.all(img<=0),0,dummy)
+        dummy = np.where(np.all(img > 0), 1, dummy)
+        dummy = np.where(np.all(img <= 0), 0, dummy)
 
         # undecided region
-        dummy = np.where(np.any(img==0),np.mean(dummy>0),dummy)
+        dummy = np.where(np.any(img == 0), np.mean(dummy > 0), dummy)
 
         # rescale between 0 and 1
         dummy = np.clip(dummy, 0, 1)
 
         return dummy
 
-    def CLIMB(self, wf, ppsz = 256):
+    def CLIMB(self, wf, ppsz=256):
         psz = ppsz * 3
         dummy = np.array(np.split(wf, ppsz))
-        dummy = np.array(np.split(np.array(dummy), ppsz, axis = 2))
-        subarray = dummy[:,:,0,0]
+        dummy = np.array(np.split(np.array(dummy), ppsz, axis=2))
+        subarray = dummy[:, :, 0, 0]
 
         flat = dummy.reshape(-1, 3, 3)
         vmap_mask = vmap(self.area, in_axes=(0))
 
         soft_bin = vmap_mask(flat).reshape(ppsz, ppsz)
 
-        return soft_bin
+        return soft_bin
```

### Comparing `dLuxToliman-0.1.2/dLuxToliman/optics.py` & `dLuxToliman-0.1.3/dLuxToliman/optics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,145 +1,140 @@
 from __future__ import annotations
 import jax.numpy as np
 import dLux.utils as dlu
 from jax import Array, vmap
 import dLux
 import os
 
-
-MixedAlphaCen = lambda : dLuxToliman.sources.MixedAlphaCen
+MixedAlphaCen = lambda: dLuxToliman.sources.MixedAlphaCen
 
 __all__ = ["TolimanOptics"]
 
-OpticalLayer = lambda : dLux.optical_layers.OpticalLayer
-AngularOptics = lambda : dLux.optics.AngularOptics
+OpticalLayer = lambda: dLux.optical_layers.OpticalLayer
+AngularOptics = lambda: dLux.optics.AngularOptics
 
 
 class TolimanOptics(AngularOptics()):
     """
     A model of the Toliman optical system.
 
     Its default parameters are:
 
     """
 
-    def __init__(self, 
+    def __init__(self,
 
-        wf_npixels = 256,
-        psf_npixels = 256,
-        psf_oversample = 2,
-        psf_pixel_scale = 0.375, # arcsec
-
-        mask = None,
-
-        radial_orders    : Array = None,
-        noll_indices     : Array = None,
-        coefficients = None,
-        # amplitude : float = 0.,
-        # seed : int = 0,
+                 wf_npixels=256,
+                 psf_npixels=256,
+                 psf_oversample=2,
+                 psf_pixel_scale=0.375,  # arcsec
 
-        m1_diameter = 0.125,
-        m2_diameter = 0.032,
-        
-        nstruts = 3,
-        strut_width = 0.002,
-        strut_rotation=-np.pi/2
+                 mask=None,
+
+                 radial_orders: Array = None,
+                 noll_indices: Array = None,
+                 coefficients=None,
+                 # amplitude : float = 0.,
+                 # seed : int = 0,
+
+                 m1_diameter=0.125,
+                 m2_diameter=0.032,
+
+                 n_struts=3,
+                 strut_width=0.002,
+                 strut_rotation=-np.pi / 2
 
-        ) -> TolimanOptics:
+                 ) -> TolimanOptics:
         """
         Constructs a simple model of the Toliman Optical Systems
 
         In this class units are different:
         - psf_pixel_scale is in unit of arcseconds
         """
 
         # Diameter
         diameter = m1_diameter
 
         # Generate Aperture
         aperture = dLux.apertures.ApertureFactory(
-            npixels         = wf_npixels,
-            radial_orders   = radial_orders,
-            noll_indices    = noll_indices,
-            coefficients    = coefficients,
-            secondary_ratio = m2_diameter/m1_diameter,
-            nstruts         = nstruts,
-            strut_ratio     = strut_width/m1_diameter)
+            npixels=wf_npixels,
+            radial_orders=radial_orders,
+            noll_indices=noll_indices,
+            coefficients=coefficients,
+            secondary_ratio=m2_diameter / m1_diameter,
+            nstruts=n_struts,
+            strut_ratio=strut_width / m1_diameter)
 
         # Generate Mask
         if mask is None:
             path = os.path.join(os.path.dirname(__file__), "diffractive_pupil.npy")
             mask = dlu.scale_array(np.load(path), wf_npixels, order=1)
-            
+
             # Enforce full binary
             mask = mask.at[np.where(mask <= 0.5)].set(0.)
             mask = mask.at[np.where(mask > 0.5)].set(1.)
 
             # Enforce full binary
             mask = dlu.phase_to_opd(mask * np.pi, 585e-9)
 
         # Propagator Properties
         psf_npixels = int(psf_npixels)
         psf_oversample = float(psf_oversample)
         psf_pixel_scale = float(psf_pixel_scale)
 
         super().__init__(wf_npixels=wf_npixels, diameter=diameter,
-            aperture=aperture, mask=mask, psf_npixels=psf_npixels, 
-            psf_oversample=psf_oversample, psf_pixel_scale=psf_pixel_scale)
-
+                         aperture=aperture, mask=mask, psf_npixels=psf_npixels,
+                         psf_oversample=psf_oversample, psf_pixel_scale=psf_pixel_scale)
 
     def _apply_aperture(self, wavelength, offset):
         """
         Overwrite so mask can be stored as array
         """
         wf = self._construct_wavefront(wavelength, offset)
         wf *= self.aperture
         wf = wf.normalise()
         wf += self.mask
         return wf
 
 
-
-
-
 class TolimanSpikes(TolimanOptics):
     """
     A model of the Toliman optical system.
 
     Its default parameters are:
 
     """
-    grating_depth  : float
-    grating_period : float
-    spike_npixels  : int
-
-    def __init__(self, 
-
-        wf_npixels = 256,
-        psf_npixels = 256,
-        psf_oversample = 2,
-        psf_pixel_scale = 0.375, # arcsec
-        spike_npixels = 512,
-
-        mask = None,
-        zernikes = None,
-        amplitude : float = 0.,
-        seed : int = 0,
-
-        m1_diameter = 0.13, # Double check this
-        m2_diameter = 0.032,
-        
-        nstruts = 3,
-        strut_width = 0.002,
-        strut_rotation=-np.pi/2,
+    grating_depth: float
+    grating_period: float
+    spike_npixels: int
+
+    def __init__(self,
+
+                 wf_npixels=256,
+                 psf_npixels=256,
+                 psf_oversample=2,
+                 psf_pixel_scale=0.375,  # arcsec
+                 spike_npixels=512,
+
+                 mask=None,
+                 zernikes=None,
+                 amplitude: float = 0.,
+                 seed: int = 0,
+
+                 m1_diameter=0.13,  # Double check this
+                 m2_diameter=0.032,
+
+                 n_struts=3,
+                 strut_width=0.002,
+                 strut_rotation=-np.pi / 2,
 
-        grating_depth = 100., # nm
-        grating_period = 300, # um
+                 grating_depth=100.,  # nm
+                 grating_period=300,  # um
 
-        ) -> TolimanOptics:
+                 ) -> TolimanOptics:
         """
         Constructs a simple model of the Toliman Optical Systems
 
         In this class units are different:
         - psf_pixel_scale is in unit of arcseconds
         grating depth is in nm
         grating period is in um
@@ -147,47 +142,45 @@
 
         # Diameter
         self.grating_depth = grating_depth
         self.grating_period = grating_period
         self.spike_npixels = spike_npixels
 
         super().__init__(
-            wf_npixels      = wf_npixels, 
-            psf_npixels     = psf_npixels, 
-            psf_oversample  = psf_oversample, 
-            psf_pixel_scale = psf_pixel_scale, 
-            mask            = mask, 
-            zernikes        = zernikes, 
-            amplitude       = amplitude, 
-            seed            = seed, 
-            m1_diameter     = m1_diameter, 
-            m2_diameter     = m2_diameter, 
-            nstruts         = nstruts, 
-            strut_width     = strut_width, 
-            strut_rotation  = strut_rotation
-            )
-
+            wf_npixels=wf_npixels,
+            psf_npixels=psf_npixels,
+            psf_oversample=psf_oversample,
+            psf_pixel_scale=psf_pixel_scale,
+            mask=mask,
+            zernikes=zernikes,
+            amplitude=amplitude,
+            seed=seed,
+            m1_diameter=m1_diameter,
+            m2_diameter=m2_diameter,
+            n_struts=n_struts,
+            strut_width=strut_width,
+            strut_rotation=strut_rotation
+        )
 
     def model_spike(self, wavelengths, offset, weights, angles, sign, center):
         """
         
         """
         propagator = vmap(self.model_spike_mono, (0, None, 0, None, None))
         psfs = propagator(wavelengths, offset, angles, sign, center)
         psfs *= weights[..., None, None]
         return psfs.sum(0)
 
-
     def model_spike_mono(self, wavelength, offset, angle, sign, center):
         """
         
         """
         # Construct and tilt
-        wf = dLux.wavefronts.Wavefront(self.aperture.shape[-1], self.diameter, 
-            wavelength)
+        wf = dLux.wavefronts.Wavefront(self.aperture.shape[-1], self.diameter,
+                                       wavelength)
 
         # Addd offset and tilt
         wf = wf.tilt_wavefront(offset - sign * angle)
 
         # Apply aperture and normalise
         wf *= self.aperture
         wf = wf.normalise()
@@ -200,51 +193,48 @@
         true_pixel_scale = self.psf_pixel_scale / self.psf_oversample
         pixel_scale = dlu.arcseconds_to_radians(true_pixel_scale)
         wf = wf.shifted_MFT(self.spike_npixels, pixel_scale, shift=shift)
 
         # Return PSF
         return wf.psf
 
-
     def get_diffraction_angles(self, wavelenghts):
         """
         
         """
-        period = self.grating_period * 1e-6 # Convert to meters
-        angles = np.arcsin(wavelengths / period) / np.sqrt(2) # Radians
+        period = self.grating_period * 1e-6  # Convert to meters
+        angles = np.arcsin(wavelengths / period) / np.sqrt(2)  # Radians
         return dlu.radians_to_arcseconds(angles)
-    
 
     def model_spikes(self, wavelengths, offset, weights):
         """
         
         """
         # Get center shift values
-        period = self.grating_period * 1e-6 # Convert to meters
-        angles = np.arcsin(wavelengths / period) / np.sqrt(2) # Radians
+        period = self.grating_period * 1e-6  # Convert to meters
+        angles = np.arcsin(wavelengths / period) / np.sqrt(2)  # Radians
         # angles = get_diffraction_angles(wavelengths)
         true_pixel_scale = self.psf_pixel_scale / self.psf_oversample
         pixel_scale = dlu.arcseconds_to_radians(true_pixel_scale)
-        center = angles.mean(0)//pixel_scale
+        center = angles.mean(0) // pixel_scale
 
         # Model
         signs = np.array([[-1, +1], [+1, +1], [-1, -1], [+1, -1]])
         propagator = vmap(self.model_spike, (None, None, None, None, 0, None))
         return propagator(wavelengths, offset, weights, angles, signs, center)
 
-
     def full_model(self, source, cent_nwavels=5):
         """
         Returns the diffraction spikes of the PSF
 
         source should be an MixedAplhaCen object
         """
         if not isinstance(source, MixedAlphaCen()):
             raise TypeError("source must be a MixedAlphaCen object")
-        
+
         # Get Values
         wavelengths = source.wavelengths
         weights = source.norm_weights
         fluxes = source.raw_fluxes
         positions = source.xy_positions
         fratio = source.mixing
 
@@ -257,19 +247,19 @@
 
         # Model Central
         # TODO: Downsample central wavelengths and weights
         central_wavelegths = wavelengths
         central_weights = weights
         propagator = vmap(self.propagate, in_axes=(None, 0, 0))
         central_psfs = propagator(
-            central_wavelegths, 
-            positions, 
+            central_wavelegths,
+            positions,
             central_weights)
         central_psfs *= central_flux * fluxes[:, None, None]
 
         # Model spikes
         propagator = vmap(self.model_spikes, in_axes=(None, 0, 0))
         spikes = propagator(wavelengths, positions, weights)
         spikes *= corner_flux * fluxes[:, None, None, None] / 4
 
         # Return
-        return central_psfs.sum(0), spikes.sum(0)
+        return central_psfs.sum(0), spikes.sum(0)
```

### Comparing `dLuxToliman-0.1.2/dLuxToliman/sources.py` & `dLuxToliman-0.1.3/dLuxToliman/sources.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,112 +1,136 @@
 from __future__ import annotations
-import jax.numpy as np
-import jax.random as jr
-import dLux.utils as dlu
 from jax import Array, vmap
+import jax.numpy as np
 import matplotlib.pyplot as plt
 import dLux
+import dLux.utils as dlu
 
+# TODO check if this lambda was necessary
+Source = lambda: dLux.sources.BaseSource
+Optics = lambda: dLux.core.BaseOptics
 
-Source = lambda : dLux.sources.BaseSource
-Optics = lambda : dLux.core.BaseOptics
-
-
-__all__ = ["AlphaCen"] #, "MixedAlphaCen"]
+__all__ = ["AlphaCen"]  # , "MixedAlphaCen"]
 
 
-class AlphaCen(Source()):
+class AlphaCen(dLux.sources.BaseSource):
     """
-    
-    """
-    separation     : float
-    x_position     : tuple
-    y_position     : tuple
+    A parametrised model of the Alpha Centauri binary pair.
+
+    Parameters
+    ----------
+    n_wavels : int
+        The number of wavelengths to model.
+    separation : float
+        The binary separation of the two stars in arcseconds.
     position_angle : float
-    log_flux       : float
-    contrast       : float
-    wavelengths    : Array
-    weights        : Array
-
-    def __init__(self, 
-        nwavels = 5,
-        x_position = 0., # arcseconds
-        y_position = 0., # arcseconds
-        separation = 10., # arcseconds
-        position_angle = 90, # Degrees
-        weights = None,
-        log_flux = 5, # Photons TODO: Find true flux
-        A_mag = 1.33,
-        B_mag = 0.01,
-        ):
+        The position angle of the binary pair in degrees.
+    x_position : float
+        The horizontal offset of the image in arcseconds.
+    y_position : float
+        The vertical offset of the image in arcseconds.
+    log_flux : float
+        The log10 of the total number of photons in the image.
+    contrast : float
+        The flux ratio of Alpha Cen A / Alpha Cen B.
+    bandpass : tuple
+        The wavelength range of the image in nanometers, with syntax (min, max).
+    weights : Array
+    TODO im not actually sure
+
+    Attributes
+    ----------
+
+    Methods
+    -------
+    TODO CONTINUE
+    """
+    separation: float
+    position_angle: float
+    x_position: float
+    y_position: float
+    log_flux: float
+    contrast: float
+    bandpass: tuple
+    weights: Array
+    wavelengths: Array
+
+    # TODO : update default values
+    # TODO: Add bandpass as a parameter?
+    def __init__(self,
+                 n_wavels=3,
+                 separation=10.,  # arcseconds
+                 position_angle=90,  # degrees
+                 x_position=0.,  # arcseconds
+                 y_position=0.,  # arcseconds
+                 log_flux=6.832,  # Photons
+                 contrast=3.37,
+                 bandpass=(530, 640),  # nm
+                 weights=None,
+                 ):
         """
         
         """
         # Positional Parameters
         self.x_position = x_position
         self.y_position = y_position
         self.separation = separation
         self.position_angle = position_angle
 
-        # Flux & Constrast
+        # Flux & Contrast
         self.log_flux = log_flux
-        self.contrast = 10**((A_mag - B_mag)/2.5)
+        self.contrast = contrast
 
-        # Spectrum (Uniform)
-        self.wavelengths = np.linspace(530e-9, 640e-9, nwavels)
+        # Spectrum (Uniform)  # TODO : Phoenix Models?
+        self.bandpass = bandpass
+        self.wavelengths = 1e-9 * np.linspace(bandpass[0], bandpass[1], n_wavels)
         if weights is None:
-            self.weights = np.ones((2, nwavels))/nwavels
+            self.weights = np.ones((2, n_wavels)) / n_wavels
         else:
             self.weights = weights
 
-
     def normalise(self):
         """
         
         """
-        return self.multiply('weights', 1/self.weights.sum(1)[:, None])
-    
+        return self.multiply('weights', 1 / self.weights.sum(1)[:, None])
 
     @property
     def xy_positions(self):
         """
         
         """
         # Calculate
-        r = self.separation/2
+        r = self.separation / 2
         phi = dlu.deg_to_rad(self.position_angle)
-        sep_vec = np.array([r*np.sin(phi), r*np.cos(phi)])
+        sep_vec = np.array([r * np.sin(phi), r * np.cos(phi)])
 
         # Add to Position vectors
         pos_vec = np.array([self.x_position, self.y_position])
         output_vec = np.array([pos_vec + sep_vec, pos_vec - sep_vec])
         return dlu.arcsec_to_rad(output_vec)
 
-
     @property
     def raw_fluxes(self):
         """
         This casts log flux to be the total (not mean) flux.
         """
         flux = (10 ** self.log_flux) / 2
         flux_A = 2 * self.contrast * flux / (1 + self.contrast)
         flux_B = 2 * flux / (1 + self.contrast)
         return np.array([flux_A, flux_B])
-    
-    
+
     @property
     def norm_weights(self):
         """
         
         """
-        return self.weights/self.weights.sum(1)[:, None]
-
+        return self.weights / self.weights.sum(1)[:, None]
 
-    def model(self      : Source(),
-              optics    : Optics()) -> Array:
+    def model(self: Source(), optics: Optics()) -> Array:
         """
         Method to model the psf of the point source through the optics.
 
         Parameters
         ----------
         optics : Optics
             The optics through which to model the source objects.
@@ -114,15 +138,15 @@
             The detector object that is observing the psf.
         filter_in : Filter = None
             The filter through which the source is being observed.
 
         Returns
         -------
         psf : Array
-            The psf of the source source modelled through the optics.
+            The psf of the source modelled through the optics.
         """
         # Get Values
         weights = self.norm_weights
         fluxes = self.raw_fluxes
         positions = self.xy_positions
 
         # vmap propagator
@@ -133,42 +157,42 @@
         input_weights = weights * fluxes[:, None]
         psfs = propagator(self.wavelengths, positions)
         psfs *= input_weights[..., None, None]
         return psfs.sum((0, 1))
 
 
 def get_mixed_alpha_cen_spectra(
-    nwavels    : int, 
-    min_wavel  : float = 545e-9, 
-    max_wavels : float = 645e-9
-    ):
+        nwavels: int,
+        min_wavel: float = 545e-9,
+        max_wavels: float = 645e-9
+):
     """
     
     """
     # Import Here to prevent issues with google colab install, for example
     import pysynphot as S
 
     alpha_cen_a_spectrum: float = S.Icat("phoenix",
-        5790, # Surface temp (K)
-        0.2,  # Metalicity (Unit?)
-        4.0,) # Surface gravity (unit?)
+                                         5790,  # Surface temp (K)
+                                         0.2,  # Metalicity (Unit?)
+                                         4.0, )  # Surface gravity (unit?)
     alpha_cen_a_spectrum.convert('flam')
     alpha_cen_a_spectrum.convert('m')
 
     alpha_cen_b_spectrum: float = S.Icat("phoenix",
-        5260, # Surface temp (K)
-        0.23, # Metalicity (Unit?)
-        4.37) # Surface gravity (unit?)
+                                         5260,  # Surface temp (K)
+                                         0.23,  # Metalicity (Unit?)
+                                         4.37)  # Surface gravity (unit?)
     alpha_cen_b_spectrum.convert('flam')
     alpha_cen_b_spectrum.convert('m')
 
     spot_spectrum: float = S.Icat("phoenix",
-        4000, # Surface temp (K)
-        0.23, # Metalicity (Unit?)
-        4.37) # Surface gravity (unit?)
+                                  4000,  # Surface temp (K)
+                                  0.23,  # Metalicity (Unit?)
+                                  4.37)  # Surface gravity (unit?)
     spot_spectrum.convert('flam')
     spot_spectrum.convert('m')
 
     # Full spectrum
     wavelengths = np.linspace(545e-9, 645e-9, nwavels)
     Aspec = alpha_cen_a_spectrum.sample(wavelengths)
     Bspec = alpha_cen_b_spectrum.sample(wavelengths)
@@ -177,86 +201,80 @@
     Aspec /= Aspec.max()
     Bspec /= Bspec.max()
     Sspec /= Sspec.max()
 
     return np.array([Aspec, Bspec, Sspec]), wavelengths
 
 
-
-
-
 class MixedAlphaCen(AlphaCen):
-    mixing         : float
-    
+    mixing: float
 
-    def __init__(self, 
-        nwavels = 101,
-        x_position = 0., # arcseconds
-        y_position = 0., # arcseconds
-        separation = 10., # arcseconds
-        position_angle = 90, # Degrees
-        weights = None,
-        mixing = 0.05,
-        log_flux = 5, # Photons TODO: Find true flux
-        A_mag = 1.33,
-        B_mag = 0.01,
-        ):
+    def __init__(self,
+                 n_wavels=101,
+                 x_position=0.,  # arcseconds
+                 y_position=0.,  # arcseconds
+                 separation=10.,  # arcseconds
+                 position_angle=90,  # Degrees
+                 weights=None,
+                 mixing=0.05,
+                 log_flux=5,  # Photons TODO: Find true flux
+                 A_mag=1.33,
+                 B_mag=0.01,
+                 ):
         """
         
         """
         self.mixing = mixing
-        weights, wavelengths = get_mixed_alpha_cen_spectra(nwavels)
-        super().__init__(nwavels, x_position, y_position, separation, 
-            position_angle, weights, log_flux, A_mag, B_mag)
+        weights, wavelengths = get_mixed_alpha_cen_spectra(n_wavels)
+        super().__init__(n_wavels, x_position, y_position, separation,
+                         position_angle, weights, log_flux, A_mag, B_mag)
 
         def plot(self):
             """
             
             """
             plt.figure(figsize=(12, 4))
             plt.subplot(1, 2, 1)
             plt.title(f"Alpha Cen A, f: {f}")
             plt.xlabel("Wavelength (nm)")
             plt.ylabel("Weight")
-            plt.plot(spec_wavelengths*1e9, MixedA, label='Mixed')
-            plt.plot(spec_wavelengths*1e9, SpecA, label='Main')
-            plt.plot(spec_wavelengths*1e9, SpottedA, label='Spotted')
+            plt.plot(spec_wavelengths * 1e9, MixedA, label='Mixed')
+            plt.plot(spec_wavelengths * 1e9, SpecA, label='Main')
+            plt.plot(spec_wavelengths * 1e9, SpottedA, label='Spotted')
             plt.legend()
 
-            SpecB = (1-f)*Bspec
-            SpottedB = f*Sspec
+            SpecB = (1 - f) * Bspec
+            SpottedB = f * Sspec
             MixedB = SpecB + SpottedB
             plt.subplot(1, 2, 2)
             plt.title("Alpha Cen B, f: {f}")
             plt.xlabel("Wavelength (nm)")
             plt.ylabel("Weight")
-            plt.plot(spec_wavelengths*1e9, MixedB, label='Mixed')
-            plt.plot(spec_wavelengths*1e9, SpecB, label='Main')
-            plt.plot(spec_wavelengths*1e9, SpottedB, label='Spotted')
+            plt.plot(spec_wavelengths * 1e9, MixedB, label='Mixed')
+            plt.plot(spec_wavelengths * 1e9, SpecB, label='Main')
+            plt.plot(spec_wavelengths * 1e9, SpottedB, label='Spotted')
             plt.legend()
             plt.show()
 
-
     @property
     def norm_weights(self):
         """
         
         """
         # Get Spectra
         Spotted = self.mixing * self.weights[2]
         MixedA = (1 - self.mixing) * self.weights[0] + Spotted
         MixedB = (1 - self.mixing) * self.weights[1] + Spotted
         weights = np.array([MixedA, MixedB])
 
         # Normalise
         return weights / weights.sum(1)[:, None]
 
-
-    def model(self      : Source,
-              optics    : Optics) -> Array:
+    def model(self: Source,
+              optics: Optics) -> Array:
         """
         Method to model the psf of the point source through the optics.
 
         Parameters
         ----------
         optics : Optics
             The optics through which to model the source objects.
@@ -264,23 +282,23 @@
             The detector object that is observing the psf.
         filter_in : Filter = None
             The filter through which the source is being observed.
 
         Returns
         -------
         psf : Array
-            The psf of the source source modelled through the optics.
+            The psf of the source modelled through the optics.
         """
         # Get Values
         weights = self.norm_weights
         fluxes = self.raw_fluxes
         positions = self.xy_positions
 
         # vmap propagator
         source_propagator = vmap(optics.propagate_mono, in_axes=(0, None))
         propagator = vmap(source_propagator, in_axes=(None, 0))
 
         # Model PSF
         input_weights = weights * fluxes[:, None]
         psfs = propagator(self.wavelengths, positions)
         psfs *= input_weights[..., None, None]
-        return psfs.sum((0, 1))
+        return psfs.sum((0, 1))
```

### Comparing `dLuxToliman-0.1.2/dLuxToliman.egg-info/PKG-INFO` & `dLuxToliman-0.1.3/dLuxToliman.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dLuxToliman
-Version: 0.1.2
+Version: 0.1.3
 Summary: A repo to hold the canonical dLux Toliman models.
 Home-page: https://github.com/maxecharles/dLuxToliman
 Author: Max Charles
 Author-email: max.charles@sydney.edu.au
 Project-URL: Bug Tracker, https://github.com/maxecharles/dLuxToliman/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -14,25 +14,24 @@
 
 # dLuxToliman
 
 [![PyPI version](https://badge.fury.io/py/dLuxToliman.svg)](https://badge.fury.io/py/dLuxToliman)
 [![License](https://img.shields.io/badge/license-BSD%203--Clause-blue.svg)](LICENSE)
 
 ## Description
+This repository/package contains pre-built ∂Lux models of the Toliman optical system, and pre-built parametrised ∂Lux source objects for Alpha Centauri.
 
 [∂Lux](https://louisdesdoigts.github.io/dLux/) is an open-source differentiable optical modelling framework harnessing the structural isomorphism between optical systems and neural networks, giving forwards models of optical system as a _parametric neural network_.
 ∂Lux is built in [Zodiax](https://github.com/LouisDesdoigts/zodiax) which is an open-source object-oriented [Jax](https://github.com/google/jax) framework built as an extension of [Equinox](https://github.com/patrick-kidger/equinox) for scientific programming.
 
 The primary goal of the Toliman mission is to discover Earth-sized exoplanets orbiting in Alpha Centauri, the closest star system to our own.
 To achieve this, the mission will employ a novel telescope design that will be able to detect subtle changes in the positions of the Alpha Centauri binary pair.
 These changes are caused by the gravitational reflex motion induced by an Earth-sized companion, and this cutting-edge technology will enable scientists to identify exoplanets too small to be detected by conventional telescopes.
 Toliman utilises a binary phase diffraction pupil to grasp the expected microarcsecond-scale astrometric signal.
 
-**This repository/package contains pre-built ∂Lux models of the Toliman optical system**, and pre-built parametrised ∂Lux source objects for Alpha Centauri.
-
 ## Installation
 
 `dLuxToliman` is pip-installable. To install the latest release, simply run:
 
 ```bash
 pip install dLuxToliman
 ```
@@ -43,24 +42,27 @@
 
 ```python
 # imports
 import dLuxToliman as dlT
 from matplotlib import pyplot as plt
 
 osys = dlT.TolimanOptics(psf_npixels=128, psf_oversample=1)  # creating Toliman optical system
-source = dlT.AlphaCen(nwavels=3, separation=8, position_angle=30)  # creating Alpha Centauri source
+source = dlT.AlphaCen(n_wavels=3, separation=8, position_angle=30)  # creating Alpha Centauri source
 psf = osys.model(source)  # running optical simulation
 
 # plotting
-plt.imshow(psf**.5, cmap = 'inferno')
+plt.imshow(psf ** .5, cmap='inferno')
 plt.title('Toliman $\sqrt{PSF}$')
 plt.show()
 ```
 
-The above code generates the PSF for the Toliman optical system, with the Alpha Centauri source, and plots the PSF on a square root stretch.
+![Example Image](./assets/basic_toliman_psf.jpg)
+
+## Contributors
+[Max Charles](https://github.com/maxecharles), [Louis Desdoigts](https://github.com/LouisDesdoigts), [Benjamin Pope](https://github.com/benjaminpope), and [Peter Tuthill](https://github.com/ptuthill).
 
 ## License
 
 This package is released under the BSD 3-Clause License. See the [LICENSE](LICENSE) file for more information.
 
 ## Support
```

