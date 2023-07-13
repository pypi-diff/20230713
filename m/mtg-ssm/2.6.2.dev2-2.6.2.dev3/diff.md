# Comparing `tmp/mtg_ssm-2.6.2.dev2.tar.gz` & `tmp/mtg_ssm-2.6.2.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtg_ssm-2.6.2.dev2.tar", last modified: Thu Jul 13 08:17:27 2023, max compression
+gzip compressed data, was "mtg_ssm-2.6.2.dev3.tar", last modified: Thu Jul 13 08:23:07 2023, max compression
```

## Comparing `mtg_ssm-2.6.2.dev2.tar` & `mtg_ssm-2.6.2.dev3.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.372111 mtg_ssm-2.6.2.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.360111 mtg_ssm-2.6.2.dev2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.360111 mtg_ssm-2.6.2.dev2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/.github/workflows/integration.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-07-13 08:17:27.372111 mtg_ssm-2.6.2.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/TODO.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.360111 mtg_ssm-2.6.2.dev2/mtg_ssm/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-13 08:17:27.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.364111 mtg_ssm-2.6.2.dev2/mtg_ssm/containers/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/containers/bundles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/containers/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/containers/counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/containers/indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/containers/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.364111 mtg_ssm-2.6.2.dev2/mtg_ssm/mtg/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/mtg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/mtg/util.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.364111 mtg_ssm-2.6.2.dev2/mtg_ssm/scryfall/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/scryfall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/scryfall/fetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/scryfall/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.364111 mtg_ssm-2.6.2.dev2/mtg_ssm/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/serialization/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/serialization/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/serialization/xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)    10331 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/ssm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.364111 mtg_ssm-2.6.2.dev2/mtg_ssm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-07-13 08:17:27.000000 mtg_ssm-2.6.2.dev2/mtg_ssm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-13 08:17:27.000000 mtg_ssm-2.6.2.dev2/mtg_ssm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 08:17:27.000000 mtg_ssm-2.6.2.dev2/mtg_ssm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 08:17:27.000000 mtg_ssm-2.6.2.dev2/mtg_ssm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-13 08:17:27.000000 mtg_ssm-2.6.2.dev2/mtg_ssm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 08:17:27.000000 mtg_ssm-2.6.2.dev2/mtg_ssm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 08:17:27.372111 mtg_ssm-2.6.2.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.368111 mtg_ssm-2.6.2.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.368111 mtg_ssm-2.6.2.dev2/tests/containers/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/containers/test_bundles.py
--rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/containers/test_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/containers/test_indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/containers/test_legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.368111 mtg_ssm-2.6.2.dev2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/data/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/data/bulk_data.json
--rw-r--r--   0 runner    (1001) docker     (123)   456765 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/data/cards.json
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/data/migrations.json
--rw-r--r--   0 runner    (1001) docker     (123)    31317 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/data/sets.json
--rw-r--r--   0 runner    (1001) docker     (123)    15912 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/data/sets1.json
--rw-r--r--   0 runner    (1001) docker     (123)    15519 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/data/sets2.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     6683 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/gen_testdata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.368111 mtg_ssm-2.6.2.dev2/tests/mtg/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/mtg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/mtg/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.372111 mtg_ssm-2.6.2.dev2/tests/scryfall/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/scryfall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/scryfall/test_fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.372111 mtg_ssm-2.6.2.dev2/tests/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/serialization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.372111 mtg_ssm-2.6.2.dev2/tests/serialization/__snapshots__/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/serialization/__snapshots__/test_csv.ambr
--rw-r--r--   0 runner    (1001) docker     (123)    22102 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/serialization/__snapshots__/test_xlsx.ambr
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/serialization/test_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/serialization/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/serialization/test_xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)    16267 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/test_ssm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:23:07.982684 mtg_ssm-2.6.2.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:23:07.974684 mtg_ssm-2.6.2.dev3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:23:07.974684 mtg_ssm-2.6.2.dev3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/.github/workflows/integration.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-07-13 08:23:07.982684 mtg_ssm-2.6.2.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/TODO.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:23:07.974684 mtg_ssm-2.6.2.dev3/mtg_ssm/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/mtg_ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-13 08:23:07.000000 mtg_ssm-2.6.2.dev3/mtg_ssm/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:23:07.978684 mtg_ssm-2.6.2.dev3/mtg_ssm/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/mtg_ssm/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/mtg_ssm/containers/bundles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/mtg_ssm/containers/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/mtg_ssm/containers/counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/mtg_ssm/containers/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/mtg_ssm/containers/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:23:07.978684 mtg_ssm-2.6.2.dev3/mtg_ssm/mtg/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/mtg_ssm/mtg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/mtg_ssm/mtg/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/mtg_ssm/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:23:07.978684 mtg_ssm-2.6.2.dev3/mtg_ssm/scryfall/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/mtg_ssm/scryfall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/mtg_ssm/scryfall/fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/mtg_ssm/scryfall/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:23:07.978684 mtg_ssm-2.6.2.dev3/mtg_ssm/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/mtg_ssm/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/mtg_ssm/serialization/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/mtg_ssm/serialization/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/mtg_ssm/serialization/xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10331 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/mtg_ssm/ssm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:23:07.978684 mtg_ssm-2.6.2.dev3/mtg_ssm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-07-13 08:23:07.000000 mtg_ssm-2.6.2.dev3/mtg_ssm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-13 08:23:07.000000 mtg_ssm-2.6.2.dev3/mtg_ssm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 08:23:07.000000 mtg_ssm-2.6.2.dev3/mtg_ssm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 08:23:07.000000 mtg_ssm-2.6.2.dev3/mtg_ssm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-13 08:23:07.000000 mtg_ssm-2.6.2.dev3/mtg_ssm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 08:23:07.000000 mtg_ssm-2.6.2.dev3/mtg_ssm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 08:23:07.982684 mtg_ssm-2.6.2.dev3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:23:07.978684 mtg_ssm-2.6.2.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:23:07.978684 mtg_ssm-2.6.2.dev3/tests/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/tests/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/tests/containers/test_bundles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/tests/containers/test_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/tests/containers/test_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/tests/containers/test_legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:23:07.982684 mtg_ssm-2.6.2.dev3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/tests/data/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/tests/data/bulk_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)   456765 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/tests/data/cards.json
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/tests/data/migrations.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31317 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/tests/data/sets.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15912 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/tests/data/sets1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15519 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/tests/data/sets2.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6683 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/tests/gen_testdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:23:07.982684 mtg_ssm-2.6.2.dev3/tests/mtg/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/tests/mtg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/tests/mtg/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:23:07.982684 mtg_ssm-2.6.2.dev3/tests/scryfall/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/tests/scryfall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/tests/scryfall/test_fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:23:07.982684 mtg_ssm-2.6.2.dev3/tests/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/tests/serialization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:23:07.982684 mtg_ssm-2.6.2.dev3/tests/serialization/__snapshots__/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/tests/serialization/__snapshots__/test_csv.ambr
+-rw-r--r--   0 runner    (1001) docker     (123)    22102 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/tests/serialization/__snapshots__/test_xlsx.ambr
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/tests/serialization/test_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/tests/serialization/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/tests/serialization/test_xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16267 2023-07-13 08:22:53.000000 mtg_ssm-2.6.2.dev3/tests/test_ssm.py
```

### Comparing `mtg_ssm-2.6.2.dev2/.github/workflows/integration.yml` & `mtg_ssm-2.6.2.dev3/.github/workflows/integration.yml`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/.github/workflows/publish.yml` & `mtg_ssm-2.6.2.dev3/.github/workflows/publish.yml`

 * *Files 8% similar despite different names*

