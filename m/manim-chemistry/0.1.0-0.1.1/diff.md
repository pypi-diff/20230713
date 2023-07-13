# Comparing `tmp/manim-chemistry-0.1.0.tar.gz` & `tmp/manim-chemistry-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manim-chemistry-0.1.0.tar", last modified: Fri May 19 16:51:43 2023, max compression
+gzip compressed data, was "manim-chemistry-0.1.1.tar", last modified: Thu Jul 13 11:36:05 2023, max compression
```

## Comparing `manim-chemistry-0.1.0.tar` & `manim-chemistry-0.1.1.tar`

### file list

```diff
@@ -1,78 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:51:43.152508 manim-chemistry-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:51:43.136508 manim-chemistry-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:51:43.140508 manim-chemistry-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:51:43.140508 manim-chemistry-0.1.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16860 2023-05-19 16:51:43.152508 manim-chemistry-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/TODO.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:51:43.140508 manim-chemistry-0.1.0/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/assets/Elements_EN.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:51:43.140508 manim-chemistry-0.1.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:51:43.144508 manim-chemistry-0.1.0/examples/element_files/
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/examples/element_files/Elementos.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/examples/element_files/dimethylpropane.mol
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/examples/element_files/heme_2d.mol
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/examples/element_files/heme_group.mol
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/examples/element_files/morphine.mol
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/examples/element_files/morphine3d.mol
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/examples/examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:51:43.148508 manim-chemistry-0.1.0/examples/examples_assets/
--rw-r--r--   0 runner    (1001) docker     (123)    54656 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/examples/examples_assets/2D_morphine_bad.png
--rw-r--r--   0 runner    (1001) docker     (123)    83346 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/examples/examples_assets/2D_morphine_bond_numbering.png
--rw-r--r--   0 runner    (1001) docker     (123)    54441 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/examples/examples_assets/2D_morphine_corrected_bonds.png
--rw-r--r--   0 runner    (1001) docker     (123)    93200 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/examples/examples_assets/BohrDiagram_ManimCE_v0.17.3.png
--rw-r--r--   0 runner    (1001) docker     (123)   219228 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/examples/examples_assets/Draw3DMorphine_ManimCE_v0.17.3.png
--rw-r--r--   0 runner    (1001) docker     (123)    24751 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/examples/examples_assets/DrawCarbonElement_ManimCE_v0.17.3.png
--rw-r--r--   0 runner    (1001) docker     (123)   439644 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/examples/examples_assets/DrawPeriodicTable_ManimCE_v0.17.3.png
--rw-r--r--   0 runner    (1001) docker     (123)   241773 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/examples/examples_assets/Fullerene.png
--rw-r--r--   0 runner    (1001) docker     (123)   297681 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/examples/examples_assets/TinPhases.png
--rw-r--r--   0 runner    (1001) docker     (123)    31707 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/examples/examples_assets/orbitals_example.png
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 16:51:43.152508 manim-chemistry-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:51:43.136508 manim-chemistry-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:51:43.148508 manim-chemistry-0.1.0/src/manim_chemistry/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/src/manim_chemistry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:51:43.148508 manim-chemistry-0.1.0/src/manim_chemistry/bohr_atom/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/src/manim_chemistry/bohr_atom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/src/manim_chemistry/bohr_atom/bohr_atom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:51:43.148508 manim-chemistry-0.1.0/src/manim_chemistry/element/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/src/manim_chemistry/element/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/src/manim_chemistry/element/element.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:51:43.148508 manim-chemistry-0.1.0/src/manim_chemistry/future_classes/
--rw-r--r--   0 runner    (1001) docker     (123)    16183 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/src/manim_chemistry/future_classes/future_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:51:43.148508 manim-chemistry-0.1.0/src/manim_chemistry/orbitals/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/src/manim_chemistry/orbitals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/src/manim_chemistry/orbitals/orbitals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:51:43.148508 manim-chemistry-0.1.0/src/manim_chemistry/periodic_table/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/src/manim_chemistry/periodic_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/src/manim_chemistry/periodic_table/table_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:51:43.152508 manim-chemistry-0.1.0/src/manim_chemistry/threeD/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/src/manim_chemistry/threeD/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/src/manim_chemistry/threeD/threedatom.py
--rw-r--r--   0 runner    (1001) docker     (123)    12384 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/src/manim_chemistry/threeD/threedbond.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/src/manim_chemistry/threeD/threedmolecule.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/src/manim_chemistry/threeD/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:51:43.152508 manim-chemistry-0.1.0/src/manim_chemistry/twoD/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/src/manim_chemistry/twoD/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/src/manim_chemistry/twoD/atom.py
--rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/src/manim_chemistry/twoD/bond.py
--rw-r--r--   0 runner    (1001) docker     (123)    10038 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/src/manim_chemistry/twoD/molecule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:51:43.152508 manim-chemistry-0.1.0/src/manim_chemistry/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/src/manim_chemistry/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/src/manim_chemistry/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:51:43.148508 manim-chemistry-0.1.0/src/manim_chemistry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16860 2023-05-19 16:51:43.000000 manim-chemistry-0.1.0/src/manim_chemistry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-19 16:51:43.000000 manim-chemistry-0.1.0/src/manim_chemistry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:51:43.000000 manim-chemistry-0.1.0/src/manim_chemistry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-19 16:51:43.000000 manim-chemistry-0.1.0/src/manim_chemistry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-19 16:51:43.000000 manim-chemistry-0.1.0/src/manim_chemistry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-19 16:51:43.000000 manim-chemistry-0.1.0/src/manim_chemistry.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:51:43.152508 manim-chemistry-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-05-19 16:51:25.000000 manim-chemistry-0.1.0/tests/test_working.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:36:05.407765 manim-chemistry-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:36:05.395765 manim-chemistry-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:36:05.399765 manim-chemistry-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:36:05.399765 manim-chemistry-0.1.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18220 2023-07-13 11:36:05.407765 manim-chemistry-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16321 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/TODO.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:36:05.399765 manim-chemistry-0.1.1/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/assets/Elements_EN.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:36:05.399765 manim-chemistry-0.1.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:36:05.399765 manim-chemistry-0.1.1/examples/element_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/examples/element_files/Elementos.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/examples/element_files/dimethylpropane.mol
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/examples/element_files/heme_2d.mol
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/examples/element_files/heme_group.mol
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/examples/element_files/morphine.mol
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/examples/element_files/morphine3d.mol
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/examples/examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:36:05.403765 manim-chemistry-0.1.1/examples/examples_assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    54656 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/examples/examples_assets/2D_morphine_bad.png
+-rw-r--r--   0 runner    (1001) docker     (123)    83346 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/examples/examples_assets/2D_morphine_bond_numbering.png
+-rw-r--r--   0 runner    (1001) docker     (123)    54441 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/examples/examples_assets/2D_morphine_corrected_bonds.png
+-rw-r--r--   0 runner    (1001) docker     (123)    93200 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/examples/examples_assets/BohrDiagram_ManimCE_v0.17.3.png
+-rw-r--r--   0 runner    (1001) docker     (123)   219228 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/examples/examples_assets/Draw3DMorphine_ManimCE_v0.17.3.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24751 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/examples/examples_assets/DrawCarbonElement_ManimCE_v0.17.3.png
+-rw-r--r--   0 runner    (1001) docker     (123)   439644 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/examples/examples_assets/DrawPeriodicTable_ManimCE_v0.17.3.png
+-rw-r--r--   0 runner    (1001) docker     (123)   241773 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/examples/examples_assets/Fullerene.png
+-rw-r--r--   0 runner    (1001) docker     (123)    64536 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/examples/examples_assets/NamedMoleculeExample_ManimCE_v0.17.3.png
+-rw-r--r--   0 runner    (1001) docker     (123)   297681 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/examples/examples_assets/TinPhases.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31707 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/examples/examples_assets/orbitals_example.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 11:36:05.407765 manim-chemistry-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:36:05.395765 manim-chemistry-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:36:05.403765 manim-chemistry-0.1.1/src/manim_chemistry/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/src/manim_chemistry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:36:05.403765 manim-chemistry-0.1.1/src/manim_chemistry/bohr_atom/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/src/manim_chemistry/bohr_atom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/src/manim_chemistry/bohr_atom/bohr_atom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:36:05.403765 manim-chemistry-0.1.1/src/manim_chemistry/element/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/src/manim_chemistry/element/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/src/manim_chemistry/element/element.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:36:05.403765 manim-chemistry-0.1.1/src/manim_chemistry/future_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    16183 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/src/manim_chemistry/future_classes/future_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:36:05.403765 manim-chemistry-0.1.1/src/manim_chemistry/orbitals/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/src/manim_chemistry/orbitals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/src/manim_chemistry/orbitals/orbitals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:36:05.403765 manim-chemistry-0.1.1/src/manim_chemistry/periodic_table/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/src/manim_chemistry/periodic_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/src/manim_chemistry/periodic_table/table_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:36:05.407765 manim-chemistry-0.1.1/src/manim_chemistry/threeD/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/src/manim_chemistry/threeD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/src/manim_chemistry/threeD/threedatom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12384 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/src/manim_chemistry/threeD/threedbond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/src/manim_chemistry/threeD/threedmolecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/src/manim_chemistry/threeD/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:36:05.407765 manim-chemistry-0.1.1/src/manim_chemistry/twoD/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/src/manim_chemistry/twoD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/src/manim_chemistry/twoD/atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/src/manim_chemistry/twoD/bond.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/src/manim_chemistry/twoD/molecule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:36:05.407765 manim-chemistry-0.1.1/src/manim_chemistry/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/src/manim_chemistry/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/src/manim_chemistry/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:36:05.403765 manim-chemistry-0.1.1/src/manim_chemistry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18220 2023-07-13 11:36:05.000000 manim-chemistry-0.1.1/src/manim_chemistry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-13 11:36:05.000000 manim-chemistry-0.1.1/src/manim_chemistry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 11:36:05.000000 manim-chemistry-0.1.1/src/manim_chemistry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-13 11:36:05.000000 manim-chemistry-0.1.1/src/manim_chemistry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 11:36:05.000000 manim-chemistry-0.1.1/src/manim_chemistry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-13 11:36:05.000000 manim-chemistry-0.1.1/src/manim_chemistry.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:36:05.407765 manim-chemistry-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-07-13 11:35:50.000000 manim-chemistry-0.1.1/tests/test_working.py
```

### Comparing `manim-chemistry-0.1.0/.github/workflows/python-publish.yml` & `manim-chemistry-0.1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `manim-chemistry-0.1.0/.github/workflows/tests.yml` & `manim-chemistry-0.1.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `manim-chemistry-0.1.0/LICENSE.md` & `manim-chemistry-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `manim-chemistry-0.1.0/PKG-INFO` & `manim-chemistry-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: manim-chemistry
-Version: 0.1.0
-Summary: Draws molecules. Nice!
+Version: 0.1.1
+Summary: Manim Chemistry is a plugin for Manim which aims to make easier the animation of molecules and other chemistry-related objects such as orbitals, bohr diagrams and more.
 Author-email: UMDQ <unmoldequimica@gmail.com>
 Maintainer-email: UMDQ <unmoldequimica@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 UMDQ
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -32,26 +32,41 @@
 - [Create a periodic table](#create-a-periodic-table)
 - [Making atomic orbitals](#making-atomic-orbitals)
 - [Making Bohr diagrams](#making-bohr-diagrams)
 - [Reading .mol files](#reading-mol-files)
 - [Typical issues with .mol files](#typical-issues-with-mol-files)
 - [Take a look to examples](#)
 - [Made with manimChemistry](#made-with-manimchemistry)
+- [How to contact](#how-to-contact)
+- [Great contributers](#great-contributers)
 
 # Installation.
 
-Right now this can be installed cloning the repo:
+You can install via pip:
+
+```
+pip install manim_chemistry
+```
+
+You can also clone the repo and install it from here:
 
 ```
 git clone https://github.com/UnMolDeQuimica/manim-Chemistry.git
 cd manim-Chemistry 
 python -m pip install .
 ```
 
-Soon this will be available in pip.
+or
+
+```
+git clone https://github.com/UnMolDeQuimica/manim-Chemistry.git
+cd manim-Chemistry 
+python -m pip install -e .
+```
+
 
 # What is manim-Chemistry?
 
 manim-Chemistry is a manim plugin designed to make chemistry animations easier.
 
 To my knowledge, there is only another plugin related to chemistry called [chanim](https://github.com/kilacoda/chanim) that aims to import to manim the chemfig package (and does an amazing job!).
 
@@ -95,15 +110,15 @@
 
 ```
 from manim import *
 from manim_chemistry import *
 
 class TwoDMoleculeScene(Scene):
    def construct(self):
