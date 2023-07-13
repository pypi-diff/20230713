# Comparing `tmp/wecopttool-2.5.0.tar.gz` & `tmp/wecopttool-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wecopttool-2.5.0.tar", last modified: Sun May 21 07:14:41 2023, max compression
+gzip compressed data, was "wecopttool-2.6.0.tar", last modified: Thu Jul 13 20:53:49 2023, max compression
```

## Comparing `wecopttool-2.5.0.tar` & `wecopttool-2.6.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:14:41.319364 wecopttool-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-21 07:14:27.000000 wecopttool-2.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-21 07:14:27.000000 wecopttool-2.5.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-21 07:14:41.319364 wecopttool-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-21 07:14:27.000000 wecopttool-2.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-21 07:14:27.000000 wecopttool-2.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 07:14:41.319364 wecopttool-2.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:14:41.315364 wecopttool-2.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    55413 2023-05-21 07:14:27.000000 wecopttool-2.5.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-05-21 07:14:27.000000 wecopttool-2.5.0/tests/test_hydrostatics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12237 2023-05-21 07:14:27.000000 wecopttool-2.5.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-05-21 07:14:27.000000 wecopttool-2.5.0/tests/test_pto.py
--rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-05-21 07:14:27.000000 wecopttool-2.5.0/tests/test_waves.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:14:41.315364 wecopttool-2.5.0/wecopttool/
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-21 07:14:27.000000 wecopttool-2.5.0/wecopttool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    85594 2023-05-21 07:14:27.000000 wecopttool-2.5.0/wecopttool/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-05-21 07:14:27.000000 wecopttool-2.5.0/wecopttool/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-05-21 07:14:27.000000 wecopttool-2.5.0/wecopttool/hydrostatics.py
--rw-r--r--   0 runner    (1001) docker     (123)    34338 2023-05-21 07:14:27.000000 wecopttool-2.5.0/wecopttool/pto.py
--rw-r--r--   0 runner    (1001) docker     (123)    18012 2023-05-21 07:14:27.000000 wecopttool-2.5.0/wecopttool/waves.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 07:14:41.315364 wecopttool-2.5.0/wecopttool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-21 07:14:41.000000 wecopttool-2.5.0/wecopttool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-21 07:14:41.000000 wecopttool-2.5.0/wecopttool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 07:14:41.000000 wecopttool-2.5.0/wecopttool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-21 07:14:41.000000 wecopttool-2.5.0/wecopttool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-21 07:14:41.000000 wecopttool-2.5.0/wecopttool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:53:49.040675 wecopttool-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-13 20:53:36.000000 wecopttool-2.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-13 20:53:36.000000 wecopttool-2.6.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-13 20:53:49.040675 wecopttool-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-13 20:53:36.000000 wecopttool-2.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-13 20:53:36.000000 wecopttool-2.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 20:53:49.040675 wecopttool-2.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:53:49.036675 wecopttool-2.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    57162 2023-07-13 20:53:36.000000 wecopttool-2.6.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-13 20:53:36.000000 wecopttool-2.6.0/tests/test_hydrostatics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12237 2023-07-13 20:53:36.000000 wecopttool-2.6.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-07-13 20:53:36.000000 wecopttool-2.6.0/tests/test_pto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-07-13 20:53:36.000000 wecopttool-2.6.0/tests/test_waves.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:53:49.040675 wecopttool-2.6.0/wecopttool/
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-07-13 20:53:36.000000 wecopttool-2.6.0/wecopttool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87143 2023-07-13 20:53:36.000000 wecopttool-2.6.0/wecopttool/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-07-13 20:53:36.000000 wecopttool-2.6.0/wecopttool/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-07-13 20:53:36.000000 wecopttool-2.6.0/wecopttool/hydrostatics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34512 2023-07-13 20:53:36.000000 wecopttool-2.6.0/wecopttool/pto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18012 2023-07-13 20:53:36.000000 wecopttool-2.6.0/wecopttool/waves.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:53:49.040675 wecopttool-2.6.0/wecopttool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-13 20:53:49.000000 wecopttool-2.6.0/wecopttool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-13 20:53:49.000000 wecopttool-2.6.0/wecopttool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 20:53:49.000000 wecopttool-2.6.0/wecopttool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-13 20:53:49.000000 wecopttool-2.6.0/wecopttool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 20:53:49.000000 wecopttool-2.6.0/wecopttool.egg-info/top_level.txt
```

### Comparing `wecopttool-2.5.0/LICENSE` & `wecopttool-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wecopttool-2.5.0/NOTICE` & `wecopttool-2.6.0/NOTICE`

 * *Files identical despite different names*

### Comparing `wecopttool-2.5.0/PKG-INFO` & `wecopttool-2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wecopttool
-Version: 2.5.0
+Version: 2.6.0
 Summary: WEC Design Optimization Toolbox
 Author: Sandia National Laboratories
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Documentation, https://sandialabs.github.io/WecOptTool/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `wecopttool-2.5.0/README.md` & `wecopttool-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `wecopttool-2.5.0/pyproject.toml` & `wecopttool-2.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wecopttool"
-version = "2.5.0"
+version = "2.6.0"
 description = "WEC Design Optimization Toolbox"
 readme = "README.md"
 authors = [
     {name = "Sandia National Laboratories"},
 ]
 urls = {Documentation = "https://sandialabs.github.io/WecOptTool/"}
 requires-python = ">=3.8"
