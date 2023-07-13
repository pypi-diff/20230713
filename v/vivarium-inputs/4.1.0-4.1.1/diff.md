# Comparing `tmp/vivarium_inputs-4.1.0.tar.gz` & `tmp/vivarium_inputs-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vivarium_inputs-4.1.0.tar", last modified: Fri Jun  2 00:21:01 2023, max compression
+gzip compressed data, was "vivarium_inputs-4.1.1.tar", last modified: Thu Jul 13 20:22:10 2023, max compression
```

## Comparing `vivarium_inputs-4.1.0.tar` & `vivarium_inputs-4.1.1.tar`

### file list

```diff
@@ -1,76 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:21:01.486185 vivarium_inputs-4.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-02 00:21:01.486185 vivarium_inputs-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:21:01.482185 vivarium_inputs-4.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/docs/nitpick-exceptions
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:21:01.482185 vivarium_inputs-4.1.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:21:01.482185 vivarium_inputs-4.1.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/docs/source/_static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:21:01.482185 vivarium_inputs-4.1.0/docs/source/api_reference/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/docs/source/api_reference/core.rst
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/docs/source/api_reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/docs/source/api_reference/interface.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/docs/source/api_reference/mapping_extension.rst
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/docs/source/api_reference/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7821 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:21:01.482185 vivarium_inputs-4.1.0/docs/source/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/docs/source/tutorials/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/docs/source/tutorials/pulling_data.rst
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 00:21:01.486185 vivarium_inputs-4.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1613 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:21:01.482185 vivarium_inputs-4.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:21:01.486185 vivarium_inputs-4.1.0/src/vivarium_inputs/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19647 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     6983 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:21:01.486185 vivarium_inputs-4.1.0/src/vivarium_inputs/mapping_extension/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/mapping_extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/mapping_extension/alternative_risk_factor.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/mapping_extension/alternative_risk_factor_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/mapping_extension/health_technology.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/mapping_extension/health_technology_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/mapping_extension/healthcare_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/mapping_extension/healthcare_entity_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:21:01.486185 vivarium_inputs-4.1.0/src/vivarium_inputs/testing/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/testing/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)    18148 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/utility_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:21:01.486185 vivarium_inputs-4.1.0/src/vivarium_inputs/validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    84467 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/validation/raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/validation/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)    57659 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/src/vivarium_inputs/validation/sim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:21:01.486185 vivarium_inputs-4.1.0/src/vivarium_inputs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-02 00:21:01.000000 vivarium_inputs-4.1.0/src/vivarium_inputs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-02 00:21:01.000000 vivarium_inputs-4.1.0/src/vivarium_inputs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 00:21:01.000000 vivarium_inputs-4.1.0/src/vivarium_inputs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 00:21:01.000000 vivarium_inputs-4.1.0/src/vivarium_inputs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-02 00:21:01.000000 vivarium_inputs-4.1.0/src/vivarium_inputs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-02 00:21:01.000000 vivarium_inputs-4.1.0/src/vivarium_inputs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:21:01.486185 vivarium_inputs-4.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:21:01.486185 vivarium_inputs-4.1.0/tests/extract/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/tests/extract/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/tests/extract/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/tests/extract/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/tests/extract/test_get_measure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/tests/extract/test_utility_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/tests/test_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:21:01.486185 vivarium_inputs-4.1.0/tests/validation/
--rw-r--r--   0 runner    (1001) docker     (123)    15435 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/tests/validation/test_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/tests/validation/test_shared.py
--rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-06-02 00:20:45.000000 vivarium_inputs-4.1.0/tests/validation/test_sim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:22:10.971866 vivarium_inputs-4.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:22:10.959866 vivarium_inputs-4.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:22:10.959866 vivarium_inputs-4.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-13 20:22:10.971866 vivarium_inputs-4.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:22:10.959866 vivarium_inputs-4.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/docs/nitpick-exceptions
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:22:10.959866 vivarium_inputs-4.1.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:22:10.959866 vivarium_inputs-4.1.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/docs/source/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:22:10.959866 vivarium_inputs-4.1.1/docs/source/api_reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/docs/source/api_reference/core.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/docs/source/api_reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/docs/source/api_reference/interface.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/docs/source/api_reference/mapping_extension.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/docs/source/api_reference/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:22:10.959866 vivarium_inputs-4.1.1/docs/source/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/docs/source/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/docs/source/tutorials/pulling_data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 20:22:10.971866 vivarium_inputs-4.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1895 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:22:10.951866 vivarium_inputs-4.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:22:10.959866 vivarium_inputs-4.1.1/src/vivarium_inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/src/vivarium_inputs/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/src/vivarium_inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 20:22:09.000000 vivarium_inputs-4.1.1/src/vivarium_inputs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19727 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/src/vivarium_inputs/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9565 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/src/vivarium_inputs/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6983 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/src/vivarium_inputs/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/src/vivarium_inputs/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:22:10.963866 vivarium_inputs-4.1.1/src/vivarium_inputs/mapping_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/src/vivarium_inputs/mapping_extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/src/vivarium_inputs/mapping_extension/alternative_risk_factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/src/vivarium_inputs/mapping_extension/alternative_risk_factor_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/src/vivarium_inputs/mapping_extension/health_technology.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/src/vivarium_inputs/mapping_extension/health_technology_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/src/vivarium_inputs/mapping_extension/healthcare_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/src/vivarium_inputs/mapping_extension/healthcare_entity_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:22:10.963866 vivarium_inputs-4.1.1/src/vivarium_inputs/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/src/vivarium_inputs/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/src/vivarium_inputs/testing/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18148 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/src/vivarium_inputs/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/src/vivarium_inputs/utility_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:22:10.963866 vivarium_inputs-4.1.1/src/vivarium_inputs/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/src/vivarium_inputs/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84465 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/src/vivarium_inputs/validation/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/src/vivarium_inputs/validation/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57659 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/src/vivarium_inputs/validation/sim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:22:10.963866 vivarium_inputs-4.1.1/src/vivarium_inputs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-13 20:22:10.000000 vivarium_inputs-4.1.1/src/vivarium_inputs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-13 20:22:10.000000 vivarium_inputs-4.1.1/src/vivarium_inputs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 20:22:10.000000 vivarium_inputs-4.1.1/src/vivarium_inputs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 20:22:10.000000 vivarium_inputs-4.1.1/src/vivarium_inputs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-13 20:22:10.000000 vivarium_inputs-4.1.1/src/vivarium_inputs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-13 20:22:10.000000 vivarium_inputs-4.1.1/src/vivarium_inputs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:22:10.971866 vivarium_inputs-4.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:22:10.971866 vivarium_inputs-4.1.1/tests/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/tests/extract/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/tests/extract/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/tests/extract/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/tests/extract/test_get_measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/tests/extract/test_utility_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:22:10.971866 vivarium_inputs-4.1.1/tests/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)    15435 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/tests/validation/test_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/tests/validation/test_shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/tests/validation/test_sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-13 20:21:50.000000 vivarium_inputs-4.1.1/tox.ini
```

### Comparing `vivarium_inputs-4.1.0/CHANGELOG.rst` & `vivarium_inputs-4.1.1/CHANGELOG.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+**4.1.1 - 07/13/23**
+
+ - Update pins
+ - Changes version metadata to use setuptools_scm
+ - Adds custom get_draws kwargs to pass through to vivarium_gbd_access
+
 **4.1.0 - 06/01/23**
 
  - Update pins
  - Bugfix PAF validation
  - Support Python 3.8-3.11
 
 **4.0.10 - 12/27/22**
