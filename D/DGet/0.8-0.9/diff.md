# Comparing `tmp/DGet-0.8.tar.gz` & `tmp/DGet-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DGet-0.8.tar", last modified: Sat May 13 03:50:38 2023, max compression
+gzip compressed data, was "DGet-0.9.tar", last modified: Wed May 17 06:03:52 2023, max compression
```

## Comparing `DGet-0.8.tar` & `DGet-0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 03:50:38.779628 DGet-0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 03:50:38.775628 DGet-0.8/DGet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-13 03:50:38.000000 DGet-0.8/DGet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-13 03:50:38.000000 DGet-0.8/DGet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 03:50:38.000000 DGet-0.8/DGet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-13 03:50:38.000000 DGet-0.8/DGet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-13 03:50:38.000000 DGet-0.8/DGet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-13 03:50:38.000000 DGet-0.8/DGet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-13 03:50:26.000000 DGet-0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-13 03:50:38.779628 DGet-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-13 03:50:26.000000 DGet-0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 03:50:38.779628 DGet-0.8/dget/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-13 03:50:26.000000 DGet-0.8/dget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-13 03:50:26.000000 DGet-0.8/dget/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-13 03:50:26.000000 DGet-0.8/dget/adduct.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-13 03:50:26.000000 DGet-0.8/dget/convolve.py
--rw-r--r--   0 runner    (1001) docker     (123)    15695 2023-05-13 03:50:26.000000 DGet-0.8/dget/dget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-13 03:50:26.000000 DGet-0.8/dget/formula.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-13 03:50:26.000000 DGet-0.8/dget/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 03:50:38.779628 DGet-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-13 03:50:26.000000 DGet-0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 03:50:38.779628 DGet-0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-13 03:50:26.000000 DGet-0.8/tests/test_adduct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-13 03:50:26.000000 DGet-0.8/tests/test_dget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-13 03:50:26.000000 DGet-0.8/tests/test_formula.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:03:52.029902 DGet-0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:03:52.029902 DGet-0.9/DGet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-17 06:03:52.000000 DGet-0.9/DGet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-17 06:03:52.000000 DGet-0.9/DGet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 06:03:52.000000 DGet-0.9/DGet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-17 06:03:52.000000 DGet-0.9/DGet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-17 06:03:52.000000 DGet-0.9/DGet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-17 06:03:52.000000 DGet-0.9/DGet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-17 06:03:40.000000 DGet-0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-17 06:03:52.029902 DGet-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-17 06:03:40.000000 DGet-0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:03:52.029902 DGet-0.9/dget/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-17 06:03:40.000000 DGet-0.9/dget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-05-17 06:03:40.000000 DGet-0.9/dget/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-17 06:03:40.000000 DGet-0.9/dget/adduct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-17 06:03:40.000000 DGet-0.9/dget/convolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15979 2023-05-17 06:03:40.000000 DGet-0.9/dget/dget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-17 06:03:40.000000 DGet-0.9/dget/formula.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-17 06:03:40.000000 DGet-0.9/dget/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 06:03:52.029902 DGet-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-17 06:03:40.000000 DGet-0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:03:52.029902 DGet-0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-17 06:03:41.000000 DGet-0.9/tests/test_adduct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-17 06:03:41.000000 DGet-0.9/tests/test_dget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-17 06:03:41.000000 DGet-0.9/tests/test_formula.py
```

### Comparing `DGet-0.8/DGet.egg-info/PKG-INFO` & `DGet-0.9/DGet.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DGet
-Version: 0.8
+Version: 0.9
 Summary: Calculates compound deuteration from ToF-MS data.
 Home-page: https://github.com/djdt/dget
 Author: djdt
 License: GPL3
 Project-URL: Documentation, https://dget.readthedocs.io
 Project-URL: Source, https://github.com/djdt/dget
 Project-URL: Web App, https://djdt.github.io/dget
```

### Comparing `DGet-0.8/LICENSE` & `DGet-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `DGet-0.8/PKG-INFO` & `DGet-0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DGet
-Version: 0.8
+Version: 0.9
 Summary: Calculates compound deuteration from ToF-MS data.
 Home-page: https://github.com/djdt/dget
 Author: djdt
 License: GPL3
 Project-URL: Documentation, https://dget.readthedocs.io
 Project-URL: Source, https://github.com/djdt/dget
 Project-URL: Web App, https://djdt.github.io/dget
```