```

### Comparing `wecopttool-2.5.0/tests/test_core.py` & `wecopttool-2.6.0/tests/test_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -929,41 +929,79 @@
 
     @pytest.fixture(scope="class")
     def tol(self, data):
         """Tolerance for function :python:`check_linear_damping`."""
         return 0.01
 
     @pytest.fixture(scope="class")
-    def data_new(self, data, tol):
+    def data_new_uniform(self, data, tol):
         """Hydrodynamic data structure for which the function
         :python:`check_linear_damping` has been called.
         """
         return wot.check_linear_damping(data, tol)
 
-    def test_friction(self, data_new, tol):
+    @pytest.fixture(scope="class")
+    def data_new_nonuniform(self, data, tol):
+        """Hydrodynamic data structure for which the function
+        :python:`check_linear_damping` has been called.
+        """
+        # TODO: clean this up when fixing the dim order discrepancy
+        data['radiation_damping'] = data['radiation_damping'].transpose('omega', ...)
+        return wot.check_linear_damping(data, tol, False)
+
+    def test_friction(self, data_new_uniform, tol):
         """Test that the modified friction diagonal has the expected
-        value.
+        value for a uniform shift.
         """
-        assert np.allclose(np.diagonal(data_new.friction.values), tol)
+        assert np.allclose(np.diagonal(data_new_uniform.friction.values), tol)
 
-    def test_only_diagonal_friction(self, data, data_new):
-        """Test that only the diagonal was changed."""
+    def test_only_diagonal_friction(self, data, data_new_uniform):
+        """Test that only the diagonal was changed for a uniform shift."""
         data_org = data.copy(deep=True)
         def nodiag(x):
             return x.friction.values - np.diag(np.diagonal(x.friction.values))
-        assert np.allclose(nodiag(data_new), nodiag(data_org))
+        assert np.allclose(nodiag(data_new_uniform), nodiag(data_org))
 
-    def test_only_friction(self, data, data_new):
+    def test_only_friction(self, data, data_new_uniform):
         """Test that only the friction is changed in the hydrodynamic
-        data.
+        data for a uniform shift.
         """
-        data_new_nofric = data_new.copy(deep=True).drop_vars('friction')
+        data_new_nofric = data_new_uniform.copy(deep=True
+                                                ).drop_vars('friction')
         data_org_nofric = data.copy(deep=True).drop_vars('friction')
         assert data_new_nofric.equals(data_org_nofric)
 
