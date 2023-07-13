# Comparing `tmp/pymatgen-analysis-defects-2023.6.1.tar.gz` & `tmp/pymatgen-analysis-defects-2023.7.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymatgen-analysis-defects-2023.6.1.tar", last modified: Wed May 31 07:26:34 2023, max compression
+gzip compressed data, was "pymatgen-analysis-defects-2023.7.12.tar", last modified: Thu Jul 13 00:14:31 2023, max compression
```

## Comparing `pymatgen-analysis-defects-2023.6.1.tar` & `pymatgen-analysis-defects-2023.7.12.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:26:34.322738 pymatgen-analysis-defects-2023.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-31 07:26:34.322738 pymatgen-analysis-defects-2023.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:26:34.318738 pymatgen-analysis-defects-2023.6.1/pymatgen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:26:34.318738 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:26:34.318738 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    30806 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/ccd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    28813 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:26:34.318738 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/corrections/
--rw-r--r--   0 runner    (1001) docker     (123)    14730 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/corrections/freysoldt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/corrections/kumagai.py
--rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/finder.py
--rw-r--r--   0 runner    (1001) docker     (123)    17827 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/recombination.py
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/supercells.py
--rw-r--r--   0 runner    (1001) docker     (123)    42555 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/thermo.py
--rw-r--r--   0 runner    (1001) docker     (123)    38571 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:26:34.318738 pymatgen-analysis-defects-2023.6.1/pymatgen_analysis_defects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-31 07:26:34.000000 pymatgen-analysis-defects-2023.6.1/pymatgen_analysis_defects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-31 07:26:34.000000 pymatgen-analysis-defects-2023.6.1/pymatgen_analysis_defects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 07:26:34.000000 pymatgen-analysis-defects-2023.6.1/pymatgen_analysis_defects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-31 07:26:34.000000 pymatgen-analysis-defects-2023.6.1/pymatgen_analysis_defects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-31 07:26:34.000000 pymatgen-analysis-defects-2023.6.1/pymatgen_analysis_defects.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 07:26:34.322738 pymatgen-analysis-defects-2023.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:26:34.322738 pymatgen-analysis-defects-2023.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/tests/test_ccd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-31 07:26:16.000000 pymatgen-analysis-defects-2023.6.1/tests/test_corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-31 07:26:17.000000 pymatgen-analysis-defects-2023.6.1/tests/test_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-31 07:26:17.000000 pymatgen-analysis-defects-2023.6.1/tests/test_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-31 07:26:17.000000 pymatgen-analysis-defects-2023.6.1/tests/test_recombination.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-31 07:26:17.000000 pymatgen-analysis-defects-2023.6.1/tests/test_supercells.py
--rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-05-31 07:26:17.000000 pymatgen-analysis-defects-2023.6.1/tests/test_thermo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-05-31 07:26:17.000000 pymatgen-analysis-defects-2023.6.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:14:31.625632 pymatgen-analysis-defects-2023.7.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-13 00:14:31.625632 pymatgen-analysis-defects-2023.7.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:14:31.613632 pymatgen-analysis-defects-2023.7.12/pymatgen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:14:31.613632 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:14:31.621632 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30806 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/ccd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28813 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:14:31.621632 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/corrections/
+-rw-r--r--   0 runner    (1001) docker     (123)    14730 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/corrections/freysoldt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/corrections/kumagai.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/recombination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/supercells.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42555 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/thermo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38571 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:14:31.625632 pymatgen-analysis-defects-2023.7.12/pymatgen_analysis_defects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-13 00:14:31.000000 pymatgen-analysis-defects-2023.7.12/pymatgen_analysis_defects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-13 00:14:31.000000 pymatgen-analysis-defects-2023.7.12/pymatgen_analysis_defects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 00:14:31.000000 pymatgen-analysis-defects-2023.7.12/pymatgen_analysis_defects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-13 00:14:31.000000 pymatgen-analysis-defects-2023.7.12/pymatgen_analysis_defects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-13 00:14:31.000000 pymatgen-analysis-defects-2023.7.12/pymatgen_analysis_defects.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 00:14:31.625632 pymatgen-analysis-defects-2023.7.12/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:14:31.625632 pymatgen-analysis-defects-2023.7.12/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/tests/test_ccd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-13 00:14:12.000000 pymatgen-analysis-defects-2023.7.12/tests/test_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-13 00:14:13.000000 pymatgen-analysis-defects-2023.7.12/tests/test_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-13 00:14:13.000000 pymatgen-analysis-defects-2023.7.12/tests/test_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-13 00:14:13.000000 pymatgen-analysis-defects-2023.7.12/tests/test_recombination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-13 00:14:13.000000 pymatgen-analysis-defects-2023.7.12/tests/test_supercells.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-07-13 00:14:13.000000 pymatgen-analysis-defects-2023.7.12/tests/test_thermo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-13 00:14:13.000000 pymatgen-analysis-defects-2023.7.12/tests/test_utils.py
```

### Comparing `pymatgen-analysis-defects-2023.6.1/LICENSE` & `pymatgen-analysis-defects-2023.7.12/LICENSE`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.6.1/PKG-INFO` & `pymatgen-analysis-defects-2023.7.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymatgen-analysis-defects
-Version: 2023.6.1
+Version: 2023.7.12
 Summary: Pymatgen extension for defects analysis
 Author-email: Jimmy-Xuan Shen <jmmshn@gmail.com>
 License: modified BSD
 Project-URL: documentation, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: homepage, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: repository, https://github.com/materialsproject/pymatgen-analysis-defects
 Keywords: high-throughput,automated,dft,defects
```