### Comparing `DGet-0.8/README.rst` & `DGet-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `DGet-0.8/dget/__main__.py` & `DGet-0.9/dget/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         default="[M]+",
         help="Type of adduct in form [xM<+-><adduct>]x<+->. Valid examples are [M]-, "
         "[M+H]+, [2M+Na2]2+, [M-H2]2-. Defaults to [M]+.",
     )
     parser.add_argument(
         "--autoadduct",
         action="store_true",
-        help="Guess the adduct from the mass spectra base peak. Overrides --adduct.",
+        help="Guess the adduct from the mass spectra. Overrides --adduct.",
     )
     parser.add_argument("tofdata", type=Path, help="Path to mass spec data file.")
     parser.add_argument("--delimiter", default="\t", help="MS data file delimiter.")
     parser.add_argument(
         "--columns",
         metavar=("MASS", "SIGNAL"),
         type=int,
@@ -86,15 +86,15 @@
         adduct=args.adduct,
         number_states=args.nstates,
         loadtxt_kws=loadtxt_kws,
     )
     if args.autoadduct:
         adduct, diff = dget.guess_adduct_from_base_peak()
         dget.adduct = adduct
-        print(f"Adduct difference from base peak m/z: {diff:.4f}")
+        print(f"Adduct difference from adduct base peak m/z: {diff:.4f}")
         print()
 
     dget.mass_width = args.masswidth
     if args.realign:
         offset = dget.align_tof_with_spectra()
         print(f"Re-aligned ToF data by shifting {offset:.2f} m/z")
         print()
```

### Comparing `DGet-0.8/dget/adduct.py` & `DGet-0.9/dget/adduct.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Class for adduct calculations."""
 
 import re
+from typing import Tuple
 
 from molmass import Composition, Formula, Spectrum
 
 
 class Adduct(object):
     """Class used to create a ``molmass.Formula`` from a base ``molmass.Formula``
     and an adduct string. This string should be in the format *[nM+nX-nY]n+* where
@@ -67,12 +68,19 @@
         return self.formula.composition()
 
     @property
     def spectrum(self) -> Spectrum:
         """The spectrum of the adduct."""
         return self.formula.spectrum()
 
+    def mz_range(self, min_fraction: float = 0.0) -> Tuple[float, float]:
+        """Return the spectrum mz range."""
+        mzs = list(
+            v.mz for v in self.formula.spectrum(min_fraction=min_fraction).values()
+        )
+        return min(mzs), max(mzs)
+
     def __str__(self) -> str:
         return f"{self.adduct}, M={self.base.formula}"
 
     def __repr__(self) -> str:
         return f"Adduct({self.adduct!r}, M={self.base.formula!r})"
```

### Comparing `DGet-0.8/dget/convolve.py` & `DGet-0.9/dget/convolve.py`

 * *Files identical despite different names*

### Comparing `DGet-0.8/dget/dget.py` & `DGet-0.9/dget/dget.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     Attributes:
         deuterated_formula: formula of fully deuterated molecule
         tofdata: path to mass spectra text file, or tuple of masses, signals
         adduct: form of adduct ion, see `dget.adduct`
         number_states: number of deuterated states to calculate
         signal_mass_width: range around each m/z to search for maxima or integrate
         signal_method: detection mode, valid values are 'peak area', 'peak height'
