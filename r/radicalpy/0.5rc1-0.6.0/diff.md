# Comparing `tmp/radicalpy-0.5rc1.tar.gz` & `tmp/radicalpy-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radicalpy-0.5rc1.tar", last modified: Fri Dec  2 05:37:43 2022, max compression
+gzip compressed data, was "radicalpy-0.6.0.tar", last modified: Wed Jul 12 09:01:35 2023, max compression
```

## Comparing `radicalpy-0.5rc1.tar` & `radicalpy-0.6.0.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 05:37:42.992740 radicalpy-0.5rc1/
--rw-r--r--   0 runner    (1001) docker     (116)     1068 2022-12-02 05:37:31.000000 radicalpy-0.5rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-12-02 05:37:31.000000 radicalpy-0.5rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)      369 2022-12-02 05:37:42.992740 radicalpy-0.5rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       23 2022-12-02 05:37:31.000000 radicalpy-0.5rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-12-02 05:37:42.992740 radicalpy-0.5rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      947 2022-12-02 05:37:31.000000 radicalpy-0.5rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 05:37:42.988740 radicalpy-0.5rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 05:37:42.992740 radicalpy-0.5rc1/src/radicalpy/
--rw-r--r--   0 runner    (1001) docker     (116)       79 2022-12-02 05:37:31.000000 radicalpy-0.5rc1/src/radicalpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1642 2022-12-02 05:37:31.000000 radicalpy-0.5rc1/src/radicalpy/classical.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 05:37:42.992740 radicalpy-0.5rc1/src/radicalpy/data/
--rw-r--r--   0 runner    (1001) docker     (116)     2681 2022-12-02 05:37:31.000000 radicalpy-0.5rc1/src/radicalpy/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2498 2022-12-02 05:37:31.000000 radicalpy-0.5rc1/src/radicalpy/data/constants.json
--rw-r--r--   0 runner    (1001) docker     (116)      396 2022-12-02 05:37:31.000000 radicalpy-0.5rc1/src/radicalpy/data/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 05:37:42.992740 radicalpy-0.5rc1/src/radicalpy/data/molecules/
--rw-r--r--   0 runner    (1001) docker     (116)      471 2022-12-02 05:37:31.000000 radicalpy-0.5rc1/src/radicalpy/data/molecules/2_6_aqds.json
--rw-r--r--   0 runner    (1001) docker     (116)      405 2022-12-02 05:37:31.000000 radicalpy-0.5rc1/src/radicalpy/data/molecules/adenine_cation.json
--rw-r--r--   0 runner    (1001) docker     (116)     6719 2022-12-02 05:37:31.000000 radicalpy-0.5rc1/src/radicalpy/data/molecules/flavin_anion.json
--rw-r--r--   0 runner    (1001) docker     (116)     1444 2022-12-02 05:37:31.000000 radicalpy-0.5rc1/src/radicalpy/data/molecules/flavin_neutral.json
--rw-r--r--   0 runner    (1001) docker     (116)     3297 2022-12-02 05:37:31.000000 radicalpy-0.5rc1/src/radicalpy/data/molecules/tryptophan_cation.json
--rw-r--r--   0 runner    (1001) docker     (116)     3293 2022-12-02 05:37:31.000000 radicalpy-0.5rc1/src/radicalpy/data/molecules/tyrosine_neutral.json
--rw-r--r--   0 runner    (1001) docker     (116)    27847 2022-12-02 05:37:31.000000 radicalpy-0.5rc1/src/radicalpy/data/spin_data.json
--rw-r--r--   0 runner    (1001) docker     (116)     5138 2022-12-02 05:37:31.000000 radicalpy-0.5rc1/src/radicalpy/estimations.py
--rw-r--r--   0 runner    (1001) docker     (116)     2984 2022-12-02 05:37:31.000000 radicalpy-0.5rc1/src/radicalpy/kinetics.py
--rw-r--r--   0 runner    (1001) docker     (116)     6190 2022-12-02 05:37:31.000000 radicalpy-0.5rc1/src/radicalpy/plot.py
--rw-r--r--   0 runner    (1001) docker     (116)     5024 2022-12-02 05:37:31.000000 radicalpy-0.5rc1/src/radicalpy/relaxation.py
--rw-r--r--   0 runner    (1001) docker     (116)    32550 2022-12-02 05:37:31.000000 radicalpy-0.5rc1/src/radicalpy/simulation.py
--rw-r--r--   0 runner    (1001) docker     (116)     7022 2022-12-02 05:37:31.000000 radicalpy-0.5rc1/src/radicalpy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 05:37:42.992740 radicalpy-0.5rc1/src/radicalpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      369 2022-12-02 05:37:42.000000 radicalpy-0.5rc1/src/radicalpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      976 2022-12-02 05:37:42.000000 radicalpy-0.5rc1/src/radicalpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-02 05:37:42.000000 radicalpy-0.5rc1/src/radicalpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       36 2022-12-02 05:37:42.000000 radicalpy-0.5rc1/src/radicalpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       16 2022-12-02 05:37:42.000000 radicalpy-0.5rc1/src/radicalpy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 05:37:42.992740 radicalpy-0.5rc1/src/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-12-02 05:37:31.000000 radicalpy-0.5rc1/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    47664 2022-12-02 05:37:31.000000 radicalpy-0.5rc1/src/tests/radpy.py
--rw-r--r--   0 runner    (1001) docker     (116)      219 2022-12-02 05:37:31.000000 radicalpy-0.5rc1/src/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (116)      957 2022-12-02 05:37:31.000000 radicalpy-0.5rc1/src/tests/test_estimations.py
--rw-r--r--   0 runner    (1001) docker     (116)    19932 2022-12-02 05:37:31.000000 radicalpy-0.5rc1/src/tests/test_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:01:35.253023 radicalpy-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-07-12 09:01:23.000000 radicalpy-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-07-12 09:01:35.249023 radicalpy-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-07-12 09:01:23.000000 radicalpy-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-07-12 09:01:23.000000 radicalpy-0.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:01:35.249023 radicalpy-0.6.0/radicalpy/
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-07-12 09:01:23.000000 radicalpy-0.6.0/radicalpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4924 2023-07-12 09:01:23.000000 radicalpy-0.6.0/radicalpy/classical.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:01:35.249023 radicalpy-0.6.0/radicalpy/data/
+-rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-07-12 09:01:23.000000 radicalpy-0.6.0/radicalpy/data/constants.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:01:35.249023 radicalpy-0.6.0/radicalpy/data/molecules/
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-07-12 09:01:23.000000 radicalpy-0.6.0/radicalpy/data/molecules/2_6_aqds.json
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-07-12 09:01:23.000000 radicalpy-0.6.0/radicalpy/data/molecules/adenine_cation.json
+-rw-r--r--   0 runner    (1001) docker     (122)     6719 2023-07-12 09:01:23.000000 radicalpy-0.6.0/radicalpy/data/molecules/flavin_anion.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-07-12 09:01:23.000000 radicalpy-0.6.0/radicalpy/data/molecules/flavin_neutral.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3297 2023-07-12 09:01:23.000000 radicalpy-0.6.0/radicalpy/data/molecules/tryptophan_cation.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3293 2023-07-12 09:01:23.000000 radicalpy-0.6.0/radicalpy/data/molecules/tyrosine_neutral.json
+-rw-r--r--   0 runner    (1001) docker     (122)    27847 2023-07-12 09:01:23.000000 radicalpy-0.6.0/radicalpy/data/spin_data.json
+-rw-r--r--   0 runner    (1001) docker     (122)    16112 2023-07-12 09:01:23.000000 radicalpy-0.6.0/radicalpy/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20261 2023-07-12 09:01:23.000000 radicalpy-0.6.0/radicalpy/estimations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5054 2023-07-12 09:01:23.000000 radicalpy-0.6.0/radicalpy/kinetics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6252 2023-07-12 09:01:23.000000 radicalpy-0.6.0/radicalpy/plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9710 2023-07-12 09:01:23.000000 radicalpy-0.6.0/radicalpy/relaxation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-07-12 09:01:23.000000 radicalpy-0.6.0/radicalpy/shared.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25083 2023-07-12 09:01:23.000000 radicalpy-0.6.0/radicalpy/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11422 2023-07-12 09:01:23.000000 radicalpy-0.6.0/radicalpy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:01:35.249023 radicalpy-0.6.0/radicalpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-07-12 09:01:35.000000 radicalpy-0.6.0/radicalpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      872 2023-07-12 09:01:35.000000 radicalpy-0.6.0/radicalpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 09:01:35.000000 radicalpy-0.6.0/radicalpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-12 09:01:35.000000 radicalpy-0.6.0/radicalpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-12 09:01:35.000000 radicalpy-0.6.0/radicalpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-07-12 09:01:23.000000 radicalpy-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-12 09:01:35.253023 radicalpy-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 09:01:35.249023 radicalpy-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3157 2023-07-12 09:01:23.000000 radicalpy-0.6.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3948 2023-07-12 09:01:23.000000 radicalpy-0.6.0/tests/test_estimations.py
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-07-12 09:01:23.000000 radicalpy-0.6.0/tests/test_relaxations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-07-12 09:01:23.000000 radicalpy-0.6.0/tests/test_shared.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19571 2023-07-12 09:01:23.000000 radicalpy-0.6.0/tests/test_simulation.py
```

### Comparing `radicalpy-0.5rc1/LICENSE` & `radicalpy-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `radicalpy-0.5rc1/src/radicalpy/data/constants.json` & `radicalpy-0.6.0/radicalpy/data/constants.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9970238095238095%*

 * *Differences: {"'rw'": "{'value': 1.6e-10}"}*

```diff
@@ -108,10 +108,10 @@
         "unit": "J T^{-1}",
         "value": 1.41060671e-26
     },
     "rw": {
         "alt_def": "average of 1.6 to 3.2 A (1/2 to 1 hydration shell)",
         "name": "hydration layer",
         "unit": "m",
-        "value": 2.4e-10
+        "value": 1.6e-10
     }
 }