```

### Comparing `vivarium_inputs-4.1.0/CODE_OF_CONDUCT.rst` & `vivarium_inputs-4.1.1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.0/CONTRIBUTING.rst` & `vivarium_inputs-4.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.0/LICENSE.txt` & `vivarium_inputs-4.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.0/PKG-INFO` & `vivarium_inputs-4.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vivarium_inputs
-Version: 4.1.0
+Version: 4.1.1
 Summary: Transformations and artifact building for the vivarium microsimulation project.
 Home-page: https://github.com/ihmeuw/vivarium_inputs
 Author: The vivarium developers
 Author-email: vivarium.dev@gmail.com
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: data
```

### Comparing `vivarium_inputs-4.1.0/README.rst` & `vivarium_inputs-4.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.0/docs/Makefile` & `vivarium_inputs-4.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.0/docs/source/conf.py` & `vivarium_inputs-4.1.1/docs/source/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,21 +29,21 @@
     exec(f.read(), about)
 
 sys.path.insert(0, str(Path("..").resolve()))
 
 # -- Project information -----------------------------------------------------
 
 project = about["__title__"]
-copyright = f'2021, {about["__author__"]}'
+copyright = f'2023, {about["__author__"]}'
 author = about["__author__"]
 
 # The short X.Y version.