-        spectrum_min_fraction: limit spectra to entries with at least this fraction
         loadtxt_kws: parameters passed to `numpy.loadtxt`,
             defaults to {'delimiter': ',', 'usecols': (0, 1)}
     """
 
     common_adducts = [
         "[M]+",
         "[M+H]+",
@@ -53,15 +52,14 @@
         self,
         deuterated_formula: str | Formula,
         tofdata: str | Path | Tuple[np.ndarray, np.ndarray],
         adduct: str = "[M]+",
         number_states: int | None = None,
         signal_mass_width: float = 0.5,
         signal_mode: str = "peak height",
-        spectrum_min_fraction: float = 0.01,
         loadtxt_kws: dict | None = None,
     ):
         if isinstance(deuterated_formula, str):
             deuterated_formula = Formula(deuterated_formula)
 
         _loadtxt_kws = {"delimiter": ",", "usecols": (0, 1)}
         if loadtxt_kws is not None:
@@ -74,20 +72,24 @@
         self.adduct = Adduct(deuterated_formula, adduct)
 
         if self.deuterium_count == 0:
             raise ValueError(
                 f"formula: {self.adduct.base.formula} does not contain deuterium"
             )
 
+        if number_states is not None and number_states < 1:
+            raise ValueError("'number_states' must be > 0")
         self.number_states = number_states
+
         self.mass_width = signal_mass_width
+
         if signal_mode not in ["peak area", "peak height"]:
             raise ValueError("signal_mode must be one of 'peak area', 'peak height'.")
+
         self.signal_mode = signal_mode
-        self.spectra_min_fraction = spectrum_min_fraction
 
         if isinstance(tofdata, (str | Path)):
             self.x, self.y = self._read_tofdata(tofdata, **_loadtxt_kws)
         else:
             self.x, self.y = tofdata[0], tofdata[1]
 
     @property
@@ -154,24 +156,23 @@
     @property
     def deuteration_states(self) -> np.ndarray:
         """Indexes of the valid deuteration states.
 
         Valid states are those Dx-Dn, where n is the number of deuterium atoms
         in the base molecule as x is either:
             ``n - self.number_states``
-            ``n - the 2nd last D with a probability < 0.5%``
+            ``n - the 2nd last D with a probability < 0.1%``
         """
         if self.number_states is None:
-            prob = self.deuteration_probabilites
-            idx = np.flatnonzero((prob[:-1] < 0.005) & (prob[1] < 0.005)) - 1
-            nstates = idx[-1] if idx.size > 0 else self.deuterium_count
+            prob = np.concatenate([[0], self.deuteration_probabilites])
+            idx = np.flatnonzero((prob[:-1] < 0.01) & (prob[1:] < 0.01))
+            nstates = idx[-1] if idx.size > 0 else 0
         else:
-            nstates = self.number_states
-        print(self.deuterium_count - nstates)
-        return np.arange(self.deuterium_count - nstates, self.deuterium_count + 1)
+            nstates = self.deuterium_count + 1 - self.number_states
+        return np.arange(max(nstates, 0), self.deuterium_count + 1)
 
     @property
     def formula(self) -> Formula:
         """The adduct formula."""
         return self.adduct.formula
 
     @property
@@ -287,54 +288,60 @@
         baseline = np.percentile(self.y[start:end], percentile)
         self.y -= baseline
         return baseline
 
     def guess_adduct_from_base_peak(
         self,
         adducts: List[Formula] | None = None,
-        mass_range: Tuple[float, float] | None = None,
     ) -> Tuple[Adduct, float]:
-        """Finds the adduct closest to the m/z of the largest tof peak.
+        """Search for the adduct with the highest intensity.
 
+        If multiple adducts have the maximum intensity then the adduct with the
+        monoisotopic mass closest to the local base peak is returned.
         This function will work best with highly deuterated samples.
 
         Args:
             adducts: adducts to try, defaults to DGet.common_adducts
-            mass_range: range to search for base peak, defaults to whole spectra
 
         Returns:
             best adduct
-            mass difference from base peak
+            mass difference from adducts base peak
         """
         if adducts is None:
             adducts = DGet.common_adducts
 
         formulas = []
         for adduct in adducts:
             try:
                 formulas.append(Adduct(self.adduct.base, adduct))
             except ValueError:
                 pass
 
         masses = np.array([f.formula.isotope.mz for f in formulas])
+        ranges = np.stack([f.mz_range(min_fraction=0.01) for f in formulas], axis=0)
+        ranges += (-0.5, 0.5)  # expand search by 0.5 Da
 