```

### Comparing `radicalpy-0.5rc1/src/radicalpy/data/molecules/flavin_anion.json` & `radicalpy-0.6.0/radicalpy/data/molecules/flavin_anion.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.5rc1/src/radicalpy/data/molecules/flavin_neutral.json` & `radicalpy-0.6.0/radicalpy/data/molecules/flavin_neutral.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.5rc1/src/radicalpy/data/molecules/tryptophan_cation.json` & `radicalpy-0.6.0/radicalpy/data/molecules/tryptophan_cation.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.5rc1/src/radicalpy/data/molecules/tyrosine_neutral.json` & `radicalpy-0.6.0/radicalpy/data/molecules/tyrosine_neutral.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.5rc1/src/radicalpy/data/spin_data.json` & `radicalpy-0.6.0/radicalpy/data/spin_data.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.5rc1/src/radicalpy/plot.py` & `radicalpy-0.6.0/radicalpy/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,19 +162,20 @@
     ax.set_zlabel("$Z$ (nm)", size=14)
     # plt.xlim([-1, 1]); plt.ylim([-1, 1])
     plt.tick_params(labelsize=14)
     fig.set_size_inches(10, 10)
 
 
 def spin_state_labels(sim: HilbertSimulation):
-    if sim.num_electrons != 2:
+    if len(sim.radicals) != 2:
         raise ValueError(
             "Density matrix plotting make little sense for non-radical pairs!"
         )
-    multiplicities = sim.multiplicities[sim.num_electrons :]
+    # multiplicities = sim.multiplicities[len(sim.radicals) :]
+    multiplicities = [r.multiplicity for r in sim.radicals]
     old_labels = [
         State.TRIPLET_PLUS.value,
         State.TRIPLET_ZERO.value,
         State.SINGLET.value,
         State.TRIPLET_MINUS.value,
     ]
     for m in multiplicities:
```

### Comparing `radicalpy-0.5rc1/src/radicalpy/simulation.py` & `radicalpy-0.6.0/radicalpy/simulation.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 import enum
 from math import prod
 from typing import Iterable, Optional
 
 import numpy as np
 import scipy as sp
+from tqdm import tqdm
 
 from . import utils
-from .data import (MOLECULE_DATA, SPIN_DATA, gamma_mT, get_molecules,
-                   multiplicity, pauli)
+from .data import Molecule
 
 
 class State(enum.Enum):
     EQUILIBRIUM = "Eq"
     SINGLET = "S"
     TRIPLET = "T"
     TRIPLET_ZERO = "T_0"
@@ -23,278 +23,34 @@
 
 
 class Basis(enum.Enum):
     ZEEMAN = "Zeeman"
     ST = "ST"
 
 
-class Molecule:
-    """Representation of a molecule for the simulation.
-
-    Args:
-        radical (str): the name of the `Molecule`, defaults to `""`
-
-        nuclei (list[str]): list of atoms from the molecule (or from
-            the database), defaults to `[]`
-
-        multiplicities (list[int]): list of multiplicities of the
-            atoms and their isotopes (when not using the database),
-            defaults to `[]`
-
-        gammas_mT (list[float]): list of gyromagnetic ratios of the
-            atoms and their isotopes (when not using the database),
-            defaults to `[]`
-
-        hfcs (list[float]): list of hyperfine coupling constants of
-            the atoms and their isotopes (when not using the
-            database), defaults to `[]`
-
-    A molecule is represented by hyperfine coupling constants, spin
-    multiplicities and gyromagnetic ratios (gammas, specified in mT)
-    of its nuclei.  When using the database, one needs to specify the
-    name of the molecule and the list of its nuclei.
-
-    >>> Molecule(radical="adenine_cation",
-    ...          nuclei=["N6-H1", "N6-H2"])
-    Molecule: adenine_cation
-      HFCs: [-0.63, -0.66]
-      Multiplicities: [3, 3]
-      Magnetogyric ratios (mT): [19337.792, 19337.792]
-      Number of particles: 2
-
-
-    If the wrong molecule name is given, the error helps you find the
-    valid options.
-
-    >>> Molecule("foobar", ["H1"])
-    Traceback (most recent call last):
-    ...
-    ValueError: Available molecules below:
-    2_6_aqds
-    adenine_cation
-    flavin_anion
-    flavin_neutral
-    tryptophan_cation
-    tyrosine_neutral
-
-    Similarly, giving a list of incorrect atom names will also result
-    in a helpful error message listing the available atoms.
-
-    >>> Molecule("tryptophan_cation", ["buz"])
-    Traceback (most recent call last):
-    ...
-    ValueError: Available nuclei below.
-    Hbeta1 (hfc = 1.6045)
-    H1 (hfc = -0.5983)
-    H4 (hfc = -0.4879)
-    H7 (hfc = -0.3634)
-    N1 (hfc = 0.32156666666666667)
-    H2 (hfc = -0.278)
-    N* (hfc = 0.1465)
-    Halpha (hfc = -0.09306666666666667)
-    Hbeta2 (hfc = 0.04566666666666666)
-    H5 (hfc = -0.04)
-    H6 (hfc = -0.032133333333333326)
-
-    >>> Molecule("adenine_cation", ["buz"])
-    Traceback (most recent call last):
-    ...
-    ValueError: Available nuclei below.
-    N6-H2 (hfc = -0.66)
-    N6-H1 (hfc = -0.63)
-    C8-H (hfc = -0.55)
-
-    One can also specify a list of custom hyperfine coupling constants
-    along with a list of their respective isotope names.
-
-    >>> Molecule(nuclei=["1H", "14N"], hfcs=[0.41, 1.82])
-    Molecule: N/A
-      HFCs: [0.41, 1.82]
-      Multiplicities: [2, 3]
-      Magnetogyric ratios (mT): [267522.18744, 19337.792]
-      Number of particles: 2
-
-    Same as above, but with an informative molecule name (doesn't
-    affect behaviour):
-
-    >>> Molecule("isotopes", nuclei=["15N", "15N"], hfcs=[0.3, 1.7])
-    Molecule: isotopes
-      HFCs: [0.3, 1.7]
-      Multiplicities: [2, 2]
-      Magnetogyric ratios (mT): [-27126.180399999997, -27126.180399999997]
-      Number of particles: 2
-
-    A molecule with no HFCs, for one proton radical pair simulations
-    (for simple simulations -- often with *fantastic* low-field
-    effects):
-
-    >>> Molecule("kryptonite")
-    Molecule: kryptonite
-      HFCs: []
-      Multiplicities: []
-      Magnetogyric ratios (mT): []
-      Number of particles: 0
-
-    Manual input for all relevant values (multiplicities, gammas,
-    HFCs):
-
-    >>> Molecule(multiplicities=[2, 2, 3],
-    ...          gammas_mT=[267522.18744, 267522.18744, 19337.792],
-    ...          hfcs=[0.42, 1.01, 1.33])
-    Molecule: N/A
-      HFCs: [0.42, 1.01, 1.33]
-      Multiplicities: [2, 2, 3]
-      Magnetogyric ratios (mT): [267522.18744, 267522.18744, 19337.792]
-      Number of particles: 3
-
-    Same as above with an informative molecule name:
-
-    >>> Molecule("my_flavin", multiplicities=[2], gammas_mT=[267522.18744], hfcs=[0.5])
-    Molecule: my_flavin
-      HFCs: [0.5]
-      Multiplicities: [2]
-      Magnetogyric ratios (mT): [267522.18744]
-      Number of particles: 1
-
-    """
-
-    def __init__(
-        self,
-        radical: str = "",
-        nuclei: list[str] = [],
-        multiplicities: list[int] = [],
-        gammas_mT: list[float] = [],
-        hfcs: list[float] = [],
-    ):
-        self.radical = radical if radical else "N/A"
-        self.nuclei = nuclei
-        self.custom_molecule = True
-        if nuclei:
-            if self._check_molecule_or_spin_db(radical, nuclei):
-                self._init_from_molecule_db(radical, nuclei)
-            else:
-                self._init_from_spin_db(radical, nuclei, hfcs)
-        else:
-            if self._check_molecule_or_spin_db(radical, nuclei):
-                self._init_from_molecule_db(radical, nuclei)
-            else:
-                self.multiplicities = multiplicities
-                self.gammas_mT = gammas_mT
-                self.hfcs = hfcs
-        if self.hfcs and isinstance(self.hfcs[0], list):
-            self.hfcs = [np.array(h) for h in self.hfcs]
-        assert len(self.multiplicities) == self.num_particles
-        assert len(self.gammas_mT) == self.num_particles
-        assert len(self.hfcs) == self.num_particles
-
-    def __repr__(self) -> str:
-        """Pretty print the molecule.
-
-        Returns:
-            str: Representation of a molecule.
-        """
-        return (
-            f"Molecule: {self.radical}"
-            # f"\n  Nuclei: {self.nuclei}"
-            f"\n  HFCs: {self.hfcs}"
-            f"\n  Multiplicities: {self.multiplicities}"
-            f"\n  Magnetogyric ratios (mT): {self.gammas_mT}"
-            f"\n  Number of particles: {self.num_particles}"
-            # f"\n  elements: {self.elements}"
-        )
-
-    def _check_molecule_or_spin_db(self, radical, nuclei):
-        if radical in MOLECULE_DATA:
-            self._check_nuclei(nuclei)
-            return True
-        else:
-            # TODO: needs to fail with nuclei == [] + wrong molecule
-            # name
-            if all(n in SPIN_DATA for n in nuclei):
-                return False
-            else:
-                available = "\n".join(get_molecules().keys())
-                raise ValueError(f"Available molecules below:\n{available}")
-
-    def _check_nuclei(self, nuclei: list[str]) -> None:
-        molecule_data = MOLECULE_DATA[self.radical]["data"]
-        for nucleus in nuclei:
-            if nucleus not in molecule_data:
-                keys = molecule_data.keys()
-                hfcs = [molecule_data[k]["hfc"] for k in keys]
-                hfcs = [
-                    utils.isotropic(np.array(h)) if isinstance(h, list) else h
-                    for h in hfcs
-                ]
-                pairs = sorted(
-                    zip(keys, hfcs), key=lambda t: np.abs(t[1]), reverse=True
-                )
-                available = "\n".join([f"{k} (hfc = {h})" for k, h in pairs])
-                raise ValueError(f"Available nuclei below.\n{available}")
-
-    def _init_from_molecule_db(self, radical: str, nuclei: list[str]) -> None:
-        data = MOLECULE_DATA[radical]["data"]
-        elem = [data[n]["element"] for n in nuclei]
-        self.radical = radical
-        self.gammas_mT = [gamma_mT(e) for e in elem]
-        self.multiplicities = [multiplicity(e) for e in elem]
-        self.hfcs = [data[n]["hfc"] for n in nuclei]
-        self.custom_molecule = False
-
-    def _init_from_spin_db(
-        self, radical: str, nuclei: list[str], hfcs: list[float]
-    ) -> None:
-        self.multiplicities = [multiplicity(e) for e in nuclei]
-        self.gammas_mT = [gamma_mT(e) for e in nuclei]
-        self.hfcs = hfcs
-
-    @property
-    def effective_hyperfine(self) -> float:
-        if self.custom_molecule:
-            multiplicities = self.multiplicities
-            hfcs = self.hfcs
-        else:
-            # TODO: this can fail with wrong molecule name
-            data = MOLECULE_DATA[self.radical]["data"]
-            nuclei = list(data.keys())
-            elem = [data[n]["element"] for n in nuclei]
-            multiplicities = [multiplicity(e) for e in elem]
-            hfcs = [data[n]["hfc"] for n in nuclei]
-
-        # spin quantum number
-        s = np.array(list(map(utils.spin_quantum_number, multiplicities)))
-        hfcs = [utils.isotropic(h) if isinstance(h, list) else h for h in hfcs]
-        hfcs = np.array(hfcs)
-        return np.sqrt((4 / 3) * sum((hfcs**2 * s) * (s + 1)))
-
-    @property
-    def num_particles(self) -> int:
-        """Return the number of isotopes in the molecule."""
-        return len(self.multiplicities)
-
-
-class KineticsRelaxationBase:
+class HilbertIncoherentProcessBase:
     def __init__(self, rate_constant: float):
         self.rate = rate_constant
 
     def init(self, sim):
         pass
 
     def adjust_hamiltonian(self, *args, **kwargs):
         return
 
     def adjust_product_probabilities(self, *args, **kwargs):
         return
 
     @property
     def rate_constant(self) -> float:
+        """Rate of the incoherent process."""
         return self.rate
 
-    def _name(self):
-        return f"Kinetics: {type(self).__name__}"
+    def _name(self) -> str:
+        return str(type(self).__name__)
 
     def __repr__(self) -> str:
         lines = [
             self._name(),
             f"Rate constant: {self.rate}",
         ]
         return "\n".join(lines)
@@ -305,110 +61,64 @@
 
     Args:
         molecules (list[Molecule]): List of `Molecule` objects.
 
         custom_gfactor (bool): Flag to use g-factors instead of the
             default gyromagnetic ratio gamma.
 
-    >>> HilbertSimulation([Molecule("flavin_anion", ["N5"]),
-    ...                    Molecule("tryptophan_cation", ["Hbeta1", "H1"])])
+    >>> HilbertSimulation([Molecule.fromdb("flavin_anion", ["N5"]),
+    ...                    Molecule.fromdb("tryptophan_cation", ["Hbeta1", "H1"])])
     Number of electrons: 2
     Number of nuclei: 3
     Number of particles: 5
     Multiplicities: [2, 2, 3, 2, 2]
     Magnetogyric ratios (mT): [-176085963.023, -176085963.023, 19337.792, 267522.18744, 267522.18744]
-    Nuclei: ['N5', 'Hbeta1', 'H1']
+    Nuclei: [14N(19337792.0, 3, 0.5141 <anisotropic available>), 1H(267522187.44, 2, 1.605 <anisotropic available>), 1H(267522187.44, 2, -0.5983 <anisotropic available>)]
     Couplings: [0, 1, 1]