+    def test_damping(self, data_new_nonuniform, tol):
+        """Test that the modified radiation damping diagonal has the expected
+        value for a non-uniform shift.
+        """
+        assert np.allclose(
+            np.diagonal(data_new_nonuniform.radiation_damping.values,
+                        axis1=1, axis2=2),
+                        tol)
+
+    def test_only_diagonal_damping(self, data_new_nonuniform):
+        """Test that no off-diagonal radiation damping terms are nonzero
+        for a non-uniform shift.
+        """
+        assert (
+            np.prod(
+            np.shape(data_new_nonuniform.radiation_damping.values)[:-1]) == 
+            np.count_nonzero(data_new_nonuniform.radiation_damping.values)
+        )
+
+    def test_only_rd(self, data, data_new_nonuniform):
+        """Test that only the radiation damping is changed in the hydrodynamic
+        data for a non-uniform shift.
+        """
+        data_new_nord = data_new_nonuniform.copy(
+            deep=True).drop_vars('radiation_damping')
+        data_org_nord = data.copy(deep=True).drop_vars('radiation_damping')
+        assert data_new_nord.equals(data_org_nord)
+        
 
 class TestCheckImpedance:
     """Test functions :python:`hydrodynamic_impedance` and 
     :python:`check_impedance`."""
 
     @pytest.fixture(scope="class")
     def data(self, hydro_data):
```

### Comparing `wecopttool-2.5.0/tests/test_hydrostatics.py` & `wecopttool-2.6.0/tests/test_hydrostatics.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.5.0/tests/test_integration.py` & `wecopttool-2.6.0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.5.0/tests/test_pto.py` & `wecopttool-2.6.0/tests/test_pto.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.5.0/tests/test_waves.py` & `wecopttool-2.6.0/tests/test_waves.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.5.0/wecopttool/__init__.py` & `wecopttool-2.6.0/wecopttool/__init__.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.5.0/wecopttool/core.py` & `wecopttool-2.6.0/wecopttool/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -286,14 +286,15 @@
         bem_data: Union[Dataset, Union[str, Path]],
         inertia_matrix: Optional[ndarray] = None,
         hydrostatic_stiffness: Optional[ndarray] = None,
         friction: Optional[ndarray] = None,
         f_add: Optional[TIForceDict] = None,
         constraints: Optional[Iterable[Mapping]] = None,
         min_damping: Optional[float] = _default_min_damping,
+        uniform_shift: Optional[bool] = True,
         dof_names: Optional[Iterable[str]] = None,
         ) -> TWEC:
         """Create a WEC object from linear hydrodynamic coefficients
         obtained using the boundary element method (BEM) code Capytaine.
 
         The :python:`bem_data` can be a dataset or the name of a
         *NetCDF* file containing the dataset.
@@ -346,14 +347,19 @@
             List of constraints, see documentation for
             :py:func:`scipy.optimize.minimize` for description and
             options of constraints dictionaries.
             If :python:`None`: empty list :python:`[]`.
         min_damping
             Minimum damping level to ensure a stable system.
             See :py:func:`wecopttool.check_linear_damping` for more details.
+        uniform_shift
+            Boolean determining whether damping corrections shifts the damping
+            values uniformly for all frequencies or only for frequencies below
+            :python:`min_damping`.
+            See :py:func:`wecopttool.check_linear_damping` for more details.
         dof_names
             Names of the different degrees of freedom (e.g.
             :python:`'Heave'`).
             If :python:`None` the names
             :python:`['DOF_0', ..., 'DOF_N']` are used.
 
         Raises
@@ -385,15 +391,16 @@
 
         # frequency array
         f1, nfreq = frequency_parameters(
             hydro_data.omega.values/(2*np.pi), False)
 
         # check real part of damping diagonal > 0
         if min_damping is not None:
-            hydro_data = check_linear_damping(hydro_data, min_damping)
+            hydro_data = check_linear_damping(
+                hydro_data, min_damping, uniform_shift)
 
         # forces in the dynamics equations
         linear_force_functions = standard_forces(hydro_data)
         f_add = f_add if (f_add is not None) else {}
         forces = linear_force_functions | f_add
         # constraints
         constraints = constraints if (constraints is not None) else []
@@ -1830,46 +1837,66 @@
     """
     cpy.io.xarray.separate_complex_values(data).to_netcdf(fpath)
 
 
 def check_linear_damping(
     hydro_data: Dataset,
     min_damping: Optional[float] = 1e-6,
+    uniform_shift: Optional[bool] = True,
 ) -> Dataset:
     """Ensure that the linear hydrodynamics (friction + radiation
     damping) have positive damping.
 
-    Shifts the :python:`friction` up if necessary.
-    Returns the (possibly) updated Dataset with
+    Shifts the :python:`friction` or :python:`radiation_damping` up
+    if necessary. Returns the (possibly) updated Dataset with
     :python:`damping` :math:`>=` :python:`min_damping`.
 
     Parameters
     ----------
     hydro_data
         Linear hydrodynamic data.
     min_damping
         Minimum threshold for damping. Default is 1e-6.
+    uniform_shift
+        Boolean that determines whether the damping correction for each
+        degree of freedom is frequency dependent or not. If :python:`True`,
+        the damping correction is applied to :python:`friction` and shifts the
+        damping for all frequencies. If :python:`False`, the damping correction
+        is applied to :python:`radiation_damping` and only shifts the 
+        damping for frequencies with negative damping values. Default is
+        :python:`True`.
     """
     hydro_data_new = hydro_data.copy(deep=True)
     radiation = hydro_data_new['radiation_damping']
     friction = hydro_data_new['friction']
     ndof = len(hydro_data_new.influenced_dof)
     assert ndof == len(hydro_data.radiating_dof)
     for idof in range(ndof):
         iradiation = radiation.isel(radiating_dof=idof, influenced_dof=idof)
         ifriction = friction.isel(radiating_dof=idof, influenced_dof=idof)