-        if mass_range is not None:
-            idx = np.searchsorted(self.x, mass_range)
-            start, end = np.clip(idx, 0, self.x.size)
-        else:
-            start, end = 0, self.x.size
-        if start == end:
-            raise ValueError(
-                "unable to get adduct, entire m/z range falls outside spectra"
-            )
+        # idx of start - end of each range
+        idx = np.searchsorted(self.x, ranges)
+        idx = np.clip(idx, 0, self.x.size - 1)
+
+        # max intensity for each adduct
+        intensities = np.maximum.reduceat(self.y, idx.flat)[::2]
+        max_intenstites = np.flatnonzero(intensities == intensities.max())
 
+        start = np.min(idx[max_intenstites, 0])
+        end = np.max(idx[max_intenstites, 1])
         base = self.x[start:end][np.argmax(self.y[start:end])]
-        diffs = masses - base
-        best = np.argmin(np.abs(diffs))
-        return formulas[best], diffs[best]
+        # multiple adducts overlap with base peak
+        if max_intenstites.size > 1:
+            best = max_intenstites[np.argmin(np.abs(base - masses[max_intenstites]))]
+        else:
+            best = max_intenstites[0]
+
+        return formulas[best], masses[best] - base
 
     def plot_predicted_spectra(
         self,
         ax: "matplotlib.axes.Axes",
         mass_range: Tuple[float, float] | str = "targets",  # noqa: F821
         color_probabilites: bool = False,
     ) -> None:
```

### Comparing `DGet-0.8/dget/formula.py` & `DGet-0.9/dget/formula.py`

 * *Files identical despite different names*

### Comparing `DGet-0.8/dget/plot.py` & `DGet-0.9/dget/plot.py`

 * *Files identical despite different names*

### Comparing `DGet-0.8/setup.py` & `DGet-0.9/setup.py`

 * *Files identical despite different names*

### Comparing `DGet-0.8/tests/test_adduct.py` & `DGet-0.9/tests/test_adduct.py`

 * *Files identical despite different names*

### Comparing `DGet-0.8/tests/test_dget.py` & `DGet-0.9/tests/test_dget.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,50 @@
 from pathlib import Path
 
 import numpy as np
+import pytest
 from molmass import Formula
 
 from dget import DGet
 
 data_path = Path(__file__).parent.joinpath("data")
 
+formulas = {
+    "C12HD8N": ("[M-H]-", 94.4),
+    "C42H69D13NO8P": ("[M+H]+", 99.0),
+    "C16H11D7N2O4S": ("[M-H]-", 95.4),
+    "C57H3D101O6": ("[M+Na]+", 95.1),
+    "C13H9D7N2O2": ("[M+Na]+", 94.9),
+}
 
-def test_dget_know_data():
-    formulas = {
-        "C12HD8N": ("[M-H]-", 94.4),
-        "C42H69D13NO8P": ("[M+H]+", 99.0),
-        "C16H11D7N2O4S": ("[M-H]-", 95.4),
-        "C57H3D101O6": ("[M+Na]+", 95.1),
-        # "C13H9D7N2O2": ("[M+Na]+", 94.9),
-    }
 
+def test_dget_know_data():
     for formula, (adduct, percent_d) in formulas.items():
         dget = DGet(
             formula,
             data_path.joinpath(f"{formula}.txt"),
             adduct=adduct,
             loadtxt_kws={"delimiter": "\t"},
         )
         dget.align_tof_with_spectra()
         # This test is too lenient, but best we can do with the data we have
         assert np.isclose(dget.deuteration * 100.0, percent_d, atol=1.6)
 
 
+def test_dget_auto_adduct():
+    for formula, (adduct, _) in formulas.items():
+        dget = DGet(
+            formula,
+            data_path.joinpath(f"{formula}.txt"),
+            loadtxt_kws={"delimiter": "\t"},
+        )
+        best, _ = dget.guess_adduct_from_base_peak()
+        assert best.adduct == adduct
+
+
 def test_deuteration():
     dget = DGet("C2H5D1", tofdata=(np.array([0.0, 999.0]), np.array([0.0, 0.0])))
     dget._probabilities = np.array([1.0, 0.0])
     assert np.isclose(dget.deuteration, 0.0)
     dget._probabilities = np.array([0.5, 0.5])
     assert np.isclose(dget.deuteration, 0.5)
     dget._probabilities = np.array([0.0, 1.0])