-    HFCs (mT): [array([[-0.06819637,  0.01570029,  0.08701531],
-           [ 0.01570029, -0.03652102,  0.27142597],
-           [ 0.08701531,  0.27142597,  1.64713923]]), array([[ 1.5808, -0.0453, -0.0506],
-           [-0.0453,  1.5575,  0.0988],
-           [-0.0506,  0.0988,  1.6752]]), array([[-0.992 , -0.2091, -0.2003],
-           [-0.2091, -0.2631,  0.2803],
-           [-0.2003,  0.2803, -0.5398]])]
+    HFCs (mT): [0.5141 <anisotropic available>, 1.605 <anisotropic available>, -0.5983 <anisotropic available>]
     """
 
     def __init__(
         self,
         molecules: list[Molecule],
         custom_gfactors: bool = False,
         basis: Basis = Basis.ST,
     ):
         self.molecules = molecules
         self.custom_gfactors = custom_gfactors
         self.basis = basis
 
     @property
     def coupling(self):
-        return sum([[i] * m.num_particles for i, m in enumerate(self.molecules)], [])
-
-    @property
-    def electrons(self):
-        return ["E"] * self.num_electrons
-
-    @property
-    def hfcs(self):
-        return sum([m.hfcs for m in self.molecules], [])
-
-    @property
-    def num_electrons(self):
-        return len(self.molecules)
-
-    @property
-    def num_nuclei(self):
-        return sum([m.num_particles for m in self.molecules])
-
-    @property
-    def num_particles(self):
-        return self.num_electrons + self.num_nuclei
-
-    @property
-    def electron_multiplicities(self):
-        return list(map(multiplicity, self.electrons))
-
-    @property
-    def nuclei_multiplicities(self):
-        return sum([m.multiplicities for m in self.molecules], [])
-
-    @property
-    def multiplicities(self):
-        return self.electron_multiplicities + self.nuclei_multiplicities
+        return sum([[i] * len(m.nuclei) for i, m in enumerate(self.molecules)], [])
 
     @property
-    def electron_gammas_mT(self):
-        g = 2.0023  # free electron g-factor
-        gfactor = [g, g]
-        if self.custom_gfactors:
-            # overwrite gfactor list TODO
-            pass
-        # muB = 9.274e-24
-        # hbar = 1.05459e-34
-        # return [gfactor[i] * muB / hbar / 1000 for i in range(self.num_electrons)]
-        return [gamma_mT(e) * gfactor[i] / g for i, e in enumerate(self.electrons)]
+    def radicals(self):
+        return [m.radical for m in self.molecules]
 
     @property
-    def nuclei_gammas_mT(self):
-        return sum([m.gammas_mT for m in self.molecules], [])
+    def nuclei(self):
+        return sum([[n for n in m.nuclei] for m in self.molecules], [])
 
     @property
-    def gammas_mT(self):
-        return self.electron_gammas_mT + self.nuclei_gammas_mT
+    def particles(self):
+        return self.radicals + self.nuclei
 
     def __repr__(self) -> str:
         return "\n".join(
             [
                 # "Simulation summary:",
-                f"Number of electrons: {self.num_electrons}",
-                f"Number of nuclei: {len(self.hfcs)}",
-                f"Number of particles: {self.num_particles}",
-                f"Multiplicities: {self.multiplicities}",
-                f"Magnetogyric ratios (mT): {self.gammas_mT}",
+                f"Number of electrons: {len(self.radicals)}",
+                f"Number of nuclei: {len(self.nuclei)}",
+                f"Number of particles: {len(self.particles)}",
+                f"Multiplicities: {[p.multiplicity for p in self.particles]}",
+                f"Magnetogyric ratios (mT): {[p.gamma_mT for p in self.particles]}",
                 f"Nuclei: {sum([m.nuclei for m in self.molecules], [])}",
                 f"Couplings: {self.coupling}",
-                f"HFCs (mT): {self.hfcs}",
+                f"HFCs (mT): {[n.hfc for n in self.nuclei]}",
                 # "",
                 # f"Simulated molecules:\n{molecules}",
             ]
         )
 
     def ST_basis(self, M):
         # T+  T0  S  T-
@@ -417,39 +127,86 @@
                 [1, 0, 0, 0],
                 [0, 1 / np.sqrt(2), 1 / np.sqrt(2), 0],
                 [0, -1 / np.sqrt(2), 1 / np.sqrt(2), 0],
                 [0, 0, 0, 1],
             ]
         )
 
-        C = np.kron(ST, np.eye(prod(self.nuclei_multiplicities)))
+        C = np.kron(ST, np.eye(prod([n.multiplicity for n in self.nuclei])))
         return C @ M @ C.T
 
+    @staticmethod
+    def pauli(mult: int):
+        """Generate Pauli matrices.
+
+        Generates the Pauli matrices corresponding to a given multiplicity.
+
+        Args:
+            mult (int): The multiplicity of the element.
+
+        Return:
+            dict: A dictionary containing 6 `np.array` matrices of
+            shape `(mult, mult)`:
+
+            - the unit operator `result["u"]`,
+            - raising operator `result["p"]`,
+            - lowering operator `result["m"]`,
+            - Pauli matrix for x axis `result["x"]`,
+            - Pauli matrix for y axis `result["y"]`,
+            - Pauli matrix for z axis `result["z"]`.
+        """
+        assert mult > 1
+        result = {}
+        if mult == 2:
+            result["u"] = np.array([[1, 0], [0, 1]])
+            result["p"] = np.array([[0, 1], [0, 0]])
+            result["m"] = np.array([[0, 0], [1, 0]])
+            result["x"] = 0.5 * np.array([[0.0, 1.0], [1.0, 0.0]])
+            result["y"] = 0.5 * np.array([[0.0, -1.0j], [1.0j, 0.0]])
+            result["z"] = 0.5 * np.array([[1.0, 0.0], [0.0, -1.0]])
+        else:
+            spin = (mult - 1) / 2
+            prjs = np.arange(mult - 1, -1, -1) - spin
+
+            p_data = np.sqrt(spin * (spin + 1) - prjs * (prjs + 1))
+            m_data = np.sqrt(spin * (spin + 1) - prjs * (prjs - 1))
+
+            result["u"] = np.eye(mult)
+            result["p"] = sp.sparse.spdiags(p_data, [1], mult, mult).toarray()
+            result["m"] = sp.sparse.spdiags(m_data, [-1], mult, mult).toarray()
+            result["x"] = 0.5 * (result["p"] + result["m"])
+            result["y"] = -0.5 * 1j * (result["p"] - result["m"])
+            result["z"] = sp.sparse.spdiags(prjs, 0, mult, mult).toarray()
+        return result
+
     def spin_operator(self, idx: int, axis: str) -> np.ndarray:
-        """Construct the spin operator for a particle.
+        """Construct the spin operator.
 
         Args:
 
             idx (int): Index of the particle.
 
             axis (str): Axis, i.e. ``"x"``, ``"y"`` or ``"z"``.
 
         Returns:
+
             np.ndarray: Spin operator for a particle in the
-            `HilbertSimulation` system simulated.
+            `HilbertSimulation` system with indexing `idx` and axis
+            `axis`.
 
         Construct the spin operator for the particle with index
         `idx` in the `HilbertSimulation`.
+
         """
-        assert 0 <= idx and idx < len(self.multiplicities)
-        assert axis in "xyz"
+        assert 0 <= idx and idx < len(self.particles)
+        assert axis in "xyzpmu"
 
-        sigma = pauli(self.multiplicities[idx])[axis]
-        eye_before = np.eye(prod(m for m in self.multiplicities[:idx]))
-        eye_after = np.eye(prod(m for m in self.multiplicities[idx + 1 :]))
+        sigma = self.pauli(self.particles[idx].multiplicity)[axis]
+        eye_before = np.eye(prod(p.multiplicity for p in self.particles[:idx]))
+        eye_after = np.eye(prod(p.multiplicity for p in self.particles[idx + 1 :]))
 
         spinop = np.kron(np.kron(eye_before, sigma), eye_after)
         if self.basis == Basis.ST:
             return self.ST_basis(spinop)
         else:
             return spinop
 
@@ -472,16 +229,15 @@
                 for j, ax2 in enumerate("xyz")
             ]
         )
 
     def projection_operator(self, state: State):
         """Construct.
 
-        .. todo::
-            Write proper docs.
+        .. todo::     Write proper docs.
         """
         # Spin operators
         SAx, SAy, SAz = [self.spin_operator(0, ax) for ax in "xyz"]
         SBx, SBy, SBz = [self.spin_operator(1, ax) for ax in "xyz"]
 
         # Product operators
         SASB = self.product_operator(0, 1)
@@ -521,69 +277,66 @@
             B0 (float): External magnetic field intensity (milli
             Tesla).
 
         Returns:
             np.ndarray: The Zeeman Hamiltonian corresponding to the
             system described by the `Quantum` simulation object and
             the external magnetic field intensity `B`.
-
         """
         if theta is None and phi is None:
             return self.zeeman_hamiltonian_1d(B0)
         else:
             return self.zeeman_hamiltonian_3d(B0, theta, phi)
 
     def zeeman_hamiltonian_1d(self, B0: float) -> np.ndarray:
         axis = "z"
-        gammas = enumerate(self.gammas_mT)
+        gammas = enumerate(p.gamma_mT for p in self.particles)
         return -B0 * sum(g * self.spin_operator(i, axis) for i, g in gammas)
 
     def zeeman_hamiltonian_3d(
         self, B0: float, theta: float = 0, phi: float = 0
     ) -> np.ndarray:
         particles = np.array(
             [
                 [self.spin_operator(idx, axis) for axis in "xyz"]
-                for idx in range(self.num_particles)
+                for idx in range(len(self.particles))
             ]
         )
         rotation = utils.spherical_to_cartesian(theta, phi)
-        omega = B0 * self.gammas_mT[0]
+        omega = B0 * self.radicals[0].gamma_mT
         return omega * np.einsum("j,ijkl->kl", rotation, particles)
 
     def hyperfine_hamiltonian(self, hfc_anisotropy: bool = False) -> np.ndarray:
         """Construct the Hyperfine Hamiltonian.
 
         Construct the Hyperfine Hamiltonian based on the magnetic
         field.
 
         Returns:
             np.ndarray: The Hyperfine Hamiltonian corresponding to the
             system described by the `Quantum` simulation object.
-
         """
         if hfc_anisotropy:
-            for h in self.hfcs:
-                if not isinstance(h, np.ndarray) and h.shape == (3, 3):
+            for h in [n.hfc for n in self.nuclei]:
+                # TODO(vatai) try except not is None
+                if h.anisotropic is None:
                     raise ValueError(
-                        "Not all molecules have 3x3 HFC tensors! Please use `hfc_anisotropy=False`"
+                        "Not all molecules have anisotropic HFCs! Please use `hfc_anisotropy=False`"
                     )
 
         if hfc_anisotropy:
             prodop = self.product_operator_3d
-            hfcs = self.hfcs
+            hfcs = [n.hfc.anisotropic for n in self.nuclei]
         else:
             prodop = self.product_operator
-            hfcs = [
-                utils.isotropic(h) if isinstance(h, np.ndarray) else h
-                for h in self.hfcs
-            ]
+            hfcs = [n.hfc.isotropic for n in self.nuclei]
         return sum(
             [
-                self.gammas_mT[ei] * prodop(ei, self.num_electrons + ni, hfcs[ni])
+                self.particles[ei].gamma_mT
+                * prodop(ei, len(self.radicals) + ni, hfcs[ni])
                 for ni, ei in enumerate(self.coupling)
             ]
         )
 
     def exchange_hamiltonian(self, J: float) -> np.ndarray:
         """Construct the Exchange Hamiltonian.
 
@@ -594,17 +347,16 @@
         .. todo::
             Write proper docs.
 
         Returns:
             np.ndarray: The Exchange (J-coupling) Hamiltonian
             corresponding to the system described by the `Quantum`
             simulation object and the coupling constant `J`.
-
         """
-        Jcoupling = self.gammas_mT[0] * J
+        Jcoupling = self.radicals[0].gamma_mT * J
         SASB = self.product_operator(0, 1)
         return Jcoupling * (2 * SASB + 0.5 * np.eye(*SASB.shape))
 
     def dipolar_hamiltonian(self, D: float or np.ndarray) -> np.ndarray:
         """Construct the Dipolar Hamiltonian.
 
         Construct the Dipolar Hamiltonian based on dipolar coupling
