# Comparing `tmp/chemistry_tools-1.0.0b1.tar.gz` & `tmp/chemistry_tools-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemistry_tools-1.0.0b1.tar", last modified: Mon Jul 10 12:58:02 2023, max compression
+gzip compressed data, was "chemistry_tools-1.0.0b2.tar", last modified: Thu Jul 13 20:50:11 2023, max compression
```

## Comparing `chemistry_tools-1.0.0b1.tar` & `chemistry_tools-1.0.0b2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0 runner    (1001) docker     (122)     6033 2023-07-10 12:58:02.768788 chemistry_tools-1.0.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      207 2023-07-10 12:58:02.768788 chemistry_tools-1.0.0b1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     9971 2023-07-10 12:58:02.772788 chemistry_tools-1.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7652 2023-07-10 12:58:02.760788 chemistry_tools-1.0.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     6895 2023-07-10 12:58:02.768788 chemistry_tools-1.0.0b1/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/_memoized_property.py
--rw-r--r--   0 runner    (1001) docker     (122)     6505 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/toxnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     3098 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/cas.py
--rw-r--r--   0 runner    (1001) docker     (122)    17733 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/spectrum_similarity.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     8040 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/units.py
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/_memoized_property.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1354 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     8850 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/names.py
--rw-r--r--   0 runner    (1001) docker     (122)     7739 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     4375 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2875 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/property_format.py
--rw-r--r--   0 runner    (1001) docker     (122)    33686 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/lanthanides.py
--rw-r--r--   0 runner    (1001) docker     (122)     3591 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     3029 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/_isotope_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    12747 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/chalcogens.py
--rw-r--r--   0 runner    (1001) docker     (122)    12879 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/pnictogens.py
--rw-r--r--   0 runner    (1001) docker     (122)    19571 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/classes.py
--rw-r--r--   0 runner    (1001) docker     (122)    13576 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/alkaline_earth_metals.py
--rw-r--r--   0 runner    (1001) docker     (122)    14102 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/noble_gases.py
--rw-r--r--   0 runner    (1001) docker     (122)     7933 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14069 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/alkali_metals.py
--rw-r--r--   0 runner    (1001) docker     (122)    64225 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/transition_metals.py
--rw-r--r--   0 runner    (1001) docker     (122)     6594 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/_elements.py
--rw-r--r--   0 runner    (1001) docker     (122)    12668 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/halogens.py
--rw-r--r--   0 runner    (1001) docker     (122)    13191 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/triels.py
--rw-r--r--   0 runner    (1001) docker     (122)    12749 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/tetrels.py
--rw-r--r--   0 runner    (1001) docker     (122)    25825 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/elements/actinides.py
--rw-r--r--   0 runner    (1001) docker     (122)    10097 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/formulae/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5706 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/formulae/html.py
--rw-r--r--   0 runner    (1001) docker     (122)    10217 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/formulae/species.py
--rw-r--r--   0 runner    (1001) docker     (122)     4085 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/formulae/dataarray.py
--rw-r--r--   0 runner    (1001) docker     (122)    12587 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/formulae/parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     4482 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/formulae/iso_dist.py
--rw-r--r--   0 runner    (1001) docker     (122)     6979 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/formulae/compound.py
--rw-r--r--   0 runner    (1001) docker     (122)     4211 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/formulae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5771 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/formulae/latex.py
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/formulae/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4154 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/formulae/composition.py
--rw-r--r--   0 runner    (1001) docker     (122)     9673 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/formulae/_parser_core.py
--rw-r--r--   0 runner    (1001) docker     (122)    27405 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/formulae/formula.py
--rw-r--r--   0 runner    (1001) docker     (122)     6106 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/formulae/unicode.py
--rw-r--r--   0 runner    (1001) docker     (122)     2149 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/lookup.py
--rw-r--r--   0 runner    (1001) docker     (122)     2957 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/full_record.py
--rw-r--r--   0 runner    (1001) docker     (122)     4751 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3933 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/description.py
--rw-r--r--   0 runner    (1001) docker     (122)     5840 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     4880 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/bond.py
--rw-r--r--   0 runner    (1001) docker     (122)     3151 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)     1915 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/enums.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    14771 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/compound.py
--rw-r--r--   0 runner    (1001) docker     (122)     5676 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/atom.py
--rw-r--r--   0 runner    (1001) docker     (122)     2061 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/images.py
--rw-r--r--   0 runner    (1001) docker     (122)     2958 2023-07-10 12:57:30.968613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     9048 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/pug_rest.py
--rw-r--r--   0 runner    (1001) docker     (122)     3911 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/synonyms.py
--rw-r--r--   0 runner    (1001) docker     (122)    19312 2023-07-10 12:57:30.972613 chemistry_tools-1.0.0b1/chemistry_tools/pubchem/properties.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6033 2023-07-13 20:50:11.320987 chemistry_tools-1.0.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-07-13 20:50:11.324987 chemistry_tools-1.0.0b2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     9971 2023-07-13 20:50:11.328987 chemistry_tools-1.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7652 2023-07-13 20:50:11.312987 chemistry_tools-1.0.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     6895 2023-07-13 20:50:11.324987 chemistry_tools-1.0.0b2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/_memoized_property.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6505 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/toxnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3098 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/cas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17866 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/spectrum_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     8040 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/units.py
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/_memoized_property.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1354 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8850 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/names.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7739 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4375 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2875 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/property_format.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33686 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/lanthanides.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3591 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3029 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/_isotope_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12747 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/chalcogens.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12879 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/pnictogens.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19571 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13576 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/alkaline_earth_metals.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14102 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/noble_gases.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7933 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14069 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/alkali_metals.py
+-rw-r--r--   0 runner    (1001) docker     (122)    64225 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/transition_metals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6594 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/_elements.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12668 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/halogens.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13191 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/triels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12749 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/tetrels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25825 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/elements/actinides.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10097 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/formulae/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5706 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/formulae/html.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10217 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/formulae/species.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4085 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/formulae/dataarray.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12587 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/formulae/parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4482 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/formulae/iso_dist.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6979 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/formulae/compound.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4211 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/formulae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5771 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/formulae/latex.py
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/formulae/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4154 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/formulae/composition.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9673 2023-07-13 20:49:33.036247 chemistry_tools-1.0.0b2/chemistry_tools/formulae/_parser_core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27405 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/formulae/formula.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6106 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/formulae/unicode.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2149 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2957 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/full_record.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4751 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3933 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/description.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5840 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4880 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/bond.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3151 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1915 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/enums.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    14771 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/compound.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5676 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/atom.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2061 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/images.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2958 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     9048 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/pug_rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3911 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/synonyms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19312 2023-07-13 20:49:33.040247 chemistry_tools-1.0.0b2/chemistry_tools/pubchem/properties.py
```

### Comparing `chemistry_tools-1.0.0b1/pyproject.toml` & `chemistry_tools-1.0.0b2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "chemistry_tools"
-version = "1.0.0b1"
+version = "1.0.0b2"
 description = "Python tools for analysis of chemical compounds."
 readme = "README.rst"
 keywords = [ "chemistry", "utility",]
 dynamic = []
 dependencies = [
     "apeye>=0.9.1",
     "cachecontrol>=0.13.1",
```

### Comparing `chemistry_tools-1.0.0b1/PKG-INFO` & `chemistry_tools-1.0.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chemistry-tools
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: Python tools for analysis of chemical compounds.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: LGPL-3.0-or-later
 Keywords: chemistry,utility
 Home-page: https://github.com/domdfcoding/chemistry_tools
 Project-URL: Issue Tracker, https://github.com/domdfcoding/chemistry_tools/issues
 Project-URL: Source Code, https://github.com/domdfcoding/chemistry_tools
@@ -167,15 +167,15 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/chemistry_tools
 	:target: https://github.com/domdfcoding/chemistry_tools/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/chemistry_tools
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/chemistry_tools/v1.0.0b1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/chemistry_tools/v1.0.0b2
 	:target: https://github.com/domdfcoding/chemistry_tools/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/chemistry_tools
 	:target: https://github.com/domdfcoding/chemistry_tools/commit/master
 	:alt: GitHub last commit
```

### Comparing `chemistry_tools-1.0.0b1/LICENSE` & `chemistry_tools-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/README.rst` & `chemistry_tools-1.0.0b2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/chemistry_tools
 	:target: https://github.com/domdfcoding/chemistry_tools/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/chemistry_tools
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/chemistry_tools/v1.0.0b1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/chemistry_tools/v1.0.0b2
 	:target: https://github.com/domdfcoding/chemistry_tools/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/chemistry_tools
 	:target: https://github.com/domdfcoding/chemistry_tools/commit/master
 	:alt: GitHub last commit
```

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/toxnet.py` & `chemistry_tools-1.0.0b2/chemistry_tools/toxnet.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/cas.py` & `chemistry_tools-1.0.0b2/chemistry_tools/cas.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/spectrum_similarity.py` & `chemistry_tools-1.0.0b2/chemistry_tools/spectrum_similarity.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,33 +52,34 @@
 # stdlib
 from typing import Mapping, Optional, Sequence, Tuple, Union
 
 # 3rd party
 import numpy
 import pandas  # type: ignore[import]
 
-__all__ = ["spectrum_similarity", "normalize", "create_array"]
+__all__ = ["spectrum_similarity", "normalize", "create_array", "SpectrumSimilarity"]
 
 
 class SpectrumSimilarity:
 	"""
 	Calculate the similarity score for two mass spectra.
 
-	:param spec_top: Array containing the experimental spectrum's peak list with the m/z values in the
+	:param spec_top: Array containing the experimental spectrum's peak list with the *m/z* values in the
 		first column and corresponding intensities in the second
-	:param spec_bottom: Array containing the reference spectrum's peak list with the m/z values in the
+	:param spec_bottom: Array containing the reference spectrum's peak list with the *m/z* values in the
 		first column and corresponding intensities in the second
 	:param b: numeric value specifying the baseline threshold for peak identification.
 		Expressed as a percent of the maximum intensity.
-	:param x_threshold: numeric value specifying
 	:param xlim: tuple of length 2, defining the beginning and ending values of the x-axis.
 
 	.. versionadded:: 1.0.0
 
-	.. TODO: t: numeric value specifying the tolerance used to align the m/z values of the two spectra.
+	.. TODO:
+		x_threshold: numeric value specifying
+		t: numeric value specifying the tolerance used to align the *m/z* values of the two spectra.
 	"""
 
 	top_df: pandas.DataFrame
 	_top_df_plot: pandas.DataFrame  # includes peaks below ``b``
 	bottom_df: pandas.DataFrame
 	_bottom_df_plot: pandas.DataFrame  # includes peaks below ``b``
 	b: float
@@ -125,15 +126,17 @@
 	def _calculate_score(self, alignment: pandas.DataFrame) -> float:
 		u = numpy.array(alignment.iloc[:, 1])
 		v = numpy.array(alignment.iloc[:, 2])
 
 		return numpy.dot(u, v) / (numpy.sqrt(numpy.sum(numpy.square(u))) * numpy.sqrt(numpy.sum(numpy.square(v))))
 
 	def score(self) -> Tuple[float, float]:
-		# similarity score calculation
+		"""
+		Returns the similarity score.
+		"""
 
 		# Unimplemented R code
 		# alignment <- alignment[alignment[,1] >= x.threshold, ]
 
 		similarity_score = self._calculate_score(self.alignment)
 		reverse_similarity_score = self._calculate_score(self.reverse_alignment)
 
@@ -272,19 +275,21 @@
 		print_alignment: bool = False,
 		print_graphic: bool = True,
 		output_list: bool = False,
 		) -> Union[Tuple[float, float], Tuple[float, float, pandas.DataFrame]]:
 	"""
 	Calculate the similarity score for two mass spectra.
 
-	:param spec_top: Array containing the experimental spectrum's peak list with the m/z values in the
+	.. attention:: The :class:`~.SpectrumSimilarity` class is recommended over this function.
+
+	:param spec_top: Array containing the experimental spectrum's peak list with the *m/z* values in the
 		first column and corresponding intensities in the second
-	:param spec_bottom: Array containing the reference spectrum's peak list with the m/z values in the
+	:param spec_bottom: Array containing the reference spectrum's peak list with the *m/z* values in the
 		first column and corresponding intensities in the second
-	:param t: numeric value specifying the tolerance used to align the m/z values of the two spectra.
+	:param t: numeric value specifying the tolerance used to align the *m/z* values of the two spectra.
 	:param b: numeric value specifying the baseline threshold for peak identification.
 		Expressed as a percent of the maximum intensity.
 	:param top_label: string to label the top spectrum.
 	:param bottom_label: string to label the bottom spectrum.
 	:param xlim: tuple of length 2, defining the beginning and ending values of the x-axis.
 	:param x_threshold:
 	:param print_alignment:  whether the intensities should be printed
@@ -455,15 +460,15 @@
 
 	# http://jonathansoma.com/lede/foundations/classes/pandas%20columns%20and%20functions/apply-a-function-to-every-row-in-a-pandas-dataframe/
 	return (row["intensity"] / float(max_val)) * 100.0
 
 
 def create_array(intensities: Sequence[float], mz: Sequence[float]) -> numpy.ndarray:
 	"""
-	Create a :class:`numpy.ndarray`, in a format appropriate for :func:`~.spectrum_similarity`,
+	Create a :class:`numpy.ndarray`, in a format appropriate for :class:`~.SpectrumSimilarity`,
 	from a list of intensities and a list of *m/z* values.
 
 	:param intensities: List of intensities
 	:param mz: List of *m/z* values.
 	"""  # noqa: D400
 
 	return numpy.column_stack((mz, intensities))
```

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/units.py` & `chemistry_tools-1.0.0b2/chemistry_tools/units.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/cache.py` & `chemistry_tools-1.0.0b2/chemistry_tools/cache.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/names.py` & `chemistry_tools-1.0.0b2/chemistry_tools/names.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/constants.py` & `chemistry_tools-1.0.0b2/chemistry_tools/constants.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/__init__.py` & `chemistry_tools-1.0.0b2/chemistry_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/property_format.py` & `chemistry_tools-1.0.0b2/chemistry_tools/property_format.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/elements/lanthanides.py` & `chemistry_tools-1.0.0b2/chemistry_tools/elements/lanthanides.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/elements/_table.py` & `chemistry_tools-1.0.0b2/chemistry_tools/elements/_table.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/elements/_isotope_data.py` & `chemistry_tools-1.0.0b2/chemistry_tools/elements/_isotope_data.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/elements/chalcogens.py` & `chemistry_tools-1.0.0b2/chemistry_tools/elements/chalcogens.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/elements/pnictogens.py` & `chemistry_tools-1.0.0b2/chemistry_tools/elements/pnictogens.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/elements/classes.py` & `chemistry_tools-1.0.0b2/chemistry_tools/elements/classes.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/elements/alkaline_earth_metals.py` & `chemistry_tools-1.0.0b2/chemistry_tools/elements/alkaline_earth_metals.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/elements/noble_gases.py` & `chemistry_tools-1.0.0b2/chemistry_tools/elements/noble_gases.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/elements/__init__.py` & `chemistry_tools-1.0.0b2/chemistry_tools/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/elements/alkali_metals.py` & `chemistry_tools-1.0.0b2/chemistry_tools/elements/alkali_metals.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/elements/transition_metals.py` & `chemistry_tools-1.0.0b2/chemistry_tools/elements/transition_metals.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/elements/_elements.py` & `chemistry_tools-1.0.0b2/chemistry_tools/elements/_elements.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/elements/halogens.py` & `chemistry_tools-1.0.0b2/chemistry_tools/elements/halogens.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/elements/triels.py` & `chemistry_tools-1.0.0b2/chemistry_tools/elements/triels.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/elements/tetrels.py` & `chemistry_tools-1.0.0b2/chemistry_tools/elements/tetrels.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/elements/actinides.py` & `chemistry_tools-1.0.0b2/chemistry_tools/elements/actinides.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/formulae/utils.py` & `chemistry_tools-1.0.0b2/chemistry_tools/formulae/utils.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/formulae/html.py` & `chemistry_tools-1.0.0b2/chemistry_tools/formulae/html.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/formulae/species.py` & `chemistry_tools-1.0.0b2/chemistry_tools/formulae/species.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/formulae/dataarray.py` & `chemistry_tools-1.0.0b2/chemistry_tools/formulae/dataarray.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/formulae/parser.py` & `chemistry_tools-1.0.0b2/chemistry_tools/formulae/parser.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/formulae/iso_dist.py` & `chemistry_tools-1.0.0b2/chemistry_tools/formulae/iso_dist.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/formulae/compound.py` & `chemistry_tools-1.0.0b2/chemistry_tools/formulae/compound.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/formulae/__init__.py` & `chemistry_tools-1.0.0b2/chemistry_tools/formulae/__init__.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/formulae/latex.py` & `chemistry_tools-1.0.0b2/chemistry_tools/formulae/latex.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/formulae/composition.py` & `chemistry_tools-1.0.0b2/chemistry_tools/formulae/composition.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/formulae/_parser_core.py` & `chemistry_tools-1.0.0b2/chemistry_tools/formulae/_parser_core.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/formulae/formula.py` & `chemistry_tools-1.0.0b2/chemistry_tools/formulae/formula.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/formulae/unicode.py` & `chemistry_tools-1.0.0b2/chemistry_tools/formulae/unicode.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/pubchem/lookup.py` & `chemistry_tools-1.0.0b2/chemistry_tools/pubchem/lookup.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/pubchem/full_record.py` & `chemistry_tools-1.0.0b2/chemistry_tools/pubchem/full_record.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/pubchem/utils.py` & `chemistry_tools-1.0.0b2/chemistry_tools/pubchem/utils.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/pubchem/description.py` & `chemistry_tools-1.0.0b2/chemistry_tools/pubchem/description.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/pubchem/errors.py` & `chemistry_tools-1.0.0b2/chemistry_tools/pubchem/errors.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/pubchem/bond.py` & `chemistry_tools-1.0.0b2/chemistry_tools/pubchem/bond.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/pubchem/enums.py` & `chemistry_tools-1.0.0b2/chemistry_tools/pubchem/enums.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/pubchem/enums.pyi` & `chemistry_tools-1.0.0b2/chemistry_tools/pubchem/enums.pyi`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/pubchem/compound.py` & `chemistry_tools-1.0.0b2/chemistry_tools/pubchem/compound.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/pubchem/atom.py` & `chemistry_tools-1.0.0b2/chemistry_tools/pubchem/atom.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/pubchem/images.py` & `chemistry_tools-1.0.0b2/chemistry_tools/pubchem/images.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/pubchem/__init__.py` & `chemistry_tools-1.0.0b2/chemistry_tools/pubchem/__init__.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/pubchem/pug_rest.py` & `chemistry_tools-1.0.0b2/chemistry_tools/pubchem/pug_rest.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/pubchem/synonyms.py` & `chemistry_tools-1.0.0b2/chemistry_tools/pubchem/synonyms.py`

 * *Files identical despite different names*

### Comparing `chemistry_tools-1.0.0b1/chemistry_tools/pubchem/properties.py` & `chemistry_tools-1.0.0b2/chemistry_tools/pubchem/properties.py`

 * *Files identical despite different names*

