# Comparing `tmp/spectrally_regularised_lvms-0.1.2.tar.gz` & `tmp/spectrally_regularised_lvms-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrally_regularised_lvms-0.1.2.tar", max compression
+gzip compressed data, was "spectrally_regularised_lvms-0.1.3.tar", max compression
```

## Comparing `spectrally_regularised_lvms-0.1.2.tar` & `spectrally_regularised_lvms-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1090 2023-04-28 07:39:34.154025 spectrally_regularised_lvms-0.1.2/LICENSE
--rw-r--r--   0        0        0     1778 2023-06-30 09:54:42.114178 spectrally_regularised_lvms-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3762 2023-06-18 11:04:30.198907 spectrally_regularised_lvms-0.1.2/README.md
--rw-r--r--   0        0        0     1201 2023-06-30 09:54:42.125360 spectrally_regularised_lvms-0.1.2/spectrally_regularised_LVMs/__init__.py
--rw-r--r--   0        0        0    32459 2023-05-29 12:05:32.601314 spectrally_regularised_lvms-0.1.2/spectrally_regularised_LVMs/cost_functions.py
--rw-r--r--   0        0        0    21405 2023-05-26 12:13:55.515128 spectrally_regularised_lvms-0.1.2/spectrally_regularised_LVMs/helper_methods.py
--rw-r--r--   0        0        0    13584 2023-05-26 12:13:55.515631 spectrally_regularised_lvms-0.1.2/spectrally_regularised_LVMs/negen_approx.py
--rw-r--r--   0        0        0    16767 2023-06-09 10:22:09.397167 spectrally_regularised_lvms-0.1.2/spectrally_regularised_LVMs/spectral_regulariser.py
--rw-r--r--   0        0        0    52758 2023-06-30 09:53:06.824340 spectrally_regularised_lvms-0.1.2/spectrally_regularised_LVMs/spectrally_regularised_model.py
--rw-r--r--   0        0        0     5077 1970-01-01 00:00:00.000000 spectrally_regularised_lvms-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-04-28 07:39:34.154025 spectrally_regularised_lvms-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1824 2023-07-13 08:24:35.903193 spectrally_regularised_lvms-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4073 2023-07-13 08:35:47.247708 spectrally_regularised_lvms-0.1.3/README.md
+-rw-r--r--   0        0        0     1163 2023-07-13 08:24:35.910612 spectrally_regularised_lvms-0.1.3/spectrally_regularised_LVMs/__init__.py
+-rw-r--r--   0        0        0    37266 2023-07-13 08:06:30.606068 spectrally_regularised_lvms-0.1.3/spectrally_regularised_LVMs/cost_functions.py
+-rw-r--r--   0        0        0    21098 2023-07-13 08:06:30.606563 spectrally_regularised_lvms-0.1.3/spectrally_regularised_LVMs/helper_methods.py
+-rw-r--r--   0        0        0    13584 2023-05-26 12:13:55.515631 spectrally_regularised_lvms-0.1.3/spectrally_regularised_LVMs/negen_approx.py
+-rw-r--r--   0        0        0    16767 2023-06-09 10:22:09.397167 spectrally_regularised_lvms-0.1.3/spectrally_regularised_LVMs/spectral_regulariser.py
+-rw-r--r--   0        0        0    54459 2023-07-13 08:06:30.608585 spectrally_regularised_lvms-0.1.3/spectrally_regularised_LVMs/spectrally_regularised_model.py
+-rw-r--r--   0        0        0     5382 1970-01-01 00:00:00.000000 spectrally_regularised_lvms-0.1.3/PKG-INFO
```

### Comparing `spectrally_regularised_lvms-0.1.2/LICENSE` & `spectrally_regularised_lvms-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrally_regularised_lvms-0.1.2/pyproject.toml` & `spectrally_regularised_lvms-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "spectrally-regularised-LVMs"
-version = "0.1.2"
-description = "An implementation of linear LVMs with a spectral regulariser."
+version = "0.1.3"
+description = "A framework of linear LVMs with spectral regularisation."
 authors = ["Ryan Balshaw <ryanbalshaw81@gmail.com>"]
 maintainers = ["Ryan Balshaw <ryanbalshaw81@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/RyanBalshaw/spectrally-regularised-LVMs"
 repository = "https://github.com/RyanBalshaw/spectrally-regularised-LVMs"
 documentation = "https://spectrally-regularised-lvms.readthedocs.io/en/latest/"
@@ -45,14 +45,16 @@
 [tool.poetry.group.docs.dependencies]
 myst-parser = ">=0.16"
 sphinx = ">=4.0"
 sphinx-autobuild = ">=2021.0"
 sphinx-rtd-theme = ">=1.0"
 numpydoc = "^1.5.0"
 autodocsumm = "^0.2.11"
+sphinx-book-theme = "^1.0.1"
+furo = "^2023.5.20"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.urls]
 "Bug tracker" = "https://github.com/RyanBalshaw/spectrally-regularised-LVMs/issues"