@@ -613,33 +365,32 @@
         .. todo::
             Write proper docs.
 
         Returns:
             np.ndarray: The Dipolar Hamiltonian corresponding to the
             system described by the `Quantum` simulation object and
             dipolar coupling constant `D`.
-
         """
         if isinstance(D, np.ndarray):
             return self.dipolar_hamiltonian_3d(D)
         else:
             return self.dipolar_hamiltonian_1d(D)
 
     def dipolar_hamiltonian_1d(self, D: float) -> np.ndarray:
         SASB = self.product_operator(0, 1)
         SAz = self.spin_operator(0, "z")
         SBz = self.spin_operator(1, "z")
-        omega = (2 / 3) * self.gammas_mT[0] * D
+        omega = (2 / 3) * self.radicals[0].gamma_mT * D
         return omega * (3 * SAz * SBz - SASB)
 
     def dipolar_hamiltonian_3d(self, dipolar_tensor: np.ndarray) -> np.ndarray:
-        ne = self.num_electrons
+        ne = len(self.radicals)
         return -sum(
             [
-                -self.gammas_mT[0]
+                -self.radicals[0].gamma_mT
                 * self.product_operator_3d(ei, ne + ni, dipolar_tensor)
                 for ni, ei in enumerate(self.coupling)
             ]
         )
 
     def total_hamiltonian(
         self,
@@ -652,28 +403,38 @@
     ) -> np.ndarray:
         """Construct the final (total) Hamiltonian.
 
         Construct the final (total)
 
         .. todo::
             Write proper docs.
-
         """
         H = (
             self.zeeman_hamiltonian(B, theta, phi)
             + self.hyperfine_hamiltonian(hfc_anisotropy)
             + self.exchange_hamiltonian(J)
             + self.dipolar_hamiltonian(D)
         )
         return self.convert(H)
 
     def time_evolution(
         self, init_state: State, time: np.ndarray, H: np.ndarray
     ) -> np.ndarray:
-        """Evolve the system through time."""
+        """Evolve the system through time.
+
+        Args:
+                init_state (State): blah blah
+
+                time (np.ndarray): blah blah
+
+                H (np.ndarray): blah blah
+
+        Returns:
+                np.ndarray: blah blah
+        """
         dt = time[1] - time[0]
         propagator = self.unitary_propagator(H, dt)
 
         rho0 = self.initial_density_matrix(init_state, H)
         rhos = np.zeros([len(time), *rho0.shape], dtype=complex)
         rhos[0] = rho0
         for t in range(1, len(time)):
@@ -684,18 +445,18 @@
         """Calculate the probability of the observable from the densities."""
         if obs == State.EQUILIBRIUM:
             raise ValueError("Observable state should not be EQUILIBRIUM")
         obs = self.observable_projection_operator(obs)
         return np.real(np.trace(obs @ rhos, axis1=-2, axis2=-1))
 
     @staticmethod
-    def product_yield(probuct_probability, time, k):
+    def product_yield(product_probability, time, k):
         """Calculate the product yield and the product yield sum."""
-        product_yield = sp.integrate.cumtrapz(probuct_probability, time, initial=0) * k
-        product_yield_sum = np.trapz(probuct_probability, dx=time[1]) * k
+        product_yield = sp.integrate.cumtrapz(product_probability, time, initial=0) * k
+        product_yield_sum = np.trapz(product_probability, dx=time[1]) * k
         return product_yield, product_yield_sum
 
     def apply_liouville_hamiltonian_modifiers(self, H, modifiers):
         for K in modifiers:  # skip in hilbert
             K.init(self)
             K.adjust_hamiltonian(H)
 
@@ -726,15 +487,15 @@
         """
         H_zee = self.zeeman_hamiltonian(1, theta, phi)
         shape = H_zee.shape
         H_zee = self.convert(H_zee)
         if shape != H_zee.shape:
             shape = [shape[0] * shape[0], 1]
         rhos = np.zeros([len(B), len(time), *shape], dtype=complex)