-        morphine = MMoleculeObject.from_mol_file("morphine.mol")
+        morphine = MMoleculeObject.from_mol_file("morphine.mol", add_bonds_numbering=True)
         self.add(morphine)
 ```
 
 We get
 
 ![plot](/examples/examples_assets/2D_morphine_bond_numbering.png)
 
@@ -120,14 +135,31 @@
 ```
 
 Result:
 ![plot](/examples/examples_assets/2D_morphine_corrected_bonds.png)
 
 Now we are talking!
 
+### Named Molecules:
+
+You may want to add a name to a molecule. It is very simple, but it is handy to do all in the same object. You can create a NamedMolecule similarly to how you create a MMoleculeObject:
+
+```
+from manim import *
+from manim_chemistry import *
+
+class NamedMoleculeExample(Scene):
+    def construct(self):
+        named_molecule = NamedMolecule.from_mol_file(name="Morphine", filename="morphine.mol")
+        self.add(diagram)
+```
+![plot](/examples/examples_assets/NamedMoleculeExample_ManimCE_v0.17.3.png)
+
+You can also provided an already created molecule or an already created text and the NamedMolecule class will group them. This allows greater control for the user.
+
 ## Create 3D molecule:
 
 Creating a 3D molecule requires a bit more effort. We need two things:
 
 1. A .mol file (like before)
 2. A csv data file with data for your atoms. You can find an example inside the examples folder called "Elementos.csv". 
 