```diff
@@ -5,17 +5,19 @@
   push:
     branches:
       - trunk
     tags:
       - "**"
 
 jobs:
-  build-n-publish:
+  pypi-publish:
     runs-on: ubuntu-latest
     name: Build and publish Python 🐍 distributions 📦 to PyPI and TestPyPI
+    permissions:
+      id-token: write
 
     steps:
       - uses: actions/checkout@v3
         with:
           # setuptools_scm needs the git history
           fetch-depth: 0
 
@@ -32,16 +34,15 @@
         run: >-
           python -m build
           --sdist
           --wheel
           --outdir dist/
 
       - name: Publish distribution 📦 to Test PyPI
-        uses: pypa/gh-action-pypi-publish@v1.8.6
+        uses: pypa/gh-action-pypi-publish@release/v1.8
         with:
-          password: ${{ secrets.TEST_PYPI_API_TOKEN }}
-          repository_url: https://test.pypi.org/legacy/
+          repository-url: https://test.pypi.org/legacy/
 
       - name: Publish distribution 📦 to PyPI
-        uses: pypa/gh-action-pypi-publish@v1.8.6
+        uses: pypa/gh-action-pypi-publish@release/v1.8
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `mtg_ssm-2.6.2.dev2/.github/workflows/run-tests.yml` & `mtg_ssm-2.6.2.dev3/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/.gitignore` & `mtg_ssm-2.6.2.dev3/.gitignore`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/.pre-commit-config.yaml` & `mtg_ssm-2.6.2.dev3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/LICENSE.txt` & `mtg_ssm-2.6.2.dev3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/PKG-INFO` & `mtg_ssm-2.6.2.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtg_ssm
-Version: 2.6.2.dev2
+Version: 2.6.2.dev3
 Summary: A tool to manage Magic: the Gathering collection spreadsheets
 Author-email: George Leslie-Waksman <waksman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/gwax/mtg_ssm
 Project-URL: Bug Tracker, https://github.com/gwax/mtg_ssm/issues
 Keywords: mtg,magic,collection,tracking,spreadsheet
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mtg_ssm-2.6.2.dev2/README.rst` & `mtg_ssm-2.6.2.dev3/README.rst`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/mtg_ssm/containers/bundles.py` & `mtg_ssm-2.6.2.dev3/mtg_ssm/containers/bundles.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/mtg_ssm/containers/collection.py` & `mtg_ssm-2.6.2.dev3/mtg_ssm/containers/collection.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/mtg_ssm/containers/counts.py` & `mtg_ssm-2.6.2.dev3/mtg_ssm/containers/counts.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/mtg_ssm/containers/indexes.py` & `mtg_ssm-2.6.2.dev3/mtg_ssm/containers/indexes.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/mtg_ssm/containers/legacy.py` & `mtg_ssm-2.6.2.dev3/mtg_ssm/containers/legacy.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/mtg_ssm/mtg/util.py` & `mtg_ssm-2.6.2.dev3/mtg_ssm/mtg/util.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/mtg_ssm/scryfall/fetcher.py` & `mtg_ssm-2.6.2.dev3/mtg_ssm/scryfall/fetcher.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/mtg_ssm/scryfall/models.py` & `mtg_ssm-2.6.2.dev3/mtg_ssm/scryfall/models.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/mtg_ssm/serialization/csv.py` & `mtg_ssm-2.6.2.dev3/mtg_ssm/serialization/csv.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/mtg_ssm/serialization/interface.py` & `mtg_ssm-2.6.2.dev3/mtg_ssm/serialization/interface.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/mtg_ssm/serialization/xlsx.py` & `mtg_ssm-2.6.2.dev3/mtg_ssm/serialization/xlsx.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/mtg_ssm/ssm.py` & `mtg_ssm-2.6.2.dev3/mtg_ssm/ssm.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/mtg_ssm.egg-info/PKG-INFO` & `mtg_ssm-2.6.2.dev3/mtg_ssm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtg-ssm
-Version: 2.6.2.dev2
+Version: 2.6.2.dev3
 Summary: A tool to manage Magic: the Gathering collection spreadsheets
 Author-email: George Leslie-Waksman <waksman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/gwax/mtg_ssm
 Project-URL: Bug Tracker, https://github.com/gwax/mtg_ssm/issues
 Keywords: mtg,magic,collection,tracking,spreadsheet
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mtg_ssm-2.6.2.dev2/mtg_ssm.egg-info/SOURCES.txt` & `mtg_ssm-2.6.2.dev3/mtg_ssm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/pylintrc` & `mtg_ssm-2.6.2.dev3/pylintrc`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/pyproject.toml` & `mtg_ssm-2.6.2.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/tests/conftest.py` & `mtg_ssm-2.6.2.dev3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/tests/containers/test_bundles.py` & `mtg_ssm-2.6.2.dev3/tests/containers/test_bundles.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/tests/containers/test_counts.py` & `mtg_ssm-2.6.2.dev3/tests/containers/test_counts.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/tests/containers/test_indexes.py` & `mtg_ssm-2.6.2.dev3/tests/containers/test_indexes.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/tests/containers/test_legacy.py` & `mtg_ssm-2.6.2.dev3/tests/containers/test_legacy.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/tests/data/bulk_data.json` & `mtg_ssm-2.6.2.dev3/tests/data/bulk_data.json`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/tests/data/cards.json` & `mtg_ssm-2.6.2.dev3/tests/data/cards.json`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/tests/data/migrations.json` & `mtg_ssm-2.6.2.dev3/tests/data/migrations.json`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/tests/data/sets.json` & `mtg_ssm-2.6.2.dev3/tests/data/sets.json`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/tests/data/sets1.json` & `mtg_ssm-2.6.2.dev3/tests/data/sets1.json`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/tests/data/sets2.json` & `mtg_ssm-2.6.2.dev3/tests/data/sets2.json`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/tests/gen_testdata.py` & `mtg_ssm-2.6.2.dev3/tests/gen_testdata.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/tests/mtg/test_util.py` & `mtg_ssm-2.6.2.dev3/tests/mtg/test_util.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/tests/scryfall/test_fetcher.py` & `mtg_ssm-2.6.2.dev3/tests/scryfall/test_fetcher.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/tests/serialization/__snapshots__/test_csv.ambr` & `mtg_ssm-2.6.2.dev3/tests/serialization/__snapshots__/test_csv.ambr`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/tests/serialization/__snapshots__/test_xlsx.ambr` & `mtg_ssm-2.6.2.dev3/tests/serialization/__snapshots__/test_xlsx.ambr`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/tests/serialization/test_csv.py` & `mtg_ssm-2.6.2.dev3/tests/serialization/test_csv.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/tests/serialization/test_interface.py` & `mtg_ssm-2.6.2.dev3/tests/serialization/test_interface.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/tests/serialization/test_xlsx.py` & `mtg_ssm-2.6.2.dev3/tests/serialization/test_xlsx.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev2/tests/test_ssm.py` & `mtg_ssm-2.6.2.dev3/tests/test_ssm.py`

 * *Files identical despite different names*

