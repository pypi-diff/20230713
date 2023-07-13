# Comparing `tmp/ensembleperturbation-1.2.3.tar.gz` & `tmp/ensembleperturbation-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensembleperturbation-1.2.3.tar", max compression
+gzip compressed data, was "ensembleperturbation-1.2.4.tar", max compression
```

## Comparing `ensembleperturbation-1.2.3.tar` & `ensembleperturbation-1.2.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     7048 2023-07-03 13:55:29.074694 ensembleperturbation-1.2.3/LICENSE
--rw-r--r--   0        0        0     1554 2023-07-03 13:55:29.074694 ensembleperturbation-1.2.3/README.md
--rw-r--r--   0        0        0        3 2023-07-03 13:55:29.082694 ensembleperturbation-1.2.3/ensembleperturbation/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 13:55:29.082694 ensembleperturbation-1.2.3/ensembleperturbation/client/__init__.py
--rw-r--r--   0        0        0     3803 2023-07-03 13:55:29.082694 ensembleperturbation-1.2.3/ensembleperturbation/client/combine_results.py
--rw-r--r--   0        0        0     1952 2023-07-03 13:55:29.082694 ensembleperturbation-1.2.3/ensembleperturbation/client/make_storm_ensemble.py
--rw-r--r--   0        0        0     5792 2023-07-03 13:55:29.082694 ensembleperturbation-1.2.3/ensembleperturbation/client/perturb_tracks.py
--rw-r--r--   0        0        0     2566 2023-07-03 13:55:29.082694 ensembleperturbation-1.2.3/ensembleperturbation/client/plot_results.py
--rw-r--r--   0        0        0        0 2023-07-03 13:55:29.082694 ensembleperturbation-1.2.3/ensembleperturbation/parsing/__init__.py
--rw-r--r--   0        0        0    32929 2023-07-03 13:55:29.082694 ensembleperturbation-1.2.3/ensembleperturbation/parsing/adcirc.py
--rw-r--r--   0        0        0    24828 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/parsing/comparison.py
--rw-r--r--   0        0        0    46714 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/parsing/schism.py
--rw-r--r--   0        0        0      545 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/parsing/utilities.py
--rw-r--r--   0        0        0        0 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/perturbation/__init__.py
--rw-r--r--   0        0        0    75293 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/perturbation/atcf.py
--rw-r--r--   0        0        0        0 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/plotting/__init__.py
--rw-r--r--   0        0        0    10510 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/plotting/gdal_dataset.py
--rw-r--r--   0        0        0     5453 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/plotting/geometry.py
--rw-r--r--   0        0        0     1590 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/plotting/map.py
--rw-r--r--   0        0        0     9135 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/plotting/nodes.py
--rw-r--r--   0        0        0    14013 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/plotting/perturbation.py
--rw-r--r--   0        0        0    20066 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/plotting/surrogate.py
--rw-r--r--   0        0        0     4623 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/plotting/taylor_diagram.py
--rw-r--r--   0        0        0      908 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/plotting/utilities.py
--rw-r--r--   0        0        0        0 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/uncertainty_quantification/__init__.py
--rw-r--r--   0        0        0     2663 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/uncertainty_quantification/ensemble_array.py
--rw-r--r--   0        0        0    11112 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/uncertainty_quantification/karhunen_loeve_expansion.py
--rw-r--r--   0        0        0     5332 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/uncertainty_quantification/polynomial_chaos.py
--rw-r--r--   0        0        0    23410 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/uncertainty_quantification/surrogate.py
--rw-r--r--   0        0        0     5066 2023-07-03 13:55:29.086694 ensembleperturbation-1.2.3/ensembleperturbation/utilities.py
--rw-r--r--   0        0        0     2326 2023-07-03 13:55:35.030723 ensembleperturbation-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     3723 2023-07-03 13:55:35.847128 ensembleperturbation-1.2.3/setup.py
--rw-r--r--   0        0        0     3731 2023-07-03 13:55:35.847636 ensembleperturbation-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     7048 2023-07-13 13:20:22.129835 ensembleperturbation-1.2.4/LICENSE
+-rw-r--r--   0        0        0     1554 2023-07-13 13:20:22.129835 ensembleperturbation-1.2.4/README.md
+-rw-r--r--   0        0        0        3 2023-07-13 13:20:22.137836 ensembleperturbation-1.2.4/ensembleperturbation/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 13:20:22.137836 ensembleperturbation-1.2.4/ensembleperturbation/client/__init__.py
+-rw-r--r--   0        0        0     3803 2023-07-13 13:20:22.137836 ensembleperturbation-1.2.4/ensembleperturbation/client/combine_results.py
+-rw-r--r--   0        0        0     1952 2023-07-13 13:20:22.137836 ensembleperturbation-1.2.4/ensembleperturbation/client/make_storm_ensemble.py
+-rw-r--r--   0        0        0     5792 2023-07-13 13:20:22.137836 ensembleperturbation-1.2.4/ensembleperturbation/client/perturb_tracks.py
+-rw-r--r--   0        0        0     2566 2023-07-13 13:20:22.137836 ensembleperturbation-1.2.4/ensembleperturbation/client/plot_results.py
+-rw-r--r--   0        0        0        0 2023-07-13 13:20:22.137836 ensembleperturbation-1.2.4/ensembleperturbation/parsing/__init__.py
+-rw-r--r--   0        0        0    32929 2023-07-13 13:20:22.137836 ensembleperturbation-1.2.4/ensembleperturbation/parsing/adcirc.py
+-rw-r--r--   0        0        0    24828 2023-07-13 13:20:22.137836 ensembleperturbation-1.2.4/ensembleperturbation/parsing/comparison.py
+-rw-r--r--   0        0        0    46714 2023-07-13 13:20:22.137836 ensembleperturbation-1.2.4/ensembleperturbation/parsing/schism.py
+-rw-r--r--   0        0        0      545 2023-07-13 13:20:22.137836 ensembleperturbation-1.2.4/ensembleperturbation/parsing/utilities.py
+-rw-r--r--   0        0        0        0 2023-07-13 13:20:22.137836 ensembleperturbation-1.2.4/ensembleperturbation/perturbation/__init__.py
+-rw-r--r--   0        0        0    75288 2023-07-13 13:20:22.141836 ensembleperturbation-1.2.4/ensembleperturbation/perturbation/atcf.py
+-rw-r--r--   0        0        0        0 2023-07-13 13:20:22.141836 ensembleperturbation-1.2.4/ensembleperturbation/plotting/__init__.py
+-rw-r--r--   0        0        0    10510 2023-07-13 13:20:22.141836 ensembleperturbation-1.2.4/ensembleperturbation/plotting/gdal_dataset.py
+-rw-r--r--   0        0        0     5453 2023-07-13 13:20:22.141836 ensembleperturbation-1.2.4/ensembleperturbation/plotting/geometry.py
+-rw-r--r--   0        0        0     1590 2023-07-13 13:20:22.141836 ensembleperturbation-1.2.4/ensembleperturbation/plotting/map.py
+-rw-r--r--   0        0        0     9135 2023-07-13 13:20:22.141836 ensembleperturbation-1.2.4/ensembleperturbation/plotting/nodes.py
+-rw-r--r--   0        0        0    14013 2023-07-13 13:20:22.141836 ensembleperturbation-1.2.4/ensembleperturbation/plotting/perturbation.py
+-rw-r--r--   0        0        0    20066 2023-07-13 13:20:22.141836 ensembleperturbation-1.2.4/ensembleperturbation/plotting/surrogate.py
+-rw-r--r--   0        0        0     4623 2023-07-13 13:20:22.141836 ensembleperturbation-1.2.4/ensembleperturbation/plotting/taylor_diagram.py
+-rw-r--r--   0        0        0      908 2023-07-13 13:20:22.141836 ensembleperturbation-1.2.4/ensembleperturbation/plotting/utilities.py
+-rw-r--r--   0        0        0        0 2023-07-13 13:20:22.141836 ensembleperturbation-1.2.4/ensembleperturbation/uncertainty_quantification/__init__.py
+-rw-r--r--   0        0        0     2663 2023-07-13 13:20:22.141836 ensembleperturbation-1.2.4/ensembleperturbation/uncertainty_quantification/ensemble_array.py
+-rw-r--r--   0        0        0    11112 2023-07-13 13:20:22.141836 ensembleperturbation-1.2.4/ensembleperturbation/uncertainty_quantification/karhunen_loeve_expansion.py
+-rw-r--r--   0        0        0     5332 2023-07-13 13:20:22.141836 ensembleperturbation-1.2.4/ensembleperturbation/uncertainty_quantification/polynomial_chaos.py
+-rw-r--r--   0        0        0    23410 2023-07-13 13:20:22.141836 ensembleperturbation-1.2.4/ensembleperturbation/uncertainty_quantification/surrogate.py
+-rw-r--r--   0        0        0     5066 2023-07-13 13:20:22.141836 ensembleperturbation-1.2.4/ensembleperturbation/utilities.py
+-rw-r--r--   0        0        0     2288 2023-07-13 13:20:32.246227 ensembleperturbation-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3726 2023-07-13 13:20:33.134222 ensembleperturbation-1.2.4/setup.py
+-rw-r--r--   0        0        0     3737 2023-07-13 13:20:33.134690 ensembleperturbation-1.2.4/PKG-INFO
```

### Comparing `ensembleperturbation-1.2.3/LICENSE` & `ensembleperturbation-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.3/README.md` & `ensembleperturbation-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.3/ensembleperturbation/client/combine_results.py` & `ensembleperturbation-1.2.4/ensembleperturbation/client/combine_results.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.3/ensembleperturbation/client/make_storm_ensemble.py` & `ensembleperturbation-1.2.4/ensembleperturbation/client/make_storm_ensemble.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.3/ensembleperturbation/client/perturb_tracks.py` & `ensembleperturbation-1.2.4/ensembleperturbation/client/perturb_tracks.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.3/ensembleperturbation/client/plot_results.py` & `ensembleperturbation-1.2.4/ensembleperturbation/client/plot_results.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.3/ensembleperturbation/parsing/adcirc.py` & `ensembleperturbation-1.2.4/ensembleperturbation/parsing/adcirc.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.3/ensembleperturbation/parsing/comparison.py` & `ensembleperturbation-1.2.4/ensembleperturbation/parsing/comparison.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.3/ensembleperturbation/parsing/schism.py` & `ensembleperturbation-1.2.4/ensembleperturbation/parsing/schism.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.3/ensembleperturbation/parsing/utilities.py` & `ensembleperturbation-1.2.4/ensembleperturbation/parsing/utilities.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.3/ensembleperturbation/perturbation/atcf.py` & `ensembleperturbation-1.2.4/ensembleperturbation/perturbation/atcf.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import chaospy
 from chaospy import Distribution
 from dateutil.parser import parse as parse_date
 import numpy
 from numpy import floor, interp, sign
 from pandas import DataFrame