-version = about["__version__"]
+version = vivarium_inputs.__version__
 # The full version, including alpha/beta/rc tags.
-release = about["__version__"]
+release = vivarium_inputs.__version__
 
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 
 needs_sphinx = "4.0"
```

### Comparing `vivarium_inputs-4.1.0/docs/source/tutorials/pulling_data.rst` & `vivarium_inputs-4.1.1/docs/source/tutorials/pulling_data.rst`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.0/setup.py` & `vivarium_inputs-4.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,19 +17,21 @@
     install_requirements = [
         "numpy",
         "scipy",
         "pandas",
         "click",
         "joblib",
         "tables",
-        "vivarium>=1.2.0",
+        "vivarium>=1.2.1",
         "gbd_mapping>=3.1.0, <4.0.0",
         "loguru",
     ]
 
+    setup_requires = ["setuptools_scm"]
+
     data_requires = ["vivarium-gbd-access>=3.0.7, <4.0.0", "core-maths"]
 
     test_requirements = [
         "pytest",
         "pytest-mock",
         "hypothesis",
     ]
@@ -37,15 +39,14 @@
     doc_requirements = [
         "sphinx>=4.0",
         "sphinx-rtd-theme",
     ]
 
     setup(
         name=about["__title__"],
-        version=about["__version__"],
         description=about["__summary__"],
         long_description=long_description,
         url=about["__uri__"],
         author=about["__author__"],
         author_email=about["__email__"],
         package_dir={"": "src"},
         packages=find_packages(where="src"),
@@ -55,8 +56,14 @@
         extras_require={
             "docs": doc_requirements,
             "test": test_requirements,
             "data": data_requires,
             "dev": doc_requirements + test_requirements + data_requires,
         },
         zip_safe=False,
+        use_scm_version={
+            "write_to": "src/vivarium_inputs/_version.py",
+            "write_to_template": '__version__ = "{version}"\n',
+            "tag_regex": r"^(?P<prefix>v)?(?P<version>[^\+]+)(?P<suffix>.*)?$",
+        },
+        setup_requires=setup_requires,
     )
```

### Comparing `vivarium_inputs-4.1.0/src/vivarium_inputs/core.py` & `vivarium_inputs-4.1.1/src/vivarium_inputs/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     DataDoesNotExistError,
     InvalidQueryError,
     Population,
 )
 from vivarium_inputs.mapping_extension import AlternativeRiskFactor, HealthcareEntity
 
 