@@ -44,24 +56,68 @@
     dget._probabilities = np.array([0.1, 0.3, 0.6])
     assert np.isclose(dget.deuteration, 0.75)
 
     dget = DGet("C2H2D4", tofdata=(np.array([0.0, 999.0]), np.array([0.0, 0.0])))
     dget._probabilities = np.array([0.4, 0.2, 0.2, 0.1, 0.1])
     assert np.isclose(dget.deuteration, 0.325)
     dget._probabilities = np.array([0.5, 0.0, 0.0, 0.0, 0.5])
-    assert np.all(dget.deuteration_states == [2, 3, 4])
+    assert np.all(dget.deuteration_states == [3, 4])
     assert np.isclose(dget.deuteration, 1.0)
     dget._probabilities = np.array([0.1, 0.1, 0.2, 0.2, 0.4])
     assert np.isclose(dget.deuteration, 0.675)
     dget._probabilities = np.array([0.5, 0.0, 0.0, 0.0, 0.5])
-    dget.number_states = 4
+    dget.number_states = 5
     assert np.all(dget.deuteration_states == [0, 1, 2, 3, 4])
     assert np.isclose(dget.deuteration, 0.5)
 
 
+def test_number_states():
+    # Known error
+    dget = DGet("C6D6ClN", tofdata=(np.array([0.0, 999.0]), np.array([0.0, 0.0])))
+    dget._probabilities = np.array(
+        [
+            0.0,
+            0.0,
+            0.00722939,
+            0.02384589,
+            0.02229065,
+            0.19356285,
+            0.75307123,
+        ]
+    )
+    assert np.all(dget.deuteration_states == [2, 3, 4, 5, 6])
+
+    dget = DGet(
+        "CD5", number_states=3, tofdata=(np.array([0.0, 999.0]), np.array([0.0, 0.0]))
+    )
+    assert np.all(dget.deuteration_states == [3, 4, 5])
+    dget = DGet(
+        "CD5", number_states=30, tofdata=(np.array([0.0, 999.0]), np.array([0.0, 0.0]))
+    )
+    assert np.all(dget.deuteration_states == [0, 1, 2, 3, 4, 5])
+    with pytest.raises(ValueError):
+        dget = DGet(
+            "CD5",
+            number_states=0,
+            tofdata=(np.array([0.0, 999.0]), np.array([0.0, 0.0])),
+        )
+
+    dget = DGet("CD5", tofdata=(np.array([0.0, 999.0]), np.array([0.0, 0.0])))
+    dget._probabilities = np.array([0.0, 0.0, 0.0, 0.0, 0.0, 1.0])
+    assert np.all(dget.deuteration_states == [4, 5])
+    dget._probabilities = np.array([0.0, 0.0, 0.0, 0.0, 0.5, 0.5])
+    assert np.all(dget.deuteration_states == [3, 4, 5])
+    dget._probabilities = np.array([0.0, 0.0, 0.5, 0.0, 0.0, 0.5])
+    assert np.all(dget.deuteration_states == [4, 5])
+    dget._probabilities = np.array([0.0, 0.0, 0.0, 0.5, 0.0, 0.5])
+    assert np.all(dget.deuteration_states == [2, 3, 4, 5])
+    dget._probabilities = np.array([0.0, 0.3, 0.0, 0.4, 0.0, 0.3])
+    assert np.all(dget.deuteration_states == [0, 1, 2, 3, 4, 5])
+
+
 def test_targets():
     dget = DGet("C20D6", tofdata=(np.array([0.0, 999.0]), np.array([0.0, 0.0])))
     formulas = ["C20H6", "C20H5D", "C20H4D2", "C20H3D3", "C20H2D4", "C20HD5", "C20D6"]
 
     assert np.allclose(dget.targets[:7], [Formula(f).isotope.mz for f in formulas])
     assert np.allclose(
         dget.targets[6:],
```

### Comparing `DGet-0.8/tests/test_formula.py` & `DGet-0.9/tests/test_formula.py`

 * *Files identical despite different names*