### Comparing `pymatgen-analysis-defects-2023.6.1/README.rst` & `pymatgen-analysis-defects-2023.7.12/README.rst`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/ccd.py` & `pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/ccd.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/constants.py` & `pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/constants.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/core.py` & `pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/core.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/corrections/freysoldt.py` & `pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/corrections/freysoldt.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/corrections/kumagai.py` & `pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/corrections/kumagai.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/finder.py` & `pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/finder.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/generators.py` & `pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,61 +203,59 @@
     def __init__(self, min_dist: float = 0.5) -> None:
         self.min_dist = min_dist
 
     def generate(
         self,
         structure: Structure,
         insertions: dict[str, list[list[float]]],
-        multiplicies: dict[str, list[int]] | None = None,
+        multiplicities: dict[str, list[int]] | None = None,
         **kwargs,
     ) -> Generator[Interstitial, None, None]:
         """Generate interstitials.
 
         Args:
             structure: The bulk structure the interstitials are generated from.
             insertions: The insertions to be made given as a dictionary {"Mg": [[0.0, 0.0, 0.0], [0.5, 0.5, 0.5]]}.
-            multiplicies: The multiplicities of the insertions to be made given as a dictionary {"Mg": [1, 2]}.
+            multiplicities: The multiplicities of the insertions to be made given as a dictionary {"Mg": [1, 2]}.
             **kwargs: Additional keyword arguments for the ``Interstitial`` constructor.
 
         Returns:
             Generator[Interstitial, None, None]: Generator that yields a list of ``Interstitial`` objects
         """
-        if multiplicies is None:
-            multiplicies = {
+        if multiplicities is None:
+            multiplicities = {
                 el_str: [1] * len(coords) for el_str, coords in insertions.items()
             }
 
         for el_str, coords in insertions.items():
-            for i, coord in enumerate(
-                self._filter_colliding(coords, structure=structure)
-            ):
-                mul = multiplicies[el_str][i]
+            for i, coord in self._filter_colliding(coords, structure=structure):
+                mul = multiplicities[el_str][i]
                 isite = PeriodicSite(
                     species=Species(el_str), coords=coord, lattice=structure.lattice
                 )
                 yield Interstitial(structure, isite, multiplicity=mul, **kwargs)
 
     def _filter_colliding(
         self, fcoords: list[list[float]], structure: Structure
-    ) -> Generator[list[float], None, None]:
+    ) -> Generator[tuple[int, list[float]], None, None]:
         """Check the sites for collisions.
 
         Args:
             fcoords: List of fractional coordinates of the sites.
             structure: The bulk structure the interstitials placed in.
         """
         unique_fcoords = set(tuple(f) for f in fcoords)
         cleaned_fcoords = remove_collisions(
             fcoords=list(unique_fcoords), structure=structure, min_dist=self.min_dist
         )
         cleaned_fcoords = set(tuple(f) for f in cleaned_fcoords)
-        for fc in fcoords:
+        for i, fc in enumerate(fcoords):
             if tuple(fc) not in cleaned_fcoords:
                 continue
-            yield fc
+            yield i, fc
 
 
 class VoronoiInterstitialGenerator(InterstitialGenerator):
     """Generator for interstitials based on a simple Voronoi.
 
     Attributes:
         clustering_tol: Tolerance for clustering the Voronoi nodes.
@@ -279,15 +277,15 @@
     ) -> None:
         self.clustering_tol = clustering_tol
         self.min_dist = min_dist
         self.ltol = ltol
         self.stol = stol
         self.angle_tol = angle_tol
         self.top_kwargs = kwargs
-        super().__init__()
+        super().__init__(min_dist=min_dist)
 
     def generate(self, structure: Structure, insert_species: set[str] | list[str], **kwargs) -> Generator[Interstitial, None, None]:  # type: ignore[override]
         """Generate interstitials.
 
         Args:
             structure: The bulk structure the interstitials inserted in.
             insert_species: The species to be inserted.