-def get_data(entity, measure: str, location: Union[str, int]):
+def get_data(entity, measure: str, location: Union[str, int], **get_draws_kwargs):
     measure_handlers = {
         # Cause-like measures
         "incidence_rate": (get_incidence_rate, ("cause", "sequela")),
         "raw_incidence_rate": (get_raw_incidence_rate, ("cause", "sequela")),
         "prevalence": (get_prevalence, ("cause", "sequela")),
         "birth_prevalence": (get_birth_prevalence, ("cause", "sequela")),
         "disability_weight": (get_disability_weight, ("cause", "sequela")),
@@ -74,15 +74,15 @@
 
     if entity.kind not in entity_types:
         raise InvalidQueryError(f"{measure.capitalize()} not available for {entity.kind}.")
 
     location_id = (
         utility_data.get_location_id(location) if isinstance(location, str) else location
     )
-    data = handler(entity, location_id)
+    data = handler(entity, location_id, **get_draws_kwargs)
 
     if measure in [
         "structure",
         "theoretical_minimum_risk_life_expectancy",
         "estimate",
         "exposure_distribution_weights",
     ]:
@@ -213,17 +213,17 @@
     )
     data = utilities.normalize(data, fill_value=0)
     data = data.filter(DEMOGRAPHIC_COLUMNS + DRAW_COLUMNS)
     return data
 
 
 def get_exposure(
-    entity: Union[RiskFactor, AlternativeRiskFactor], location_id: int
+    entity: Union[RiskFactor, AlternativeRiskFactor], location_id: int, **get_draws_kwargs
 ) -> pd.DataFrame:
-    data = extract.extract_data(entity, "exposure", location_id)
+    data = extract.extract_data(entity, "exposure", location_id, **get_draws_kwargs)
     data = data.drop("modelable_entity_id", "columns")
 
     if entity.name in EXTRA_RESIDUAL_CATEGORY:
         cat = EXTRA_RESIDUAL_CATEGORY[entity.name]
         data = data.drop(labels=data.query("parameter == @cat").index)
         data[DRAW_COLUMNS] = data[DRAW_COLUMNS].clip(lower=MINIMUM_EXPOSURE_VALUE)
```

### Comparing `vivarium_inputs-4.1.0/src/vivarium_inputs/extract.py` & `vivarium_inputs-4.1.1/src/vivarium_inputs/extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 from typing import Union
 
 import pandas as pd
 from gbd_mapping import Cause, Covariate, Etiology, RiskFactor, Sequela
-from loguru import logger
 
 import vivarium_inputs.validation.raw as validation
 from vivarium_inputs.globals import (
     MEASURES,
     METRICS,
     OTHER_MEID,
-    RISKS_WITH_NEGATIVE_PAF,
     DataAbnormalError,
     DataDoesNotExistError,
     EmptyDataFrameException,
     InputsException,
     NoBestVersionError,
     Population,
     gbd,
 )
 from vivarium_inputs.mapping_extension import AlternativeRiskFactor, HealthcareEntity
 from vivarium_inputs.utilities import filter_to_most_detailed_causes
 
 
 def extract_data(
-    entity, measure: str, location_id: int, validate: bool = True
+    entity, measure: str, location_id: int, validate: bool = True, **get_draws_kwargs
 ) -> Union[pd.Series, pd.DataFrame]:
     """Check metadata for the requested entity-measure pair. Pull raw data from
     GBD. The only filtering that occurs is by applicable measure id, metric id,
     or to most detailed causes where relevant. If validate is turned on, will
     also pull any additional data needed for raw validation and call raw
     validation on the extracted data.
 
@@ -92,15 +90,15 @@
         ),
     }
 
     validation.check_metadata(entity, measure)
 
     try:
         main_extractor, additional_extractors = extractors[measure]
-        data = main_extractor(entity, location_id)
+        data = main_extractor(entity, location_id, **get_draws_kwargs)
     except (
         ValueError,
         AssertionError,
         EmptyDataFrameException,
         NoBestVersionError,
         InputsException,
     ) as e:
@@ -174,18 +172,18 @@
 def extract_deaths(entity: Cause, location_id: int) -> pd.DataFrame:
     data = gbd.get_codcorrect_draws(entity.gbd_id, location_id)
     data = data[data.measure_id == MEASURES["Deaths"]]
     return data
 
 
 def extract_exposure(
-    entity: Union[RiskFactor, AlternativeRiskFactor], location_id: int
+    entity: Union[RiskFactor, AlternativeRiskFactor], location_id: int, **get_draws_kwargs
 ) -> pd.DataFrame:
     if entity.kind == "risk_factor":
-        data = gbd.get_exposure(entity.gbd_id, location_id)
+        data = gbd.get_exposure(entity.gbd_id, location_id, **get_draws_kwargs)
         allowable_measures = [
             MEASURES["Proportion"],
             MEASURES["Continuous"],
             MEASURES["Prevalence"],
         ]
         proper_measure_id = set(data.measure_id).intersection(allowable_measures)
         if len(proper_measure_id) != 1:
```

### Comparing `vivarium_inputs-4.1.0/src/vivarium_inputs/globals.py` & `vivarium_inputs-4.1.1/src/vivarium_inputs/globals.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.0/src/vivarium_inputs/interface.py` & `vivarium_inputs-4.1.1/src/vivarium_inputs/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 from gbd_mapping import ModelableEntity
 
 import vivarium_inputs.validation.sim as validation
 from vivarium_inputs import core, extract, utilities, utility_data
 from vivarium_inputs.globals import Population
 
 
-def get_measure(entity: ModelableEntity, measure: str, location: str) -> pd.DataFrame:
+def get_measure(
+    entity: ModelableEntity, measure: str, location: str, **get_draws_kwargs
+) -> pd.DataFrame:
     """Pull GBD data for measure and entity and prep for simulation input,
     including scrubbing all GBD conventions to replace IDs with meaningful
     values or ranges and expanding over all demographic dimensions. To pull data
     using this function, please have at least 50GB of memory available.
 
     Available measures:
 