-        dmin = (iradiation+ifriction).min()
-        if dmin <= 0.0 + min_damping:
+        if uniform_shift:
+            dmin = (iradiation+ifriction).min()
+            if dmin <= 0.0 + min_damping:
+                dof = hydro_data_new.influenced_dof.values[idof]
+                delta = min_damping-dmin
+                _log.warning(
+                    f'Linear damping for DOF "{dof}" has negative or close ' +
+                    'to zero terms. Shifting up via linear friction of ' +
+                    f'{delta.values} N/(m/s).')
+                hydro_data_new['friction'][idof, idof] = (ifriction + delta)
+        else:
+            new_damping = iradiation.where(
+                iradiation+ifriction>min_damping, other=min_damping)
             dof = hydro_data_new.influenced_dof.values[idof]
-            delta = min_damping-dmin
-            _log.warning(
-                f'Linear damping for DOF "{dof}" has negative or close to ' +
-                'zero terms. Shifting up via linear friction of ' +
-                f'{delta.values} N/(m/s).')
-            hydro_data_new['friction'][idof, idof] = (ifriction + delta)
+            if (new_damping==min_damping).any():
+                _log.warning(
+                    f'Linear damping for DOF "{dof}" has negative or close to ' +
+                    'zero terms. Shifting up damping terms to a minimum of ' +
+                    f'{min_damping} N/(m/s)')
+            hydro_data_new['radiation_damping'][:, idof, idof] = new_damping
     return hydro_data_new
 
 
 def check_impedance(
     Zi: ArrayLike,
     min_damping: Optional[float] = 1e-6,
 ) -> DataArray:
```

### Comparing `wecopttool-2.5.0/wecopttool/geom.py` & `wecopttool-2.6.0/wecopttool/geom.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.5.0/wecopttool/hydrostatics.py` & `wecopttool-2.6.0/wecopttool/hydrostatics.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.5.0/wecopttool/pto.py` & `wecopttool-2.6.0/wecopttool/pto.py`

 * *Files 0% similar despite different names*

```diff
@@ -723,69 +723,73 @@
         acc_fd = wec.td_to_fd(acc_td[::nsubsteps])
 
         # force
         force_td = self.force(wec, x_wec, x_opt, waves, nsubsteps)
         force_fd = wec.td_to_fd(force_td[::nsubsteps])
 
         # power