-from pandas.core.common import SettingWithCopyWarning
+from pandas.errors import SettingWithCopyWarning
 import pint
 from pint import Quantity, UnitStrippedWarning
 from pint_pandas import PintArray, PintType
 from pyproj import CRS, Transformer
 from pyproj.enums import TransformDirection
 from scipy.special import erfinv
 from shapely.geometry import LineString
```

### Comparing `ensembleperturbation-1.2.3/ensembleperturbation/plotting/gdal_dataset.py` & `ensembleperturbation-1.2.4/ensembleperturbation/plotting/gdal_dataset.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.3/ensembleperturbation/plotting/geometry.py` & `ensembleperturbation-1.2.4/ensembleperturbation/plotting/geometry.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.3/ensembleperturbation/plotting/map.py` & `ensembleperturbation-1.2.4/ensembleperturbation/plotting/map.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.3/ensembleperturbation/plotting/nodes.py` & `ensembleperturbation-1.2.4/ensembleperturbation/plotting/nodes.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.3/ensembleperturbation/plotting/perturbation.py` & `ensembleperturbation-1.2.4/ensembleperturbation/plotting/perturbation.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.3/ensembleperturbation/plotting/surrogate.py` & `ensembleperturbation-1.2.4/ensembleperturbation/plotting/surrogate.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.3/ensembleperturbation/plotting/taylor_diagram.py` & `ensembleperturbation-1.2.4/ensembleperturbation/plotting/taylor_diagram.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.3/ensembleperturbation/plotting/utilities.py` & `ensembleperturbation-1.2.4/ensembleperturbation/plotting/utilities.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.3/ensembleperturbation/uncertainty_quantification/ensemble_array.py` & `ensembleperturbation-1.2.4/ensembleperturbation/uncertainty_quantification/ensemble_array.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.3/ensembleperturbation/uncertainty_quantification/karhunen_loeve_expansion.py` & `ensembleperturbation-1.2.4/ensembleperturbation/uncertainty_quantification/karhunen_loeve_expansion.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.3/ensembleperturbation/uncertainty_quantification/polynomial_chaos.py` & `ensembleperturbation-1.2.4/ensembleperturbation/uncertainty_quantification/polynomial_chaos.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.3/ensembleperturbation/uncertainty_quantification/surrogate.py` & `ensembleperturbation-1.2.4/ensembleperturbation/uncertainty_quantification/surrogate.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.3/ensembleperturbation/utilities.py` & `ensembleperturbation-1.2.4/ensembleperturbation/utilities.py`

 * *Files identical despite different names*

### Comparing `ensembleperturbation-1.2.3/pyproject.toml` & `ensembleperturbation-1.2.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'ensembleperturbation'
-version = "1.2.3"
+version = "1.2.4"
 description = 'perturbation of coupled model input over a space of input variables'
 authors = ['Zach Burnett <zachary.burnett@noaa.gov>']
 license = 'CC0-1.0'
 readme = 'README.md'
 repository = 'https://github.com/noaa-ocs-modeling/EnsemblePerturbation.git'
 documentation = 'https://ensembleperturbation.readthedocs.io'
 