@@ -49,15 +51,15 @@
 
     Returns
     -------
     pandas.DataFrame
         Dataframe standardized to the format expected by `vivarium` simulations.
 
     """
-    data = core.get_data(entity, measure, location)
+    data = core.get_data(entity, measure, location, **get_draws_kwargs)
     data = utilities.scrub_gbd_conventions(data, location)
     validation.validate_for_simulation(data, entity, measure, location)
     data = utilities.split_interval(data, interval_column="age", split_column_prefix="age")
     data = utilities.split_interval(data, interval_column="year", split_column_prefix="year")
     return utilities.sort_hierarchical_data(data)
```

### Comparing `vivarium_inputs-4.1.0/src/vivarium_inputs/mapping_extension/alternative_risk_factor.py` & `vivarium_inputs-4.1.1/src/vivarium_inputs/mapping_extension/alternative_risk_factor.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.0/src/vivarium_inputs/mapping_extension/alternative_risk_factor_template.py` & `vivarium_inputs-4.1.1/src/vivarium_inputs/mapping_extension/alternative_risk_factor_template.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.0/src/vivarium_inputs/mapping_extension/healthcare_entity_template.py` & `vivarium_inputs-4.1.1/src/vivarium_inputs/mapping_extension/healthcare_entity_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,11 +24,10 @@
     """Holder of healthcare modelable entities"""
 
     __slots__ = ("outpatient_visits", "inpatient_visits")
 
     def __init__(
         self, outpatient_visits: HealthcareEntity, inpatient_visits: HealthcareEntity
     ):
-
         super().__init__()
         self.outpatient_visits = outpatient_visits
         self.inpatient_visits = inpatient_visits
```

### Comparing `vivarium_inputs-4.1.0/src/vivarium_inputs/utilities.py` & `vivarium_inputs-4.1.1/src/vivarium_inputs/utilities.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.0/src/vivarium_inputs/utility_data.py` & `vivarium_inputs-4.1.1/src/vivarium_inputs/utility_data.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.0/src/vivarium_inputs/validation/raw.py` & `vivarium_inputs-4.1.1/src/vivarium_inputs/validation/raw.py`

 * *Files 0% similar despite different names*

```diff
@@ -1221,15 +1221,14 @@
 
     check_cause_yll_yld_only_restrictions(data, entity)
 
 
 def validate_etiology_population_attributable_fraction(
     data: pd.DataFrame, entity: Etiology, context: RawValidationContext
 ) -> None:
-
     """Check the standard set of validations on raw etiology population
     attributable fraction data for entity. Check age group and sex ids
     and restrictions.
 
     Additionally, check yll/yld only restrictions to ensure that data
     do not include the data with the excluded measure_id by restrictions.
 