@@ -298,29 +296,38 @@
         cand_sites_and_mul = [*self._get_candidate_sites(structure)]
         for species in insert_species:
             cand_sites = [cand_site for cand_site, mul in cand_sites_and_mul]
             multiplicity = [mul for cand_site, mul in cand_sites_and_mul]
             yield from super().generate(
                 structure,
                 insertions={species: cand_sites},
-                multiplicies={species: multiplicity},
+                multiplicities={species: multiplicity},
                 **kwargs,
             )
 
     def _get_candidate_sites(
         self, structure: Structure
     ) -> Generator[tuple[list[float], int], None, None]:
         """Get the candidate sites for interstitials.
 
         Args:
             structure: The bulk structure the interstitials inserted in.
         """
         framework = list(structure.symbol_set)
         top = TopographyAnalyzer(
-            structure, framework, [], check_volume=False, **self.top_kwargs
+            structure,
+            framework,
+            [],
+            check_volume=False,
+            clustering_tol=self.clustering_tol,
+            min_dist=self.min_dist,
+            ltol=self.ltol,
+            stol=self.stol,
+            angle_tol=self.angle_tol,
+            **self.top_kwargs,
         )
         insert_sites = dict()
         multiplicity: dict[int, int] = dict()
         for fpos, lab in top.labeled_sites:
             if lab in insert_sites:
                 multiplicity[lab] += 1
                 continue
@@ -379,15 +386,15 @@
             cand_sites = [cand_site for cand_site, mul in cand_sites_and_mul]
             if self.max_insertions is not None:
                 cand_sites = cand_sites[: self.max_insertions]
             multiplicity = [mul for cand_site, mul in cand_sites_and_mul]
             yield from super().generate(
                 chgcar.structure,
                 insertions={species: cand_sites},
-                multiplicies={species: multiplicity},
+                multiplicities={species: multiplicity},
                 **kwargs,
             )
 
     def _get_candidate_sites(self, chgcar: Chgcar):
         cia = ChargeInsertionAnalyzer(
             chgcar,
             clustering_tol=self.clustering_tol,
```

### Comparing `pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/recombination.py` & `pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/recombination.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/supercells.py` & `pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/supercells.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/thermo.py` & `pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/thermo.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.6.1/pymatgen/analysis/defects/utils.py` & `pymatgen-analysis-defects-2023.7.12/pymatgen/analysis/defects/utils.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.6.1/pymatgen_analysis_defects.egg-info/PKG-INFO` & `pymatgen-analysis-defects-2023.7.12/pymatgen_analysis_defects.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymatgen-analysis-defects
-Version: 2023.6.1
+Version: 2023.7.12
 Summary: Pymatgen extension for defects analysis
 Author-email: Jimmy-Xuan Shen <jmmshn@gmail.com>
 License: modified BSD
 Project-URL: documentation, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: homepage, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: repository, https://github.com/materialsproject/pymatgen-analysis-defects
 Keywords: high-throughput,automated,dft,defects
```

### Comparing `pymatgen-analysis-defects-2023.6.1/pymatgen_analysis_defects.egg-info/SOURCES.txt` & `pymatgen-analysis-defects-2023.7.12/pymatgen_analysis_defects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.6.1/pyproject.toml` & `pymatgen-analysis-defects-2023.7.12/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -31,18 +31,18 @@
   "jupyter-book>=0.13.1",
 ]
 pydefect = ["pydefect>=0.6.2"]
 
 strict = [
   "pymatgen>=2023.5.8",
   "dscribe==1.2.2",
-  "scikit-image==0.19.3",
+  "scikit-image==0.20.0",
   "pytest==7.2.2",
   "pytest-cov==4.0.0",
-  "pre-commit==3.1.0",
+  "pre-commit==3.3.3",
   "mp-pyrho==0.3.0",
   "numpy==1.23.5"
 ]
 
 tests = ["pytest==7.2.2", "pytest-cov==4.0.0"]
 
 [tool.setuptools.dynamic]
```

### Comparing `pymatgen-analysis-defects-2023.6.1/tests/test_ccd.py` & `pymatgen-analysis-defects-2023.7.12/tests/test_ccd.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.6.1/tests/test_core.py` & `pymatgen-analysis-defects-2023.7.12/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.6.1/tests/test_corrections.py` & `pymatgen-analysis-defects-2023.7.12/tests/test_corrections.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.6.1/tests/test_finder.py` & `pymatgen-analysis-defects-2023.7.12/tests/test_finder.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.6.1/tests/test_generators.py` & `pymatgen-analysis-defects-2023.7.12/tests/test_generators.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.6.1/tests/test_recombination.py` & `pymatgen-analysis-defects-2023.7.12/tests/test_recombination.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.6.1/tests/test_supercells.py` & `pymatgen-analysis-defects-2023.7.12/tests/test_supercells.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.6.1/tests/test_thermo.py` & `pymatgen-analysis-defects-2023.7.12/tests/test_thermo.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.6.1/tests/test_utils.py` & `pymatgen-analysis-defects-2023.7.12/tests/test_utils.py`

 * *Files identical despite different names*