@@ -324,17 +356,27 @@
 
 Fullerene:
 ![plot](/examples/examples_assets/Fullerene.png)
 
 Beta and alpha tin structures:
 ![plot](/examples/examples_assets/TinPhases.png)
 
-A video using both and more examples:
+Videos using manimChemistry:
 
 https://www.youtube.com/watch?v=L7OXe94_WmA
 
+https://youtu.be/KgiCl_o_Aws
+
 
 # How to contact
 You can open issues and pull requests, but if you want to contact me directly you can go to:
 - Email: unmoldequimica@gmail.com
 - YouTube: https://www.youtube.com/@unmoldequimica
 - Twitter: https://twitter.com/unmoldequimica
+
+
+# Great contributers!
+- [@chemnerd28](https://github.com/chemnerd28)
+- [@Ant-28](https://github.com/Ant-28)
+
+
+Special thanks to [@Rodrigo-Tenorio](https://github.com/Rodrigo-Tenorio) for his help in the creation of this releasable package.
```

### Comparing `manim-chemistry-0.1.0/README.md` & `manim-chemistry-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,26 +7,41 @@
 - [Create a periodic table](#create-a-periodic-table)
 - [Making atomic orbitals](#making-atomic-orbitals)
 - [Making Bohr diagrams](#making-bohr-diagrams)
 - [Reading .mol files](#reading-mol-files)
 - [Typical issues with .mol files](#typical-issues-with-mol-files)
 - [Take a look to examples](#)
 - [Made with manimChemistry](#made-with-manimchemistry)
+- [How to contact](#how-to-contact)
+- [Great contributers](#great-contributers)
 
 # Installation.
 
-Right now this can be installed cloning the repo:
+You can install via pip:
+
+```
+pip install manim_chemistry
+```
+
+You can also clone the repo and install it from here:
 
 ```
 git clone https://github.com/UnMolDeQuimica/manim-Chemistry.git
 cd manim-Chemistry 
 python -m pip install .
 ```
 
-Soon this will be available in pip.
+or
+
+```
+git clone https://github.com/UnMolDeQuimica/manim-Chemistry.git
+cd manim-Chemistry 
+python -m pip install -e .
+```
+
 
 # What is manim-Chemistry?
 
 manim-Chemistry is a manim plugin designed to make chemistry animations easier.
 
 To my knowledge, there is only another plugin related to chemistry called [chanim](https://github.com/kilacoda/chanim) that aims to import to manim the chemfig package (and does an amazing job!).
 
@@ -70,15 +85,15 @@
 
 ```
 from manim import *
 from manim_chemistry import *
 
 class TwoDMoleculeScene(Scene):
    def construct(self):
-        morphine = MMoleculeObject.from_mol_file("morphine.mol")
+        morphine = MMoleculeObject.from_mol_file("morphine.mol", add_bonds_numbering=True)
         self.add(morphine)
 ```
 
 We get
 
 ![plot](/examples/examples_assets/2D_morphine_bond_numbering.png)
 
@@ -95,14 +110,31 @@
 ```
 
 Result:
 ![plot](/examples/examples_assets/2D_morphine_corrected_bonds.png)
 
 Now we are talking!
 
+### Named Molecules:
+
+You may want to add a name to a molecule. It is very simple, but it is handy to do all in the same object. You can create a NamedMolecule similarly to how you create a MMoleculeObject:
+
+```
+from manim import *
+from manim_chemistry import *
+
+class NamedMoleculeExample(Scene):
+    def construct(self):
+        named_molecule = NamedMolecule.from_mol_file(name="Morphine", filename="morphine.mol")
+        self.add(diagram)
+```
+![plot](/examples/examples_assets/NamedMoleculeExample_ManimCE_v0.17.3.png)
+
+You can also provided an already created molecule or an already created text and the NamedMolecule class will group them. This allows greater control for the user.
+
 ## Create 3D molecule:
 
 Creating a 3D molecule requires a bit more effort. We need two things:
 
 1. A .mol file (like before)
 2. A csv data file with data for your atoms. You can find an example inside the examples folder called "Elementos.csv". 
 
@@ -299,17 +331,27 @@
 
 Fullerene:
 ![plot](/examples/examples_assets/Fullerene.png)
 
 Beta and alpha tin structures:
 ![plot](/examples/examples_assets/TinPhases.png)
 
-A video using both and more examples:
+Videos using manimChemistry:
 
 https://www.youtube.com/watch?v=L7OXe94_WmA
 
+https://youtu.be/KgiCl_o_Aws
+
 
 # How to contact
 You can open issues and pull requests, but if you want to contact me directly you can go to:
 - Email: unmoldequimica@gmail.com
 - YouTube: https://www.youtube.com/@unmoldequimica
 - Twitter: https://twitter.com/unmoldequimica
+
+
+# Great contributers!
+- [@chemnerd28](https://github.com/chemnerd28)
+- [@Ant-28](https://github.com/Ant-28)
+
+
+Special thanks to [@Rodrigo-Tenorio](https://github.com/Rodrigo-Tenorio) for his help in the creation of this releasable package.
```

### Comparing `manim-chemistry-0.1.0/TODO.md` & `manim-chemistry-0.1.1/TODO.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 * [ ] Solve the H problem like in HO or NH. There is a simple implementation now but not good at it's job.
 * [ ] An example gallery to show molnim capabilities.
 
 # Features that would be cool to implement
 
 Here are listed features that would be cool to implement, don't seem to hard to do but also they are not explicitly necessary for the project. Some of them might seem pretty necessary, but if there is a workaround solving the issue, they are not a priority like the list above. That being said, I will probably develop something from this instead of doing the necessary stuff before.
 
-* [ ] Actual atom numbering. At this moment we are simply numbering using the order from the .mol file, but might be good to be able to show actual numbering without working too hard. (See cannonicalization from [this](https://pubs.acs.org/doi/10.1021/acs.jcim.5b00543)
+* [ ] Actual atom numbering. At this moment we are simply numbering using the order from the .mol file, but might be good to be able to show actual numbering without working too hard. (See cannonicalization from [this](https://pubs.acs.org/doi/10.1021/acs.jcim.5b00543))
 * [ ] Support other formats. Probably something like SMILES will be the next step to improve molnim. Probably the best aproach would be create a custom internal format. When parsing a format we transform to that internal format and then we can create the molecules from it.
 * [ ] Solve the double bond issue. Now, when drawing a double bond, the bond is drawn in a direction defined by the mol file. That means we can draw a benzene ring with all the double bonds outside the ring, which is ugly af. I need to check or come up with an algorithm that solves that issue.
 * [ ] Add functional groups automatic recongition. Check [this paper](https://jcheminf.biomedcentral.com/articles/10.1186/s13321-017-0225-z). It would be really nice to add this feature.
 * [ ] Add reaction diagrams. While this might be unnecessary, I think adding a class that given some reactants, some products, reaction conditions and arrow that automates the creation creation and animation of reaction can simplify a lot of work.
 * [ ] Use graph objects from manim. Probably this can save a ton of work done "manually" in this library, but it is working at the moment.
 * [ ] Add a database for a lot of properties.
 * [ ] Add pre-built in molecules.
```

### Comparing `manim-chemistry-0.1.0/assets/Elements_EN.csv` & `manim-chemistry-0.1.1/assets/Elements_EN.csv`

 * *Files identical despite different names*

### Comparing `manim-chemistry-0.1.0/examples/element_files/Elementos.csv` & `manim-chemistry-0.1.1/examples/element_files/Elementos.csv`

 * *Files identical despite different names*

### Comparing `manim-chemistry-0.1.0/examples/element_files/dimethylpropane.mol` & `manim-chemistry-0.1.1/examples/element_files/dimethylpropane.mol`

 * *Files identical despite different names*

### Comparing `manim-chemistry-0.1.0/examples/element_files/heme_2d.mol` & `manim-chemistry-0.1.1/examples/element_files/heme_2d.mol`

 * *Files identical despite different names*

### Comparing `manim-chemistry-0.1.0/examples/element_files/heme_group.mol` & `manim-chemistry-0.1.1/examples/element_files/heme_group.mol`

 * *Files identical despite different names*

### Comparing `manim-chemistry-0.1.0/examples/element_files/morphine.mol` & `manim-chemistry-0.1.1/examples/element_files/morphine.mol`

 * *Files identical despite different names*

### Comparing `manim-chemistry-0.1.0/examples/element_files/morphine3d.mol` & `manim-chemistry-0.1.1/examples/element_files/morphine3d.mol`

 * *Files identical despite different names*

### Comparing `manim-chemistry-0.1.0/examples/examples.py` & `manim-chemistry-0.1.1/examples/examples.py`

 * *Files identical despite different names*

### Comparing `manim-chemistry-0.1.0/examples/examples_assets/2D_morphine_bad.png` & `manim-chemistry-0.1.1/examples/examples_assets/2D_morphine_bad.png`

 * *Files identical despite different names*

### Comparing `manim-chemistry-0.1.0/examples/examples_assets/2D_morphine_bond_numbering.png` & `manim-chemistry-0.1.1/examples/examples_assets/2D_morphine_bond_numbering.png`

 * *Files identical despite different names*

### Comparing `manim-chemistry-0.1.0/examples/examples_assets/2D_morphine_corrected_bonds.png` & `manim-chemistry-0.1.1/examples/examples_assets/2D_morphine_corrected_bonds.png`

 * *Files identical despite different names*

### Comparing `manim-chemistry-0.1.0/examples/examples_assets/BohrDiagram_ManimCE_v0.17.3.png` & `manim-chemistry-0.1.1/examples/examples_assets/BohrDiagram_ManimCE_v0.17.3.png`

 * *Files identical despite different names*

### Comparing `manim-chemistry-0.1.0/examples/examples_assets/Draw3DMorphine_ManimCE_v0.17.3.png` & `manim-chemistry-0.1.1/examples/examples_assets/Draw3DMorphine_ManimCE_v0.17.3.png`

 * *Files identical despite different names*

### Comparing `manim-chemistry-0.1.0/examples/examples_assets/DrawCarbonElement_ManimCE_v0.17.3.png` & `manim-chemistry-0.1.1/examples/examples_assets/DrawCarbonElement_ManimCE_v0.17.3.png`

 * *Files identical despite different names*

### Comparing `manim-chemistry-0.1.0/examples/examples_assets/DrawPeriodicTable_ManimCE_v0.17.3.png` & `manim-chemistry-0.1.1/examples/examples_assets/DrawPeriodicTable_ManimCE_v0.17.3.png`

 * *Files identical despite different names*

### Comparing `manim-chemistry-0.1.0/examples/examples_assets/Fullerene.png` & `manim-chemistry-0.1.1/examples/examples_assets/Fullerene.png`

 * *Files identical despite different names*

### Comparing `manim-chemistry-0.1.0/examples/examples_assets/TinPhases.png` & `manim-chemistry-0.1.1/examples/examples_assets/TinPhases.png`

 * *Files identical despite different names*

### Comparing `manim-chemistry-0.1.0/examples/examples_assets/orbitals_example.png` & `manim-chemistry-0.1.1/examples/examples_assets/orbitals_example.png`

 * *Files identical despite different names*

### Comparing `manim-chemistry-0.1.0/pyproject.toml` & `manim-chemistry-0.1.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "manim-chemistry"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Natural Language :: English",
 ]
-description = "Draws molecules. Nice!"
+description = "Manim Chemistry is a plugin for Manim which aims to make easier the animation of molecules and other chemistry-related objects such as orbitals, bohr diagrams and more."
 dependencies = [
     "manim",
     "numpy",
     "pandas",
 ]
 license = {file = "LICENSE.md"}
 readme = "README.md"
```

### Comparing `manim-chemistry-0.1.0/src/manim_chemistry/bohr_atom/bohr_atom.py` & `manim-chemistry-0.1.1/src/manim_chemistry/bohr_atom/bohr_atom.py`

 * *Files identical despite different names*

### Comparing `manim-chemistry-0.1.0/src/manim_chemistry/element/element.py` & `manim-chemistry-0.1.1/src/manim_chemistry/element/element.py`

 * *Files identical despite different names*

### Comparing `manim-chemistry-0.1.0/src/manim_chemistry/future_classes/future_classes.py` & `manim-chemistry-0.1.1/src/manim_chemistry/future_classes/future_classes.py`

 * *Files identical despite different names*

### Comparing `manim-chemistry-0.1.0/src/manim_chemistry/orbitals/orbitals.py` & `manim-chemistry-0.1.1/src/manim_chemistry/orbitals/orbitals.py`

 * *Files identical despite different names*

### Comparing `manim-chemistry-0.1.0/src/manim_chemistry/periodic_table/table_objects.py` & `manim-chemistry-0.1.1/src/manim_chemistry/periodic_table/table_objects.py`

 * *Files identical despite different names*

### Comparing `manim-chemistry-0.1.0/src/manim_chemistry/threeD/threedbond.py` & `manim-chemistry-0.1.1/src/manim_chemistry/threeD/threedbond.py`

 * *Files identical despite different names*

### Comparing `manim-chemistry-0.1.0/src/manim_chemistry/threeD/threedmolecule.py` & `manim-chemistry-0.1.1/src/manim_chemistry/threeD/threedmolecule.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,22 +37,18 @@
         if add_atoms:
             self.add(self.atoms)
         self.move_to(ORIGIN)
 
     def get_atoms_from_csv(self):
         atoms = OpenGLGroup()
         for _, atom in self.atoms_dict.items():
-            try:
-                element = Element.from_csv_file(
-                    self.source_csv, atom.get("element")
-                )  # TODO: Make the file an option
-                atoms.add(ThreeDAtom(element, atom.get("coords")))
-            except:
-                import ipdb
-                ipdb.set_trace()
+            element = Element.from_csv_file(
+                self.source_csv, atom.get("element")
+            )  # TODO: Make the file an option
+            atoms.add(ThreeDAtom(element, atom.get("coords")))
             
 
         return atoms
 
     def get_bonds(self):
         bonds = OpenGLGroup()
         for index, bonds_list in self.bonds_dict.items():
```

### Comparing `manim-chemistry-0.1.0/src/manim_chemistry/threeD/utils.py` & `manim-chemistry-0.1.1/src/manim_chemistry/threeD/utils.py`

 * *Files identical despite different names*

### Comparing `manim-chemistry-0.1.0/src/manim_chemistry/twoD/atom.py` & `manim-chemistry-0.1.1/src/manim_chemistry/twoD/atom.py`

 * *Files identical despite different names*

### Comparing `manim-chemistry-0.1.0/src/manim_chemistry/twoD/bond.py` & `manim-chemistry-0.1.1/src/manim_chemistry/twoD/bond.py`

 * *Files identical despite different names*

### Comparing `manim-chemistry-0.1.0/src/manim_chemistry/utils/utils.py` & `manim-chemistry-0.1.1/src/manim_chemistry/utils/utils.py`

 * *Files identical despite different names*

### Comparing `manim-chemistry-0.1.0/src/manim_chemistry.egg-info/PKG-INFO` & `manim-chemistry-0.1.1/src/manim_chemistry.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: manim-chemistry
-Version: 0.1.0
-Summary: Draws molecules. Nice!
+Version: 0.1.1
+Summary: Manim Chemistry is a plugin for Manim which aims to make easier the animation of molecules and other chemistry-related objects such as orbitals, bohr diagrams and more.
 Author-email: UMDQ <unmoldequimica@gmail.com>
 Maintainer-email: UMDQ <unmoldequimica@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 UMDQ
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -32,26 +32,41 @@
 - [Create a periodic table](#create-a-periodic-table)
 - [Making atomic orbitals](#making-atomic-orbitals)
 - [Making Bohr diagrams](#making-bohr-diagrams)
 - [Reading .mol files](#reading-mol-files)
 - [Typical issues with .mol files](#typical-issues-with-mol-files)
 - [Take a look to examples](#)
 - [Made with manimChemistry](#made-with-manimchemistry)
+- [How to contact](#how-to-contact)
+- [Great contributers](#great-contributers)
 
 # Installation.
 
-Right now this can be installed cloning the repo:
+You can install via pip:
+
+```
+pip install manim_chemistry
+```
+
+You can also clone the repo and install it from here:
 
 ```
 git clone https://github.com/UnMolDeQuimica/manim-Chemistry.git
 cd manim-Chemistry 
 python -m pip install .
 ```
 
-Soon this will be available in pip.
+or
+
+```
+git clone https://github.com/UnMolDeQuimica/manim-Chemistry.git
+cd manim-Chemistry 
+python -m pip install -e .
+```
+
 
 # What is manim-Chemistry?
 
 manim-Chemistry is a manim plugin designed to make chemistry animations easier.
 
 To my knowledge, there is only another plugin related to chemistry called [chanim](https://github.com/kilacoda/chanim) that aims to import to manim the chemfig package (and does an amazing job!).
 
@@ -95,15 +110,15 @@
 
 ```
 from manim import *
 from manim_chemistry import *
 
 class TwoDMoleculeScene(Scene):
    def construct(self):
-        morphine = MMoleculeObject.from_mol_file("morphine.mol")
+        morphine = MMoleculeObject.from_mol_file("morphine.mol", add_bonds_numbering=True)
         self.add(morphine)
 ```
 
 We get
 
 ![plot](/examples/examples_assets/2D_morphine_bond_numbering.png)
 
@@ -120,14 +135,31 @@
 ```
 
 Result:
 ![plot](/examples/examples_assets/2D_morphine_corrected_bonds.png)
 
 Now we are talking!
 
+### Named Molecules:
+
+You may want to add a name to a molecule. It is very simple, but it is handy to do all in the same object. You can create a NamedMolecule similarly to how you create a MMoleculeObject:
+
+```
+from manim import *
+from manim_chemistry import *
+
+class NamedMoleculeExample(Scene):
+    def construct(self):
+        named_molecule = NamedMolecule.from_mol_file(name="Morphine", filename="morphine.mol")
+        self.add(diagram)
+```
+![plot](/examples/examples_assets/NamedMoleculeExample_ManimCE_v0.17.3.png)
+
+You can also provided an already created molecule or an already created text and the NamedMolecule class will group them. This allows greater control for the user.
+
 ## Create 3D molecule:
 
 Creating a 3D molecule requires a bit more effort. We need two things:
 
 1. A .mol file (like before)
 2. A csv data file with data for your atoms. You can find an example inside the examples folder called "Elementos.csv". 
 
@@ -324,17 +356,27 @@
 
 Fullerene:
 ![plot](/examples/examples_assets/Fullerene.png)
 
 Beta and alpha tin structures:
 ![plot](/examples/examples_assets/TinPhases.png)
 
-A video using both and more examples:
+Videos using manimChemistry:
 
 https://www.youtube.com/watch?v=L7OXe94_WmA
 
+https://youtu.be/KgiCl_o_Aws
+
 
 # How to contact
 You can open issues and pull requests, but if you want to contact me directly you can go to:
 - Email: unmoldequimica@gmail.com
 - YouTube: https://www.youtube.com/@unmoldequimica
 - Twitter: https://twitter.com/unmoldequimica
+
+
+# Great contributers!
+- [@chemnerd28](https://github.com/chemnerd28)
+- [@Ant-28](https://github.com/Ant-28)
+
+
+Special thanks to [@Rodrigo-Tenorio](https://github.com/Rodrigo-Tenorio) for his help in the creation of this releasable package.
```

### Comparing `manim-chemistry-0.1.0/src/manim_chemistry.egg-info/SOURCES.txt` & `manim-chemistry-0.1.1/src/manim_chemistry.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .gitignore
+CHANGELOG.md
 LICENSE.md
 MANIFEST.in
 README.md
 TODO.md
 pyproject.toml
 setup.py
 .github/workflows/python-publish.yml
@@ -20,14 +21,15 @@
 examples/examples_assets/2D_morphine_bond_numbering.png
 examples/examples_assets/2D_morphine_corrected_bonds.png
 examples/examples_assets/BohrDiagram_ManimCE_v0.17.3.png
 examples/examples_assets/Draw3DMorphine_ManimCE_v0.17.3.png
 examples/examples_assets/DrawCarbonElement_ManimCE_v0.17.3.png
 examples/examples_assets/DrawPeriodicTable_ManimCE_v0.17.3.png
 examples/examples_assets/Fullerene.png
+examples/examples_assets/NamedMoleculeExample_ManimCE_v0.17.3.png
 examples/examples_assets/TinPhases.png
 examples/examples_assets/orbitals_example.png
 src/manim_chemistry/__init__.py
 src/manim_chemistry.egg-info/PKG-INFO
 src/manim_chemistry.egg-info/SOURCES.txt
 src/manim_chemistry.egg-info/dependency_links.txt
 src/manim_chemistry.egg-info/entry_points.txt
```

### Comparing `manim-chemistry-0.1.0/tests/test_working.py` & `manim-chemistry-0.1.1/tests/test_working.py`

 * *Files identical despite different names*