-        power_td = self.power(wec, x_wec, x_opt, waves, nsubsteps)
-        power_fd = wec.td_to_fd(power_td[::nsubsteps])
+        elec_power_td = self.power(wec, x_wec, x_opt, waves, nsubsteps)
+        elec_power_fd = wec.td_to_fd(elec_power_td[::nsubsteps])
 
         # mechanical power
         mech_power_td = self.mechanical_power(wec, x_wec, x_opt, waves,
                                               nsubsteps)
         mech_power_fd = wec.td_to_fd(mech_power_td[::nsubsteps])
 
+        # stack mechanical and electrical power
+        power_names = ['mech','elec']
+        power_fd = np.stack((mech_power_fd,elec_power_fd))
+        power_td = np.stack((mech_power_td,elec_power_td))
+
         pos_attr = {'long_name': 'Position', 'units': 'm or rad'}
         vel_attr = {'long_name': 'Velocity', 'units': 'm/s or rad/s'}
         acc_attr = {'long_name': 'Acceleration',
                     'units': 'm/s^2 or rad/s^2'}
         force_attr = {'long_name': 'Force or moment on WEC',
                       'units': 'N or Nm'}
         power_attr = {'long_name': 'Power', 'units': 'W'}
         mech_power_attr = {'long_name': 'Mechanical power', 'units': 'W'}
         omega_attr = {'long_name': 'Radial frequency', 'units': 'rad/s'}
         freq_attr = {'long_name': 'Frequency', 'units': 'Hz'}
         period_attr = {'long_name': 'Period', 'units': 's'}
         dof_attr = {'long_name': 'PTO degree of freedom'}
         time_attr = {'long_name': 'Time', 'units': 's'}
+        type_attr = {'long_name': 'Power type'}
 
         t_dat = wec.time_nsubsteps(nsubsteps)
 
         results_fd = Dataset(
             data_vars={
                 'pos': (['omega','dof'], pos_fd, pos_attr),
                 'vel': (['omega','dof'], vel_fd, vel_attr),
                 'acc': (['omega','dof'], acc_fd, acc_attr),
                 'force': (['omega','dof'], force_fd, force_attr),
-                'power': (['omega','dof'], power_fd, power_attr),
-                'mech_power': (['omega','dof'],
-                                mech_power_fd, mech_power_attr)
+                'power': (['type','omega','dof'], power_fd, power_attr),
             },
             coords={
                 'omega':('omega', wec.omega, omega_attr),
                 'freq':('omega', wec.frequency, freq_attr),
                 'period':('omega', wec.period, period_attr),
-                'dof':('dof', self.names, dof_attr)},
+                'dof':('dof', self.names, dof_attr),
+                'type':('type', power_names, power_attr)},
             attrs={"time_created_utc": create_time}
             )
 
         results_td = Dataset(
             data_vars={
                 'pos': (['time','dof'], pos_td, pos_attr),
                 'vel': (['time','dof'], vel_td, vel_attr),
                 'acc': (['time','dof'], acc_td, acc_attr),
                 'force': (['time','dof'], force_td, force_attr),
-                'power': (['time','dof'], power_td, power_attr),
-                'mech_power': (['time','dof'],
-                                 mech_power_td, mech_power_attr)
+                'power': (['type','time','dof'], power_td, power_attr),
             },
             coords={
                 'time':('time', t_dat, time_attr),
-                'dof':('dof', self.names, dof_attr)},
+                'dof':('dof', self.names, dof_attr),
+                'type':('type', power_names, power_attr)},
             attrs={"time_created_utc": create_time}
             )
 
         if self.impedance is not None:
         #transduced flow and effort variables
             q2_td, e2_td = self.power_variables(wec, x_wec, x_opt,
                                                 waves, nsubsteps)
```

### Comparing `wecopttool-2.5.0/wecopttool/waves.py` & `wecopttool-2.6.0/wecopttool/waves.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.5.0/wecopttool.egg-info/PKG-INFO` & `wecopttool-2.6.0/wecopttool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wecopttool
-Version: 2.5.0
+Version: 2.6.0
 Summary: WEC Design Optimization Toolbox
 Author: Sandia National Laboratories
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Documentation, https://sandialabs.github.io/WecOptTool/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