@@ -30,17 +30,17 @@
 dask = '*'
 f90nml = '*'
 fiona = '*'
 geopandas = '*'
 netcdf4 = '*'
 matplotlib = { version = '*', optional = true }
 numpy = '*'
-pandas = '<1.5.0' # SettingWithCopyWarning issue
-pint = '<0.20' # Import error for quantity from `pint-pandas`
-pint-pandas = '*'
+pandas = '>=1.5'
+pint = '<0.21' # ito() issue #105
+pint-pandas = '<0.4' # ito() issue #105
 pyproj = '>=2.6'
 tables = '*'
 typepigeon = '*'
 python-dateutil = '*'
 requests = '*'
 shapely = '*'
 scikit-learn = '*'
```

### Comparing `ensembleperturbation-1.2.3/setup.py` & `ensembleperturbation-1.2.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,17 +20,17 @@
  'coupledmodeldriver>=1.5',
  'dask',
  'f90nml',
  'fiona',
  'geopandas',
  'netcdf4',
  'numpy',
- 'pandas<1.5.0',
- 'pint-pandas',
- 'pint<0.20',
+ 'pandas>=1.5',
+ 'pint-pandas<0.4',
+ 'pint<0.21',
  'pyproj>=2.6',
  'python-dateutil',
  'requests',
  'scikit-learn',
  'shapely',
  'stormevents>=2.2.1',
  'tables',