@@ -1612,15 +1611,14 @@
     Warns
     ------
         If a wider age range is found so users can further investigate.
     """
     if entity.restrictions.yld_only or entity.restrictions.yll_only:
         pass
     else:
-
         yll_start, yll_end = (
             entity.restrictions.yll_age_group_id_start,
             entity.restrictions.yll_age_group_id_end,
         )
         yld_start, yld_end = (
             entity.restrictions.yld_age_group_id_start,
             entity.restrictions.yld_age_group_id_end,
```

### Comparing `vivarium_inputs-4.1.0/src/vivarium_inputs/validation/shared.py` & `vivarium_inputs-4.1.1/src/vivarium_inputs/validation/shared.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.0/src/vivarium_inputs/validation/sim.py` & `vivarium_inputs-4.1.1/src/vivarium_inputs/validation/sim.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.0/src/vivarium_inputs.egg-info/PKG-INFO` & `vivarium_inputs-4.1.1/src/vivarium_inputs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vivarium-inputs
-Version: 4.1.0
+Version: 4.1.1
 Summary: Transformations and artifact building for the vivarium microsimulation project.
 Home-page: https://github.com/ihmeuw/vivarium_inputs
 Author: The vivarium developers
 Author-email: vivarium.dev@gmail.com
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: data
```

### Comparing `vivarium_inputs-4.1.0/src/vivarium_inputs.egg-info/SOURCES.txt` & `vivarium_inputs-4.1.1/src/vivarium_inputs.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,40 @@
+.gitattributes
+.gitignore
+.pylintrc
+.readthedocs.yml
 AUTHORS.rst
 CHANGELOG.rst
 CODE_OF_CONDUCT.rst
 CONTRIBUTING.rst
 LICENSE.txt
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.py
+tox.ini
+.github/CODEOWNERS
+.github/pull_request_template.md
+.github/workflows/build.yml
+.github/workflows/deploy.yml
 docs/Makefile
 docs/nitpick-exceptions
 docs/source/conf.py
 docs/source/index.rst
 docs/source/_static/style.css
 docs/source/api_reference/core.rst
 docs/source/api_reference/index.rst
 docs/source/api_reference/interface.rst
 docs/source/api_reference/mapping_extension.rst
 docs/source/api_reference/utilities.rst
 docs/source/tutorials/index.rst
 docs/source/tutorials/pulling_data.rst
 src/vivarium_inputs/__about__.py
 src/vivarium_inputs/__init__.py
+src/vivarium_inputs/_version.py
 src/vivarium_inputs/core.py
 src/vivarium_inputs/extract.py
 src/vivarium_inputs/globals.py
 src/vivarium_inputs/interface.py
 src/vivarium_inputs/utilities.py
 src/vivarium_inputs/utility_data.py
 src/vivarium_inputs.egg-info/PKG-INFO
```

### Comparing `vivarium_inputs-4.1.0/tests/conftest.py` & `vivarium_inputs-4.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.0/tests/extract/test_core.py` & `vivarium_inputs-4.1.1/tests/extract/test_core.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.0/tests/extract/test_extract.py` & `vivarium_inputs-4.1.1/tests/extract/test_extract.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.0/tests/extract/test_get_measure.py` & `vivarium_inputs-4.1.1/tests/extract/test_get_measure.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.0/tests/extract/test_utility_data.py` & `vivarium_inputs-4.1.1/tests/extract/test_utility_data.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.0/tests/test_utilities.py` & `vivarium_inputs-4.1.1/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.0/tests/validation/test_raw.py` & `vivarium_inputs-4.1.1/tests/validation/test_raw.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.0/tests/validation/test_shared.py` & `vivarium_inputs-4.1.1/tests/validation/test_shared.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.0/tests/validation/test_sim.py` & `vivarium_inputs-4.1.1/tests/validation/test_sim.py`

 * *Files identical despite different names*