-        for i, B0 in enumerate(B):
+        for i, B0 in enumerate(tqdm(B)):
             H = H_base + B0 * H_zee
             H_sparse = sp.sparse.csc_matrix(H)
             rhos[i] = self.time_evolution(init_state, time, H_sparse)
         return rhos
 
     @staticmethod
     def mary_lfe_hfe(
@@ -749,24 +510,28 @@
         idx = int(len(MARY) / 2) if B[0] != 0 else 0
         minmax = max if init_state == State.SINGLET else min
         HFE = (MARY[-1] - MARY[idx]) / MARY[idx] * 100
         LFE = (minmax(MARY) - MARY[idx]) / MARY[idx] * 100
         MARY = (MARY - MARY[idx]) / MARY[idx] * 100
         return MARY, LFE, HFE
 
+    @staticmethod
+    def _square_liouville_rhos(rhos):
+        return rhos
+
     def MARY(
         self,
         init_state: State,
         obs_state: State,
         time: np.ndarray,
         B: np.ndarray,
         D: float,
         J: float,
-        kinetics: list[KineticsRelaxationBase] = [],
-        relaxations: list[KineticsRelaxationBase] = [],
+        kinetics: list[HilbertIncoherentProcessBase] = [],
+        relaxations: list[HilbertIncoherentProcessBase] = [],
         theta: Optional[float] = None,
         phi: Optional[float] = None,
         hfc_anisotropy: bool = False,
     ) -> dict:
         H = self.total_hamiltonian(B=0, D=D, J=J, hfc_anisotropy=hfc_anisotropy)
 
         self.apply_liouville_hamiltonian_modifiers(H, kinetics + relaxations)
@@ -777,15 +542,15 @@
         k = kinetics[0].rate_constant if kinetics else 1.0
         product_yields, product_yield_sums = self.product_yield(
             product_probabilities, time, k
         )
 
         dt = time[1] - time[0]
         MARY, LFE, HFE = self.mary_lfe_hfe(init_state, B, product_probabilities, dt, k)
-        rhos = utils.square_vectors(rhos)
+        rhos = self._square_liouville_rhos(rhos)
 
         return dict(
             time=time,
             B=B,
             theta=theta,
             phi=phi,
             rhos=rhos,
@@ -803,53 +568,52 @@
         time: np.ndarray,
         B: float,
         H_base: np.ndarray,
         theta: Iterable[float],
         phi: Iterable[float],
     ):
         shape = H_base.shape
-        H_base = self.convert(H_base)
         if shape != H_base.shape:
             shape = [shape[0] * shape[0], 1]
 
         rhos = np.zeros([len(theta), len(phi), len(time), *shape], dtype=complex)
 
         for i, th in enumerate(theta):
             for j, ph in enumerate(phi):
                 H_zee = self.zeeman_hamiltonian(B, th, ph)
-                H = H_base + H_zee
+                H = H_base + self.convert(H_zee)
                 rhos[i, j] = self.time_evolution(init_state, time, H)
         return rhos
 
     def anisotropy(
         self,
         init_state: State,
         obs_state: State,
         time: np.ndarray,
         theta: Iterable or float,
         phi: Iterable or float,
         B: float,
         D: np.ndarray,
         J: float,
-        kinetics: list[KineticsRelaxationBase] = [],
-        relaxations: list[KineticsRelaxationBase] = [],
+        kinetics: list[HilbertIncoherentProcessBase] = [],
+        relaxations: list[HilbertIncoherentProcessBase] = [],
     ) -> dict:
         H = self.total_hamiltonian(B=0, D=D, J=J, hfc_anisotropy=True)
 
         self.apply_liouville_hamiltonian_modifiers(H, kinetics + relaxations)
         theta, phi = utils._anisotropy_check(theta, phi)
         rhos = self.anisotropy_loop(init_state, time, B, H, theta=theta, phi=phi)
         product_probabilities = self.product_probability(obs_state, rhos)
 
         self.apply_hilbert_kinetics(time, product_probabilities, kinetics)
         k = kinetics[0].rate_constant if kinetics else 1.0
         product_yields, product_yield_sums = self.product_yield(
             product_probabilities, time, k
         )
-        rhos = utils.square_vectors(rhos)
+        rhos = self._square_liouville_rhos(rhos)
 
         return dict(
             time=time,
             B=B,
             theta=theta,
             phi=phi,
             rhos=rhos,
@@ -871,15 +635,14 @@
         Args:
             state (State): Spin state projection operator.
 
             H (np.ndarray): Spin Hamiltonian in Hilbert space.
 
         Returns:
             np.ndarray: A matrix in Hilbert space representing...
-
         """
         Pi = self.projection_operator(state)
 
         if state == State.EQUILIBRIUM:
             rho0eq = sp.sparse.linalg.expm(-1j * sp.sparse.csc_matrix(H) * Pi).toarray()
             rho0 = rho0eq / rho0eq.trace()
         else:
@@ -904,15 +667,14 @@
 
         .. todo::
             https://docs.python.org/3/library/doctest.html
 
         Example:
             >> Up, Um = UnitaryPropagator(H, 3e-9, "Hilbert")
             >> UL = UnitaryPropagator(HL, 3e-9, "Liouville")
-
         """
         Up = sp.sparse.linalg.expm(1j * H * dt)
         Um = sp.sparse.linalg.expm(-1j * H * dt)
         return Up, Um
 
     def propagate(self, propagator: np.ndarray, rho: np.ndarray) -> np.ndarray:
         Up, Um = propagator
@@ -925,32 +687,38 @@
 class LiouvilleSimulation(HilbertSimulation):
     @staticmethod
     def convert(H: np.ndarray) -> np.ndarray:
         """Convert the Hamiltonian from Hilbert to Liouville space."""
         eye = np.eye(len(H))
         return 1j * (np.kron(H, eye) - np.kron(eye, H.T))
 
+    @staticmethod
+    def _square_liouville_rhos(rhos):
+        shape = rhos.shape
+        dim = int(np.sqrt(shape[-2]))
+        return rhos.reshape(shape[0], shape[1], dim, dim)
+
     def liouville_projection_operator(self, state: State) -> np.ndarray:
         return np.reshape(self.projection_operator(state), (-1, 1))
 
     def observable_projection_operator(self, state: State) -> np.ndarray:
         Q = self.liouville_projection_operator(state)
         return Q.T
 
     def initial_density_matrix(self, state: State, H: np.ndarray) -> np.ndarray:
-        """Create an initial density matrix for time evolution of the spin Hamiltonian density matrix.
+        """Create an initial density matrix for time evolution of the spin
+        Hamiltonian density matrix.
 
         Arguments:
             state (State): a string = spin state projection operator
             spins: an integer = sum of the number of electrons and nuclei
             H: a matrix = spin Hamiltonian in Hilbert space
 
         Returns:
             A matrix in Liouville space
-
         """
         Pi = self.liouville_projection_operator(state)
         if state == State.EQUILIBRIUM:
             rho0eq = sp.sparse.linalg.expm(-1j * H * Pi)
             rho0 = rho0eq / np.trace(rho0eq)
             rho0 = np.reshape(rho0, (len(H) ** 2, 1))
         else:
@@ -972,10 +740,10 @@
         """
         return sp.sparse.linalg.expm(H * dt)
 
     def propagate(self, propagator: np.ndarray, rho: np.ndarray) -> np.ndarray:
         return propagator @ rho
 
 
-class LiouvilleKineticsRelaxationBase(KineticsRelaxationBase):
+class LiouvilleIncoherentProcessBase(HilbertIncoherentProcessBase):
     def adjust_hamiltonian(self, H: np.ndarray):
         H -= self.subH
```

### Comparing `radicalpy-0.5rc1/src/tests/test_simulation.py` & `radicalpy-0.6.0/tests/test_simulation.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,74 +3,79 @@
 import doctest
 import os
 import time
 import unittest
 
 import matplotlib.pyplot as plt
 import numpy as np
-from src.radicalpy import data as rpdata
-from src.radicalpy import estimations, kinetics, relaxation
-from src.radicalpy import simulation as rpsim
-from src.radicalpy import utils
-from src.radicalpy.simulation import Basis
+import radicalpy as rp
+from radicalpy import estimations, kinetics, relaxation
+from radicalpy.simulation import Basis
 
-import tests.radpy as radpy
+from . import radpy
 
 # np.seterr(divide="raise", invalid="raise")
 
 RUN_SLOW_TESTS = "INSIDE_EMACS" not in os.environ  # or True
 MEASURE_TIME = False
 
 
 PARAMS = dict(
     B=np.random.uniform(size=20),
     J=np.random.uniform(),
     D=np.random.uniform(),
 )
 
 RADICAL_PAIR = [
-    rpsim.Molecule("flavin_anion", ["H29"]),
-    rpsim.Molecule("adenine_cation"),
-    # rpsim.Molecule("adenine_cation", ["C8-H"]),
+    rp.simulation.Molecule.fromdb("flavin_anion", ["H29"]),
+    rp.simulation.Molecule.fromdb("adenine_cation"),
+    # rp.simulation.Molecule("adenine_cation", ["C8-H"]),
 ]
 
 RADICAL_PAIR_RAW = [
-    rpsim.Molecule(
-        multiplicities=[2, 2],
-        gammas_mT=[rpdata.gamma_mT("E"), rpdata.gamma_mT("E")],
-        hfcs=[0, 0],
+    rp.simulation.Molecule(
+        "",
+        nuclei=[
+            rp.data.Nucleus(rp.data.Isotope("E").gamma_mT, 2, 0.0),
+            rp.data.Nucleus(rp.data.Isotope("E").gamma_mT, 2, 0.0),
+        ],
+    ),
+    rp.simulation.Molecule(
+        "",
+        nuclei=[
+            rp.data.Nucleus(rp.data.Isotope("E").gamma_mT, 2, 0.0),
+        ],
     ),
-    rpsim.Molecule(multiplicities=[2], gammas_mT=[rpdata.gamma_mT("E")], hfcs=[0]),
 ]
 
 
 def load_tests(loader, tests, ignore):
-    tests.addTests(doctest.DocTestSuite(rpsim))
+    tests.addTests(doctest.DocTestSuite(rp.simulation))
     tests.addTests(doctest.DocTestSuite(kinetics))
     return tests
 
 
-def state2radpy(state: rpsim.State) -> str:
+def state2radpy(state: rp.simulation.State) -> str:
     return (
         str(state.value)
         .replace("+", "p")
         .replace("-", "m")
         .replace("/", "")
         .replace("_", "")
         .replace("\\", "")
     )
 
 
 class MoleculeTests(unittest.TestCase):
     def test_effective_hyperfine(self):
-        flavin = rpsim.Molecule("flavin_anion", ["N5"])
+        flavin = rp.simulation.Molecule.fromdb("flavin_anion", ["N5"])
         self.assertAlmostEqual(flavin.effective_hyperfine, 1.4239723207027404)
 
     def test_manual_effective_hyperfine(self):
-        nuclei = ["14N"] * 4 + ["1H"] * 12
+        isotopes = ["14N"] * 4 + ["1H"] * 12
         hfcs = [
             0.5233,
             0.1887,
             -0.0035,
             -0.0383,
             0.0565,
             -0.1416,
@@ -81,157 +86,140 @@
             0.4399,
             0.4399,
             0.0099,
             0.407,
             0.407,
             -0.0189,
         ]
-        flavin = rpsim.Molecule(nuclei=nuclei, hfcs=hfcs)
+
+        flavin = rp.simulation.Molecule.fromisotopes(isotopes, hfcs)
         self.assertAlmostEqual(flavin.effective_hyperfine, 1.3981069)
 
 
 class HilbertTests(unittest.TestCase):
     def setUp(self):
         if MEASURE_TIME:
             self.start_time = time.time()
-        self.data = rpsim.MOLECULE_DATA["adenine_cation"]["data"]
-        self.sim = rpsim.HilbertSimulation(RADICAL_PAIR, basis=Basis.ZEEMAN)
-        self.gamma_mT = rpdata.gamma_mT("E")
+        self.data = rp.data.Molecule.load_molecule_json("adenine_cation")["data"]
+        self.sim = rp.simulation.HilbertSimulation(RADICAL_PAIR, basis=Basis.ZEEMAN)
+        self.gamma_mT = rp.data.Isotope("E").gamma_mT
         self.dt = 0.01
         self.t_max = 1.0
         self.time = np.arange(0, self.t_max, self.dt)
 
     def tearDown(self):
         if MEASURE_TIME:
             print(f"Time: {time.time() - self.start_time}")
 
-    @unittest.skip("Maybe bad test")
-    def test_molecule_properties(self):
-        molecule = rpsim.Molecule("adenine_cation", ["N6-H1", "C8-H"])
-        for prop in ["hfc", "element"]:
-            for i, h in enumerate(molecule._get_properties(prop)):
-                assert h == molecule._get_property(i, prop)
-
-    @unittest.skip("Maybe bad test")
-    def test_molecule_name(self):
-        molecule = rpsim.Molecule("adenine_cation", ["N6-H1", "C8-H"])
-        for i, h in enumerate(molecule.hfcs):
-            assert h == self.data[molecule.nuclei[i]]["hfc"]
-        for i, g in enumerate(molecule.gammas_mT):
-            elem = self.data[molecule.nuclei[i]]["element"]
-            assert g == rpdata.gamma_mT(elem)
-        for i, m in enumerate(molecule.multiplicities):
-            elem = self.data[molecule.nuclei[i]]["element"]
-            assert m == rpdata.multiplicity(elem)
-
     def test_molecule_raw(self):
         hfcs = [0.1, 0.2]
         multiplicities = [2, 3]
         gammas_mT = [3.14, 2.71]
 
-        molecule = rpsim.Molecule(
-            hfcs=hfcs, multiplicities=multiplicities, gammas_mT=gammas_mT
-        )
-        for i in range(2):
-            assert hfcs[i] == molecule.hfcs[i]
-            assert multiplicities[i] == molecule.multiplicities[i]
-            assert gammas_mT[i] == molecule.gammas_mT[i]
+        nuclei = [
+            rp.data.Nucleus(gammas_mT[0], multiplicities[0], rp.data.Hfc(hfcs[0])),
+            rp.data.Nucleus(gammas_mT[1], multiplicities[1], rp.data.Hfc(hfcs[1])),
+        ]
+        molecule = rp.simulation.Molecule(nuclei=nuclei)
+        for i, n in enumerate(molecule.nuclei):
+            self.assertEqual(hfcs[i], n.hfc.isotropic)
+            self.assertEqual(multiplicities[i], n.multiplicity)
+            self.assertEqual(gammas_mT[i], n.gamma_mT)
 
     def test_molecule_empty(self):
         """Test empty molecule.
 
         A silly test which verifies that the "empty" molecule has:
         - shape = (4, 4)
         - exactly two non-zero entries, and
         - those entries have opposite signs.
-
         """
-        mol = rpsim.Molecule()
-        sim = rpsim.HilbertSimulation([mol, mol])
+        mol = rp.simulation.Molecule()
+        sim = rp.simulation.HilbertSimulation([mol, mol])
         HZ = sim.zeeman_hamiltonian(0.5)
         nz = HZ != 0
         assert HZ.shape == (4, 4)
         assert len(HZ[nz]) == 2
         assert np.sum(HZ) == 0
 
     def test_HZ_raw(self):
         ################
         # RadicalPy code
-        sim = rpsim.HilbertSimulation(RADICAL_PAIR_RAW)
+        sim = rp.simulation.HilbertSimulation(RADICAL_PAIR_RAW)
         HZ = sim.zeeman_hamiltonian(PARAMS["B"][0])
 
         #########################
         # Assume this is correct!
         omega_e = PARAMS["B"][0] * self.gamma_mT
         electrons = sum(
-            [radpy.np_spinop(radpy.np_Sz, i, sim.num_particles) for i in range(2)]
+            [radpy.np_spinop(radpy.np_Sz, i, len(sim.particles)) for i in range(2)]
         )
-        omega_n = PARAMS["B"][0] * rpdata.gamma_mT("E")
+        omega_n = PARAMS["B"][0] * rp.data.Isotope("E").gamma_mT
         nuclei = sum(
             [
-                radpy.np_spinop(radpy.np_Sz, i, sim.num_particles)
-                for i in range(2, sim.num_particles)
+                radpy.np_spinop(radpy.np_Sz, i, len(sim.particles))
+                for i in range(2, len(sim.particles))
             ]
         )
         HZ_true = -omega_e * electrons - omega_n * nuclei
         assert np.all(
             np.isclose(HZ, HZ_true)
         ), "Zeeman Hamiltonian not calculated properly."
 
     def test_HZ(self):
         HZ = self.sim.zeeman_hamiltonian(PARAMS["B"][0])
 
         #########################
         # Assume this is correct!
         omega_e = PARAMS["B"][0] * self.gamma_mT
         electrons = sum(
-            [radpy.np_spinop(radpy.np_Sz, i, self.sim.num_particles) for i in range(2)]
+            [radpy.np_spinop(radpy.np_Sz, i, len(self.sim.particles)) for i in range(2)]
         )
-        omega_n = PARAMS["B"][0] * rpdata.gamma_mT("1H")
+        omega_n = PARAMS["B"][0] * rp.data.Isotope("1H").gamma_mT
         nuclei = sum(
             [
-                radpy.np_spinop(radpy.np_Sz, i, self.sim.num_particles)
-                for i in range(2, self.sim.num_particles)
+                radpy.np_spinop(radpy.np_Sz, i, len(self.sim.particles))
+                for i in range(2, len(self.sim.particles))
             ]
         )
         HZ_true = -omega_e * electrons - omega_n * nuclei
 
         assert np.all(
             np.isclose(HZ, HZ_true)
         ), "Zeeman Hamiltonian not calculated properly."
 
     def test_HH(self):
         couplings = self.sim.coupling
-        hfcs = self.sim.hfcs
+        hfcs = [n.hfc for n in self.sim.nuclei]
         HH_true = sum(
             [
                 radpy.HamiltonianHyperfine(
-                    self.sim.num_particles,
+                    len(self.sim.particles),
                     ei,
                     2 + ni,
-                    utils.isotropic(hfcs[ni]),
+                    hfcs[ni].isotropic,
                     self.gamma_mT,
                 )
                 for ni, ei in enumerate(couplings)
             ]
         )
         assert np.all(
             self.sim.hyperfine_hamiltonian() == HH_true
         ), "Hyperfine Hamiltonian not calculated properly."
 
     def test_HE(self):
         HE_true = radpy.HamiltonianExchange(
-            self.sim.num_particles, PARAMS["J"], gamma=self.gamma_mT
+            len(self.sim.particles), PARAMS["J"], gamma=self.gamma_mT
         )
         HE = self.sim.exchange_hamiltonian(PARAMS["J"])
         np.testing.assert_almost_equal(HE, HE_true)
 
     def test_HD(self):
         HD_true = radpy.HamiltonianDipolar(
-            self.sim.num_particles, PARAMS["D"], self.gamma_mT
+            len(self.sim.particles), PARAMS["D"], self.gamma_mT
         )
         HD = self.sim.dipolar_hamiltonian(PARAMS["D"])
         np.testing.assert_almost_equal(HD, HD_true)
 
     @unittest.skip("This needs to be figured out")
     def test_HH_3D(self):
         # from SingletYield.ipynb do
@@ -269,76 +257,72 @@
                     [-2.38856, 1.8683, 0.514044],
                     [1.8683, -40.6401, 0.0339364],
                     [0.514044, 0.0339364, -27.8618],
                 ]
             )
         ) * MHz2mT
 