```

### Comparing `spectrally_regularised_lvms-0.1.2/README.md` & `spectrally_regularised_lvms-0.1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,52 +2,53 @@
 ![GitHub license](https://img.shields.io/github/license/RyanBalshaw/spectrally-regularised-LVMs)
 ![GitHub last commit](https://img.shields.io/github/last-commit/RyanBalshaw/spectrally-regularised-LVMs)
 ![PyPI](https://img.shields.io/pypi/v/spectrally-regularised-lvms)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/spectrally-regularised-lvms?color=blueviolet)
 ![Read the Docs](https://img.shields.io/readthedocs/spectrally-regularised-lvms?color=informational)
 ![GitHub issues](https://img.shields.io/github/issues/RyanBalshaw/spectrally-regularised-LVMs?color=critical)
 
-*Current version:* 0.1.1
-
-Spectrally-regularised-LVMs is a Python-based package which facilitates the estimation of the linear latent variable model (LVM) parameters with a unique spectral regularisation term in single channel time-series applications.
+*Spectrally-regularised-LVMs* is a Python-based [package](https://pypi.org/project/spectrally-regularised-lvms/) which facilitates the estimation of the linear latent variable model (LVM) parameters with a unique spectral regularisation term in single channel time-series applications.
 
 ## Purpose
-LVMs are a statistical methodology which tries to capture the underlying structure in some observed data. This package caters to single channel time-series applications and provides a methodology to estimate the LVM parameters. The model parameters are encouraged to be diverse via a spectral regularisation term which penalises source duplication of the spectral information captured by the latent sources.
+LVMs are a statistical methodology which try to capture the underlying structure in some observed data. This package caters to single channel time-series applications and provides a methodology to estimate the LVM parameters. The model parameters are encouraged to capture non-duplicate information via a spectral regularisation term which penalises source duplication of the spectral information captured by the latent sources.
 
-The purpose of this package is to provide a complete methodology that caters to a variety of LVM objective functions.
+The purpose of this package is to provide a complete framework for LVMs with spectral regularisation that caters to a variety of LVM objective functions.
 
 # Documentation
-Please visit [the docs](http://spectrally-regularised-lvms.readthedocs.io/) for all supporting documentation for this package.
+Please visit the [documentation](http://spectrally-regularised-lvms.readthedocs.io/) page for all supporting documentation for this package.
 
 # Installation
 The package is designed to be used through the Python API, and  can be installed using [pip](https://pypi.org/project/pip/):
 ```console
 $ pip install spectrally-regularised-LVMs
 ```
 
+A more detailed discussion regarding installation is given in the [documentation](http://spectrally-regularised-lvms.readthedocs.io/).
+
 # Requirements
 
 This package used Python ≥ 3.10 or later to run. For other python dependencies, please check the `pyproject.toml`
 [file](https://github.com/RyanBalshaw/spectrally-regularised-LVMs/blob/main/pyproject.toml) included in this repository. The dependencies of this package are as follows:
 
-|          Package                   	           | Version 	  |
-|:----------------------------------------------:|:----------:|
-|    [Python](https://www.python.org/)      	    | ≥ 3.10  	  |
-|     [Numpy](https://numpy.org/)         	      | ≥ 1.23.1 	 |
-|   [Matplotlib](https://matplotlib.org/)    	   | ≥ 3.5.2 	  |
-|     [SciPy](https://scipy.org/)         	      | ≥ 1.8.1 	  |
-|  [scikit-learn](https://scikit-learn.org/)  	  | ≥ 1.1.2 	  |
-|   [tqdm](https://github.com/tqdm/tqdm)     	   | ≥ 4.64.1 	 |
-| [SymPy](https://www.sympy.org/en/index.html) 	 | ≥ 1.1.1 	  |
+|           Package                   	           | Version 	  |
+|:-----------------------------------------------:|:----------:|
+|    [Python](https://www.python.org/)      	     | ≥ 3.10  	  |
+|      [Numpy](https://numpy.org/)         	      | ≥ 1.23.1 	 |
+|   [Matplotlib](https://matplotlib.org/)    	    | ≥ 3.5.2 	  |
+|      [SciPy](https://scipy.org/)         	      | ≥ 1.8.1 	  |
+|  [scikit-learn](https://scikit-learn.org/)  	   | ≥ 1.1.2 	  |
+|   [tqdm](https://github.com/tqdm/tqdm)     	    | ≥ 4.64.1 	 |
+| [SymPy](https://www.sympy.org/en/index.html) 	  | ≥ 1.1.1 	  |
+| [Poetry](https://python-poetry.org/) 	 | ≥ 1.4 	  |
 
 # API usage
 Please visit [the docs](http://spectrally-regularised-lvms.readthedocs.io/) for all supporting API documentation for this package.
 
 # Contributing
-This package uses [Poetry](https://python-poetry.org/) for dependency management and Python packaging and [git](https://git-scm.com/) for version control. To get started, first install git and Poetry and then clone this repository via
+This package uses [Poetry](https://python-poetry.org/) for dependency management and Python packaging and [git](https://git-scm.com/) for version control. To get started, first install git and Poetry. Then one may clone this repository via
 ```console
 $ git clone git@github.com:RyanBalshaw/spectrally-regularised-LVMs.git
 $ cd spectrally-regularised-LVMs
 ```
 
 Then, install the necessary dependencies in a local environment via
 ```console
```

### Comparing `spectrally_regularised_lvms-0.1.2/spectrally_regularised_LVMs/__init__.py` & `spectrally_regularised_lvms-0.1.3/spectrally_regularised_LVMs/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 # Copyright 2023-present Ryan Balshaw
 """Spectrally-regularised-LVMs. Train linear LVMs with the addition
  of a spectral regularisation term with minimal effort."""
-from .cost_functions import NegentropyCost, SympyCost, UserCost, VarianceCost
+from .cost_functions import ExplicitCost, NegentropyCost, SymbolicCost, VarianceCost
 from .helper_methods import (
     BatchSampler,
     DataProcessor,
     DeflationOrthogonalisation,
     QuasiNewton,
     hankel_matrix,
 )
 from .negen_approx import CubeObject, ExpObject, LogcoshObject, QuadObject
 from .spectral_regulariser import SpectralObjective
 from .spectrally_regularised_model import LinearModel
 
 __author__ = "Ryan Balshaw"
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 __email__ = "ryanbalshaw81@gmail.com"
-__description__ = (
-    "Train linear LVMs with the addition "
-    "of a spectral regularisation term with minimal effort."
-)
+__description__ = "A framework of linear LVMs with spectral regularisation."
 __uri__ = "http://spectrally-regularised-lvms.readthedocs.io/"
 __all__ = [
     "SpectralObjective",
     "NegentropyCost",
-    "SympyCost",
-    "UserCost",
+    "SymbolicCost",
+    "ExplicitCost",
     "VarianceCost",
     "hankel_matrix",
     "LinearModel",
     "BatchSampler",
     "DataProcessor",
     "DeflationOrthogonalisation",
     "QuasiNewton",
```

### Comparing `spectrally_regularised_lvms-0.1.2/spectrally_regularised_LVMs/cost_functions.py` & `spectrally_regularised_lvms-0.1.3/spectrally_regularised_LVMs/cost_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,162 +4,269 @@
 one can use, using user-defined analytical functions based off
 SymPy and NumPy.
 
 Additionally, there are two specific methods implemented here:
 - principal component analysis
 - negentropy-based independent component analysis.
 """
+import warnings
+
 import numpy as np
 import sympy as sp
 
 from .negen_approx import initialise_sources
 
 
 class CostClass(object):
     """
-    Base class for different formulations of the user
-    cost function.
+    Base class for different formulations of the user cost function. All children
+    classes are expected to have _cost, _cost_gradient, and _cost_hessian instance
+    attribute. These attributes are accessed by the methods of CostClass
+    for ease of use.
 
     Methods
     -------
-    set_cost(cost_func)
-        This method takes in a cost_func variable and sets it as
-        an internal attribute self._cost.
-
-    set_gradient(cost_gradient)
-        This method takes in a cost_gradient variable and sets it as
-        an internal attribute self._cost_gradient.
+    cost(X, w, y)
+        This method accesses the internal self._cost instance attribute and
+        returns its output self._cost(X, w, y).
 
-    set_hessian(cost_hessian)
-        This method takes in a cost_hessian variable and sets it as
-        an internal attribute self._cost_hessian.
+    cost_gradient(X, w, y)
+        This method accesses the internal self._cost_gradient instance attribute and
+        returns its output self._cost_gradient(X, w, y).
 
-    get_cost()
-        This method return the internal self._cost instance.
+    cost_hessian(X, w, y)
+        This method accesses the internal self._cost_hessian instance attribute and
+        returns its output self._cost_hessian(X, w, y).
 
-    get_gradient()
-        This method return the internal self._cost_gradient instance.
+    finite_difference_grad(X, w, y, step_size)
+        The method returns the central finite difference approximation to the gradient.
 
-    get_hessian()
-        This method return the internal self._cost_hessian instance.
+    finite_difference_hess(X, w, y, step_size)
+        The method returns the central finite difference approximation to the Hessian.
 
     check_gradient(X, w, y, step_size)
         This method takes in an initial set of variables X, w, y, and a
         finite difference step size. The function is used to check the
         self._cost_gradient method using a central finite-difference
         approach.
 
     check_hessian(X, w, y, step_size)
         This method takes in an initial set of variables X, w, y, and a
         finite difference step size. The function is used to check the
         self._cost_hessian method using a central finite-difference
         approach.
     """
 
-    def __init__(self, verbose: bool = True):
+    def __init__(
+        self,
+        use_hessian: bool = True,
+        verbose: bool = False,
+        finite_diff_flag: bool = False,
+    ):
         """
 
         Parameters
         ----------
+        use_hessian : bool
+            A flag to control whether you use the Hessian or not.
+            This is useful in the parameter estimation step, as you may wish to just
+            perform steepest descent instead of using Newton's method.
+
         verbose : bool
             A boolean flag to control any possible
             print statements.
+
+        finite_diff_flag: bool
+            A boolean flag to control whether a finite difference approximation
+            is to be used for the gradient and hessian
         """
-        self._cost = None
-        self._cost_gradient = None
-        self._cost_hessian = None
+
+        self.use_hessian = use_hessian
         self.verbose = verbose
+        self.finite_diff_flag = finite_diff_flag
 
-    def set_cost(self, cost_func):
+    def cost(self, X, w, y):
         """
-        This method allows one to set their cost function.
+        A method that returns the cost function for the inputs.
 
         Parameters
         ----------
-        cost_func : function
-            The users cost function.
+        X : ndarray
+            The feature matrix of size (n_samples, n_features)
 
-        Examples
-        --------
-        cost_func = lambda X, w, y: -1 * np.mean(y ** 2, axis=0)
+        w : ndarray
+            The transformation vector of size (n_features, 1)
+
+        y : ndarray
+            The transformed variable y = X @ w of size (n_samples, 1)
 
+        Returns
+        -------
+        cost function evaluation of (X, w, y)
         """
-        self._cost = cost_func
 
-    def set_gradient(self, cost_gradient):
+        return self._cost(X, w, y)
+
+    def cost_gradient(self, X, w, y):
         """
-        This method allows one to set their gradient vector.
+        A method that returns the cost function gradient for the inputs.
 
         Parameters
         ----------
-        cost_gradient : function
-            The users gradient vector of the cost function.
+        X : ndarray
+            The feature matrix of size (n_samples, n_features)
 
-        Examples
-        --------
-        cost_gradient = lambda X, w, y: -2 * np.mean(y * X, axis=0,
-            keepdims=True)
+        w : ndarray
+            The transformation vector of size (n_features, 1)
 
+        y : ndarray
+            The transformed variable y = X @ w of size (n_samples, 1)
+
+        Returns
+        -------
+        derivative function evaluation of (X, w, y)
         """
-        self._cost_gradient = cost_gradient
 
-    def set_hessian(self, cost_hessian):
+        if self.finite_diff_flag:
+            return self.finite_difference_grad(X, w, y, step_size=1e-4)
+
+        else:
+            return self._cost_gradient(X, w, y)
+
+    def cost_hessian(self, X, w, y):
         """
-        This method allows one to set their objective Hessian (optional).
+        A method that returns the Hessian function for the inputs.
 
         Parameters
         ----------
-        cost_hessian : function
-            The users gradient vector of the cost function.
-
-        Examples
-        --------
-        cost_hessian = lambda X, w, y: -2 /X.shape[0] * (X.T @ X)
+        X : ndarray
+            The feature matrix of size (n_samples, n_features)
 
-        """
-        self._cost_hessian = cost_hessian
+        w : ndarray
+            The transformation vector of size (n_features, 1)
 
-    def get_cost(self):
-        """
-        Method to return the cost function to the user.
+        y : ndarray
+            The transformed variable y = X @ w of size (n_samples, 1)
 
         Returns
         -------
-        cost_func if attribute exists, else None.
+        Hessian function evaluation of (X, w, y)
         """
-        if hasattr(self, "_cost"):
-            return self._cost
+        if self.use_hessian:
+            if self.finite_diff_flag:
+                return self.finite_difference_hess(X, w, y, step_size=1e-4)
+
+            else:
+                return self._cost_hessian(X, w, y)
+
         else:
-            return None
+            return np.eye(w.shape[0])
 
-    def get_gradient(self):
+    def finite_difference_grad(self, X, w, y, step_size: float):
         """
-        Method to return the derivative function to the user.
+        Finite difference gradient approximation (central difference)
+
+        Parameters
+        ----------
+        X : ndarray
+            An array of size n_samples x n_features.
+
+        w : ndarray
+            An column vector of size n_features x 1
+
+        y : ndarray
+            An column vector of size n_features x 1. Expected to be
+            equivalent to X @ w.
+
+        step_size : float (default = 1e-4)
+            The finite difference step size.
 
         Returns
         -------
-        cost_gradient if attribute exists, else None.
+        grad_fd : ndarray
+            The finite difference approximation to the gradient
         """
-        if hasattr(self, "_cost_gradient"):
-            return self._cost_gradient
-        else:
-            return None
 
-    def get_hessian(self):
+        if self.verbose:
+            print("Finite difference gradient approximation...")
+
+        grad_fd = np.zeros_like(w)
+        w0 = w.copy()
+
+        for i in range(grad_fd.shape[0]):
+            e_i = np.zeros_like(w0)
+            e_i[i, 0] = step_size
+
+            # Calculate sensitivity change in y as well!
+            y_f = X @ (w0 + e_i)
+            y_b = X @ (w0 - e_i)
+
+            f_f = self._cost(X, w0 + e_i, y_f)
+            f_b = self._cost(X, w0 - e_i, y_b)
+
+            grad_fd[i, 0] = (f_f - f_b) / (2 * step_size)
+
+        return grad_fd
+
+    def finite_difference_hess(self, X, w, y, step_size: float):
         """
-        A method to return the hessian function to the user.
+        Finite difference Hessian approximation (central difference)
+
+        Parameters
+        ----------
+        X : ndarray
+            An array of size n_samples x n_features.
+
+        w : ndarray
+            An column vector of size n_features x 1
+
+        y : ndarray
+            An column vector of size n_features x 1. Expected to be
+            equivalent to X @ w.
+
+        step_size : float (default = 1e-4)
+            The finite difference step size.
 
         Returns
         -------
-        cost_hessian if attribute exists, else None.
+        hess_fd : ndarray
+            The finite difference approximation to the hessian
         """
-        if hasattr(self, "_cost_hessian"):
-            return self._cost_hessian
-        else:
-            return None
+
+        if self.verbose:
+            print("Finite difference hessian approximation...")
+
+        D, _ = w.shape
+
+        w0 = w.copy()
+
+        hess_fd = np.zeros((D, D))
+
+        for i in range(D):
+            e_i = np.zeros_like(w0)
+            e_i[i, 0] = step_size
+
+            for j in range(D):
+                e_j = np.zeros_like(w0)
+                e_j[j, 0] = step_size
+
+                # Calculate sensitivity change in y as well!
+                y1 = X @ (w0 + e_i + e_j)
+                y2 = X @ (w0 + e_i - e_j)
+                y3 = X @ (w0 - e_i + e_j)
+                y4 = X @ (w0 - e_i - e_j)
+
+                f1 = self._cost(X, w0 + e_i + e_j, y1)
+                f2 = self._cost(X, w0 + e_i - e_j, y2)
+                f3 = self._cost(X, w0 - e_i + e_j, y3)
+                f4 = self._cost(X, w0 - e_i - e_j, y4)
+
+                hess_fd[i, j] = (f1 - f2 - f3 + f4) / (4 * step_size**2)
+
+        return hess_fd
 
     def check_gradient(self, X, w, y, step_size: float = 1e-4):
         """
         This method checks the self._cost_gradient function to determine
         whether the gradient implementation is correct based off the
         objective function.
 
@@ -179,53 +286,46 @@
             The finite difference step size.
 
         Returns
         -------
         grad_current : ndarray
             The gradient based off the internal self._cost_gradient instance.
 
-        grad_check : ndarray
+        grad_fd : ndarray
             The finite-difference approximation to the gradient
 
         grad_norm : ndarray
             The L2 norm between the analytical gradient and the finite difference
             approximation.
 
         Note that this is a helper method. costClass operates as a base class,
         so you will find that methods such as self.cost() and self.cost_gradient()
         are accessed but never defined. I use a child class to define these methods.
         """
-        # Finite difference gradient approximation (central difference)
 
         if self.verbose:
             print("\nChecking the gradient using central difference approximation...")
-        w0 = w.copy().reshape(-1, 1)
-
-        grad_current = self._cost_gradient(X, w0, y).reshape(-1, 1)
-        grad_check = np.zeros_like(grad_current)
 
-        for i in range(grad_check.shape[0]):
-            e_i = np.zeros_like(w0)
-            e_i[i, 0] = step_size
-
-            # Calculate sensitivity change in y as well!
-            y_f = X @ (w0 + e_i)
-            y_b = X @ (w0 - e_i)
+        if self.finite_diff_flag:
+            warnings.warn(
+                "finite_diff_flag = True, evaluation of gradient norm" " will be zero.",
+                RuntimeWarning,
+            )
 
-            f_f = self._cost(X, w0 + e_i, y_f)
-            f_b = self._cost(X, w0 - e_i, y_b)
+        w0 = w.copy().reshape(-1, 1)
 
-            grad_check[i, 0] = (f_f - f_b) / (2 * step_size)
+        grad_current = self.cost_gradient(X, w0, y).reshape(-1, 1)
+        grad_fd = self.finite_difference_grad(X, w0, y, step_size)
 
-        grad_norm = np.linalg.norm(grad_current - grad_check)
+        grad_norm = np.linalg.norm(grad_current - grad_fd)
 
         if self.verbose:
-            print(f"Finished! The gradient norm is: {np.round(grad_norm)}")
+            print(f"Finished! The gradient norm is: {grad_norm}")
 
-        return grad_current, grad_check, grad_norm
+        return grad_current, grad_fd, grad_norm
 
     def check_hessian(self, X, w, y, step_size: float = 1e-4):
         """
         This method checks the self._cost_hessian function to determine
         whether the hessian implementation is correct based off the
         user-defined objective function.
 
@@ -256,55 +356,37 @@
             The L2 norm (average of the row-wise L2 norm) between the analytical
             hessian and the finite difference approximation.
 
         Note that this is a helper method. costClass operates as a base class,
         so you will find that methods such as self.cost() and self.cost_hessian()
         are accessed but never defined. I use a child class to define these methods.
         """
-        # Finite difference Hessian approximation (central difference)
 
         if self.verbose:
             print("\nChecking the hessian using central difference approximation...")
 
-        w0 = w.copy().reshape(-1, 1)
-        hess_current = self._cost_hessian(X, w0, y)
-        hess_check = np.zeros_like(hess_current)
-
-        r, c = hess_check.shape
-
-        for i in range(r):
-            e_i = np.zeros_like(w0)
-            e_i[i, 0] = step_size
-
-            for j in range(c):
-                e_j = np.zeros_like(w0)
-                e_j[j, 0] = step_size
-
-                # Calculate sensitivity change in y as well!
-                y1 = X @ (w0 + e_i + e_j)
-                y2 = X @ (w0 + e_i - e_j)
-                y3 = X @ (w0 - e_i + e_j)
-                y4 = X @ (w0 - e_i - e_j)
-
-                f1 = self._cost(X, w0 + e_i + e_j, y1)
-                f2 = self._cost(X, w0 + e_i - e_j, y2)
-                f3 = self._cost(X, w0 - e_i + e_j, y3)
-                f4 = self._cost(X, w0 - e_i - e_j, y4)
+        if self.finite_diff_flag:
+            warnings.warn(
+                "finite_diff_flag = True, evaluation of Hessian norm" " will be zero.",
+                RuntimeWarning,
+            )
 
-                hess_check[i, j] = (f1 - f2 - f3 + f4) / (4 * step_size**2)
+        w0 = w.copy().reshape(-1, 1)
+        hess_current = self.cost_hessian(X, w0, y)
+        hess_fd = self.finite_difference_hess(X, w0, y, step_size)
 
-        hess_norm = np.mean(np.linalg.norm(hess_current - hess_check, axis=1))
+        hess_norm = np.linalg.norm(hess_current - hess_fd)
 
         if self.verbose:
-            print(f"Finished! The hessian norm (row-wise) is: {np.round(hess_norm)}")
+            print(f"Finished! The hessian norm is: {hess_norm}")
 
-        return hess_current, hess_check, hess_norm
+        return hess_current, hess_fd, hess_norm
 
 
-class UserCost(CostClass):
+class ExplicitCost(CostClass):
     """
     An object that implements the general user cost function
     class. This allows the user to manually define their cost function
     and associated gradient vector and hessian. Inherits from costClass.
 
     The user is asked to define their objective function, gradient function, and
     hessian function which take in three inputs: X, w, y. This can be done using
@@ -313,263 +395,343 @@
 
     Assumed function format from user: func(X, w, y) where X is a ndarray
     with shape (n_samples, n_features), w is a ndarray with shape (n_features, 1)
     and y is the linear transformation X @ w with shape (n_samples, 1).
 
     Methods
     -------
-    cost(X, w, y)
-        This method accesses the internal self._cost instance attribute and
-        returns its output self._cost(X, w, y).
+    set_cost(cost_func)
+        This method takes in a cost_func variable and sets it as
+        an internal attribute self._cost.
 
-    cost_gradient(X, w, y)
-        This method accesses the internal self._cost_gradient instance attribute and
-        returns its output self._cost_gradient(X, w, y).
+    set_gradient(cost_gradient)
+        This method takes in a cost_gradient variable and sets it as
+        an internal attribute self._cost_gradient.
 
-    cost_hessian(X, w, y)
-        This method accesses the internal self._cost_hessian instance attribute and
-        returns its output self._cost_hessian(X, w, y).
+    set_hessian(cost_hessian)
+        This method takes in a cost_hessian variable and sets it as
+        an internal attribute self._cost_hessian.
+
+    get_cost()
+        This method returns the internal self._cost attribute.
+
+    get_gradient()
+        This method returns the internal self._cost_gradient attribute.
+
+    get_hessian()
+        This method returns the internal self._cost_hessian attribute.
     """
 
-    def __init__(self, use_hessian: bool = True, verbose: bool = True):
+    def __init__(
+        self,
+        use_hessian: bool = True,
+        verbose: bool = False,
+        finite_diff_flag: bool = False,
+    ):
         """
         Parameters
         ----------
         use_hessian : bool
             A flag to control whether you use the Hessian or not.
             This is useful in the parameter estimation step, as you may wish to just
             perform steepest descent instead of using Newton's method.
+
+        verbose : bool
+            A boolean flag to control any possible
+            print statements.
+
+        finite_diff_flag: bool
+            A boolean flag to control whether a finite difference approximation
+            is to be used for the gradient and hessian
         """
-        super().__init__(verbose)
-        self.use_hessian = use_hessian
+        super().__init__(use_hessian, verbose, finite_diff_flag)
 
-    def cost(self, X, w, y):
+    def set_cost(self, cost_func):
         """
-        A method that returns the cost function for the inputs.
+        This method allows one to set their cost function.
 
         Parameters
         ----------
-        X : ndarray
-            The feature matrix of size (n_samples, n_features)
-
-        w : ndarray
-            The transformation vector of size (n_features, 1)
+        cost_func : function
+            The users cost function.
 
-        y : ndarray
-            The transformed variable y = X @ w of size (n_samples, 1)
+        Examples
+        --------
+        cost_func = lambda X, w, y: -1 * np.mean(y ** 2, axis=0)
 
-        Returns
-        -------
-        cost function evalation of (X, w, y)
         """
-        return self._cost(X, w, y)
+        self._cost = cost_func
 
-    def cost_gradient(self, X, w, y):
+    def set_gradient(self, cost_gradient):
         """
-        A method that returns the cost function gradient for the inputs.
+        This method allows one to set their gradient vector.
 
         Parameters
         ----------
-        X : ndarray
-            The feature matrix of size (n_samples, n_features)
-
-        w : ndarray
-            The transformation vector of size (n_features, 1)
+        cost_gradient : function
+            The users gradient vector of the cost function.
 
-        y : ndarray
-            The transformed variable y = X @ w of size (n_samples, 1)
+        Examples
+        --------
+        cost_gradient = lambda X, w, y: -2 * np.mean(y * X, axis=0,
+            keepdims=True)
 
-        Returns
-        -------
-        derivative function evalation of (X, w, y)
         """
-        return self._cost_gradient(X, w, y)
+        self._cost_gradient = cost_gradient
 
-    def cost_hessian(self, X, w, y):
+    def set_hessian(self, cost_hessian):
         """
-        A method that returns the Hessian function for the inputs.
+        This method allows one to set their objective Hessian (optional).
 
         Parameters
         ----------
-        X : ndarray
-            The feature matrix of size (n_samples, n_features)
+        cost_hessian : function
+            The users gradient vector of the cost function.
 
-        w : ndarray
-            The transformation vector of size (n_features, 1)
+        Examples
+        --------
+        cost_hessian = lambda X, w, y: -2 /X.shape[0] * (X.T @ X)
 
-        y : ndarray
-            The transformed variable y = X @ w of size (n_samples, 1)
+        """
+        self._cost_hessian = cost_hessian
+
+    def get_cost(self):
+        """
+        Method to return the cost function to the user.
 
         Returns
         -------
-        Hessian function evalation of (X, w, y)
+        cost_func if attribute exists, else None.
         """
-        if self.use_hessian:
-            return self._cost_hessian(X, w, y)
+        if hasattr(self, "_cost"):
+            return self._cost
+        else:
+            return None
+
+    def get_gradient(self):
+        """
+        Method to return the derivative function to the user.
 
+        Returns
+        -------
+        cost_gradient if attribute exists, else None.
+        """
+        if hasattr(self, "_cost_gradient"):
+            return self._cost_gradient
         else:
-            return np.eye(w.shape[0])
+            return None
+
+    def get_hessian(self):
+        """
+        A method to return the hessian function to the user.
+
+        Returns
+        -------
+        cost_hessian if attribute exists, else None.
+        """
+        if hasattr(self, "_cost_hessian"):
+            return self._cost_hessian
+        else:
+            return None
 
 
-class SympyCost(CostClass):
+class SymbolicCost(CostClass):
     """
     This class implements a general user cost function class based off SymPy.
     This allows the user to manually define a symbolic representation of their
     cost function, and the necessary higher-order derivatives are calculated
-    symbolically and then lambdified.
+    symbolically.
 
     Inherits from costClass.
 
     The user is asked to define their objective function loss based off of three inputs:
-    X, w, and y. X, w, and y are sp.IndexedBase instances with a set size (based off
-    user input).
+    z, its indexable variable i, and the number of indices n, i.e. i in [0, n - 1]. In
+    code, z[i] = w^T x_i represents the latent transform of the ith x vector.
 
     This can be done using the set_ methods that are available to an instance of this
     class, which is inherited from costClass.
 
-    Assumed function format from user: func(X, w, y) where X is a ndarray
-    with shape (n_samples, n_features), w is a ndarray with shape (n_features, 1)
-    and y is the linear transformation X @ w with shape (n_samples, 1).
-
-    Note that while y is an input that is given for repeatability,
-
     Methods
     -------
-    cost(X, w, y)
-        This method accesses the internal self._cost instance attribute and
-        returns its output self._cost(X, w, y).
+    set_cost(cost_func)
+        This method takes in the symbolic expression of a users cost function and then
+        stores it as a class instance.
 
-    cost_gradient(X, w, y)
-        This method accesses the internal self._cost_gradient instance attribute and
-        returns its output self._cost_gradient(X, w, y).
+    get_sympy_parameters()
+        This method gets the indexed random variable z, its index variable i and n,
+        where n is the number of samples z[i], i = 0, ..., n - 1. Example cost function:
+        loss = -1/n * sp.Sum((z[i])**2, (i))
+
+    implement_cost()
+        This method converts the symbolic loss/cost function to a numerical form.
+
+    implement_first_derivative()
+        This method converts the symbolic derivative of the loss to a numerical form.
+
+    implement_second_derivative()
+        This method converts the symbolic second derivative (index-wise) to a numerical
+        form.
+
+    implement_methods()
+        This method runs all three implement_* methods in succession.
+
+    _cost(X, w, y)
+        This method returns the cost function value based off the symbolic loss.
+
+    _cost_gradient(X, w, y)
+        This method returns the gradient of the cost function based off the symbolic
+        loss.
+
+    _cost_hessian(X, w, y)
+        This method returns the Hessian of the cost function based off the symbolic
+        loss.
 
-    cost_hessian(X, w, y)
-        This method accesses the internal self._cost_hessian instance attribute and
-        returns its output self._cost_hessian(X, w, y).
     """
 
     def __init__(
         self,
-        n_samples: int,
-        n_features: int,
         use_hessian: bool = False,
-        verbose: bool = True,
+        verbose: bool = False,
+        finite_diff_flag: bool = False,
     ):
         """
 
         Parameters
         ----------
-        n_samples : int
-            The number of samples in X.
+        use_hessian : bool
+            A flag to control whether you use the Hessian or not.
+            This is useful in the parameter estimation step, as you may wish to just
+            perform steepest descent instead of using Newton's method.
 
-        n_features : int
-            The number of features in X.
+        verbose : bool
+            A boolean flag to control any possible
+            print statements.
 
-        use_hessian : bool (default = True)
-            A flag to specify whether the Hessian (2nd derivative) of the loss
-            function must be used. If use_hessian = False, the .cost_hessian()
-            method returns and identity matrix.
-
-        verbose : bool (default = True)
-            A flag to control the verbosity of different method calls.
-        """
-        super().__init__(verbose)
-        self.n_samples = n_samples
-        self.n_features = n_features
-        self.use_hessian = use_hessian
+        finite_diff_flag: bool
+            A boolean flag to control whether a finite difference approximation
+            is to be used for the gradient and hessian
+        """
+        super().__init__(use_hessian, verbose, finite_diff_flag)
+
+        if self.use_hessian and not self.finite_diff_flag:
+            warnings.warn(
+                "Running the Sympy cost with an exact hessian calculation can"
+                " cause significant slowdowns. You may be better off using a"
+                " finite difference or quasi-Newton approximation scheme.",
+                RuntimeWarning,
+            )
 
     def set_cost(self, cost_func):
-        # overwrites the base method
         """
         This method allows one to set their cost function (overwrites default).
 
         Parameters
         ----------
         cost_func : function
             The users cost function defined symbolically.
 
         """
         self._sympy_cost = cost_func
 
-    def get_model_parameters(self):
+        # Create the first and second derivative methods
+        self.implement_methods()
+
+    def get_symbolic_parameters(self):
         """
 
         Returns
         -------
-        X: sp.IndexedBase instance
-            An indexable SymPy matrix of size (n_samples, n_features)
+        z: sp.IndexedBase instance
+            An indexable variable that represents the transformation of the i^th
+            data vector z_i = w.T @ x_i
 
-        w:  sp.IndexedBase instance
+        i: sp.Idx instance
             An indexable SymPy matrix of size (n_features, 1)
 
-        (i, j): tuple
+        n: sp.Idx instance
             A set of index variables that can be used to iterate over
             the X and w sp.IndexedBase instances.
 
         """
-        i, j = sp.symbols("i j", cls=sp.Idx)
 
-        self.w = sp.IndexedBase("w", shape=(self.n_features, 1))
-        self.X = sp.IndexedBase("X", shape=(self.n_samples, self.n_features))
-        self.y = sp.symbols("y")  # Placeholder variable
+        # Create the size variable N
+        self.n = sp.symbols("n", integer=True)
 
-        return self.X, self.w, (i, j)
+        # Create the iteration variables i, j, k
+        self.j = sp.Idx("j", self.n)
+        self.k = sp.Idx("k", self.n)
+        self.l = sp.Idx("l", self.n)
+
+        # Create the latent variable z (to be indexed)
+        self.z = sp.IndexedBase("z")
+
+        return self.z, self.j, self.n
 
     def implement_cost(self):
         """
         A method that lambdifies the user's cost function.
         """
         print("Lambdifying the sympy cost function...")
 
-        self._cost = sp.lambdify(
-            (self.X, self.w, self.y), self._sympy_cost
-        )  # Will overwrite the sympy variable
+        self._cost_ = sp.lambdify([self.z, self.n], self._sympy_cost)
+        # Will overwrite the sympy variable
 
     def implement_first_derivative(self):
         """
         A method that symbolically computes the gradient of the user's cost function,
         and then lambdifies it so that it can be used.
 
         The call occurs by iterating over the indices of w in (0, n_features - 1),
         deriving each gradient index using SymPy's .diff() method and storing each
         gradient computation in a SymPy matrix.
         """
         if self.verbose:
-            print("Deriving and lambdifying the sympy derivative function...")
+            print("Deriving and lambdifying the sympy gradient function...")
 
-        self._first_derivative_sympy = sp.Matrix(
-            [self._sympy_cost.diff(self.w[i, 0]) for i in range(self.n_features)]
-        )
-        self._cost_gradient = sp.lambdify(
-            (self.X, self.w, self.y), self._first_derivative_sympy
-        )
+        cost_gradient = sp.diff(self._sympy_cost, self.z[self.k])
+
+        self._cost_gradient_ = sp.lambdify([self.z, self.k, self.n], cost_gradient)
+
+        # self._first_derivative_sympy = sp.Matrix(
+        #     [self._sympy_cost.diff(self.w[i, 0]) for i in range(self.n_features)]
+        # )
+        # self._cost_gradient = sp.lambdify(
+        #     (self.X, self.w, self.y), self._first_derivative_sympy
+        # )
 
     def implement_second_derivative(self):
         """
         A method that symbolically computes the Hessian of the user's cost function, and
         then lambdifies it so that it can be used.
 
         The call occurs by iterating over the indices of w in (0, n_features - 1),
         deriving the gradient vector w.r.t w[i, 0] and storing the Hessian computation
         in a SymPy matrix.
         """
         if self.verbose:
             print("Deriving and lambdifying the sympy Hessian function...")
 
         if self.use_hessian:
-            self._second_derivative_sympy = sp.BlockMatrix(
-                [
-                    self._first_derivative_sympy.diff(self.w[i, 0])
-                    for i in range(self.n_features)
-                ]
-            )
-            self._cost_hessian = sp.lambdify(
-                (self.X, self.w, self.y), self._second_derivative_sympy
+            cost_gradient = sp.diff(self._sympy_cost, self.z[self.k])
+            cost_hessian = sp.diff(cost_gradient, self.z[self.l])
+
+            self._cost_hessian_ = sp.lambdify(
+                [self.z, self.k, self.l, self.n], cost_hessian
             )
 
+            # self._second_derivative_sympy = sp.BlockMatrix(
+            #     [
+            #         self._first_derivative_sympy.diff(self.w[i, 0])
+            #         for i in range(self.n_features)
+            #     ]
+            # )
+            # self._cost_hessian = sp.lambdify(
+            #     (self.X, self.w, self.y), self._second_derivative_sympy
+            # )
+
         else:
             self._cost_hessian = lambda X, w, y: np.eye(w.shape[0])
 
     def implement_methods(self):
         """
         This method combines the implement_* methods into one call. The idea was to
         provide access to a set lambdification process through one instance call.
@@ -592,70 +754,15 @@
         else:
             print(
                 "Please first initialise the sympy cost function "
                 "using inst.set_cost()."
             )
             raise AttributeError
 
-    def _check_X(self, X):
-        """
-        This method checks the shape of X to ensure it matches the pre-defined shape
-        provided by the user.
-
-        Parameters
-        ----------
-        X : ndarray
-            The input X matrix.
-
-        Raises
-        -------
-        AssertionError
-            This is raised if the shape of X, given to and cost, cost_gradient or
-            cost_hessian call does not match the pre-defined shape given on instant
-            creation.
-
-        """
-        r, c = X.shape
-        assert r == self.n_samples, print(
-            f"Number of samples ({r}) in X  does not match the"
-            f" expected value: {self.n_samples}."
-        )
-        assert c == self.n_features, print(
-            f"Number of features ({c}) in X does not match the"
-            f" expected value: {self.n_features}."
-        )
-
-    def _check_w(self, w):
-        """
-        This method checks the shape of X to ensure it matches the pre-defined shape
-        provided by the user.
-
-        Parameters
-        ----------
-        w : ndarray
-            The input w vector.
-
-        Raises
-        -------
-        AssertionError
-            This is raised if the shape of X, given to and cost, cost_gradient or
-            cost_hessian call does not match the pre-defined shape given on instant
-            creation.
-
-        """
-        r, c = w.shape
-        assert r == self.n_features, print(
-            f"Number of samples ({r}) in w  does not match the"
-            f" expected value: {self.n_features}."
-        )
-        assert c == 1, print(
-            f"Number of features ({c}) in w does not match the" f" expected value: {1}."
-        )
-
-    def cost(self, X, w, y):
+    def _cost(self, X, w, y):
         """
         A method that returns the cost function for the inputs.
 
         Parameters
         ----------
         X : ndarray
             The feature matrix of size (n_samples, n_features)
@@ -666,23 +773,23 @@
         y : ndarray
             The transformed variable y = X @ w of size (n_samples, 1)
 
         Returns
         -------
         cost function evaluation of (X, w, y)
         """
-        self._check_X(X)
-        self._check_w(w)
 
         if not hasattr(self, "_cost"):
             self.implement_methods()  # Ensure creation of _methods.
 
-        return self._cost(X, w, y)
+        N = X.shape[0]
 
-    def cost_gradient(self, X, w, y):
+        return self._cost_(y[:, 0], N)
+
+    def _cost_gradient(self, X, w, y):
         """
         A method that returns the cost function gradient for the inputs.
 
         Parameters
         ----------
         X : ndarray
             The feature matrix of size (n_samples, n_features)
@@ -693,17 +800,25 @@
         y : ndarray
             The transformed variable y = X @ w of size (n_samples, 1)
 
         Returns
         -------
         derivative function evaluation of (X, w, y)
         """
-        return self._cost_gradient(X, w, y)
 
-    def cost_hessian(self, X, w, y):
+        N, D = X.shape
+
+        grad_vector = np.zeros((D, 1))
+
+        for i in range(N):
+            grad_vector += self._cost_gradient_(y[:, 0], i, N) * X[[i], :].T
+
+        return grad_vector
+
+    def _cost_hessian(self, X, w, y):
         """
         A method that returns the Hessian function for the inputs.
 
         Parameters
         ----------
         X : ndarray
             The feature matrix of size (n_samples, n_features)
@@ -714,75 +829,111 @@
         y : ndarray
             The transformed variable y = X @ w of size (n_samples, 1)
 
         Returns
         -------
         Hessian function evaluation of (X, w, y)
         """
-        if self.use_hessian:
-            return self._cost_hessian(X, w, y)
 
-        else:
-            return np.eye(w.shape[0])
+        N, D = X.shape
+
+        hess_mat = np.zeros((D, D))
+
+        for j in range(N):
+            x_j = X[[j], :].T
+
+            hess_inner = np.zeros((D, D))
+
+            for k in range(N):
+                x_k = X[[k], :].T
+
+                hess_inner += self._cost_hessian_(y[:, 0], j, k, N) * (x_k @ x_j.T)
+
+            hess_mat += hess_inner
+
+        return hess_mat
 
 
 class NegentropyCost(CostClass):
     """
     This class implements the Negentropy cost that is commonly applied to ICA
     via negentropy maximisation or kurtosis maximisation. Inherits from CostClass.
 
     Assumed function format: func(X, w, y) where X is a ndarray
     with shape (n_samples, n_features), w is a ndarray with shape (n_features, 1)
     and y is the linear transformation X @ w with shape (n_samples, 1).
 
     Methods
     -------
-    cost(X, w, y)
-        This method calculates and returns the negentropy approximation
-        objective function.
-
-    cost_gradient(X, w, y)
-        This method calculates and returns the gradient of the negentropy
-        approximation objective function.
+    _cost(X, w, y)
+        This method returns the cost function value for the Negentropy loss.
 
-    cost_hessian(X, w, y)
-        This method calculates and returns the Hessian of the negentropy
-        approximation objective function.
+    _cost_gradient(X, w, y)
+        This method returns the gradient of the cost function for the Negentropy
+        loss.
+
+    _cost_hessian(X, w, y)
+        This method returns the Hessian of the cost function for the Negentropy
+        loss.
     """
 
-    def __init__(self, source_name: str, source_params: dict, verbose: bool = True):
+    def __init__(
+        self,
+        source_name: str,
+        source_params: dict,
+        use_approx: bool = True,
+        use_hessian: bool = True,
+        verbose: bool = False,
+        finite_diff_flag: bool = False,
+    ):
         """
 
         Parameters
         ----------
         source_name : str
             The name of the source function used for negentropy estimation.
             Options: logcosh, exp, quad, cube
 
         source_params :  dict
             A dictionary containing the source parameter {'alpha': 1}
 
+        use_approx : bool
+            Defines whether a term in the Negentropy jacobian is approximated or not.
+            This approximation is common in the ICA approach by hyvarinen.
+
+        use_hessian : bool
+            A flag to control whether you use the Hessian or not.
+            This is useful in the parameter estimation step, as you may wish to just
+            perform steepest descent instead of using Newton's method.
+
         verbose : bool
-            Controls the verbosity of the instance.
+            A boolean flag to control any possible
+            print statements.
+
+        finite_diff_flag: bool
+            A boolean flag to control whether a finite difference approximation
+            is to be used for the gradient and hessian
         """
-        super().__init__(verbose)
+        super().__init__(use_hessian, verbose, finite_diff_flag)
+
         self.source_name = source_name
         self.source_params = source_params  # dictionary of parameters
+        self.use_approx = use_approx
 
         # Initialise the source PDFs
         self.source_instance, self.source_expectation = initialise_sources(
             source_name, self.source_params
         )
 
         # Enable compatability with CostClass
-        self.set_cost(self.cost)
-        self.set_gradient(self.cost_gradient)
-        self.set_hessian(self.cost_hessian)
+        # self.set_cost(self.cost)
+        # self.set_gradient(self.cost_gradient)
+        # self.set_hessian(self.cost_hessian)
 
-    def cost(self, X, w, y):  # Important to negentropy-based ICA
+    def _cost(self, X, w, y):  # Important to negentropy-based ICA
         """
         Negentropy-estimate calculation for the objective function.
 
         Parameters
         ----------
         X : ndarray
             The feature matrix of size (n_samples, n_features)
@@ -803,15 +954,15 @@
             EG_y = np.mean(self.source_instance.function(y))
 
         else:
             EG_y = np.mean(self.source_instance.function(y), axis=0)
 
         return -1 * (EG_y - self.source_expectation) ** 2
 
-    def cost_gradient(self, X, w, y):
+    def _cost_gradient(self, X, w, y):
         """
         A method that returns the negentropy cost function gradient for the inputs.
 
         Parameters
         ----------
         X : ndarray
             The feature matrix of size (n_samples, n_features)
@@ -822,102 +973,113 @@
         y : ndarray
             The transformed variable y = X @ w of size (n_samples, 1)
 
         Returns
         -------
         Derivative of the negetropy function evaluation using (X, w, y)
         """
+
         g_y = self.source_instance.first_derivative(y)
 
         # Calculate the expectation
         expectation = np.mean(g_y * X, axis=0, keepdims=True).T
 
         # Calculate the derivative scale with the missing term
         r = np.mean(self.source_instance.function(y)) - self.source_expectation
 
         # Calculate the gradient vector
         grad_vector = -2 * r * expectation
 
         return grad_vector
 
-    def cost_hessian(self, X, w, y, approx_flag=True):
+    def _cost_hessian(self, X, w, y):
         """
         A method that returns the negentropy cost function Hessian for the inputs.
 
         Parameters
         ----------
         X : ndarray
             The feature matrix of size (n_samples, n_features)
 
         w : ndarray
             The transformation vector of size (n_features, 1)
 
         y : ndarray
             The transformed variable y = X @ w of size (n_samples, 1)
 
-        approx_flag : bool (default = True)
-            This flag specifies whether an approximation to the expectation in the
-            Hessian is used or not.
-
         Returns
         -------
         Hessian of the negentropy function evaluation using (X, w, y)
         """
         N, m = X.shape
 
         # Compute g'(y)
         g_prime_y = self.source_instance.second_derivative(y)
 
+        # Calculate the gradient vector
+        negentropy_gradient = self.cost_gradient(X, w, y)
+
+        # Calculate the scalar r term
+        r = np.mean(self.source_instance.function(y)) - self.source_expectation
+
         # t0 = time.time()
-        if approx_flag:
+        if self.use_approx:
             # t0 = time.time()
             expectation = np.mean(g_prime_y) * np.eye(m)
         # t1 = time.time()
 
         else:
+            negentropy_gradient /= -2 * r
             expectation = np.zeros((m, m))
 
             for n in range(N):
                 expectation += np.dot(X[[n], :].T, X[[n], :]) * g_prime_y[n]
 
             expectation /= N
 
-        # Calculate the gradient vector
-        negentropy_gradient = self.cost_gradient(X, w, y)
-
-        # Calculate the scalar r term
-        r = np.mean(self.source_instance.function(y)) - self.source_expectation
-
         # Calculate the gradient outer product
         grad_outer = negentropy_gradient @ negentropy_gradient.T
 
         # Calculate the Jacobian (Hessian)
         jacobian = -2 * (grad_outer + r * expectation)
 
         return jacobian
 
 
-class VarianceCost(UserCost):
+class VarianceCost(ExplicitCost):
     """
     This method implements the PCA variance maximisation objective. It inherits from
     the UserCost class and simply implements the three necessary components.
     """
 
-    def __init__(self, use_hessian: bool = True, verbose: bool = True):
+    def __init__(
+        self,
+        use_hessian: bool = True,
+        verbose: bool = False,
+        finite_diff_flag: bool = False,
+    ):
         """
         Defines the attributes for the user_cost class
 
         Parameters
         ----------
         use_hessian : bool
             A flag to control whether you use the Hessian or not.
             This is useful in the parameter estimation step, as you may wish to just
             perform steepest descent instead of using Newton's method.
+
+        verbose : bool
+            A boolean flag to control any possible
+            print statements.
+
+        finite_diff_flag: bool
+            A boolean flag to control whether a finite difference approximation
+            is to be used for the gradient and hessian
         """
-        super().__init__(use_hessian, verbose)
+        super().__init__(use_hessian, verbose, finite_diff_flag)
 
         def loss(X, w, y):
             """
             The PCA variance maximisation cost function for an optimisation
             framework which performs minimisation.
 
             Parameters
@@ -975,15 +1137,17 @@
             y : ndarray
                 The transformed variable y = X @ w of size (n_samples, 1)
 
             Returns
             -------
             Hessian of the negative of latent variance.
             """
-            return -2 * np.cov(X, rowvar=False)
+            N = X.shape[0]
+
+            return -2 / N * (X.T @ X)
 
         self.set_cost(loss)
         self.set_gradient(grad)
         self.set_hessian(hess)
 
 
 # if __name__ == "__main__":
```

### Comparing `spectrally_regularised_lvms-0.1.2/spectrally_regularised_LVMs/helper_methods.py` & `spectrally_regularised_lvms-0.1.3/spectrally_regularised_LVMs/helper_methods.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2023-present Ryan Balshaw
 """
 The helper methods for the solver.
 
 Method 1: data_processor
-    This method implements the pre-processing steps applied to X (standardisation
+    This method implements the pre-processing steps applied to X (centering
     and/or whitening).
 
 Method 2: batch_sampler
     This is a simple batch sampler method for quicker solving.
 
 Method 3: quasi_Newton
     This is a method that implements different Hessian approximation strategies.
@@ -28,19 +28,19 @@
     """
     A method that processes the data matrices.
 
     Methods
     -------
     initialise_preprocessing(X)
         A method that initialises all the processing attributes
-        for the pre-processing (standardising with whitening). Solves
+        for the pre-processing (centering with whitening). Solves
         for the whitening transform parameters.
 
-    standardise_data(X)
-        Standardises the columns of X to be zero-mean and unit-variance.
+    center_data(X)
+        Centers the columns of X to be zero-mean.
 
     preprocess_data(X)
         Transforms the X matrix to the whitened space (if required).
 
     unprocess_data(X)
         Transforms an X matrix from the whitened space to the data space.
     """
@@ -74,25 +74,22 @@
         -------
         self
         """
 
         # Extract Nsamples and Nfeatures
         Ns, Nf = X.shape
 
-        # Get the mean and standard deviation (always automatically z-score)
+        # Get the feature-wise means
         self.mean_ = np.mean(X, axis=0, keepdims=True)
-        self.std_ = np.std(X, axis=0, keepdims=True)
 
         if self.whiten:
             # Decompose X
             # rows of Vh are the eigenvectors of A^H A (i.e., Vh = U^T)
             # Columns of U are eigenvectors of A A^H
-            U, s, Vh = np.linalg.svd(
-                (copy.deepcopy(X) - self.mean_) / self.std_, full_matrices=False
-            )
+            U, s, Vh = np.linalg.svd(copy.deepcopy(X) - self.mean_, full_matrices=False)
 
             eigenvalues = s**2 / (Ns - 1)
 
             if self.var_PCA is not None:
                 # TODO improve var_PCA option
 
                 cumsum = np.cumsum(eigenvalues / np.sum(eigenvalues))
@@ -116,32 +113,32 @@
         else:
             self.Vh = np.eye(Nf)
             self.latent_transform = np.eye(Nf)
             self.recover_transform = np.eye(Nf)
 
         return self
 
-    def standardise_data(self, X):
+    def center_data(self, X):
         """
-        A method that standardises the row of the data matrix X
+        A method that centers the rows of the data matrix X
 
         Parameters
         ----------
         X: ndarray
             The original feature matrix X.
 
         Returns
         -------
-        X_standardised: ndarray
-            Zero-mean, unit variance feature matrix.
+        X_centered: ndarray
+            Zero-mean feature matrix.
         """
 
-        X_standardised = (X - self.mean_) / self.std_
+        X_centered = X - self.mean_
 
-        return X_standardised
+        return X_centered
 
     def preprocess_data(self, X):
         """
         A method that pre-processes the data matrix X
 
         Parameters
         ----------
@@ -149,18 +146,18 @@
             The original feature matrix X.
 
         Returns
         -------
         X_whitened: ndarray
             The whitened feature matrix.
         """
-        X_standardised = self.standardise_data(X)
+        X_centered = self.center_data(X)
 
-        X_whitened = (X_standardised @ self.latent_transform.T) @ self.Vh
-        # X_whitened = np.dot(X_standardised, self.latent_transform.T)
+        X_whitened = (X_centered @ self.latent_transform.T) @ self.Vh
+        # X_whitened = np.dot(X_centered, self.latent_transform.T)
 
         return X_whitened
 
     def unprocess_data(self, X):
         """
         A method that un-whitens the whitened data matrix X
 
@@ -171,15 +168,14 @@
 
         Returns
         -------
         X_unwhitened: ndarray
             The un-whitened feature matrix
         """
         X_unwhitened = np.dot(np.dot(X, self.recover_transform.T), self.Vh)
-        # X_unwhitened = np.dot(X, self.recover_transform.T)
 
         return X_unwhitened
 
 
 class BatchSampler(object):
     """
     This is a simple iterator instance that can be called during runtime using:
```

### Comparing `spectrally_regularised_lvms-0.1.2/spectrally_regularised_LVMs/negen_approx.py` & `spectrally_regularised_lvms-0.1.3/spectrally_regularised_LVMs/negen_approx.py`

 * *Files identical despite different names*

### Comparing `spectrally_regularised_lvms-0.1.2/spectrally_regularised_LVMs/spectral_regulariser.py` & `spectrally_regularised_lvms-0.1.3/spectrally_regularised_LVMs/spectral_regulariser.py`

 * *Files identical despite different names*

### Comparing `spectrally_regularised_lvms-0.1.2/spectrally_regularised_LVMs/spectrally_regularised_model.py` & `spectrally_regularised_lvms-0.1.3/spectrally_regularised_LVMs/spectrally_regularised_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 from .cost_functions import CostClass
 from .helper_methods import (
     BatchSampler,
     DataProcessor,
     DeflationOrthogonalisation,
     QuasiNewton,
+    hankel_matrix,
 )
 from .spectral_regulariser import SpectralObjective
 
 
 def initialise_W(n_sources: int, n_features: int, init_type: str):
     """
     A method that initialises the W matrix.
@@ -163,40 +164,48 @@
         dictionary and X (X defines the pre-processing steps).
     """
 
     def __init__(
         self,
         n_sources: int,  # keep
         cost_instance: cost_inst,
+        Lw: int,
+        Lsft: int,
         whiten: bool = True,  # keep
         init_type: str = "broadband",
         perform_gso: bool = True,
         batch_size: int | None = None,
         var_PCA: bool | None = None,
         alpha_reg: float = 1.0,
         sumt_flag: bool = False,
         sumt_parameters: dict[str, float] | None = None,
         organise_by_kurt: bool = False,
         hessian_update_type: str = "actual",
         use_ls: bool = True,
-        use_hessian: bool = True,
+        second_order: bool = True,
         save_dir: str | None = None,
         verbose: bool = False,
     ):
         """
         The initialisation of the linear_model class.
 
         Parameters
         ----------
         n_sources : int
             The number of latent sources that are to be estimated.
 
         cost_instance : instance which inherits from CostClass
             The objective function instance that the user chooses.
 
+        Lw : int
+            The window length of the hankel matrix signal segments
+
+        Lsft : int
+            The shift parameter for the hankel matrix.
+
         whiten : bool (default = True)
             Specifies whether the data matrix X is to be whitened. By default, all X
             matrices are standardised.
 
         init_type : str (default = 'broadband')
             The initialisation strategy for W. Options are 'broadband' or 'random'.
             'broadband' sets each w vector to a dirac delta, while 'random' randomly
@@ -238,30 +247,32 @@
             estimation or if quasi-Newton strategies are to be employed. Options
             are: 'actual', 'SR1', 'DFP', 'BFGS'.
 
         use_ls : bool (default = True)
             A flag that specifies whether a linear line search is to be performed
             on the .
 
-        use_hessian : bool (default = True)
+        second_order : bool (default = True)
             This flag specifies whether a second or first order optimisation method
-            is used. If use_hessian = False then the method defaults to gradient
+            is used. If second_order = False then the method defaults to gradient
             descent.
 
         save_dir : str | None (default = None)
             Defines whether visualisation of the parameter estimation properties are
             to be stored in some directory. If a string is entered, this string is
             expected to be the directory in which the figures are to be saved.
 
         verbose : bool (default = False)
             Defines the verbosity mode for the parameter estimation step.
         """
         # Initialise instances
         self.n_sources = n_sources
-        self.cost_instance = cost_instance  # ({'source_name':'exp', 'alpha':1})
+        self.cost_instance = cost_instance
+        self.Lw = Lw
+        self.Lsft = Lsft
         self.whiten = whiten
         self.var_PCA = var_PCA
         self.init_type = init_type.lower()
         self.organise_by_kurt = (
             organise_by_kurt  # A flag used to organise the ICA components
         )
         self.perform_gso = perform_gso
@@ -269,18 +280,21 @@
         self.alpha_reg = alpha_reg
         self.sumt_flag = sumt_flag  # SUMT approach to alpha_reg
         self.sumt_parameters = sumt_parameters  # Parameters for SUMT updating
         self.hessian_update_type = (
             hessian_update_type.lower()
         )  # Type of jacobian update
         self.use_ls = use_ls
-        self.use_hessian = use_hessian
+        self.second_order = second_order
         self.save_dir = save_dir
         self.verbose = verbose
 
+        # Turn off the cost instance verbosity
+        self.cost_instance.verbose = False
+
         # Sequential unconstrained minimisation technique parameters
         if self.sumt_flag:
             if self.sumt_parameters is None:  # Initialise
                 self.sumt_parameters = {
                     "alpha_init": 0.1,
                     "alpha_end": 100,
                     "alpha_multiplier": 10,
@@ -291,26 +305,26 @@
                 "alpha_end"
             ]  # Overrides the default value
             self.alpha_multiplier = self.sumt_parameters["alpha_multiplier"]
 
             self.alpha_cnt = 0
 
         # Quasi-Newton solvers
-        if self.hessian_update_type != "actual":
+        if self.hessian_update_type != "actual" and self.second_order:
             self.quasi_newton_inst = QuasiNewton(
                 self.hessian_update_type, use_inverse=True
             )
             print("Using a quasi-Newton iteration scheme.")
 
-        if self.hessian_update_type != "actual" and self.use_hessian:
-            print(
-                "Selected quasi-Newton scheme but opted to "
-                "not use hessian in update step."
-                "\nDefaulting to quasi-Newton scheme."
-            )
+        # Adjust second order flag in cost instance
+        if self.second_order:
+            self.cost_instance.use_hessian = True
+
+        else:
+            self.cost_instance.use_hessian = False
 
         if type(self.n_sources) != int:
             print("Please enter in a valid number of sources.")
             raise SystemExit
 
         if not self.whiten:
             if self.cost_instance.__class__.__name__ == "NegentropyCost":
@@ -324,14 +338,17 @@
         # Initialise the processor instance  (could be in base class except for var_PCA)
         self.processor_inst = DataProcessor(self.whiten, self.var_PCA)
 
         if self.perform_gso:
             # Initialise the orthogonalisation instance (could be in base class)
             self.gs_inst = DeflationOrthogonalisation()
 
+    def get_hankel(self, x_signal):
+        return hankel_matrix(x_signal.squeeze(), self.Lw, self.Lsft)
+
     def kurtosis(self, y):
         """
 
         Parameters
         ----------
         y : ndarray
             A vector or matrix of samples. If y is a vector, it is expected to be
@@ -772,15 +789,15 @@
         """
         # Define flag that allows for solver re-initialisation
         self._reinit_flag = False
 
         # Calculate the gradient
         gradient = self.lagrange_gradient(X, w, y, W, idx, lambda_vector)
 
-        if self.use_hessian:
+        if self.second_order:
             if self.hessian_update_type == "actual":
                 jacobian = self.lagrange_hessian(X, w, y, W, idx, lambda_vector)
 
                 # Compute the update
                 delta = -1 * np.linalg.solve(jacobian, gradient)
 
             else:
@@ -808,15 +825,15 @@
         # Scale delta by alpha
         delta = alpha_multiplier * delta
 
         # Split into W and Lambda updates
         delta_w, delta_lambda = delta[: w.shape[0], [0]], delta[w.shape[0] :, [0]]
 
         # Compute quasi-Newton updates, if required
-        if self.hessian_update_type != "actual" and self.use_hessian:
+        if self.hessian_update_type != "actual" and self.second_order:
             if conv_flag:  # Compute quasi-Newton updates.
                 # Compute the new parameters
                 w_new, lambda_new = self.update_params(
                     w.copy(), lambda_vector.copy(), delta_w, delta_lambda, W, idx
                 )
 
                 # Compute gradient_diff_k
@@ -837,15 +854,15 @@
 
                 self.quasi_newton_inst.initialise_jacobian(
                     delta.shape[0]
                 )  # Re-initialise the Jacobian
 
         return delta_w, delta_lambda, gradient
 
-    def spectral_trainer(self, X, W, n_iters, learning_rate, tol, Lambda, Fs):
+    def spectral_trainer(self, X, W, n_iters, learning_rate, tol, use_tol, Lambda, Fs):
         """
         This method estimates the model parameters for some X and W.
 
         Parameters
         ----------
         X : ndarray
             The data matrix X.
@@ -860,14 +877,18 @@
                 A learning rate. This is only used if required by the user, and will
                 only appear if use_ls is not activated.
 
         tol : float
                 The tolerance on the convergence error, error =| w_new^T @ w_prev - 1|.
                 Used to stop the solver if it converges.
 
+        use_tol : bool
+                A flag to specify if the convergence tolerance must be used.
+                If use_tol = False, the process will run for n_iters each time.
+
         Lambda : ndarray
                 A vector of lambda parameters for the Lagrange expressions.
 
         Fs : float
                 The sampling frequency of the observed signal. Only used if the user
                 wants to store visualisations of the solution vectors.
 
@@ -994,18 +1015,17 @@
                     pbar.set_description(
                         f"Component {idx + 1} - " f"Error: {np.round(error, 6)}"
                     )
 
                 # Update counter
                 self.cnt_iter += 1
 
-                if self._reinit_flag:
-                    error = (
-                        np.inf
-                    )  # Stops solver from terminating on quasi-Newton re-initialisation
+                if self._reinit_flag or not use_tol:
+                    # Stops solver from terminating on quasi-Newton re-initialisation
+                    error = np.inf
 
             if self.save_dir is not None:
                 fig, ax = plt.subplots(4, 2, figsize=(8, 12))
                 ax = ax.flatten()
 
                 # Create the FFT properties
                 n = w_new.shape[0]
@@ -1131,14 +1151,15 @@
     def spectral_fit(
         self,
         X,
         W,
         n_iters=1,
         learning_rate=0.1,
         tol=1e-3,
+        use_tol=True,
         Lambda=None,
         Fs: float | int = 25e3,
     ):
         """
         This method estimates the model parameters for some given X, W, and Lambda.
 
         Parameters
@@ -1156,14 +1177,18 @@
                 A learning rate. This is only used if required by the user, and will
                 only appear if use_ls is not activated.
 
         tol : float
                 The tolerance on the convergence error, error =| w_new^T @ w_prev - 1|.
                 Used to stop the solver if it converges.
 
+        use_tol : bool
+                A flag to specify if the convergence tolerance must be used.
+                If use_tol = False, the process will run for n_iters each time.
+
         Lambda : ndarray
                 A vector of lambda parameters for the Lagrange expressions.
 
         Fs : float
                 The sampling frequency of the observed signal. Only used if the user
                 wants to store visualisations of the solution vectors.
 
@@ -1174,15 +1199,15 @@
 
         Lambda_update : ndarray
                 The estimated Lambda values.
 
         """
         # Call the spectral trainer
         W_update, Lambda_update = self.spectral_trainer(
-            X, W, n_iters, learning_rate, tol, Lambda, Fs
+            X, W, n_iters, learning_rate, tol, use_tol, Lambda, Fs
         )
 
         # Calculate the excess kurtosis
         Y = np.dot(X, W_update.T)
         kurt = np.mean(Y**4, axis=0) - 3  # Excess kurtosis
 
         if self.organise_by_kurt:
@@ -1223,54 +1248,62 @@
             plt.savefig(os.path.join(self.save_dir, save_name))
             plt.close("all")
 
         return W_update, Lambda_update
 
     def fit(
         self,
-        X,
-        n_iters=100,
-        learning_rate=1,
-        tol=1e-4,
-        Fs: int | float = 25e3,
+        x_signal,
+        n_iters: int = 500,
+        learning_rate: float = 1.0,
+        tol: float = 1e-4,
+        use_tol: bool = True,
+        Fs: float = 1.0,
     ):
         """
         This method follows the scikit-learn API call and estimates the model parameters
         based off the users initialisation choices.
 
         Parameters
         ----------
-        X : ndarray
-            The data matrix X.
+        x_signal : ndarray
+                        The single channel vibration data signal.
 
         n_iters : int
                         The max number of iterations that are to be performed for each
                         source.
 
         learning_rate : float
-                        A learning rate. This is only used if required by the user, and
-                        will only appear if use_ls is not activated.
+                        The learning rate. This is only used if required by the user,
+                        and will only appear if use_ls is not activated.
 
         tol : float
                         The tolerance on the convergence error,
                         error =| w_new^T @ w_prev - 1|. Used to stop the solver
                         if it converges.
 
+        use_tol : bool
+                        A flag to specify if the convergence tolerance must be used.
+                        If use_tol = False, the process will run for n_iters each time.
+
         Fs : float
                         The sampling frequency of the observed signal. Only used if
                         the user wants to store visualisations of the solution vectors.
 
         Returns
         -------
         self : instance
                         This method returns self so that it can be chained onto the
                         initialisation of the class via
                         model_inst = LinearModel(...).fit(...).
 
         """
+        # Hankelise data
+        X = self.get_hankel(x_signal)
+
         # Initialise pre-processing
         self.processor_inst.initialise_preprocessing(X)
 
         # Pre-process the data
         X_preprocess = self.processor_inst.preprocess_data(X)
 
         # Get number of sources
@@ -1306,14 +1339,15 @@
             while self.alpha_reg <= self.alpha_end:
                 W_update, Lambda_update = self.spectral_fit(
                     X_preprocess,
                     W_iters[-1],
                     n_iters,
                     learning_rate,
                     tol,
+                    use_tol,
                     lambda_iters[-1],
                     Fs,
                 )
 
                 # Store solution and parameters
                 param_iters.append(
                     (
@@ -1387,14 +1421,15 @@
         else:
             W_update, Lambda_update = self.spectral_fit(
                 X_preprocess,
                 W,
                 n_iters,
                 learning_rate,
                 tol,
+                use_tol,
                 Lambda,
                 Fs,
             )
 
             # Store the parameters
             self.W = W_update
             self.Lambda = Lambda_update
@@ -1403,62 +1438,75 @@
         # Compute the excess kurtosis of the model
         Y = np.dot(X_preprocess, self.W.T)
 
         self.excess_kurtosis_ = np.mean(Y**4, axis=0) - 3  # Excess kurtosis
 
         return self
 
-    def transform(self, X):
+    def transform(self, x_signal):
         """
         This method transforms a data matrix X to the latent space.
 
         Parameters
         ----------
-        X : ndarray
-            The data matrix X.
+        x_signal : ndarray
+            The single channel vibration data signal.
 
         Returns
         -------
         Z : ndarray
             The projection of X to the latent space.
         """
+        # Hankelise data
+        X = self.get_hankel(x_signal)
 
+        # Transform the latent space
         Z = self.processor_inst.preprocess_data(X) @ self.W.T
 
         return Z
 
-    def inverse_transform(self, Z, full_inverse: bool = False):
+    def inverse_transform(self, Z, full_inverse: bool = True):
         """
-        This method transforms a latent matrix X to the latent space.
+        This method transforms a latent matrix Z to the data space.
 
         Parameters
         ----------
         Z : ndarray
             The latent matrix Z.
 
         full_inverse : bool
             A flag to specify whether the recovered data matrix X must be
-            returned in standardised form or in the original, un-standardised
+            returned in centered form or in the original, un-centered
             domain.
 
         Returns
         -------
         X_recon : ndarray
             The reconstruction of X from the latent matrix Z.
         """
         Z_ = Z.copy()
 
         # Transform back to the training feature space
-        X_recon = np.dot(Z_, self.W)
 
-        # Un-process the data (still zero-mean, unit-variance)
+        # Compute the (Moore-Penrose) pseudo-inverse of a matrix.
+        # For the orthonormal case, the inverse is just equal to W^T.
+        # See: https://w.wiki/72DE
+        if self.perform_gso:
+            X_recon = np.dot(Z_, self.W)
+
+        else:
+            pinv = np.linalg.pinv(self.W)
+
+            X_recon = Z_ @ pinv.T
+
+        # Un-process the data (still zero-mean)
         X_recon = self.processor_inst.unprocess_data(X_recon)
 
-        if full_inverse:
-            X_recon = (X_recon * self.processor_inst.std_) + self.processor_inst.mean_
+        if full_inverse:  # Recover the mean
+            X_recon = X_recon + self.processor_inst.mean_
 
         return X_recon
 
     @staticmethod
     def compute_spectral_W(W):
         """
         This method computes the spectral representation of the vectors in the W
@@ -1526,15 +1574,15 @@
                     np.log10(self.sumt_parameters["alpha_end"]) + 1,
                     1,
                 )
             )
 
         return dict_params
 
-    def set_model_parameters(self, X, dict_params: dict):
+    def set_model_parameters(self, x_signal, dict_params: dict):
         """
         This method takes the X matrix and a parameter dictionary, initialises the
         pre-processing components and then creates the necessary class attributes
         from the dictionary.
 
         Parameters
         ----------
@@ -1548,14 +1596,16 @@
         Returns
         -------
         self : instance
                 This method returns self so that it can be chained onto the
                 initialisation of the class via
                 model_inst = LinearModel(...).set_model_parameters(...).
         """
+        # Hankelise data
+        X = self.get_hankel(x_signal)
 
         # Initialise pre-processing
         self.processor_inst.initialise_preprocessing(X)
 
         # Store dictionary
         for k, v in dict_params.items():
             setattr(self, k, v)
```

### Comparing `spectrally_regularised_lvms-0.1.2/PKG-INFO` & `spectrally_regularised_lvms-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: spectrally-regularised-lvms
-Version: 0.1.2
-Summary: An implementation of linear LVMs with a spectral regulariser.
+Version: 0.1.3
+Summary: A framework of linear LVMs with spectral regularisation.
 Home-page: https://github.com/RyanBalshaw/spectrally-regularised-LVMs
 License: MIT
 Keywords: Linear LVMs,Spectral regularisation,Python
 Author: Ryan Balshaw
 Author-email: ryanbalshaw81@gmail.com
 Maintainer: Ryan Balshaw
 Maintainer-email: ryanbalshaw81@gmail.com
@@ -33,52 +33,53 @@
 ![GitHub license](https://img.shields.io/github/license/RyanBalshaw/spectrally-regularised-LVMs)
 ![GitHub last commit](https://img.shields.io/github/last-commit/RyanBalshaw/spectrally-regularised-LVMs)
 ![PyPI](https://img.shields.io/pypi/v/spectrally-regularised-lvms)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/spectrally-regularised-lvms?color=blueviolet)
 ![Read the Docs](https://img.shields.io/readthedocs/spectrally-regularised-lvms?color=informational)
 ![GitHub issues](https://img.shields.io/github/issues/RyanBalshaw/spectrally-regularised-LVMs?color=critical)
 
-*Current version:* 0.1.1
-
-Spectrally-regularised-LVMs is a Python-based package which facilitates the estimation of the linear latent variable model (LVM) parameters with a unique spectral regularisation term in single channel time-series applications.
+*Spectrally-regularised-LVMs* is a Python-based [package](https://pypi.org/project/spectrally-regularised-lvms/) which facilitates the estimation of the linear latent variable model (LVM) parameters with a unique spectral regularisation term in single channel time-series applications.
 
 ## Purpose
-LVMs are a statistical methodology which tries to capture the underlying structure in some observed data. This package caters to single channel time-series applications and provides a methodology to estimate the LVM parameters. The model parameters are encouraged to be diverse via a spectral regularisation term which penalises source duplication of the spectral information captured by the latent sources.
+LVMs are a statistical methodology which try to capture the underlying structure in some observed data. This package caters to single channel time-series applications and provides a methodology to estimate the LVM parameters. The model parameters are encouraged to capture non-duplicate information via a spectral regularisation term which penalises source duplication of the spectral information captured by the latent sources.
 
-The purpose of this package is to provide a complete methodology that caters to a variety of LVM objective functions.
+The purpose of this package is to provide a complete framework for LVMs with spectral regularisation that caters to a variety of LVM objective functions.
 
 # Documentation
-Please visit [the docs](http://spectrally-regularised-lvms.readthedocs.io/) for all supporting documentation for this package.
+Please visit the [documentation](http://spectrally-regularised-lvms.readthedocs.io/) page for all supporting documentation for this package.
 
 # Installation
 The package is designed to be used through the Python API, and  can be installed using [pip](https://pypi.org/project/pip/):
 ```console
 $ pip install spectrally-regularised-LVMs
 ```
 
+A more detailed discussion regarding installation is given in the [documentation](http://spectrally-regularised-lvms.readthedocs.io/).
+
 # Requirements
 
 This package used Python ≥ 3.10 or later to run. For other python dependencies, please check the `pyproject.toml`
 [file](https://github.com/RyanBalshaw/spectrally-regularised-LVMs/blob/main/pyproject.toml) included in this repository. The dependencies of this package are as follows:
 
-|          Package                   	           | Version 	  |
-|:----------------------------------------------:|:----------:|
-|    [Python](https://www.python.org/)      	    | ≥ 3.10  	  |
-|     [Numpy](https://numpy.org/)         	      | ≥ 1.23.1 	 |
-|   [Matplotlib](https://matplotlib.org/)    	   | ≥ 3.5.2 	  |
-|     [SciPy](https://scipy.org/)         	      | ≥ 1.8.1 	  |
-|  [scikit-learn](https://scikit-learn.org/)  	  | ≥ 1.1.2 	  |
-|   [tqdm](https://github.com/tqdm/tqdm)     	   | ≥ 4.64.1 	 |
-| [SymPy](https://www.sympy.org/en/index.html) 	 | ≥ 1.1.1 	  |
+|           Package                   	           | Version 	  |
+|:-----------------------------------------------:|:----------:|
+|    [Python](https://www.python.org/)      	     | ≥ 3.10  	  |
+|      [Numpy](https://numpy.org/)         	      | ≥ 1.23.1 	 |
+|   [Matplotlib](https://matplotlib.org/)    	    | ≥ 3.5.2 	  |
+|      [SciPy](https://scipy.org/)         	      | ≥ 1.8.1 	  |
+|  [scikit-learn](https://scikit-learn.org/)  	   | ≥ 1.1.2 	  |
+|   [tqdm](https://github.com/tqdm/tqdm)     	    | ≥ 4.64.1 	 |
+| [SymPy](https://www.sympy.org/en/index.html) 	  | ≥ 1.1.1 	  |
+| [Poetry](https://python-poetry.org/) 	 | ≥ 1.4 	  |
 
 # API usage
 Please visit [the docs](http://spectrally-regularised-lvms.readthedocs.io/) for all supporting API documentation for this package.
 
 # Contributing
-This package uses [Poetry](https://python-poetry.org/) for dependency management and Python packaging and [git](https://git-scm.com/) for version control. To get started, first install git and Poetry and then clone this repository via
+This package uses [Poetry](https://python-poetry.org/) for dependency management and Python packaging and [git](https://git-scm.com/) for version control. To get started, first install git and Poetry. Then one may clone this repository via
 ```console
 $ git clone git@github.com:RyanBalshaw/spectrally-regularised-LVMs.git
 $ cd spectrally-regularised-LVMs
 ```
 
 Then, install the necessary dependencies in a local environment via
 ```console
```