@@ -54,15 +54,15 @@
                      'perturb_tracks = '
                      'ensembleperturbation.client.perturb_tracks:main',
                      'plot_results = '
                      'ensembleperturbation.client.plot_results:main']}
 
 setup_kwargs = {
     'name': 'ensembleperturbation',
-    'version': '1.2.3',
+    'version': '1.2.4',
     'description': 'perturbation of coupled model input over a space of input variables',
     'long_description': '# Ensemble Perturbation\n\n[![tests](https://github.com/noaa-ocs-modeling/EnsemblePerturbation/workflows/tests/badge.svg)](https://github.com/noaa-ocs-modeling/EnsemblePerturbation/actions?query=workflow%3Atests)\n[![codecov](https://codecov.io/gh/noaa-ocs-modeling/ensembleperturbation/branch/main/graph/badge.svg?token=4DwZePHp18)](https://codecov.io/gh/noaa-ocs-modeling/ensembleperturbation)\n[![build](https://github.com/noaa-ocs-modeling/EnsemblePerturbation/workflows/build/badge.svg)](https://github.com/noaa-ocs-modeling/EnsemblePerturbation/actions?query=workflow%3Abuild)\n[![version](https://img.shields.io/pypi/v/EnsemblePerturbation)](https://pypi.org/project/EnsemblePerturbation)\n[![license](https://img.shields.io/github/license/noaa-ocs-modeling/EnsemblePerturbation)](https://creativecommons.org/share-your-work/public-domain/cc0)\n[![style](https://sourceforge.net/p/oitnb/code/ci/default/tree/_doc/_static/oitnb.svg?format=raw)](https://sourceforge.net/p/oitnb/code)\n[![documentation](https://readthedocs.org/projects/ensembleperturbation/badge/?version=latest)](https://ensembleperturbation.readthedocs.io/en/latest/?badge=latest)\n\nPython library for perturbing coupled model inputs into ensemble runs. Provides\nperturbation and results comparison.\n\n```bash\npip install ensembleperturbation\n```\n\nDocumentation can be found at https://ensembleperturbation.readthedocs.io\n\n## Command-line interface\n\n`ensembleperturbation` exposes the following CLI commands:\n\n- `make_storm_ensemble`\n- `perturb_tracks`\n- `combine_results`\n- `plot_results`\n',
     'author': 'Zach Burnett',
     'author_email': 'zachary.burnett@noaa.gov',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/noaa-ocs-modeling/EnsemblePerturbation.git',
```

### Comparing `ensembleperturbation-1.2.3/PKG-INFO` & `ensembleperturbation-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensembleperturbation
-Version: 1.2.3
+Version: 1.2.4
 Summary: perturbation of coupled model input over a space of input variables
 Home-page: https://github.com/noaa-ocs-modeling/EnsemblePerturbation.git
 License: CC0-1.0
 Author: Zach Burnett
 Author-email: zachary.burnett@noaa.gov
 Requires-Python: >=3.8,<4.0
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
@@ -29,17 +29,17 @@
 Requires-Dist: geopandas
 Requires-Dist: isort; extra == "development"
 Requires-Dist: m2r2; extra == "documentation"
 Requires-Dist: matplotlib; extra == "plotting"
 Requires-Dist: netcdf4
 Requires-Dist: numpy
 Requires-Dist: oitnb; extra == "development"
-Requires-Dist: pandas (<1.5.0)
-Requires-Dist: pint (<0.20)
-Requires-Dist: pint-pandas
+Requires-Dist: pandas (>=1.5)
+Requires-Dist: pint (<0.21)
+Requires-Dist: pint-pandas (<0.4)
 Requires-Dist: pyproj (>=2.6)
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-xdist; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: python-dateutil
 Requires-Dist: requests
 Requires-Dist: scikit-learn
```