-        flavin = rpsim.Molecule(
+        flavin = rp.simulation.Molecule(
             hfcs=[N5, N10, H5],
             multiplicities=[3, 3, 2],
             gammas_mT=[
-                rpsim.gamma_mT("14N"),
-                rpsim.gamma_mT("14N"),
-                rpsim.gamma_mT("1H"),
+                rp.simulation.gamma_mT("14N"),
+                rp.simulation.gamma_mT("14N"),
+                rp.simulation.gamma_mT("1H"),
             ],
         )
 
         H4 = 0.176 * np.eye(3)
-        ascorbic_acid = rpsim.Molecule(
+        ascorbic_acid = rp.simulation.Molecule(
             hfcs=[H4],
             multiplicities=[2],
-            gammas_mT=[rpsim.gamma_mT("1H")],
+            gammas_mT=[rp.simulation.gamma_mT("1H")],
         )
 
-        sim = rpsim.HilbertSimulation([flavin, ascorbic_acid])
+        sim = rp.simulation.HilbertSimulation([flavin, ascorbic_acid])
         H = sim.hyperfine_hamiltonian()
         # print(H.shape)
         # print(H)
         Htrue = np.load("/tmp/save.npy") * MHz2mT * 1e6
         print(Htrue[:5, :5])
         print(H[:5, :5])
         print(f"\nError: {np.linalg.norm(Htrue - H)}")
         # plt.imshow(np.real(H))
         # plt.show()
 
-    @unittest.skip("Doesn't check anything")
-    def test_3d(self):
-        H = self.sim.zeeman_hamiltonian_3d(1, 10, 20)
-
     def test_dipolar_interaction_1d(self):
-        approx = estimations.dipolar_interaction_1d(1)
+        approx = estimations.dipolar_interaction_isotropic(1)
         gold = approx
         self.assertEqual(gold, approx)
 
     def test_initial_density_matrix(self):
         H = self.sim.total_hamiltonian(PARAMS["B"][0], PARAMS["J"], PARAMS["D"])
-        for state in rpsim.State:
+        for state in rp.simulation.State:
             rho0 = self.sim.initial_density_matrix(state, H)
             rpstate = state2radpy(state)
-            rho0_true = radpy.Hilbert_initial(rpstate, self.sim.num_particles, H)
+            rho0_true = radpy.Hilbert_initial(rpstate, len(self.sim.particles), H)
             np.testing.assert_almost_equal(rho0, rho0_true)
 
     def test_unitary_propagator(self):
         dt = np.random.uniform(1e-6)
         H = self.sim.total_hamiltonian(PARAMS["B"][0], PARAMS["J"], PARAMS["D"])
         unitary_true = radpy.UnitaryPropagator(H, dt, "Hilbert")
         unitary = self.sim.unitary_propagator(H, dt)
         np.testing.assert_almost_equal(unitary_true, unitary)
 
     def test_time_evolution(self):
         k = np.random.uniform()
         H = self.sim.total_hamiltonian(PARAMS["B"][0], PARAMS["J"], PARAMS["D"])
         Kexp = kinetics.Exponential(k)
-        for init_state in rpsim.State:
-            for obs_state in rpsim.State:
-                if obs_state == rpsim.State.EQUILIBRIUM:
+        for init_state in rp.simulation.State:
+            for obs_state in rp.simulation.State:
+                if obs_state == rp.simulation.State.EQUILIBRIUM:
                     continue
                 evol_true = radpy.TimeEvolution(
-                    self.sim.num_particles,
+                    len(self.sim.particles),
                     state2radpy(init_state),
                     state2radpy(obs_state),
                     self.t_max,
                     self.dt,
                     k,
                     0,
                     H,
@@ -358,17 +342,17 @@
                 assert np.all(  # close (not equal)
                     np.isclose(pyield, evol_true[2][:-1])
                 ), "Time evolution (product yield) failed."
 
     # @unittest.skip("Not ready yet")
     def test_mary(self):
         k = np.random.uniform()
-        for init_state in rpsim.State:
-            for obs_state in rpsim.State:
-                if obs_state == rpsim.State.EQUILIBRIUM:
+        for init_state in rp.simulation.State:
+            for obs_state in rp.simulation.State:
+                if obs_state == rp.simulation.State.EQUILIBRIUM:
                     continue
                 rslt = self.sim.MARY(
                     init_state,
                     obs_state,
                     self.time,
                     B=PARAMS["B"],
                     D=PARAMS["D"],
@@ -385,19 +369,19 @@
                 #     PARAMS["B"],
                 #     H,
                 # )
 
     @unittest.skip("Numerical difference")
     def test_ST_vs_Zeeman_basis(self):
         k = np.random.uniform()
-        st_sim = rpsim.HilbertSimulation(RADICAL_PAIR, basis=Basis.ST)
+        st_sim = rp.simulation.HilbertSimulation(RADICAL_PAIR, basis=Basis.ST)
         ts = np.arange(0, 5e-6, 5e-9)
-        for i, init_state in enumerate(rpsim.State):
-            for j, obs_state in enumerate(rpsim.State):
-                if obs_state == rpsim.State.EQUILIBRIUM:
+        for i, init_state in enumerate(rp.simulation.State):
+            for j, obs_state in enumerate(rp.simulation.State):
+                if obs_state == rp.simulation.State.EQUILIBRIUM:
                     continue
                 kwargs = dict(
                     init_state=init_state,
                     obs_state=obs_state,
                     time=ts,
                     B=PARAMS["B"],
                     D=PARAMS["D"],
@@ -408,15 +392,15 @@
                 strs = st_sim.MARY(**kwargs)
 
                 key = "time_evolutions"
                 Bi = 1
                 # print(results.keys())
                 # print(results["product_yields"])
                 B = PARAMS["B"]
-                n = len(rpsim.State)
+                n = len(rp.simulation.State)
                 idx = i * n + j + 1
                 plt.subplot(n, n, idx)
 
                 title = f"{init_state.value}, {obs_state.value}"
                 suptitle = f"{key}: B={B[Bi]}"
                 plt.title(title)
                 plt.suptitle(suptitle)
@@ -424,16 +408,16 @@
                 plt.plot(strs["time"], strs[key][Bi])
         # np.testing.assert_almost_equal(rslt[key], strs[key])
         plt.show()
 
     def test_hyperfine_3d(self):
 
         results = self.sim.MARY(
-            rpsim.State.SINGLET,
-            rpsim.State.TRIPLET,
+            rp.simulation.State.SINGLET,
+            rp.simulation.State.TRIPLET,
             self.time,
             PARAMS["B"],
             PARAMS["D"],
             PARAMS["J"],
             theta=np.pi / 2,
             phi=0,
             hfc_anisotropy=True,
@@ -457,41 +441,41 @@
                 [5680970.81962565, -65574461.04030437, 34606093.12997659],
                 [-65574461.04030436, -34583196.80020875, 47131454.19638795],
                 [34606093.12997659, 47131454.19638795, 28902225.98058307],
             ]
         )
 
         molecules = [
-            rpsim.Molecule("flavin3d", nuclei=["14N"], hfcs=[N5]),
-            rpsim.Molecule(),
+            rp.simulation.Molecule.fromisotopes(["14N"], [N5], "flavin3d"),
+            rp.simulation.Molecule(),
         ]
         B0 = 0.05
         B = np.arange(-10e-3, 10e-3, 1e-3)
-        sim = rpsim.HilbertSimulation(molecules)
+        sim = rp.simulation.HilbertSimulation(molecules)
         HZ = sim.zeeman_hamiltonian_3d(B0=B0, theta=0, phi=0)
         HZt = sim.zeeman_hamiltonian_3d(B0=B0, theta=np.pi / 2, phi=0)
         HZtp = sim.zeeman_hamiltonian_3d(B0=B0, theta=np.pi / 2, phi=np.pi)
         HZp = sim.zeeman_hamiltonian_3d(B0=B0, theta=np.pi, phi=0)
         HH = sim.hyperfine_hamiltonian()
         HD = sim.dipolar_hamiltonian_3d(dipolar_tensor)
         H = HZt + HH + HD
         time = np.arange(0, 15e-6, 5e-9)
-        # rhos = sim.time_evolution(rpsim.State.SINGLET, time, H)
-        # pp = sim.product_probability(rpsim.State.TRIPLET, rhos)
+        # rhos = sim.time_evolution(rp.simulation.State.SINGLET, time, H)
+        # pp = sim.product_probability(rp.simulation.State.TRIPLET, rhos)
         # print(sim)
         # print(f"{HZ.shape=}")
         # print(f"{HH.shape=}")
         # print(f"{HD.shape=}")
         # print(f"{rhos.shape=}")
         # plt.plot(time, pp)
         # plt.show()
         # print(HZ)
         # results = sim.MARY(
-        #     rpsim.State.SINGLET,
-        #     rpsim.State.TRIPLET,
+        #     rp.simulation.State.SINGLET,
+        #     rp.simulation.State.TRIPLET,
         #     time,
         #     B,
         #     dipolar_tensor,
         #     0,
         #     kinetics=[kinetics.Exponential(3e6)],
         #     theta=np.pi / 2,
         #     phi=0,
@@ -501,49 +485,49 @@
         # plt.title(f"B={results['B'][idx]}")
         # plt.show()
         # print("DONE")
 
 
 class LiouvilleTests(unittest.TestCase):
     def setUp(self):
-        self.sim = rpsim.LiouvilleSimulation(RADICAL_PAIR, basis=Basis.ZEEMAN)
+        self.sim = rp.simulation.LiouvilleSimulation(RADICAL_PAIR, basis=Basis.ZEEMAN)
         self.dt = 0.01
         self.t_max = 1.0
         self.time = np.arange(0, self.t_max, self.dt)
 
     def test_initial_density_matrix(self):
         H = self.sim.total_hamiltonian(PARAMS["B"][0], PARAMS["J"], PARAMS["D"])
-        for state in rpsim.State:
+        for state in rp.simulation.State:
             rho0 = self.sim.initial_density_matrix(state, H)
             rpstate = state2radpy(state)
-            rho0_true = radpy.Liouville_initial(rpstate, self.sim.num_particles, H)
+            rho0_true = radpy.Liouville_initial(rpstate, len(self.sim.particles), H)
             np.testing.assert_almost_equal(rho0, rho0_true)
 
     def test_unitary_propagator(self):
         dt = np.random.uniform(0, 1e-6)
         H = self.sim.total_hamiltonian(PARAMS["B"][0], PARAMS["J"], PARAMS["D"])
         unitary_true = radpy.UnitaryPropagator(H, dt, "Liouville")
         unitary = self.sim.unitary_propagator(H, dt)
         np.testing.assert_almost_equal(unitary, unitary_true)
 
     @unittest.skipUnless(RUN_SLOW_TESTS, "slow")
     def test_kinetics(self):
         kwargs = dict(
-            init_state=rpsim.State.SINGLET,
-            obs_state=rpsim.State.TRIPLET,
+            init_state=rp.simulation.State.SINGLET,
+            obs_state=rp.simulation.State.TRIPLET,
             time=np.arange(0, 15e-6, 5e-9),
             B=np.arange(0, 20, 1),
             D=0,
             J=0,
         )
         k = 1e6
         results_haberkorn = self.sim.MARY(
             kinetics=[
-                kinetics.Haberkorn(k, rpsim.State.TRIPLET),
-                kinetics.Haberkorn(k, rpsim.State.SINGLET),
+                kinetics.Haberkorn(k, rp.simulation.State.TRIPLET),
+                kinetics.Haberkorn(k, rp.simulation.State.SINGLET),
                 kinetics.Exponential(k),
             ],
             **kwargs,
         )
         results_jones_hore = self.sim.MARY(
             kinetics=[
                 kinetics.JonesHore(k, k),
@@ -557,16 +541,16 @@
         # plt.plot(results_jones_hore["time"], results_jones_hore["time_evolutions"][idx])
         # plt.title(f"B={results_haberkorn['B'][idx]}")
         # plt.show()
         # print("DONE")
 
     def test_relaxation(self):
         kwargs = dict(
-            init_state=rpsim.State.TRIPLET,
-            obs_state=rpsim.State.TRIPLET,
+            init_state=rp.simulation.State.TRIPLET,
+            obs_state=rp.simulation.State.TRIPLET,
             time=np.arange(0, 5e-6, 1e-9),
             B=np.arange(0, 4, 1),
             D=0,
             J=0,
         )
         k = 1e6
         results = self.sim.MARY(
```

