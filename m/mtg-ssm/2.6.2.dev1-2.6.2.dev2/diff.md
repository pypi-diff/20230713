# Comparing `tmp/mtg_ssm-2.6.2.dev1.tar.gz` & `tmp/mtg_ssm-2.6.2.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtg_ssm-2.6.2.dev1.tar", last modified: Thu Jul 13 08:16:06 2023, max compression
+gzip compressed data, was "mtg_ssm-2.6.2.dev2.tar", last modified: Thu Jul 13 08:17:27 2023, max compression
```

## Comparing `mtg_ssm-2.6.2.dev1.tar` & `mtg_ssm-2.6.2.dev2.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.377427 mtg_ssm-2.6.2.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.369427 mtg_ssm-2.6.2.dev1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.369427 mtg_ssm-2.6.2.dev1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/.github/workflows/integration.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-07-13 08:16:06.377427 mtg_ssm-2.6.2.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/TODO.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.369427 mtg_ssm-2.6.2.dev1/mtg_ssm/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-13 08:16:06.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.369427 mtg_ssm-2.6.2.dev1/mtg_ssm/containers/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/containers/bundles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/containers/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/containers/counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/containers/indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/containers/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.369427 mtg_ssm-2.6.2.dev1/mtg_ssm/mtg/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/mtg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/mtg/util.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.373427 mtg_ssm-2.6.2.dev1/mtg_ssm/scryfall/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/scryfall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/scryfall/fetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/scryfall/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.373427 mtg_ssm-2.6.2.dev1/mtg_ssm/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/serialization/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/serialization/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/serialization/xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)    10331 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/ssm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.369427 mtg_ssm-2.6.2.dev1/mtg_ssm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-07-13 08:16:06.000000 mtg_ssm-2.6.2.dev1/mtg_ssm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-13 08:16:06.000000 mtg_ssm-2.6.2.dev1/mtg_ssm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 08:16:06.000000 mtg_ssm-2.6.2.dev1/mtg_ssm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 08:16:06.000000 mtg_ssm-2.6.2.dev1/mtg_ssm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-13 08:16:06.000000 mtg_ssm-2.6.2.dev1/mtg_ssm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 08:16:06.000000 mtg_ssm-2.6.2.dev1/mtg_ssm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 08:16:06.377427 mtg_ssm-2.6.2.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.373427 mtg_ssm-2.6.2.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.373427 mtg_ssm-2.6.2.dev1/tests/containers/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/containers/test_bundles.py
--rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/containers/test_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/containers/test_indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/containers/test_legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.373427 mtg_ssm-2.6.2.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/data/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/data/bulk_data.json
--rw-r--r--   0 runner    (1001) docker     (123)   456696 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/data/cards.json
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/data/migrations.json
--rw-r--r--   0 runner    (1001) docker     (123)    31317 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/data/sets.json
--rw-r--r--   0 runner    (1001) docker     (123)    15912 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/data/sets1.json
--rw-r--r--   0 runner    (1001) docker     (123)    15519 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/data/sets2.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     6683 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/gen_testdata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.373427 mtg_ssm-2.6.2.dev1/tests/mtg/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/mtg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/mtg/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.373427 mtg_ssm-2.6.2.dev1/tests/scryfall/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/scryfall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/scryfall/test_fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.377427 mtg_ssm-2.6.2.dev1/tests/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/serialization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.377427 mtg_ssm-2.6.2.dev1/tests/serialization/__snapshots__/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/serialization/__snapshots__/test_csv.ambr
--rw-r--r--   0 runner    (1001) docker     (123)    22102 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/serialization/__snapshots__/test_xlsx.ambr
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/serialization/test_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/serialization/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/serialization/test_xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)    16267 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/test_ssm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.372111 mtg_ssm-2.6.2.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.360111 mtg_ssm-2.6.2.dev2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.360111 mtg_ssm-2.6.2.dev2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/.github/workflows/integration.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-07-13 08:17:27.372111 mtg_ssm-2.6.2.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/TODO.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.360111 mtg_ssm-2.6.2.dev2/mtg_ssm/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-13 08:17:27.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.364111 mtg_ssm-2.6.2.dev2/mtg_ssm/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/containers/bundles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/containers/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/containers/counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/containers/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/containers/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.364111 mtg_ssm-2.6.2.dev2/mtg_ssm/mtg/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/mtg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/mtg/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.364111 mtg_ssm-2.6.2.dev2/mtg_ssm/scryfall/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/scryfall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/scryfall/fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/scryfall/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.364111 mtg_ssm-2.6.2.dev2/mtg_ssm/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/serialization/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/serialization/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/serialization/xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10331 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/mtg_ssm/ssm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.364111 mtg_ssm-2.6.2.dev2/mtg_ssm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-07-13 08:17:27.000000 mtg_ssm-2.6.2.dev2/mtg_ssm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-13 08:17:27.000000 mtg_ssm-2.6.2.dev2/mtg_ssm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 08:17:27.000000 mtg_ssm-2.6.2.dev2/mtg_ssm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 08:17:27.000000 mtg_ssm-2.6.2.dev2/mtg_ssm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-13 08:17:27.000000 mtg_ssm-2.6.2.dev2/mtg_ssm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 08:17:27.000000 mtg_ssm-2.6.2.dev2/mtg_ssm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 08:17:27.372111 mtg_ssm-2.6.2.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.368111 mtg_ssm-2.6.2.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.368111 mtg_ssm-2.6.2.dev2/tests/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/containers/test_bundles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/containers/test_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/containers/test_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/containers/test_legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.368111 mtg_ssm-2.6.2.dev2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/data/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/data/bulk_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)   456765 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/data/cards.json
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/data/migrations.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31317 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/data/sets.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15912 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/data/sets1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15519 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/data/sets2.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6683 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/gen_testdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.368111 mtg_ssm-2.6.2.dev2/tests/mtg/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/mtg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/mtg/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.372111 mtg_ssm-2.6.2.dev2/tests/scryfall/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/scryfall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/scryfall/test_fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.372111 mtg_ssm-2.6.2.dev2/tests/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/serialization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:17:27.372111 mtg_ssm-2.6.2.dev2/tests/serialization/__snapshots__/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/serialization/__snapshots__/test_csv.ambr
+-rw-r--r--   0 runner    (1001) docker     (123)    22102 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/serialization/__snapshots__/test_xlsx.ambr
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/serialization/test_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/serialization/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/serialization/test_xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16267 2023-07-13 08:17:15.000000 mtg_ssm-2.6.2.dev2/tests/test_ssm.py
```

### Comparing `mtg_ssm-2.6.2.dev1/.github/workflows/integration.yml` & `mtg_ssm-2.6.2.dev2/.github/workflows/integration.yml`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/.github/workflows/publish.yml` & `mtg_ssm-2.6.2.dev2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/.github/workflows/run-tests.yml` & `mtg_ssm-2.6.2.dev2/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/.gitignore` & `mtg_ssm-2.6.2.dev2/.gitignore`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/.pre-commit-config.yaml` & `mtg_ssm-2.6.2.dev2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/LICENSE.txt` & `mtg_ssm-2.6.2.dev2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/PKG-INFO` & `mtg_ssm-2.6.2.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtg_ssm
-Version: 2.6.2.dev1
+Version: 2.6.2.dev2
 Summary: A tool to manage Magic: the Gathering collection spreadsheets
 Author-email: George Leslie-Waksman <waksman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/gwax/mtg_ssm
 Project-URL: Bug Tracker, https://github.com/gwax/mtg_ssm/issues
 Keywords: mtg,magic,collection,tracking,spreadsheet
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mtg_ssm-2.6.2.dev1/README.rst` & `mtg_ssm-2.6.2.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/mtg_ssm/containers/bundles.py` & `mtg_ssm-2.6.2.dev2/mtg_ssm/containers/bundles.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/mtg_ssm/containers/collection.py` & `mtg_ssm-2.6.2.dev2/mtg_ssm/containers/collection.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/mtg_ssm/containers/counts.py` & `mtg_ssm-2.6.2.dev2/mtg_ssm/containers/counts.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/mtg_ssm/containers/indexes.py` & `mtg_ssm-2.6.2.dev2/mtg_ssm/containers/indexes.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/mtg_ssm/containers/legacy.py` & `mtg_ssm-2.6.2.dev2/mtg_ssm/containers/legacy.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/mtg_ssm/mtg/util.py` & `mtg_ssm-2.6.2.dev2/mtg_ssm/mtg/util.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/mtg_ssm/scryfall/fetcher.py` & `mtg_ssm-2.6.2.dev2/mtg_ssm/scryfall/fetcher.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/mtg_ssm/scryfall/models.py` & `mtg_ssm-2.6.2.dev2/mtg_ssm/scryfall/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,16 @@
     DOUBLE_FACED_TOKEN = "double_faced_token"
     EMBLEM = "emblem"
     AUGMENT = "augment"
     HOST = "host"
     ART_SERIES = "art_series"
     DOUBLE_SIDED = "double_sided"
     REVERSIBLE_CARD = "reversible_card"
+    MUTATE = "mutate"
+    PROTOTYPE = "prototype"
 
 
 class ScryCardFrame(str, Enum):
     """Enum for https://scryfall.com/docs/api/layouts#frames"""
 
     Y1993 = "1993"
     Y1997 = "1997"
@@ -113,14 +115,16 @@
     LESSON = "lesson"
     TEXTLESS = "textless"
     SHATTEREDGLASS = "shatteredglass"
     CONVERTDFC = "convertdfc"
     FANDFC = "fandfc"
     UPSIDEDOWNDFC = "upsidedowndfc"
     GILDED = "gilded"
+    BORDERLESS = "borderless"
+    THICK = "thick"
 
 
 class ScryBorderColor(str, Enum):
     """Enum for card border_color"""
 
     BLACK = "black"
     BORDERLESS = "borderless"
```

### Comparing `mtg_ssm-2.6.2.dev1/mtg_ssm/serialization/csv.py` & `mtg_ssm-2.6.2.dev2/mtg_ssm/serialization/csv.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/mtg_ssm/serialization/interface.py` & `mtg_ssm-2.6.2.dev2/mtg_ssm/serialization/interface.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/mtg_ssm/serialization/xlsx.py` & `mtg_ssm-2.6.2.dev2/mtg_ssm/serialization/xlsx.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/mtg_ssm/ssm.py` & `mtg_ssm-2.6.2.dev2/mtg_ssm/ssm.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/mtg_ssm.egg-info/PKG-INFO` & `mtg_ssm-2.6.2.dev2/mtg_ssm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtg-ssm
-Version: 2.6.2.dev1
+Version: 2.6.2.dev2
 Summary: A tool to manage Magic: the Gathering collection spreadsheets
 Author-email: George Leslie-Waksman <waksman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/gwax/mtg_ssm
 Project-URL: Bug Tracker, https://github.com/gwax/mtg_ssm/issues
 Keywords: mtg,magic,collection,tracking,spreadsheet
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mtg_ssm-2.6.2.dev1/mtg_ssm.egg-info/SOURCES.txt` & `mtg_ssm-2.6.2.dev2/mtg_ssm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/pylintrc` & `mtg_ssm-2.6.2.dev2/pylintrc`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/pyproject.toml` & `mtg_ssm-2.6.2.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/tests/conftest.py` & `mtg_ssm-2.6.2.dev2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/tests/containers/test_bundles.py` & `mtg_ssm-2.6.2.dev2/tests/containers/test_bundles.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/tests/containers/test_counts.py` & `mtg_ssm-2.6.2.dev2/tests/containers/test_counts.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/tests/containers/test_indexes.py` & `mtg_ssm-2.6.2.dev2/tests/containers/test_indexes.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/tests/containers/test_legacy.py` & `mtg_ssm-2.6.2.dev2/tests/containers/test_legacy.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/tests/data/bulk_data.json` & `mtg_ssm-2.6.2.dev2/tests/data/bulk_data.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333334%*

 * *Differences: {"'data'": "{0: {'download_uri': "*

 * *           "'https://data.scryfall.io/default-cards/default-cards-20230712211359.json', "*

 * *           "'updated_at': '2023-07-12T21:13:59.586000Z'}}"}*

```diff
@@ -1,18 +1,18 @@
 {
     "data": [
         {
             "content_encoding": "gzip",
             "content_type": "application/json",
             "description": "A JSON file containing every card object on Scryfall in English or the printed language if the card is only available in one language.",
-            "download_uri": "https://data.scryfall.io/default-cards/default-cards-20230316210924.json",
+            "download_uri": "https://data.scryfall.io/default-cards/default-cards-20230712211359.json",
             "id": "e2ef41e3-5778-4bc2-af3f-78eca4dd9c23",
             "name": "Default Cards",
             "object": "bulk_data",
             "type": "default_cards",
-            "updated_at": "2023-03-16T21:09:24.643000Z",
+            "updated_at": "2023-07-12T21:13:59.586000Z",
             "uri": "https://api.scryfall.com/bulk-data/e2ef41e3-5778-4bc2-af3f-78eca4dd9c23"
         }
     ],
     "has_more": false,
     "object": "list"
 }
```

### Comparing `mtg_ssm-2.6.2.dev1/tests/data/cards.json` & `mtg_ssm-2.6.2.dev2/tests/data/cards.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9881206777197278%*

 * *Differences: {'0': "{'edhrec_rank': 4512, 'penny_rank': 9108, 'prices': {'usd': '1.27', 'eur': '1.00'}}",*

 * * '1': "{'edhrec_rank': 21468, 'prices': {'usd': '0.15', 'usd_foil': '0.20', 'eur': '0.02'}}",*

 * * '10': "{'edhrec_rank': 19494, 'prices': {'usd': '0.17', 'eur': '0.02'}}",*

 * * '11': "{'edhrec_rank': 2875, 'penny_rank': 126, 'prices': {'usd': '0.42', 'eur': '0.35'}}",*

 * * '12': "{'edhrec_rank': 66, 'penny_rank': 25, 'prices': {'usd': '1.47', 'eur': '1.00', 'tix': "*

 * *       "'0.69'}}",*

 * * '13': "{'edhrec_rank': 66, 'penny_rank':  […]*

```diff
@@ -13,15 +13,15 @@
         "color_identity": [
             "W"
         ],
         "colors": [
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 4168,
+        "edhrec_rank": 4512,
         "finishes": [
             "nonfoil"
         ],
         "flavor_text": "Only leonin clerics who can survive the Razor Fields for one turning of the suns can stand in the Cave of Light.",
         "foil": false,
         "frame": "2003",
         "full_art": false,
@@ -72,21 +72,21 @@
         ],
         "name": "Leonin Abunas",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "10064324-34a0-47eb-a58e-01db10234ed9",
         "oracle_text": "Artifacts you control have hexproof. (They can't be the targets of spells or abilities your opponents control.)",
         "oversized": false,
-        "penny_rank": 8902,
+        "penny_rank": 9108,
         "power": "2",
         "prices": {
-            "eur": "0.40",
+            "eur": "1.00",
             "eur_foil": null,
             "tix": null,
-            "usd": "0.77",
+            "usd": "1.27",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A10064324-34a0-47eb-a58e-01db10234ed9&unique=prints",
         "promo": false,
         "rarity": "rare",
         "related_uris": {
@@ -155,15 +155,15 @@
         "color_identity": [
             "W"
         ],
         "colors": [
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 20524,
+        "edhrec_rank": 21468,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2003",
         "full_art": false,
@@ -220,20 +220,20 @@
         "name": "Faithful Squire // Kaiso, Memory of Loyalty",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "2358ffc2-6663-4ef3-b3a4-b036a4733ac6",
         "oversized": false,
         "power": "2",
         "prices": {
-            "eur": "0.09",
+            "eur": "0.02",
             "eur_foil": "0.59",
             "tix": "0.02",
-            "usd": "0.11",
+            "usd": "0.15",
             "usd_etched": null,
-            "usd_foil": "0.28"
+            "usd_foil": "0.20"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A2358ffc2-6663-4ef3-b3a4-b036a4733ac6&unique=prints",
         "promo": false,
         "rarity": "uncommon",
         "related_uris": {
             "edhrec": "https://edhrec.com/route/?cc=Faithful+Squire",
             "gatherer": "https://gatherer.wizards.com/Pages/Card/Details.aspx?multiverseid=74093",
@@ -270,15 +270,15 @@
         "card_back_id": "0aeebaf5-8c7d-4636-9e82-8c27447861f7",
         "cardmarket_id": 11972,
         "cmc": 0.0,
         "collector_number": "273",
         "color_identity": [],
         "colors": [],
         "digital": false,
-        "edhrec_rank": 1979,
+        "edhrec_rank": 2077,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2003",
         "full_art": false,
@@ -333,20 +333,20 @@
         "name": "Boseiju, Who Shelters All",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "36937483-30cb-449a-8028-75017a124922",
         "oracle_text": "Boseiju, Who Shelters All enters the battlefield tapped.\n{T}, Pay 2 life: Add {C}. If that mana is spent on an instant or sorcery spell, that spell can't be countered.",
         "oversized": false,
         "prices": {
-            "eur": "15.90",
-            "eur_foil": "37.50",
-            "tix": "0.22",
-            "usd": "22.68",
+            "eur": "6.95",
+            "eur_foil": "41.00",
+            "tix": "0.02",
+            "usd": "19.05",
             "usd_etched": null,
-            "usd_foil": "108.88"
+            "usd_foil": "102.45"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A36937483-30cb-449a-8028-75017a124922&unique=prints",
         "produced_mana": [
             "C"
         ],
         "promo": false,
         "rarity": "rare",
@@ -415,15 +415,15 @@
         "color_identity": [
             "W"
         ],
         "colors": [
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 12469,
+        "edhrec_rank": 13194,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2003",
         "full_art": false,
@@ -479,23 +479,23 @@
             78600
         ],
         "name": "Bushi Tenderfoot // Kenzo the Hardhearted",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "82959ca2-cd96-4cca-9ce0-afb8db209860",
         "oversized": false,
-        "penny_rank": 9564,
+        "penny_rank": 9815,
         "power": "1",
         "prices": {
-            "eur": "0.05",
-            "eur_foil": "4.95",
+            "eur": "0.08",
+            "eur_foil": "0.20",
             "tix": "0.02",
-            "usd": "0.24",
+            "usd": "0.27",
             "usd_etched": null,
-            "usd_foil": "6.85"
+            "usd_foil": "6.70"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A82959ca2-cd96-4cca-9ce0-afb8db209860&unique=prints",
         "promo": false,
         "rarity": "uncommon",
         "related_uris": {
             "edhrec": "https://edhrec.com/route/?cc=Bushi+Tenderfoot",
             "gatherer": "https://gatherer.wizards.com/Pages/Card/Details.aspx?multiverseid=78600",
@@ -536,15 +536,15 @@
         "color_identity": [
             "W"
         ],
         "colors": [
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 16876,
+        "edhrec_rank": 17787,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2003",
         "full_art": false,
@@ -600,23 +600,23 @@
         ],
         "name": "J\u00f6tun Grunt",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "43fbfeec-bcaf-48b8-befe-b7346fec5a3a",
         "oracle_text": "Cumulative upkeep\u2014Put two cards from a single graveyard on the bottom of their owner's library. (At the beginning of your upkeep, put an age counter on this permanent, then sacrifice it unless you pay its upkeep cost for each age counter on it.)",
         "oversized": false,
-        "penny_rank": 10808,
+        "penny_rank": 11340,
         "power": "4",
         "prices": {
-            "eur": "0.10",
-            "eur_foil": "0.99",
+            "eur": "0.13",
+            "eur_foil": "2.00",
             "tix": "0.02",
-            "usd": "0.17",
+            "usd": "0.20",
             "usd_etched": null,
-            "usd_foil": "7.49"
+            "usd_foil": "6.99"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A43fbfeec-bcaf-48b8-befe-b7346fec5a3a&unique=prints",
         "promo": false,
         "rarity": "uncommon",
         "related_uris": {
             "edhrec": "https://edhrec.com/route/?cc=J%C3%B6tun+Grunt",
             "gatherer": "https://gatherer.wizards.com/Pages/Card/Details.aspx?multiverseid=122075",
@@ -675,15 +675,15 @@
         "color_identity": [
             "G"
         ],
         "colors": [
             "G"
         ],
         "digital": false,
-        "edhrec_rank": 6581,
+        "edhrec_rank": 6794,
         "finishes": [
             "nonfoil"
         ],
         "foil": false,
         "frame": "1993",
         "full_art": false,
         "games": [
@@ -733,21 +733,21 @@
         ],
         "name": "Thallid",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "46abaabe-7015-4d82-a5aa-2706b1f51bed",
         "oracle_text": "At the beginning of your upkeep, put a spore counter on Thallid.\nRemove three spore counters from Thallid: Create a 1/1 green Saproling creature token.",
         "oversized": false,
-        "penny_rank": 8836,
+        "penny_rank": 9290,
         "power": "1",
         "prices": {
-            "eur": "0.05",
+            "eur": "0.10",
             "eur_foil": null,
             "tix": null,
-            "usd": "0.20",
+            "usd": "0.18",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A46abaabe-7015-4d82-a5aa-2706b1f51bed&unique=prints",
         "promo": false,
         "rarity": "common",
         "related_uris": {
@@ -808,15 +808,15 @@
         "color_identity": [
             "G"
         ],
         "colors": [
             "G"
         ],
         "digital": false,
-        "edhrec_rank": 6581,
+        "edhrec_rank": 6794,
         "finishes": [
             "nonfoil"
         ],
         "foil": false,
         "frame": "1993",
         "full_art": false,
         "games": [
@@ -866,21 +866,21 @@
         ],
         "name": "Thallid",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "46abaabe-7015-4d82-a5aa-2706b1f51bed",
         "oracle_text": "At the beginning of your upkeep, put a spore counter on Thallid.\nRemove three spore counters from Thallid: Create a 1/1 green Saproling creature token.",
         "oversized": false,
-        "penny_rank": 8836,
+        "penny_rank": 9290,
         "power": "1",
         "prices": {
-            "eur": "0.05",
+            "eur": "0.04",
             "eur_foil": null,
             "tix": null,
-            "usd": "0.18",
+            "usd": "0.20",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A46abaabe-7015-4d82-a5aa-2706b1f51bed&unique=prints",
         "promo": false,
         "rarity": "common",
         "related_uris": {
@@ -941,15 +941,15 @@
         "color_identity": [
             "G"
         ],
         "colors": [
             "G"
         ],
         "digital": false,
-        "edhrec_rank": 6581,
+        "edhrec_rank": 6794,
         "finishes": [
             "nonfoil"
         ],
         "foil": false,
         "frame": "1993",
         "full_art": false,
         "games": [
@@ -999,21 +999,21 @@
         ],
         "name": "Thallid",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "46abaabe-7015-4d82-a5aa-2706b1f51bed",
         "oracle_text": "At the beginning of your upkeep, put a spore counter on Thallid.\nRemove three spore counters from Thallid: Create a 1/1 green Saproling creature token.",
         "oversized": false,
-        "penny_rank": 8836,
+        "penny_rank": 9290,
         "power": "1",
         "prices": {
-            "eur": "0.05",
+            "eur": "0.10",
             "eur_foil": null,
             "tix": null,
-            "usd": "0.21",
+            "usd": "0.16",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A46abaabe-7015-4d82-a5aa-2706b1f51bed&unique=prints",
         "promo": false,
         "rarity": "common",
         "related_uris": {
@@ -1074,15 +1074,15 @@
         "color_identity": [
             "G"
         ],
         "colors": [
             "G"
         ],
         "digital": false,
-        "edhrec_rank": 6581,
+        "edhrec_rank": 6794,
         "finishes": [
             "nonfoil"
         ],
         "foil": false,
         "frame": "1993",
         "full_art": false,
         "games": [
@@ -1132,21 +1132,21 @@
         ],
         "name": "Thallid",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "46abaabe-7015-4d82-a5aa-2706b1f51bed",
         "oracle_text": "At the beginning of your upkeep, put a spore counter on Thallid.\nRemove three spore counters from Thallid: Create a 1/1 green Saproling creature token.",
         "oversized": false,
-        "penny_rank": 8836,
+        "penny_rank": 9290,
         "power": "1",
         "prices": {
-            "eur": "0.15",
+            "eur": "0.10",
             "eur_foil": null,
             "tix": null,
-            "usd": "0.19",
+            "usd": "0.20",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A46abaabe-7015-4d82-a5aa-2706b1f51bed&unique=prints",
         "promo": false,
         "rarity": "common",
         "related_uris": {
@@ -1189,15 +1189,15 @@
         "color_identity": [
             "B"
         ],
         "colors": [
             "B"
         ],
         "digital": false,
-        "edhrec_rank": 18712,
+        "edhrec_rank": 19494,
         "finishes": [
             "nonfoil"
         ],
         "flavor_text": "\"It keeps some out, yes. It also keeps others in!\"\n\u2014Grandmother Sengir",
         "foil": false,
         "frame": "1993",
         "full_art": false,
@@ -1253,18 +1253,18 @@
         "nonfoil": true,
         "object": "card",
         "oracle_id": "443f8dd1-333d-42c4-a286-302a9496209a",
         "oracle_text": "Defender (This creature can't attack.)\nProtection from black",
         "oversized": false,
         "power": "0",
         "prices": {
-            "eur": "0.15",
+            "eur": "0.09",
             "eur_foil": null,
             "tix": null,
-            "usd": "0.18",
+            "usd": "0.22",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A443f8dd1-333d-42c4-a286-302a9496209a&unique=prints",
         "promo": false,
         "rarity": "common",
         "related_uris": {
@@ -1307,15 +1307,15 @@
         "color_identity": [
             "B"
         ],
         "colors": [
             "B"
         ],
         "digital": false,
-        "edhrec_rank": 18712,
+        "edhrec_rank": 19494,
         "finishes": [
             "nonfoil"
         ],
         "flavor_text": "\"Just the place for a picnic.\"\n\u2014Murat, Death Speaker",
         "foil": false,
         "frame": "1993",
         "full_art": false,
@@ -1371,18 +1371,18 @@
         "nonfoil": true,
         "object": "card",
         "oracle_id": "443f8dd1-333d-42c4-a286-302a9496209a",
         "oracle_text": "Defender (This creature can't attack.)\nProtection from black",
         "oversized": false,
         "power": "0",
         "prices": {
-            "eur": "0.05",
+            "eur": "0.02",
             "eur_foil": null,
             "tix": null,
-            "usd": "0.18",
+            "usd": "0.17",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A443f8dd1-333d-42c4-a286-302a9496209a&unique=prints",
         "promo": false,
         "rarity": "common",
         "related_uris": {
@@ -1426,15 +1426,15 @@
         "color_identity": [
             "W"
         ],
         "colors": [
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 2592,
+        "edhrec_rank": 2875,
         "finishes": [
             "nonfoil"
         ],
         "flavor_text": "Ixidor had only to imagine their ruin and Akroma made it so.",
         "foil": false,
         "frame": "2003",
         "full_art": false,
@@ -1490,20 +1490,20 @@
         ],
         "name": "Akroma's Vengeance",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "ae19dce5-c9fc-4fbe-99b5-dc6a12124a68",
         "oracle_text": "Destroy all artifacts, creatures, and enchantments.\nCycling {3} ({3}, Discard this card: Draw a card.)",
         "oversized": false,
-        "penny_rank": 135,
+        "penny_rank": 126,
         "prices": {
-            "eur": "0.98",
+            "eur": "0.35",
             "eur_foil": null,
             "tix": "0.59",
-            "usd": "0.39",
+            "usd": "0.42",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Aae19dce5-c9fc-4fbe-99b5-dc6a12124a68&unique=prints",
         "promo": false,
         "rarity": "rare",
         "related_uris": {
@@ -1545,15 +1545,15 @@
         "color_identity": [
             "B"
         ],
         "colors": [
             "B"
         ],
         "digital": false,
-        "edhrec_rank": 71,
+        "edhrec_rank": 66,
         "finishes": [
             "nonfoil"
         ],
         "flavor_text": "\"If there is such a thing as too much power, I have not discovered it.\"\n\u2014Volrath",
         "foil": false,
         "frame": "2003",
         "full_art": false,
@@ -1607,20 +1607,20 @@
         ],
         "name": "Dark Ritual",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "53f7c868-b03e-4fc2-8dcf-a75bbfa3272b",
         "oracle_text": "Add {B}{B}{B}.",
         "oversized": false,
-        "penny_rank": 27,
+        "penny_rank": 25,
         "prices": {
-            "eur": "1.32",
+            "eur": "1.00",
             "eur_foil": null,
-            "tix": "0.98",
-            "usd": "0.95",
+            "tix": "0.69",
+            "usd": "1.47",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A53f7c868-b03e-4fc2-8dcf-a75bbfa3272b&unique=prints",
         "produced_mana": [
             "B"
         ],
@@ -1665,15 +1665,15 @@
         "color_identity": [
             "B"
         ],
         "colors": [
             "B"
         ],
         "digital": false,
-        "edhrec_rank": 71,
+        "edhrec_rank": 66,
         "finishes": [
             "nonfoil"
         ],
         "flavor_text": "\"Leshrac, my liege, grant me the power I am due.\"\n\u2014Lim-D\u00fbl, the Necromancer",
         "foil": false,
         "frame": "1993",
         "full_art": false,
@@ -1726,20 +1726,20 @@
         ],
         "name": "Dark Ritual",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "53f7c868-b03e-4fc2-8dcf-a75bbfa3272b",
         "oracle_text": "Add {B}{B}{B}.",
         "oversized": false,
-        "penny_rank": 27,
+        "penny_rank": 25,
         "prices": {
-            "eur": "0.46",
+            "eur": "0.70",
             "eur_foil": null,
-            "tix": "1.85",
-            "usd": "1.04",
+            "tix": "1.39",
+            "usd": "1.24",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A53f7c868-b03e-4fc2-8dcf-a75bbfa3272b&unique=prints",
         "produced_mana": [
             "B"
         ],
@@ -1842,18 +1842,18 @@
         "name": "Forest",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "b34bb2dc-c1af-4d77-b0b3-a0fb342a5fc6",
         "oracle_text": "({T}: Add {G}.)",
         "oversized": false,
         "prices": {
-            "eur": "0.20",
+            "eur": "0.72",
             "eur_foil": null,
-            "tix": "0.11",
-            "usd": "0.91",
+            "tix": "0.20",
+            "usd": "0.85",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ab34bb2dc-c1af-4d77-b0b3-a0fb342a5fc6&unique=prints",
         "produced_mana": [
             "G"
         ],
@@ -1956,18 +1956,18 @@
         "name": "Forest",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "b34bb2dc-c1af-4d77-b0b3-a0fb342a5fc6",
         "oracle_text": "({T}: Add {G}.)",
         "oversized": false,
         "prices": {
-            "eur": "0.30",
+            "eur": "0.52",
             "eur_foil": null,
             "tix": "0.80",
-            "usd": "1.01",
+            "usd": "0.92",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ab34bb2dc-c1af-4d77-b0b3-a0fb342a5fc6&unique=prints",
         "produced_mana": [
             "G"
         ],
@@ -2070,18 +2070,18 @@
         "name": "Forest",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "b34bb2dc-c1af-4d77-b0b3-a0fb342a5fc6",
         "oracle_text": "({T}: Add {G}.)",
         "oversized": false,
         "prices": {
-            "eur": "0.19",
+            "eur": "0.21",
             "eur_foil": null,
-            "tix": "2.85",
-            "usd": "0.48",
+            "tix": "2.53",
+            "usd": "0.52",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ab34bb2dc-c1af-4d77-b0b3-a0fb342a5fc6&unique=prints",
         "produced_mana": [
             "G"
         ],
@@ -2184,18 +2184,18 @@
         "name": "Snow-Covered Forest",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "5f0d3be8-e63e-4ade-ae58-6b0c14f2ce6d",
         "oracle_text": "({T}: Add {G}.)",
         "oversized": false,
         "prices": {
-            "eur": "2.75",
+            "eur": "0.75",
             "eur_foil": null,
-            "tix": "2.09",
-            "usd": "2.07",
+            "tix": "1.80",
+            "usd": "2.18",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A5f0d3be8-e63e-4ade-ae58-6b0c14f2ce6d&unique=prints",
         "produced_mana": [
             "G"
         ],
@@ -2240,15 +2240,15 @@
         "color_identity": [
             "B"
         ],
         "colors": [
             "B"
         ],
         "digital": false,
-        "edhrec_rank": 15621,
+        "edhrec_rank": 16280,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "flavor_text": "Death took his humanity but not his skill with the knife.",
         "foil": true,
         "frame": "2003",
@@ -2305,15 +2305,15 @@
         ],
         "name": "Abattoir Ghoul",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "2b211adb-de44-4468-b65d-907a09aa7e9d",
         "oracle_text": "First strike\nWhenever a creature dealt damage by Abattoir Ghoul this turn dies, you gain life equal to that creature's toughness.",
         "oversized": false,
-        "penny_rank": 4727,
+        "penny_rank": 4764,
         "power": "3",
         "prices": {
             "eur": "0.05",
             "eur_foil": "0.15",
             "tix": "0.04",
             "usd": "0.05",
             "usd_etched": null,
@@ -2411,15 +2411,15 @@
         "cardmarket_id": 250620,
         "cmc": 1.0,
         "collector_number": "51",
         "color_identity": [
             "U"
         ],
         "digital": false,
-        "edhrec_rank": 11722,
+        "edhrec_rank": 12106,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2003",
         "frame_effects": [
@@ -2469,22 +2469,22 @@
             226755
         ],
         "name": "Delver of Secrets // Insectile Aberration",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "edd531b9-f615-4399-8c8c-1c5e18c4acbf",
         "oversized": false,
-        "penny_rank": 102,
+        "penny_rank": 94,
         "prices": {
-            "eur": "0.53",
-            "eur_foil": "5.75",
-            "tix": "0.02",
-            "usd": "0.61",
+            "eur": "0.84",
+            "eur_foil": "4.85",
+            "tix": "0.03",
+            "usd": "0.41",
             "usd_etched": null,
-            "usd_foil": "6.68"
+            "usd_foil": "5.02"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Aedd531b9-f615-4399-8c8c-1c5e18c4acbf&unique=prints",
         "promo": false,
         "rarity": "common",
         "related_uris": {
             "edhrec": "https://edhrec.com/route/?cc=Delver+of+Secrets",
             "gatherer": "https://gatherer.wizards.com/Pages/Card/Details.aspx?multiverseid=226749",
@@ -2584,20 +2584,20 @@
         "name": "Forest",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "b34bb2dc-c1af-4d77-b0b3-a0fb342a5fc6",
         "oracle_text": "({T}: Add {G}.)",
         "oversized": false,
         "prices": {
-            "eur": "0.09",
-            "eur_foil": "1.00",
+            "eur": "0.15",
+            "eur_foil": "0.77",
             "tix": "0.02",
-            "usd": "0.17",
+            "usd": "0.16",
             "usd_etched": null,
-            "usd_foil": "1.44"
+            "usd_foil": "1.65"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ab34bb2dc-c1af-4d77-b0b3-a0fb342a5fc6&unique=prints",
         "produced_mana": [
             "G"
         ],
         "promo": false,
         "rarity": "common",
@@ -2700,20 +2700,20 @@
         "name": "Forest",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "b34bb2dc-c1af-4d77-b0b3-a0fb342a5fc6",
         "oracle_text": "({T}: Add {G}.)",
         "oversized": false,
         "prices": {
-            "eur": "0.09",
+            "eur": "0.15",
             "eur_foil": "0.80",
             "tix": "0.03",
-            "usd": "0.18",
+            "usd": "0.17",
             "usd_etched": null,
-            "usd_foil": "1.37"
+            "usd_foil": "1.22"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ab34bb2dc-c1af-4d77-b0b3-a0fb342a5fc6&unique=prints",
         "produced_mana": [
             "G"
         ],
         "promo": false,
         "rarity": "common",
@@ -2816,20 +2816,20 @@
         "name": "Forest",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "b34bb2dc-c1af-4d77-b0b3-a0fb342a5fc6",
         "oracle_text": "({T}: Add {G}.)",
         "oversized": false,
         "prices": {
-            "eur": "0.09",
-            "eur_foil": "0.99",
+            "eur": "0.30",
+            "eur_foil": "0.75",
             "tix": "0.03",
             "usd": "0.20",
             "usd_etched": null,
-            "usd_foil": "0.61"
+            "usd_foil": "0.53"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ab34bb2dc-c1af-4d77-b0b3-a0fb342a5fc6&unique=prints",
         "produced_mana": [
             "G"
         ],
         "promo": false,
         "rarity": "common",
@@ -2899,34 +2899,34 @@
             "arena"
         ],
         "highres_image": false,
         "id": "f7f1ce0b-6668-4d16-8fe0-07c65ce4bc82",
         "illustration_id": "06cf6a73-f000-4a7d-bd1e-e57ed1800dde",
         "image_status": "lowres",
         "image_uris": {
-            "art_crop": "https://cards.scryfall.io/art_crop/front/f/7/f7f1ce0b-6668-4d16-8fe0-07c65ce4bc82.jpg?1645415589",
-            "border_crop": "https://cards.scryfall.io/border_crop/front/f/7/f7f1ce0b-6668-4d16-8fe0-07c65ce4bc82.jpg?1645415589",
-            "large": "https://cards.scryfall.io/large/front/f/7/f7f1ce0b-6668-4d16-8fe0-07c65ce4bc82.jpg?1645415589",
-            "normal": "https://cards.scryfall.io/normal/front/f/7/f7f1ce0b-6668-4d16-8fe0-07c65ce4bc82.jpg?1645415589",
-            "png": "https://cards.scryfall.io/png/front/f/7/f7f1ce0b-6668-4d16-8fe0-07c65ce4bc82.png?1645415589",
-            "small": "https://cards.scryfall.io/small/front/f/7/f7f1ce0b-6668-4d16-8fe0-07c65ce4bc82.jpg?1645415589"
+            "art_crop": "https://cards.scryfall.io/art_crop/front/f/7/f7f1ce0b-6668-4d16-8fe0-07c65ce4bc82.jpg?1681158506",
+            "border_crop": "https://cards.scryfall.io/border_crop/front/f/7/f7f1ce0b-6668-4d16-8fe0-07c65ce4bc82.jpg?1681158506",
+            "large": "https://cards.scryfall.io/large/front/f/7/f7f1ce0b-6668-4d16-8fe0-07c65ce4bc82.jpg?1681158506",
+            "normal": "https://cards.scryfall.io/normal/front/f/7/f7f1ce0b-6668-4d16-8fe0-07c65ce4bc82.jpg?1681158506",
+            "png": "https://cards.scryfall.io/png/front/f/7/f7f1ce0b-6668-4d16-8fe0-07c65ce4bc82.png?1681158506",
+            "small": "https://cards.scryfall.io/small/front/f/7/f7f1ce0b-6668-4d16-8fe0-07c65ce4bc82.jpg?1681158506"
         },
         "keywords": [
             "Scry"
         ],
         "lang": "en",
         "layout": "normal",
         "legalities": {
             "alchemy": "not_legal",
             "brawl": "not_legal",
             "commander": "not_legal",
             "duel": "not_legal",
             "explorer": "not_legal",
             "future": "not_legal",
-            "gladiator": "legal",
+            "gladiator": "not_legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "not_legal",
             "modern": "not_legal",
             "oathbreaker": "not_legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
@@ -3014,15 +3014,15 @@
         "card_back_id": "0aeebaf5-8c7d-4636-9e82-8c27447861f7",
         "cardmarket_id": 532177,
         "cmc": 4.0,
         "collector_number": "237",
         "color_identity": [],
         "colors": [],
         "digital": false,
-        "edhrec_rank": 1393,
+        "edhrec_rank": 1473,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "flavor_text": "The Skoti owe their immortality to the elixir, and the manner of its creation is their most closely guarded secret.",
         "foil": true,
         "frame": "2015",
@@ -3077,27 +3077,27 @@
         ],
         "name": "Cosmos Elixir",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "ed7300f4-831a-4ba4-b5e6-ceba8d079eaa",
         "oracle_text": "At the beginning of your end step, draw a card if your life total is greater than your starting life total. Otherwise, you gain 2 life.",
         "oversized": false,
-        "penny_rank": 770,
+        "penny_rank": 859,
         "preview": {
             "previewed_at": "2021-01-16",
             "source": "Luca Van Deun",
             "source_uri": "https://twitter.com/LegenVD/status/1350493142966013952"
         },
         "prices": {
-            "eur": "0.94",
-            "eur_foil": "1.50",
+            "eur": "1.03",
+            "eur_foil": "1.39",
             "tix": "0.02",
-            "usd": "1.66",
+            "usd": "0.89",
             "usd_etched": null,
-            "usd_foil": "1.97"
+            "usd_foil": "0.99"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Aed7300f4-831a-4ba4-b5e6-ceba8d079eaa&unique=prints",
         "promo": false,
         "rarity": "rare",
         "related_uris": {
             "edhrec": "https://edhrec.com/route/?cc=Cosmos+Elixir",
             "gatherer": "https://gatherer.wizards.com/Pages/Card/Details.aspx?multiverseid=503853",
@@ -3152,15 +3152,15 @@
         "card_back_id": "0aeebaf5-8c7d-4636-9e82-8c27447861f7",
         "cardmarket_id": 532412,
         "cmc": 4.0,
         "collector_number": "368",
         "color_identity": [],
         "colors": [],
         "digital": false,
-        "edhrec_rank": 1393,
+        "edhrec_rank": 1473,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "frame_effects": [
@@ -3216,27 +3216,27 @@
         ],
         "name": "Cosmos Elixir",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "ed7300f4-831a-4ba4-b5e6-ceba8d079eaa",
         "oracle_text": "At the beginning of your end step, draw a card if your life total is greater than your starting life total. Otherwise, you gain 2 life.",
         "oversized": false,
-        "penny_rank": 770,
+        "penny_rank": 859,
         "preview": {
             "previewed_at": "2021-01-20",
             "source": "Luca Van Deun",
             "source_uri": "https://twitter.com/LegenVD/status/1350493142966013952"
         },
         "prices": {
-            "eur": "1.90",
-            "eur_foil": "1.80",
+            "eur": "1.80",
+            "eur_foil": "1.90",
             "tix": null,
-            "usd": "1.42",
+            "usd": "1.32",
             "usd_etched": null,
-            "usd_foil": "1.73"
+            "usd_foil": "1.58"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Aed7300f4-831a-4ba4-b5e6-ceba8d079eaa&unique=prints",
         "promo": false,
         "promo_types": [
             "boosterfun"
         ],
         "rarity": "rare",
@@ -3280,15 +3280,15 @@
         "color_identity": [
             "U"
         ],
         "colors": [
             "U"
         ],
         "digital": false,
-        "edhrec_rank": 17698,
+        "edhrec_rank": 18560,
         "finishes": [
             "nonfoil"
         ],
         "flavor_text": "These spirits of the air are winsome and wild, and cannot be truly contained. Only marginally intelligent, they often substitute whimsy for strategy, delighting in mischief and mayhem.",
         "foil": false,
         "frame": "1993",
         "full_art": false,
@@ -3341,21 +3341,21 @@
         ],
         "name": "Air Elemental",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "7744bae4-a8b7-44a5-9b4c-0048ad4cc448",
         "oracle_text": "Flying",
         "oversized": false,
-        "penny_rank": 6499,
+        "penny_rank": 6681,
         "power": "4",
         "prices": {
             "eur": "369.00",
             "eur_foil": null,
             "tix": null,
-            "usd": null,
+            "usd": "148.92",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A7744bae4-a8b7-44a5-9b4c-0048ad4cc448&unique=prints",
         "promo": false,
         "rarity": "uncommon",
         "related_uris": {
@@ -3398,15 +3398,15 @@
         "color_identity": [
             "B"
         ],
         "colors": [
             "B"
         ],
         "digital": false,
-        "edhrec_rank": 71,
+        "edhrec_rank": 66,
         "finishes": [
             "nonfoil"
         ],
         "foil": false,
         "frame": "1993",
         "full_art": false,
         "games": [
@@ -3456,20 +3456,20 @@
         ],
         "name": "Dark Ritual",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "53f7c868-b03e-4fc2-8dcf-a75bbfa3272b",
         "oracle_text": "Add {B}{B}{B}.",
         "oversized": false,
-        "penny_rank": 27,
+        "penny_rank": 25,
         "prices": {
-            "eur": "265.00",
+            "eur": "172.99",
             "eur_foil": null,
             "tix": null,
-            "usd": "315.99",
+            "usd": "336.99",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A53f7c868-b03e-4fc2-8dcf-a75bbfa3272b&unique=prints",
         "produced_mana": [
             "B"
         ],
@@ -3570,18 +3570,18 @@
         "name": "Forest",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "b34bb2dc-c1af-4d77-b0b3-a0fb342a5fc6",
         "oracle_text": "({T}: Add {G}.)",
         "oversized": false,
         "prices": {
-            "eur": "33.99",
+            "eur": "30.00",
             "eur_foil": null,
             "tix": null,
-            "usd": "53.56",
+            "usd": "45.04",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ab34bb2dc-c1af-4d77-b0b3-a0fb342a5fc6&unique=prints",
         "produced_mana": [
             "G"
         ],
@@ -3682,18 +3682,18 @@
         "name": "Forest",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "b34bb2dc-c1af-4d77-b0b3-a0fb342a5fc6",
         "oracle_text": "({T}: Add {G}.)",
         "oversized": false,
         "prices": {
-            "eur": "29.99",
+            "eur": "32.67",
             "eur_foil": null,
             "tix": null,
-            "usd": "76.63",
+            "usd": "59.85",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ab34bb2dc-c1af-4d77-b0b3-a0fb342a5fc6&unique=prints",
         "produced_mana": [
             "G"
         ],
@@ -3738,15 +3738,15 @@
         "color_identity": [
             "B"
         ],
         "colors": [
             "B"
         ],
         "digital": false,
-        "edhrec_rank": 1638,
+        "edhrec_rank": 1817,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "flavor_text": "\"Under the suns, Mirrodin kneels and begs us for perfection.\"\n\u2014Geth, Lord of the Vault",
         "foil": true,
         "frame": "2003",
@@ -3801,22 +3801,22 @@
         ],
         "name": "Black Sun's Zenith",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "038c0165-32b6-4e81-8180-604b49905207",
         "oracle_text": "Put X -1/-1 counters on each creature. Shuffle Black Sun's Zenith into its owner's library.",
         "oversized": false,
-        "penny_rank": 1796,
+        "penny_rank": 1740,
         "prices": {
-            "eur": "4.61",
-            "eur_foil": "9.49",
+            "eur": "4.72",
+            "eur_foil": "10.00",
             "tix": "0.02",
-            "usd": "5.58",
+            "usd": "4.68",
             "usd_etched": null,
-            "usd_foil": "11.92"
+            "usd_foil": "12.75"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A038c0165-32b6-4e81-8180-604b49905207&unique=prints",
         "promo": false,
         "rarity": "rare",
         "related_uris": {
             "edhrec": "https://edhrec.com/route/?cc=Black+Sun%27s+Zenith",
             "gatherer": "https://gatherer.wizards.com/Pages/Card/Details.aspx?multiverseid=214061",
@@ -3875,15 +3875,15 @@
         "color_identity": [
             "W"
         ],
         "colors": [
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 2268,
+        "edhrec_rank": 1891,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2003",
         "full_art": false,
@@ -3920,15 +3920,15 @@
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "legal",
             "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
-            "penny": "not_legal",
+            "penny": "legal",
             "pioneer": "not_legal",
             "predh": "legal",
             "premodern": "not_legal",
             "standard": "not_legal",
             "vintage": "legal"
         },
         "mana_cost": "{2}{W}{W}",
@@ -3939,22 +3939,23 @@
         ],
         "name": "Hero of Bladehold",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "454a8902-8120-4373-96ee-bbf352b04e8d",
         "oracle_text": "Battle cry (Whenever this creature attacks, each other attacking creature gets +1/+0 until end of turn.)\nWhenever Hero of Bladehold attacks, create two 1/1 white Soldier creature tokens that are tapped and attacking.",
         "oversized": false,
+        "penny_rank": 2167,
         "power": "3",
         "prices": {
-            "eur": "8.15",
-            "eur_foil": "11.00",
-            "tix": "0.10",
-            "usd": "15.49",
+            "eur": "2.00",
+            "eur_foil": "9.94",
+            "tix": "0.02",
+            "usd": "11.17",
             "usd_etched": null,
-            "usd_foil": "26.66"
+            "usd_foil": "29.49"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A454a8902-8120-4373-96ee-bbf352b04e8d&unique=prints",
         "promo": false,
         "rarity": "mythic",
         "related_uris": {
             "edhrec": "https://edhrec.com/route/?cc=Hero+of+Bladehold",
             "gatherer": "https://gatherer.wizards.com/Pages/Card/Details.aspx?multiverseid=214064",
@@ -4014,15 +4015,15 @@
         "color_identity": [
             "G"
         ],
         "colors": [
             "G"
         ],
         "digital": false,
-        "edhrec_rank": 6581,
+        "edhrec_rank": 6794,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2003",
         "full_art": false,
@@ -4076,21 +4077,21 @@
         ],
         "name": "Thallid",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "46abaabe-7015-4d82-a5aa-2706b1f51bed",
         "oracle_text": "At the beginning of your upkeep, put a spore counter on Thallid.\nRemove three spore counters from Thallid: Create a 1/1 green Saproling creature token.",
         "oversized": false,
-        "penny_rank": 8836,
+        "penny_rank": 9290,
         "power": "1",
         "prices": {
-            "eur": "0.15",
-            "eur_foil": "1.27",
+            "eur": "0.49",
+            "eur_foil": "0.15",
             "tix": "0.03",
-            "usd": "0.28",
+            "usd": "0.30",
             "usd_etched": null,
             "usd_foil": "0.51"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A46abaabe-7015-4d82-a5aa-2706b1f51bed&unique=prints",
         "promo": false,
         "rarity": "common",
         "related_uris": {
@@ -4132,15 +4133,15 @@
         "cmc": 0.0,
         "collector_number": "266",
         "color_identity": [
             "G"
         ],
         "colors": [],
         "digital": false,
-        "edhrec_rank": 127,
+        "edhrec_rank": 106,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "frame_effects": [
@@ -4205,20 +4206,20 @@
         "oversized": false,
         "preview": {
             "previewed_at": "2022-01-27",
             "source": "Wizards of the Coast",
             "source_uri": "https://www.twitch.tv/videos/1277767538"
         },
         "prices": {
-            "eur": "38.97",
-            "eur_foil": "37.72",
-            "tix": "54.84",
-            "usd": "37.02",
+            "eur": "34.99",
+            "eur_foil": "48.96",
+            "tix": "21.80",
+            "usd": "28.93",
             "usd_etched": null,
-            "usd_foil": "40.06"
+            "usd_foil": "29.73"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Abf1341dd-41a3-49f6-87ec-63170dde4324&unique=prints",
         "produced_mana": [
             "G"
         ],
         "promo": false,
         "rarity": "rare",
@@ -4261,15 +4262,15 @@
         "cmc": 0.0,
         "collector_number": "412",
         "color_identity": [
             "G"
         ],
         "colors": [],
         "digital": false,
-        "edhrec_rank": 127,
+        "edhrec_rank": 106,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "frame_effects": [
@@ -4333,20 +4334,20 @@
         "oversized": false,
         "preview": {
             "previewed_at": "2022-01-27",
             "source": "Wizards of the Coast",
             "source_uri": "https://www.twitch.tv/videos/1277767538"
         },
         "prices": {
-            "eur": "48.97",
-            "eur_foil": "69.00",
+            "eur": "47.14",
+            "eur_foil": "72.49",
             "tix": null,
-            "usd": "42.43",
+            "usd": "35.95",
             "usd_etched": null,
-            "usd_foil": "73.67"
+            "usd_foil": "63.14"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Abf1341dd-41a3-49f6-87ec-63170dde4324&unique=prints",
         "produced_mana": [
             "G"
         ],
         "promo": false,
         "promo_types": [
@@ -4391,15 +4392,15 @@
         "cmc": 0.0,
         "collector_number": "501",
         "color_identity": [
             "G"
         ],
         "colors": [],
         "digital": false,
-        "edhrec_rank": 127,
+        "edhrec_rank": 106,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "frame_effects": [
@@ -4464,20 +4465,20 @@
         "oversized": false,
         "preview": {
             "previewed_at": "2022-01-28",
             "source": "Wizards of the Coast",
             "source_uri": "https://www.twitch.tv/videos/1277767538"
         },
         "prices": {
-            "eur": "41.65",
-            "eur_foil": "54.67",
+            "eur": "37.00",
+            "eur_foil": "59.62",
             "tix": null,
-            "usd": "40.90",
+            "usd": "29.77",
             "usd_etched": null,
-            "usd_foil": "45.41"
+            "usd_foil": "38.64"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Abf1341dd-41a3-49f6-87ec-63170dde4324&unique=prints",
         "produced_mana": [
             "G"
         ],
         "promo": false,
         "promo_types": [
@@ -4579,18 +4580,18 @@
         "name": "All in Good Time",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "402ba90d-6c41-49ee-ab50-7f0a466f66fe",
         "oracle_text": "When you set this scheme in motion, take an extra turn after this one. Schemes can't be set in motion that turn.",
         "oversized": true,
         "prices": {
-            "eur": "15.00",
+            "eur": "12.99",
             "eur_foil": null,
             "tix": null,
-            "usd": "18.08",
+            "usd": "20.67",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A402ba90d-6c41-49ee-ab50-7f0a466f66fe&unique=prints",
         "promo": false,
         "rarity": "common",
         "related_uris": {
@@ -4690,20 +4691,20 @@
         "name": "Wastes",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "05d24b0c-904a-46b6-b42a-96a4d91a0dd4",
         "oracle_text": "{T}: Add {C}.",
         "oversized": false,
         "prices": {
-            "eur": "0.28",
-            "eur_foil": "6.20",
-            "tix": "0.02",
-            "usd": "1.04",
+            "eur": "0.42",
+            "eur_foil": "3.97",
+            "tix": "0.03",
+            "usd": "0.92",
             "usd_etched": null,
-            "usd_foil": "7.66"
+            "usd_foil": "7.88"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A05d24b0c-904a-46b6-b42a-96a4d91a0dd4&unique=prints",
         "produced_mana": [
             "C"
         ],
         "promo": false,
         "rarity": "common",
@@ -4801,18 +4802,18 @@
         "name": "Wastes",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "05d24b0c-904a-46b6-b42a-96a4d91a0dd4",
         "oracle_text": "{T}: Add {C}.",
         "oversized": false,
         "prices": {
-            "eur": "1.24",
+            "eur": "2.74",
             "eur_foil": null,
             "tix": null,
-            "usd": "2.69",
+            "usd": "2.72",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A05d24b0c-904a-46b6-b42a-96a4d91a0dd4&unique=prints",
         "produced_mana": [
             "C"
         ],
@@ -4915,20 +4916,20 @@
         "name": "Wastes",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "05d24b0c-904a-46b6-b42a-96a4d91a0dd4",
         "oracle_text": "{T}: Add {C}.",
         "oversized": false,
         "prices": {
-            "eur": "0.26",
-            "eur_foil": "10.99",
+            "eur": "0.58",
+            "eur_foil": "7.50",
             "tix": "0.03",
-            "usd": "1.10",
+            "usd": "1.22",
             "usd_etched": null,
-            "usd_foil": "10.49"
+            "usd_foil": "11.49"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A05d24b0c-904a-46b6-b42a-96a4d91a0dd4&unique=prints",
         "produced_mana": [
             "C"
         ],
         "promo": false,
         "rarity": "common",
@@ -5026,18 +5027,18 @@
         "name": "Wastes",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "05d24b0c-904a-46b6-b42a-96a4d91a0dd4",
         "oracle_text": "{T}: Add {C}.",
         "oversized": false,
         "prices": {
-            "eur": "0.55",
+            "eur": "1.58",
             "eur_foil": null,
             "tix": null,
-            "usd": "1.28",
+            "usd": "1.36",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A05d24b0c-904a-46b6-b42a-96a4d91a0dd4&unique=prints",
         "produced_mana": [
             "C"
         ],
@@ -5134,21 +5135,21 @@
         "multiverse_ids": [
             198073
         ],
         "name": "Academy at Tolaria West",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "15b979de-c8ee-4664-9ca7-6c4eb3346967",
-        "oracle_text": "At the beginning of your end step, if you have no cards in hand, draw seven cards.\nWhenever you roll {CHAOS}, discard your hand.",
+        "oracle_text": "At the beginning of your end step, if you have no cards in hand, draw seven cards.\nWhenever chaos ensues, discard your hand.",
         "oversized": true,
         "prices": {
-            "eur": "1.46",
+            "eur": "1.50",
             "eur_foil": null,
             "tix": null,
-            "usd": "4.99",
+            "usd": "7.86",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A15b979de-c8ee-4664-9ca7-6c4eb3346967&unique=prints",
         "promo": false,
         "rarity": "common",
         "related_uris": {
@@ -5243,21 +5244,21 @@
         "multiverse_ids": [
             226512
         ],
         "name": "Akoum",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "25650a32-4014-4065-ad01-7357c3ad3995",
-        "oracle_text": "Players may cast enchantment spells as though they had flash.\nWhenever you roll {CHAOS}, destroy target creature that isn't enchanted.",
+        "oracle_text": "Players may cast enchantment spells as though they had flash.\nWhenever chaos ensues, destroy target creature that isn't enchanted.",
         "oversized": true,
         "prices": {
-            "eur": "1.04",
+            "eur": "0.98",
             "eur_foil": null,
-            "tix": "0.03",
-            "usd": "1.22",
+            "tix": "0.16",
+            "usd": "1.29",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A25650a32-4014-4065-ad01-7357c3ad3995&unique=prints",
         "promo": false,
         "rarity": "common",
         "related_uris": {
@@ -5354,18 +5355,18 @@
         "name": "Chaotic Aether",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "6dc67a65-31bf-4535-9e02-8f6d6ecefde5",
         "oracle_text": "When you encounter Chaotic Aether, each blank roll of the planar die is a {CHAOS} roll until a player planeswalks away from a plane. (Then planeswalk away from this phenomenon.)",
         "oversized": true,
         "prices": {
-            "eur": "1.02",
+            "eur": "0.50",
             "eur_foil": null,
             "tix": null,
-            "usd": "3.24",
+            "usd": "4.33",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A6dc67a65-31bf-4535-9e02-8f6d6ecefde5&unique=prints",
         "promo": false,
         "rarity": "common",
         "related_uris": {
@@ -5561,19 +5562,19 @@
                 "name": "Ib Halfheart, Goblin Tactician",
                 "object": "related_card",
                 "type_line": "Legendary Creature \u2014 Goblin Advisor",
                 "uri": "https://api.scryfall.com/cards/d09f9597-c2a9-4c1a-8375-ab06b1a21ee3"
             },
             {
                 "component": "combo_piece",
-                "id": "0b9c68ff-1fe4-42ef-8d1f-43120de5c1ff",
+                "id": "ae883514-2e5f-4ea3-bccc-3c475f70121a",
                 "name": "Krenko, Mob Boss",
                 "object": "related_card",
                 "type_line": "Legendary Creature \u2014 Goblin Warrior",
-                "uri": "https://api.scryfall.com/cards/0b9c68ff-1fe4-42ef-8d1f-43120de5c1ff"
+                "uri": "https://api.scryfall.com/cards/ae883514-2e5f-4ea3-bccc-3c475f70121a"
             },
             {
                 "component": "combo_piece",
                 "id": "623c1d1b-69a4-4bc4-b388-17a7600fd960",
                 "name": "Swarming Goblins",
                 "object": "related_card",
                 "type_line": "Creature \u2014 Goblin",
@@ -5609,35 +5610,35 @@
                 "name": "Mogg War Marshal",
                 "object": "related_card",
                 "type_line": "Creature \u2014 Goblin Warrior",
                 "uri": "https://api.scryfall.com/cards/fc027246-1dd3-4be0-bea6-3a7476a833ce"
             },
             {
                 "component": "combo_piece",
-                "id": "f32d7ce5-078b-40ff-8ecb-34309a0e3719",
+                "id": "b36a1bc7-a080-4fb6-b975-c59bb33a090a",
                 "name": "Goblin Instigator",
                 "object": "related_card",
                 "type_line": "Creature \u2014 Goblin Rogue",
-                "uri": "https://api.scryfall.com/cards/f32d7ce5-078b-40ff-8ecb-34309a0e3719"
+                "uri": "https://api.scryfall.com/cards/b36a1bc7-a080-4fb6-b975-c59bb33a090a"
             },
             {
                 "component": "combo_piece",
                 "id": "192d77ef-e8b5-44e2-842b-2c1f342c1e69",
                 "name": "Ponyback Brigade",
                 "object": "related_card",
                 "type_line": "Creature \u2014 Goblin Warrior",
                 "uri": "https://api.scryfall.com/cards/192d77ef-e8b5-44e2-842b-2c1f342c1e69"
             },
             {
                 "component": "combo_piece",
-                "id": "dc91f536-b3e5-48d2-a306-003e1bdfe8ba",
+                "id": "585fde63-4cb5-4235-8c95-2a7a511e7c3f",
                 "name": "Jund",
                 "object": "related_card",
                 "type_line": "Plane \u2014 Alara",
-                "uri": "https://api.scryfall.com/cards/dc91f536-b3e5-48d2-a306-003e1bdfe8ba"
+                "uri": "https://api.scryfall.com/cards/585fde63-4cb5-4235-8c95-2a7a511e7c3f"
             },
             {
                 "component": "combo_piece",
                 "id": "60b0a697-e901-42d9-9833-fedfcb6db9b3",
                 "name": "Goblin Rally",
                 "object": "related_card",
                 "type_line": "Sorcery",
@@ -5729,35 +5730,35 @@
                 "name": "Goblin Assault",
                 "object": "related_card",
                 "type_line": "Enchantment",
                 "uri": "https://api.scryfall.com/cards/26bccccc-f694-47a8-90fa-e3f1f62b9664"
             },
             {
                 "component": "combo_piece",
-                "id": "7cc10c19-6ea0-4491-b118-5c5cb9f7b036",
+                "id": "98b913e1-c26d-4a7d-9671-50d483304ba3",
                 "name": "Siege-Gang Commander",
                 "object": "related_card",
                 "type_line": "Creature \u2014 Goblin",
-                "uri": "https://api.scryfall.com/cards/7cc10c19-6ea0-4491-b118-5c5cb9f7b036"
+                "uri": "https://api.scryfall.com/cards/98b913e1-c26d-4a7d-9671-50d483304ba3"
             },
             {
                 "component": "combo_piece",
                 "id": "6d6adaa2-62ac-44f3-9665-8361135ccf6a",
                 "name": "Battle Cry Goblin",
                 "object": "related_card",
                 "type_line": "Creature \u2014 Goblin",
                 "uri": "https://api.scryfall.com/cards/6d6adaa2-62ac-44f3-9665-8361135ccf6a"
             },
             {
                 "component": "combo_piece",
-                "id": "a762a954-1166-4c6c-bf87-0f68a5a24f3e",
+                "id": "2f5689e2-d8a2-442b-8027-f89686adcb67",
                 "name": "Krenko, Tin Street Kingpin",
                 "object": "related_card",
                 "type_line": "Legendary Creature \u2014 Goblin",
-                "uri": "https://api.scryfall.com/cards/a762a954-1166-4c6c-bf87-0f68a5a24f3e"
+                "uri": "https://api.scryfall.com/cards/2f5689e2-d8a2-442b-8027-f89686adcb67"
             },
             {
                 "component": "combo_piece",
                 "id": "faec8ab3-80c6-4b8f-a60d-50cc683e66b4",
                 "name": "Hunted Phantasm",
                 "object": "related_card",
                 "type_line": "Creature \u2014 Spirit",
@@ -5893,15 +5894,15 @@
         "oracle_text": "",
         "oversized": false,
         "power": "1",
         "prices": {
             "eur": null,
             "eur_foil": null,
             "tix": null,
-            "usd": "24.43",
+            "usd": "23.44",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A4465eff4-5851-4721-a248-866c686c2ab8&unique=prints",
         "promo": true,
         "promo_types": [
             "playerrewards"
@@ -5946,15 +5947,15 @@
         "color_identity": [
             "W"
         ],
         "colors": [
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 16532,
+        "edhrec_rank": 16717,
         "finishes": [
             "nonfoil"
         ],
         "flavor_text": "When an order for griffin barding comes in, blacksmiths prepare their forges for months of exacting work. They know griffins always detect imperfections and never haggle.",
         "foil": false,
         "frame": "2003",
         "full_art": false,
@@ -6013,18 +6014,18 @@
         "nonfoil": true,
         "object": "card",
         "oracle_id": "ad3d6003-66d3-486d-aa54-ddce1adb5ff1",
         "oracle_text": "Flying, vigilance",
         "oversized": false,
         "power": "2",
         "prices": {
-            "eur": "0.15",
+            "eur": "0.10",
             "eur_foil": null,
             "tix": "0.05",
-            "usd": "0.22",
+            "usd": "0.18",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Aad3d6003-66d3-486d-aa54-ddce1adb5ff1&unique=prints",
         "promo": false,
         "rarity": "uncommon",
         "related_uris": {
@@ -6067,15 +6068,15 @@
         "color_identity": [
             "B"
         ],
         "colors": [
             "B"
         ],
         "digital": false,
-        "edhrec_rank": 1638,
+        "edhrec_rank": 1817,
         "finishes": [
             "foil"
         ],
         "foil": true,
         "frame": "2003",
         "full_art": true,
         "games": [
@@ -6123,22 +6124,22 @@
         "multiverse_ids": [],
         "name": "Black Sun's Zenith",
         "nonfoil": false,
         "object": "card",
         "oracle_id": "038c0165-32b6-4e81-8180-604b49905207",
         "oracle_text": "Put X -1/-1 counters on each creature. Shuffle Black Sun's Zenith into its owner's library.",
         "oversized": false,
-        "penny_rank": 1796,
+        "penny_rank": 1740,
         "prices": {
             "eur": null,
-            "eur_foil": "13.99",
+            "eur_foil": "12.00",
             "tix": null,
             "usd": null,
             "usd_etched": null,
-            "usd_foil": "28.73"
+            "usd_foil": "27.59"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A038c0165-32b6-4e81-8180-604b49905207&unique=prints",
         "promo": true,
         "promo_types": [
             "gameday"
         ],
         "rarity": "rare",
@@ -6231,21 +6232,21 @@
         "multiverse_ids": [
             198069
         ],
         "name": "Tazeem",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "97f708de-9271-4137-a9fe-dda25b922900",
-        "oracle_text": "Creatures can't block.\nWhenever you roll {CHAOS}, draw a card for each land you control.",
+        "oracle_text": "Creatures can't block.\nWhenever chaos ensues, draw a card for each land you control.",
         "oversized": true,
         "prices": {
-            "eur": "15.00",
+            "eur": "12.50",
             "eur_foil": null,
             "tix": null,
-            "usd": "8.47",
+            "usd": "9.62",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A97f708de-9271-4137-a9fe-dda25b922900&unique=prints",
         "promo": true,
         "rarity": "rare",
         "related_uris": {
@@ -6287,15 +6288,15 @@
         "color_identity": [
             "W"
         ],
         "colors": [
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 10559,
+        "edhrec_rank": 11161,
         "finishes": [
             "foil"
         ],
         "flavor_text": "\"Dragons seek war. I bring it to them.\"",
         "foil": true,
         "frame": "2015",
         "full_art": false,
@@ -6346,23 +6347,23 @@
         "multiverse_ids": [],
         "name": "Dragonscale General",
         "nonfoil": false,
         "object": "card",
         "oracle_id": "9fc6e1db-cf09-4b8c-be4f-bb02ffe7a188",
         "oracle_text": "At the beginning of your end step, bolster X, where X is the number of tapped creatures you control. (Choose a creature with the least toughness among creatures you control and put X +1/+1 counters on it.)",
         "oversized": false,
-        "penny_rank": 5110,
+        "penny_rank": 5183,
         "power": "2",
         "prices": {
             "eur": null,
-            "eur_foil": "0.29",
+            "eur_foil": "0.95",
             "tix": null,
             "usd": null,
             "usd_etched": null,
-            "usd_foil": "0.61"
+            "usd_foil": "0.59"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A9fc6e1db-cf09-4b8c-be4f-bb02ffe7a188&unique=prints",
         "promo": true,
         "promo_types": [
             "setpromo",
             "intropack"
         ],
@@ -6408,15 +6409,15 @@
         "color_identity": [
             "W"
         ],
         "colors": [
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 10559,
+        "edhrec_rank": 11161,
         "finishes": [
             "foil"
         ],
         "flavor_text": "\"Dragons seek war. I bring it to them.\"",
         "foil": true,
         "frame": "2015",
         "full_art": false,
@@ -6467,23 +6468,23 @@
         "multiverse_ids": [],
         "name": "Dragonscale General",
         "nonfoil": false,
         "object": "card",
         "oracle_id": "9fc6e1db-cf09-4b8c-be4f-bb02ffe7a188",
         "oracle_text": "At the beginning of your end step, bolster X, where X is the number of tapped creatures you control. (Choose a creature with the least toughness among creatures you control and put X +1/+1 counters on it.)",
         "oversized": false,
-        "penny_rank": 5110,
+        "penny_rank": 5183,
         "power": "2",
         "prices": {
             "eur": null,
-            "eur_foil": "0.95",
+            "eur_foil": "1.20",
             "tix": null,
             "usd": null,
             "usd_etched": null,
-            "usd_foil": "0.44"
+            "usd_foil": "0.42"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A9fc6e1db-cf09-4b8c-be4f-bb02ffe7a188&unique=prints",
         "promo": true,
         "promo_types": [
             "setpromo",
             "prerelease",
             "datestamped"
@@ -6582,21 +6583,21 @@
         "multiverse_ids": [
             226521
         ],
         "name": "Stairs to Infinity",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "7a425df4-7010-462e-9cb5-20389bac721c",
-        "oracle_text": "Players have no maximum hand size.\nWhenever you roll the planar die, draw a card.\nWhenever you roll {CHAOS}, reveal the top card of your planar deck. You may put it on the bottom of your planar deck.",
+        "oracle_text": "Players have no maximum hand size.\nWhenever you roll the planar die, draw a card.\nWhenever chaos ensues, reveal the top card of your planar deck. You may put it on the bottom of your planar deck.",
         "oversized": true,
         "prices": {
-            "eur": "1.99",
+            "eur": "1.11",
             "eur_foil": null,
             "tix": null,
-            "usd": "3.70",
+            "usd": "5.20",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A7a425df4-7010-462e-9cb5-20389bac721c&unique=prints",
         "promo": true,
         "promo_types": [
             "instore"
@@ -6637,15 +6638,15 @@
         "card_back_id": "0aeebaf5-8c7d-4636-9e82-8c27447861f7",
         "cardmarket_id": 15173,
         "cmc": 0.0,
         "collector_number": "1",
         "color_identity": [],
         "colors": [],
         "digital": false,
-        "edhrec_rank": 8334,
+        "edhrec_rank": 8271,
         "finishes": [
             "nonfoil"
         ],
         "foil": false,
         "frame": "1993",
         "full_art": false,
         "games": [
@@ -6697,20 +6698,20 @@
         ],
         "name": "Arena",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "12326d23-1fb5-4084-a23a-d6e2c90ea36c",
         "oracle_text": "{3}, {T}: Tap target creature you control and target creature of an opponent's choice they control. Those creatures fight each other. (Each deals damage equal to its power to the other.)",
         "oversized": false,
-        "penny_rank": 5125,
+        "penny_rank": 5240,
         "prices": {
-            "eur": "5.00",
+            "eur": "4.99",
             "eur_foil": null,
             "tix": null,
-            "usd": "8.48",
+            "usd": "7.83",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A12326d23-1fb5-4084-a23a-d6e2c90ea36c&unique=prints",
         "promo": true,
         "promo_types": [
             "mediainsert"
@@ -6777,15 +6778,15 @@
         "color_identity": [
             "R"
         ],
         "colors": [
             "R"
         ],
         "digital": false,
-        "edhrec_rank": 8392,
+        "edhrec_rank": 8767,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2003",
         "full_art": false,
@@ -6837,22 +6838,22 @@
             126218
         ],
         "name": "Boom // Bust",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "514fdac0-95f4-4034-b891-283fe0fb6da6",
         "oversized": false,
-        "penny_rank": 786,
+        "penny_rank": 233,
         "prices": {
-            "eur": "0.20",
-            "eur_foil": "2.45",
-            "tix": "0.16",
-            "usd": "1.64",
+            "eur": "0.30",
+            "eur_foil": "2.00",
+            "tix": "0.03",
+            "usd": "2.13",
             "usd_etched": null,
-            "usd_foil": "13.05"
+            "usd_foil": "16.54"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A514fdac0-95f4-4034-b891-283fe0fb6da6&unique=prints",
         "promo": false,
         "rarity": "rare",
         "related_uris": {
             "edhrec": "https://edhrec.com/route/?cc=Boom+%2F%2F+Bust",
             "gatherer": "https://gatherer.wizards.com/Pages/Card/Details.aspx?multiverseid=126218",
@@ -6896,15 +6897,15 @@
         ],
         "colors": [
             "B",
             "U",
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 11400,
+        "edhrec_rank": 11936,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "flavor_text": "Altered by Phyrexian science, corrupted by black mana, and twisted by rage, Ertai still looked in the mirror and saw only glory.",
         "foil": true,
         "frame": "1997",
@@ -6959,21 +6960,21 @@
         ],
         "name": "Ertai, the Corrupted",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "36934bd0-b275-4222-926c-b5a74cf0967d",
         "oracle_text": "{U}, {T}, Sacrifice a creature or enchantment: Counter target spell.",
         "oversized": false,
-        "penny_rank": 11108,
+        "penny_rank": 11443,
         "power": "3",
         "prices": {
-            "eur": "1.28",
-            "eur_foil": "45.97",
-            "tix": "0.14",
-            "usd": "3.92",
+            "eur": "1.30",
+            "eur_foil": "89.99",
+            "tix": "0.07",
+            "usd": "2.58",
             "usd_etched": null,
             "usd_foil": "106.39"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A36934bd0-b275-4222-926c-b5a74cf0967d&unique=prints",
         "promo": false,
         "rarity": "rare",
         "related_uris": {
@@ -7020,15 +7021,15 @@
         ],
         "colors": [
             "B",
             "U",
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 11400,
+        "edhrec_rank": 11936,
         "finishes": [
             "foil"
         ],
         "flavor_text": "Altered by Phyrexian science, corrupted by black mana, and twisted by rage, Ertai still looked in the mirror and saw only glory.",
         "foil": true,
         "frame": "1997",
         "full_art": false,
@@ -7080,19 +7081,19 @@
         ],
         "name": "Ertai, the Corrupted",
         "nonfoil": false,
         "object": "card",
         "oracle_id": "36934bd0-b275-4222-926c-b5a74cf0967d",
         "oracle_text": "{U}, {T}, Sacrifice a creature or enchantment: Counter target spell.",
         "oversized": false,
-        "penny_rank": 11108,
+        "penny_rank": 11443,
         "power": "3",
         "prices": {
             "eur": null,
-            "eur_foil": "434.99",
+            "eur_foil": "269.00",
             "tix": null,
             "usd": null,
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A36934bd0-b275-4222-926c-b5a74cf0967d&unique=prints",
         "promo": false,
@@ -7155,15 +7156,15 @@
         "color_identity": [
             "W"
         ],
         "colors": [
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 2268,
+        "edhrec_rank": 1891,
         "finishes": [
             "foil"
         ],
         "foil": true,
         "frame": "2003",
         "full_art": false,
         "games": [
@@ -7198,37 +7199,38 @@
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "legal",
             "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
-            "penny": "not_legal",
+            "penny": "legal",
             "pioneer": "not_legal",
             "predh": "legal",
             "premodern": "not_legal",
             "standard": "not_legal",
             "vintage": "legal"
         },
         "mana_cost": "{2}{W}{W}",
         "multiverse_ids": [],
         "name": "Hero of Bladehold",
         "nonfoil": false,
         "object": "card",
         "oracle_id": "454a8902-8120-4373-96ee-bbf352b04e8d",
         "oracle_text": "Battle cry (Whenever this creature attacks, each other attacking creature gets +1/+0 until end of turn.)\nWhenever Hero of Bladehold attacks, create two 1/1 white Soldier creature tokens that are tapped and attacking.",
         "oversized": false,
+        "penny_rank": 2167,
         "power": "3",
         "prices": {
             "eur": null,
-            "eur_foil": "5.12",
+            "eur_foil": "1.49",
             "tix": null,
             "usd": null,
             "usd_etched": null,
-            "usd_foil": "16.62"
+            "usd_foil": "6.62"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A454a8902-8120-4373-96ee-bbf352b04e8d&unique=prints",
         "promo": true,
         "promo_types": [
             "setpromo",
             "datestamped",
             "prerelease"
@@ -7272,15 +7274,15 @@
         "cmc": 0.0,
         "collector_number": "266p",
         "color_identity": [
             "G"
         ],
         "colors": [],
         "digital": false,
-        "edhrec_rank": 127,
+        "edhrec_rank": 106,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "frame_effects": [
@@ -7335,20 +7337,20 @@
         "name": "Boseiju, Who Endures",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "bf1341dd-41a3-49f6-87ec-63170dde4324",
         "oracle_text": "{T}: Add {G}.\nChannel \u2014 {1}{G}, Discard Boseiju, Who Endures: Destroy target artifact, enchantment, or nonbasic land an opponent controls. That player may search their library for a land card with a basic land type, put it onto the battlefield, then shuffle. This ability costs {1} less to activate for each legendary creature you control.",
         "oversized": false,
         "prices": {
-            "eur": "31.67",
-            "eur_foil": "40.00",
+            "eur": "33.53",
+            "eur_foil": "35.50",
             "tix": null,
-            "usd": "34.25",
+            "usd": "29.38",
             "usd_etched": null,
-            "usd_foil": "32.17"
+            "usd_foil": "32.49"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Abf1341dd-41a3-49f6-87ec-63170dde4324&unique=prints",
         "produced_mana": [
             "G"
         ],
         "promo": true,
         "promo_types": [
@@ -7393,15 +7395,15 @@
         "cmc": 0.0,
         "collector_number": "266s",
         "color_identity": [
             "G"
         ],
         "colors": [],
         "digital": false,
-        "edhrec_rank": 127,
+        "edhrec_rank": 106,
         "finishes": [
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "frame_effects": [
             "legendary"
@@ -7456,19 +7458,19 @@
         "nonfoil": false,
         "object": "card",
         "oracle_id": "bf1341dd-41a3-49f6-87ec-63170dde4324",
         "oracle_text": "{T}: Add {G}.\nChannel \u2014 {1}{G}, Discard Boseiju, Who Endures: Destroy target artifact, enchantment, or nonbasic land an opponent controls. That player may search their library for a land card with a basic land type, put it onto the battlefield, then shuffle. This ability costs {1} less to activate for each legendary creature you control.",
         "oversized": false,
         "prices": {
             "eur": null,
-            "eur_foil": "40.00",
+            "eur_foil": "42.49",
             "tix": null,
             "usd": null,
             "usd_etched": null,
-            "usd_foil": "33.84"
+            "usd_foil": "41.55"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Abf1341dd-41a3-49f6-87ec-63170dde4324&unique=prints",
         "produced_mana": [
             "G"
         ],
         "promo": true,
         "promo_types": [
@@ -7533,15 +7535,15 @@
         "color_identity": [
             "W"
         ],
         "colors": [
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 3910,
+        "edhrec_rank": 4148,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "full_art": false,
@@ -7592,23 +7594,23 @@
         "multiverse_ids": [],
         "name": "Tithe Taker",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "c916b81f-700e-4a1a-8c8e-c4685ceaecd2",
         "oracle_text": "During your turn, spells your opponents cast cost {1} more to cast and abilities your opponents activate cost {1} more to activate unless they're mana abilities.\nAfterlife 1 (When this creature dies, create a 1/1 white and black Spirit creature token with flying.)",
         "oversized": false,
-        "penny_rank": 1661,
+        "penny_rank": 1714,
         "power": "2",
         "prices": {
-            "eur": "0.50",
-            "eur_foil": "1.25",
+            "eur": "0.77",
+            "eur_foil": "0.75",
             "tix": null,
-            "usd": "0.79",
+            "usd": "1.16",
             "usd_etched": null,
-            "usd_foil": "1.43"
+            "usd_foil": "2.62"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ac916b81f-700e-4a1a-8c8e-c4685ceaecd2&unique=prints",
         "promo": true,
         "promo_types": [
             "setpromo",
             "promopack",
             "stamped"
@@ -7673,15 +7675,15 @@
         "color_identity": [
             "W"
         ],
         "colors": [
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 3910,
+        "edhrec_rank": 4148,
         "finishes": [
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "full_art": false,
         "games": [
@@ -7731,23 +7733,23 @@
         "multiverse_ids": [],
         "name": "Tithe Taker",
         "nonfoil": false,
         "object": "card",
         "oracle_id": "c916b81f-700e-4a1a-8c8e-c4685ceaecd2",
         "oracle_text": "During your turn, spells your opponents cast cost {1} more to cast and abilities your opponents activate cost {1} more to activate unless they're mana abilities.\nAfterlife 1 (When this creature dies, create a 1/1 white and black Spirit creature token with flying.)",
         "oversized": false,
-        "penny_rank": 1661,
+        "penny_rank": 1714,
         "power": "2",
         "prices": {
             "eur": null,
-            "eur_foil": "1.40",
+            "eur_foil": "1.39",
             "tix": null,
             "usd": null,
             "usd_etched": null,
-            "usd_foil": "1.72"
+            "usd_foil": "1.66"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ac916b81f-700e-4a1a-8c8e-c4685ceaecd2&unique=prints",
         "promo": true,
         "promo_types": [
             "setpromo",
             "prerelease",
             "datestamped"
@@ -7854,19 +7856,19 @@
         "preview": {
             "previewed_at": "2018-12-17",
             "source": "Wizards of the Coast",
             "source_uri": "https://magic.wizards.com/en/articles/archive/card-preview/ravnica-allegiance-promos-and-packaging-2018-12-17"
         },
         "prices": {
             "eur": null,
-            "eur_foil": "1.85",
+            "eur_foil": "2.52",
             "tix": null,
             "usd": null,
             "usd_etched": null,
-            "usd_foil": "2.50"
+            "usd_foil": "2.42"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Abc71ebf6-2056-41f7-be35-b2e5c34afa99&unique=prints",
         "produced_mana": [
             "W"
         ],
         "promo": true,
         "rarity": "common",
@@ -7969,19 +7971,19 @@
         "preview": {
             "previewed_at": "2018-12-17",
             "source": "Wizards of the Coast",
             "source_uri": "https://magic.wizards.com/en/articles/archive/feature/magic-gathering-chandra-preview-2018-12-05"
         },
         "prices": {
             "eur": null,
-            "eur_foil": "1.58",
+            "eur_foil": "3.00",
             "tix": null,
             "usd": null,
             "usd_etched": null,
-            "usd_foil": "3.44"
+            "usd_foil": "3.58"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Abc71ebf6-2056-41f7-be35-b2e5c34afa99&unique=prints",
         "produced_mana": [
             "W"
         ],
         "promo": true,
         "rarity": "common",
@@ -8127,19 +8129,19 @@
         "name": "Nightmare Moon // Princess Luna",
         "nonfoil": false,
         "object": "card",
         "oracle_id": "e724bddb-6195-4943-b9c6-decc96717998",
         "oversized": false,
         "prices": {
             "eur": null,
-            "eur_foil": "62.90",
+            "eur_foil": "69.99",
             "tix": null,
             "usd": null,
             "usd_etched": null,
-            "usd_foil": "67.32"
+            "usd_foil": "61.72"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ae724bddb-6195-4943-b9c6-decc96717998&unique=prints",
         "promo": true,
         "rarity": "mythic",
         "related_uris": {
             "edhrec": "https://edhrec.com/route/?cc=Nightmare+Moon",
             "tcgplayer_infinite_articles": "https://infinite.tcgplayer.com/search?contentMode=article&game=magic&partner=scryfall&q=Nightmare+Moon+%2F%2F+Princess+Luna&utm_campaign=affiliate&utm_medium=api&utm_source=scryfall",
@@ -8179,15 +8181,15 @@
         "color_identity": [
             "G"
         ],
         "colors": [
             "G"
         ],
         "digital": false,
-        "edhrec_rank": 105,
+        "edhrec_rank": 108,
         "finishes": [
             "nonfoil"
         ],
         "foil": false,
         "frame": "1993",
         "full_art": false,
         "games": [
@@ -8235,20 +8237,20 @@
         "multiverse_ids": [],
         "name": "Sylvan Library",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "92eed395-62ca-4293-882b-8565c40daab5",
         "oracle_text": "At the beginning of your draw step, you may draw two additional cards. If you do, choose two cards in your hand drawn this turn. For each of those cards, pay 4 life or put the card on top of your library.",
         "oversized": false,
-        "penny_rank": 80,
+        "penny_rank": 82,
         "prices": {
-            "eur": "22.90",
+            "eur": "15.00",
             "eur_foil": null,
             "tix": null,
-            "usd": "140.40",
+            "usd": null,
             "usd_etched": null,
             "usd_foil": null
         },
         "printed_name": "Biblioth\u00e8que sylvestre",
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A92eed395-62ca-4293-882b-8565c40daab5&unique=prints",
         "promo": false,
         "rarity": "uncommon",
@@ -8309,15 +8311,15 @@
         "color_identity": [
             "W"
         ],
         "colors": [
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 3910,
+        "edhrec_rank": 4148,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "full_art": false,
@@ -8373,28 +8375,28 @@
         ],
         "name": "Tithe Taker",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "c916b81f-700e-4a1a-8c8e-c4685ceaecd2",
         "oracle_text": "During your turn, spells your opponents cast cost {1} more to cast and abilities your opponents activate cost {1} more to activate unless they're mana abilities.\nAfterlife 1 (When this creature dies, create a 1/1 white and black Spirit creature token with flying.)",
         "oversized": false,
-        "penny_rank": 1661,
+        "penny_rank": 1714,
         "power": "2",
         "preview": {
             "previewed_at": "2018-12-17",
             "source": "Wizards of the Coast",
             "source_uri": "https://magic.wizards.com/en/articles/archive/feature/ravnica-allegiance-mechanics-2018-12-17"
         },
         "prices": {
-            "eur": "0.42",
-            "eur_foil": "1.00",
+            "eur": "0.31",
+            "eur_foil": "3.00",
             "tix": "0.02",
-            "usd": "0.70",
+            "usd": "0.76",
             "usd_etched": null,
-            "usd_foil": "1.77"
+            "usd_foil": "1.80"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ac916b81f-700e-4a1a-8c8e-c4685ceaecd2&unique=prints",
         "promo": false,
         "rarity": "rare",
         "related_uris": {
             "edhrec": "https://edhrec.com/route/?cc=Tithe+Taker",
             "gatherer": "https://gatherer.wizards.com/Pages/Card/Details.aspx?multiverseid=457171",
@@ -8437,15 +8439,15 @@
         "color_identity": [
             "G"
         ],
         "colors": [
             "G"
         ],
         "digital": false,
-        "edhrec_rank": 14847,
+        "edhrec_rank": 15569,
         "finishes": [
             "foil"
         ],
         "foil": true,
         "frame": "1997",
         "full_art": false,
         "games": [
@@ -8493,23 +8495,23 @@
         "multiverse_ids": [],
         "name": "Rhox",
         "nonfoil": false,
         "object": "card",
         "oracle_id": "f6f4c684-2915-4a58-9c4b-487387f7cf73",
         "oracle_text": "You may have Rhox assign its combat damage as though it weren't blocked.\n{2}{G}: Regenerate Rhox. (The next time this creature would be destroyed this turn, it isn't. Instead tap it, remove all damage from it, and remove it from combat.)",
         "oversized": false,
-        "penny_rank": 10455,
+        "penny_rank": 10699,
         "power": "5",
         "prices": {
             "eur": null,
-            "eur_foil": "1.19",
+            "eur_foil": "0.51",
             "tix": null,
             "usd": null,
             "usd_etched": null,
-            "usd_foil": "0.74"
+            "usd_foil": "0.81"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Af6f4c684-2915-4a58-9c4b-487387f7cf73&unique=prints",
         "promo": true,
         "rarity": "rare",
         "related_uris": {
             "edhrec": "https://edhrec.com/route/?cc=Rhox",
             "tcgplayer_infinite_articles": "https://infinite.tcgplayer.com/search?contentMode=article&game=magic&partner=scryfall&q=Rhox&utm_campaign=affiliate&utm_medium=api&utm_source=scryfall",
@@ -8591,15 +8593,15 @@
                 "oracle_text": "{3}, {T}: Double the amount of each type of unspent mana you have.",
                 "type_line": "Artifact"
             }
         ],
         "collector_number": "1080",
         "color_identity": [],
         "digital": false,
-        "edhrec_rank": 3149,
+        "edhrec_rank": 2933,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "full_art": false,
@@ -8636,22 +8638,22 @@
             "vintage": "legal"
         },
         "multiverse_ids": [],
         "name": "Doubling Cube // Doubling Cube",
         "nonfoil": true,
         "object": "card",
         "oversized": false,
-        "penny_rank": 11549,
+        "penny_rank": 11717,
         "prices": {
             "eur": null,
             "eur_foil": null,
             "tix": null,
-            "usd": "7.13",
+            "usd": "8.73",
             "usd_etched": null,
-            "usd_foil": "7.37"
+            "usd_foil": "9.25"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A9afd8f12-0796-4500-aaa3-10b4a46ef6ec&unique=prints",
         "promo": false,
         "rarity": "rare",
         "related_uris": {
             "edhrec": "https://edhrec.com/route/?cc=Doubling+Cube+%2F%2F+Doubling+Cube",
             "tcgplayer_infinite_articles": "https://infinite.tcgplayer.com/search?contentMode=article&game=magic&partner=scryfall&q=Doubling+Cube+%2F%2F+Doubling+Cube&utm_campaign=affiliate&utm_medium=api&utm_source=scryfall",
@@ -8844,19 +8846,19 @@
                 "name": "Ib Halfheart, Goblin Tactician",
                 "object": "related_card",
                 "type_line": "Legendary Creature \u2014 Goblin Advisor",
                 "uri": "https://api.scryfall.com/cards/d09f9597-c2a9-4c1a-8375-ab06b1a21ee3"
             },
             {
                 "component": "combo_piece",
-                "id": "0b9c68ff-1fe4-42ef-8d1f-43120de5c1ff",
+                "id": "ae883514-2e5f-4ea3-bccc-3c475f70121a",
                 "name": "Krenko, Mob Boss",
                 "object": "related_card",
                 "type_line": "Legendary Creature \u2014 Goblin Warrior",
-                "uri": "https://api.scryfall.com/cards/0b9c68ff-1fe4-42ef-8d1f-43120de5c1ff"
+                "uri": "https://api.scryfall.com/cards/ae883514-2e5f-4ea3-bccc-3c475f70121a"
             },
             {
                 "component": "combo_piece",
                 "id": "623c1d1b-69a4-4bc4-b388-17a7600fd960",
                 "name": "Swarming Goblins",
                 "object": "related_card",
                 "type_line": "Creature \u2014 Goblin",
@@ -8892,35 +8894,35 @@
                 "name": "Mogg War Marshal",
                 "object": "related_card",
                 "type_line": "Creature \u2014 Goblin Warrior",
                 "uri": "https://api.scryfall.com/cards/fc027246-1dd3-4be0-bea6-3a7476a833ce"
             },
             {
                 "component": "combo_piece",
-                "id": "f32d7ce5-078b-40ff-8ecb-34309a0e3719",
+                "id": "b36a1bc7-a080-4fb6-b975-c59bb33a090a",
                 "name": "Goblin Instigator",
                 "object": "related_card",
                 "type_line": "Creature \u2014 Goblin Rogue",
-                "uri": "https://api.scryfall.com/cards/f32d7ce5-078b-40ff-8ecb-34309a0e3719"
+                "uri": "https://api.scryfall.com/cards/b36a1bc7-a080-4fb6-b975-c59bb33a090a"
             },
             {
                 "component": "combo_piece",
                 "id": "192d77ef-e8b5-44e2-842b-2c1f342c1e69",
                 "name": "Ponyback Brigade",
                 "object": "related_card",
                 "type_line": "Creature \u2014 Goblin Warrior",
                 "uri": "https://api.scryfall.com/cards/192d77ef-e8b5-44e2-842b-2c1f342c1e69"
             },
             {
                 "component": "combo_piece",
-                "id": "dc91f536-b3e5-48d2-a306-003e1bdfe8ba",
+                "id": "585fde63-4cb5-4235-8c95-2a7a511e7c3f",
                 "name": "Jund",
                 "object": "related_card",
                 "type_line": "Plane \u2014 Alara",
-                "uri": "https://api.scryfall.com/cards/dc91f536-b3e5-48d2-a306-003e1bdfe8ba"
+                "uri": "https://api.scryfall.com/cards/585fde63-4cb5-4235-8c95-2a7a511e7c3f"
             },
             {
                 "component": "combo_piece",
                 "id": "60b0a697-e901-42d9-9833-fedfcb6db9b3",
                 "name": "Goblin Rally",
                 "object": "related_card",
                 "type_line": "Sorcery",
@@ -9012,19 +9014,19 @@
                 "name": "Goblin Assault",
                 "object": "related_card",
                 "type_line": "Enchantment",
                 "uri": "https://api.scryfall.com/cards/26bccccc-f694-47a8-90fa-e3f1f62b9664"
             },
             {
                 "component": "combo_piece",
-                "id": "7cc10c19-6ea0-4491-b118-5c5cb9f7b036",
+                "id": "98b913e1-c26d-4a7d-9671-50d483304ba3",
                 "name": "Siege-Gang Commander",
                 "object": "related_card",
                 "type_line": "Creature \u2014 Goblin",
-                "uri": "https://api.scryfall.com/cards/7cc10c19-6ea0-4491-b118-5c5cb9f7b036"
+                "uri": "https://api.scryfall.com/cards/98b913e1-c26d-4a7d-9671-50d483304ba3"
             },
             {
                 "component": "combo_piece",
                 "id": "6d6adaa2-62ac-44f3-9665-8361135ccf6a",
                 "name": "Battle Cry Goblin",
                 "object": "related_card",
                 "type_line": "Creature \u2014 Goblin",
@@ -9122,29 +9124,29 @@
         "digital": false,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2015",
-        "full_art": false,
+        "full_art": true,
         "games": [
             "paper"
         ],
         "highres_image": true,
         "id": "d99cc0a4-4868-47f3-bd1d-f46b7cb74650",
         "illustration_id": "eec6e117-98ee-45d6-ac28-4af60ab90eb5",
         "image_status": "highres_scan",
         "image_uris": {
-            "art_crop": "https://cards.scryfall.io/art_crop/front/d/9/d99cc0a4-4868-47f3-bd1d-f46b7cb74650.jpg?1622938201",
-            "border_crop": "https://cards.scryfall.io/border_crop/front/d/9/d99cc0a4-4868-47f3-bd1d-f46b7cb74650.jpg?1622938201",
-            "large": "https://cards.scryfall.io/large/front/d/9/d99cc0a4-4868-47f3-bd1d-f46b7cb74650.jpg?1622938201",
-            "normal": "https://cards.scryfall.io/normal/front/d/9/d99cc0a4-4868-47f3-bd1d-f46b7cb74650.jpg?1622938201",
-            "png": "https://cards.scryfall.io/png/front/d/9/d99cc0a4-4868-47f3-bd1d-f46b7cb74650.png?1622938201",
-            "small": "https://cards.scryfall.io/small/front/d/9/d99cc0a4-4868-47f3-bd1d-f46b7cb74650.jpg?1622938201"
+            "art_crop": "https://cards.scryfall.io/art_crop/front/d/9/d99cc0a4-4868-47f3-bd1d-f46b7cb74650.jpg?1681768986",
+            "border_crop": "https://cards.scryfall.io/border_crop/front/d/9/d99cc0a4-4868-47f3-bd1d-f46b7cb74650.jpg?1681768986",
+            "large": "https://cards.scryfall.io/large/front/d/9/d99cc0a4-4868-47f3-bd1d-f46b7cb74650.jpg?1681768986",
+            "normal": "https://cards.scryfall.io/normal/front/d/9/d99cc0a4-4868-47f3-bd1d-f46b7cb74650.jpg?1681768986",
+            "png": "https://cards.scryfall.io/png/front/d/9/d99cc0a4-4868-47f3-bd1d-f46b7cb74650.png?1681768986",
+            "small": "https://cards.scryfall.io/small/front/d/9/d99cc0a4-4868-47f3-bd1d-f46b7cb74650.jpg?1681768986"
         },
         "keywords": [],
         "lang": "en",
         "layout": "token",
         "legalities": {
             "alchemy": "not_legal",
             "brawl": "not_legal",
@@ -9176,20 +9178,20 @@
         "nonfoil": true,
         "object": "card",
         "oracle_id": "4465eff4-5851-4721-a248-866c686c2ab8",
         "oracle_text": "",
         "oversized": false,
         "power": "1",
         "prices": {
-            "eur": "0.75",
-            "eur_foil": "1.50",
+            "eur": "0.74",
+            "eur_foil": "1.25",
             "tix": null,
-            "usd": "1.72",
+            "usd": "1.44",
             "usd_etched": null,
-            "usd_foil": "1.75"
+            "usd_foil": "1.52"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A4465eff4-5851-4721-a248-866c686c2ab8&unique=prints",
         "promo": false,
         "rarity": "common",
         "related_uris": {
             "edhrec": "https://edhrec.com/route/?cc=Goblin",
             "gatherer": "https://gatherer.wizards.com/Pages/Card/Details.aspx?multiverseid=509365",
@@ -9229,15 +9231,15 @@
         "color_identity": [
             "B"
         ],
         "colors": [
             "B"
         ],
         "digital": false,
-        "edhrec_rank": 139,
+        "edhrec_rank": 147,
         "finishes": [
             "foil"
         ],
         "flavor_text": "In matters of life and death, he trusts his gut.",
         "foil": true,
         "frame": "2003",
         "full_art": false,
@@ -9288,33 +9290,36 @@
         "multiverse_ids": [],
         "name": "Viscera Seer",
         "nonfoil": false,
         "object": "card",
         "oracle_id": "f82a4e85-526d-4456-b700-7760043a31be",
         "oracle_text": "Sacrifice a creature: Scry 1. (Look at the top card of your library. You may put that card on the bottom of your library.)",
         "oversized": false,
-        "penny_rank": 758,
+        "penny_rank": 786,
         "power": "1",
         "prices": {
             "eur": null,
             "eur_foil": null,
             "tix": null,
             "usd": null,
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Af82a4e85-526d-4456-b700-7760043a31be&unique=prints",
         "promo": false,
+        "promo_types": [
+            "serialized"
+        ],
         "rarity": "common",
         "related_uris": {
             "edhrec": "https://edhrec.com/route/?cc=Viscera+Seer",
             "tcgplayer_infinite_articles": "https://infinite.tcgplayer.com/search?contentMode=article&game=magic&partner=scryfall&q=Viscera+Seer&utm_campaign=affiliate&utm_medium=api&utm_source=scryfall",
             "tcgplayer_infinite_decks": "https://infinite.tcgplayer.com/search?contentMode=deck&game=magic&partner=scryfall&q=Viscera+Seer&utm_campaign=affiliate&utm_medium=api&utm_source=scryfall"
         },
-        "released_at": "2021-11-08",
+        "released_at": "2021-06-21",
         "reprint": true,
         "reserved": false,
         "rulings_uri": "https://api.scryfall.com/cards/dba1cf83-e13d-401e-b76f-b12a51b307f9/rulings",
         "scryfall_set_uri": "https://scryfall.com/sets/sld?utm_source=api",
         "scryfall_uri": "https://scryfall.com/card/sld/VS/viscera-seer?utm_source=api",
         "set": "sld",
         "set_id": "4d92a8a7-ccb0-437d-abdc-9d70fc5ed672",
@@ -9430,21 +9435,21 @@
             87599
         ],
         "name": "Erayo, Soratami Ascendant // Erayo's Essence",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "d83bb32d-f409-421a-9d93-bd7ea3240b47",
         "oversized": false,
-        "penny_rank": 2357,
+        "penny_rank": 2531,
         "power": "1",
         "prices": {
-            "eur": "3.99",
-            "eur_foil": "25.00",
+            "eur": "1.90",
+            "eur_foil": "19.99",
             "tix": "0.02",
-            "usd": "5.76",
+            "usd": "5.47",
             "usd_etched": null,
             "usd_foil": "40.28"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ad83bb32d-f409-421a-9d93-bd7ea3240b47&unique=prints",
         "promo": false,
         "rarity": "rare",
         "related_uris": {
@@ -9542,18 +9547,18 @@
         "name": "Happy Dead Squirrel",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "c3e5d355-fbfb-4489-aeea-8b0ea5de6fcd",
         "oracle_text": "{TK}{TK} \u2014 {T}: Add {C}{C}. Spend this mana only to cast noncreature spells.\n{TK}{TK}{TK} \u2014 Infect (This permanent deals damage to creatures in the form of -1/-1 counters and to players in the form of poison counters.)\n{TK}{TK} \u2014 3/2\n{TK}{TK}{TK}{TK} \u2014 4/7",
         "oversized": false,
         "prices": {
-            "eur": "0.19",
+            "eur": "0.18",
             "eur_foil": null,
             "tix": null,
-            "usd": "0.21",
+            "usd": "0.22",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ac3e5d355-fbfb-4489-aeea-8b0ea5de6fcd&unique=prints",
         "produced_mana": [
             "C"
         ],
@@ -9601,15 +9606,15 @@
             "R"
         ],
         "colors": [
             "G",
             "R"
         ],
         "digital": false,
-        "edhrec_rank": 3035,
+        "edhrec_rank": 3345,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "frame_effects": [
@@ -9676,20 +9681,20 @@
         "power": "4",
         "preview": {
             "previewed_at": "2019-12-24",
             "source": "Wizards of the Coast",
             "source_uri": "https://twitter.com/MTG_Arena/status/1209549655878422529"
         },
         "prices": {
-            "eur": "7.22",
-            "eur_foil": "6.00",
-            "tix": "1.50",
-            "usd": "4.12",
+            "eur": "7.00",
+            "eur_foil": "7.99",
+            "tix": "0.35",
+            "usd": "3.79",
             "usd_etched": null,
-            "usd_foil": "5.42"
+            "usd_foil": "4.60"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ae8473969-195f-41ee-a84d-463cc8c0ef02&unique=prints",
         "produced_mana": [
             "G",
             "R"
         ],
         "promo": false,
@@ -9738,44 +9743,44 @@
             "R"
         ],
         "colors": [
             "G",
             "R"
         ],
         "digital": false,
-        "edhrec_rank": 3035,
+        "edhrec_rank": 3345,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "frame_effects": [
             "nyxtouched",
             "showcase",
             "legendary",
-            "fullart"
+            "inverted"
         ],
         "full_art": true,
         "games": [
             "arena",
             "paper",
             "mtgo"
         ],
         "highres_image": true,
         "id": "4d747889-04db-4e7a-ad4c-7549514b5112",
         "illustration_id": "24343437-32f3-4f4f-be5d-5ad7a4314895",
         "image_status": "highres_scan",
         "image_uris": {
-            "art_crop": "https://cards.scryfall.io/art_crop/front/4/d/4d747889-04db-4e7a-ad4c-7549514b5112.jpg?1654049968",
-            "border_crop": "https://cards.scryfall.io/border_crop/front/4/d/4d747889-04db-4e7a-ad4c-7549514b5112.jpg?1654049968",
-            "large": "https://cards.scryfall.io/large/front/4/d/4d747889-04db-4e7a-ad4c-7549514b5112.jpg?1654049968",
-            "normal": "https://cards.scryfall.io/normal/front/4/d/4d747889-04db-4e7a-ad4c-7549514b5112.jpg?1654049968",
-            "png": "https://cards.scryfall.io/png/front/4/d/4d747889-04db-4e7a-ad4c-7549514b5112.png?1654049968",
-            "small": "https://cards.scryfall.io/small/front/4/d/4d747889-04db-4e7a-ad4c-7549514b5112.jpg?1654049968"
+            "art_crop": "https://cards.scryfall.io/art_crop/front/4/d/4d747889-04db-4e7a-ad4c-7549514b5112.jpg?1682720711",
+            "border_crop": "https://cards.scryfall.io/border_crop/front/4/d/4d747889-04db-4e7a-ad4c-7549514b5112.jpg?1682720711",
+            "large": "https://cards.scryfall.io/large/front/4/d/4d747889-04db-4e7a-ad4c-7549514b5112.jpg?1682720711",
+            "normal": "https://cards.scryfall.io/normal/front/4/d/4d747889-04db-4e7a-ad4c-7549514b5112.jpg?1682720711",
+            "png": "https://cards.scryfall.io/png/front/4/d/4d747889-04db-4e7a-ad4c-7549514b5112.png?1682720711",
+            "small": "https://cards.scryfall.io/small/front/4/d/4d747889-04db-4e7a-ad4c-7549514b5112.jpg?1682720711"
         },
         "keywords": [
             "Indestructible"
         ],
         "lang": "en",
         "layout": "normal",
         "legalities": {
@@ -9812,20 +9817,20 @@
         "power": "4",
         "preview": {
             "previewed_at": "2020-01-02",
             "source": "Wizards of the Coast",
             "source_uri": "https://magic.wizards.com/en/articles/archive/card-image-gallery/theros-beyond-death-variants"
         },
         "prices": {
-            "eur": "6.98",
-            "eur_foil": "9.90",
+            "eur": "5.50",
+            "eur_foil": "7.70",
             "tix": null,
-            "usd": "3.00",
+            "usd": "2.53",
             "usd_etched": null,
-            "usd_foil": "4.06"
+            "usd_foil": "4.53"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ae8473969-195f-41ee-a84d-463cc8c0ef02&unique=prints",
         "produced_mana": [
             "G",
             "R"
         ],
         "promo": false,
@@ -9874,15 +9879,15 @@
         "color_identity": [
             "G"
         ],
         "colors": [
             "G"
         ],
         "digital": false,
-        "edhrec_rank": 727,
+        "edhrec_rank": 724,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "flavor_text": "Ancient yet ever-young, it is wise and subtle\u2014and cruel and reckless as the spring itself.",
         "foil": true,
         "frame": "2015",
@@ -9949,20 +9954,20 @@
         "power": "5",
         "preview": {
             "previewed_at": "2020-01-09",
             "source": "The Command Zone",
             "source_uri": "https://www.youtube.com/watch?v=FrSbBMp45rg"
         },
         "prices": {
-            "eur": "9.11",
-            "eur_foil": "14.45",
-            "tix": "0.45",
-            "usd": "19.34",
+            "eur": "11.24",
+            "eur_foil": "11.00",
+            "tix": "0.40",
+            "usd": "17.71",
             "usd_etched": null,
-            "usd_foil": "22.35"
+            "usd_foil": "24.50"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A8b610f8f-c8dd-4eeb-bc6e-3bc706d5f63e&unique=prints",
         "promo": false,
         "rarity": "mythic",
         "related_uris": {
             "edhrec": "https://edhrec.com/route/?cc=Nyxbloom+Ancient",
             "gatherer": "https://gatherer.wizards.com/Pages/Card/Details.aspx?multiverseid=476441",
@@ -10004,15 +10009,15 @@
         "color_identity": [
             "G"
         ],
         "colors": [
             "G"
         ],
         "digital": false,
-        "edhrec_rank": 727,
+        "edhrec_rank": 724,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "frame_effects": [
@@ -10071,20 +10076,20 @@
         "nonfoil": true,
         "object": "card",
         "oracle_id": "8b610f8f-c8dd-4eeb-bc6e-3bc706d5f63e",
         "oracle_text": "Trample\nIf you tap a permanent for mana, it produces three times as much of that mana instead.",
         "oversized": false,
         "power": "5",
         "prices": {
-            "eur": "15.46",
-            "eur_foil": "55.00",
+            "eur": "18.00",
+            "eur_foil": "45.00",
             "tix": null,
-            "usd": "27.06",
+            "usd": "23.07",
             "usd_etched": null,
-            "usd_foil": "70.43"
+            "usd_foil": "70.31"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A8b610f8f-c8dd-4eeb-bc6e-3bc706d5f63e&unique=prints",
         "promo": false,
         "promo_types": [
             "boosterfun"
         ],
         "rarity": "mythic",
@@ -10128,15 +10133,15 @@
         "collector_number": "248",
         "color_identity": [
             "G",
             "W"
         ],
         "colors": [],
         "digital": false,
-        "edhrec_rank": 577,
+        "edhrec_rank": 554,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "full_art": false,
@@ -10192,27 +10197,27 @@
         ],
         "name": "Temple of Plenty",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "e521322b-0e83-458c-8936-7021a80ee279",
         "oracle_text": "Temple of Plenty enters the battlefield tapped.\nWhen Temple of Plenty enters the battlefield, scry 1.\n{T}: Add {G} or {W}.",
         "oversized": false,
-        "penny_rank": 976,
+        "penny_rank": 1066,
         "preview": {
             "previewed_at": "2019-12-30",
             "source": "ChannelFireball",
             "source_uri": "https://www.channelfireball.com/all-strategy/articles/3-point/theros-beyond-death-exclusive-preview/"
         },
         "prices": {
-            "eur": "0.23",
-            "eur_foil": "0.30",
+            "eur": "0.49",
+            "eur_foil": "0.25",
             "tix": "0.02",
-            "usd": "0.65",
+            "usd": "0.27",
             "usd_etched": null,
-            "usd_foil": "0.94"
+            "usd_foil": "0.75"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ae521322b-0e83-458c-8936-7021a80ee279&unique=prints",
         "produced_mana": [
             "G",
             "W"
         ],
         "promo": false,
@@ -10256,15 +10261,15 @@
         "collector_number": "351",
         "color_identity": [
             "G",
             "W"
         ],
         "colors": [],
         "digital": false,
-        "edhrec_rank": 577,
+        "edhrec_rank": 554,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "frame_effects": [
@@ -10320,27 +10325,27 @@
         "multiverse_ids": [],
         "name": "Temple of Plenty",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "e521322b-0e83-458c-8936-7021a80ee279",
         "oracle_text": "Temple of Plenty enters the battlefield tapped.\nWhen Temple of Plenty enters the battlefield, scry 1.\n{T}: Add {G} or {W}.",
         "oversized": false,
-        "penny_rank": 976,
+        "penny_rank": 1066,
         "preview": {
             "previewed_at": "2019-12-30",
             "source": "ChannelFireball",
             "source_uri": "https://www.channelfireball.com/all-strategy/articles/3-point/theros-beyond-death-exclusive-preview/"
         },
         "prices": {
-            "eur": "2.99",
-            "eur_foil": "3.40",
+            "eur": "1.80",
+            "eur_foil": "3.50",
             "tix": null,
-            "usd": "2.21",
+            "usd": "1.79",
             "usd_etched": null,
-            "usd_foil": "10.28"
+            "usd_foil": "10.41"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ae521322b-0e83-458c-8936-7021a80ee279&unique=prints",
         "produced_mana": [
             "G",
             "W"
         ],
         "promo": false,
@@ -10406,15 +10411,15 @@
         "color_identity": [
             "G"
         ],
         "colors": [
             "G"
         ],
         "digital": false,
-        "edhrec_rank": 2949,
+        "edhrec_rank": 3006,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "full_art": false,
@@ -10470,27 +10475,27 @@
         ],
         "name": "Wolfwillow Haven",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "7579f57d-c76e-4703-a030-34fb7160cb23",
         "oracle_text": "Enchant land\nWhenever enchanted land is tapped for mana, its controller adds an additional {G}.\n{4}{G}, Sacrifice Wolfwillow Haven: Create a 2/2 green Wolf creature token. Activate only during your turn.",
         "oversized": false,
-        "penny_rank": 2289,
+        "penny_rank": 2349,
         "preview": {
             "previewed_at": "2020-01-09",
             "source": "Drawza",
             "source_uri": "https://www.twitch.tv/drawza"
         },
         "prices": {
-            "eur": "0.21",
-            "eur_foil": "0.49",
+            "eur": "0.16",
+            "eur_foil": "0.10",
             "tix": "0.03",
-            "usd": "0.36",
+            "usd": "0.28",
             "usd_etched": null,
-            "usd_foil": "0.50"
+            "usd_foil": "0.64"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A7579f57d-c76e-4703-a030-34fb7160cb23&unique=prints",
         "produced_mana": [
             "G"
         ],
         "promo": false,
         "rarity": "uncommon",
@@ -10551,15 +10556,15 @@
         "color_identity": [
             "G"
         ],
         "colors": [
             "G"
         ],
         "digital": false,
-        "edhrec_rank": 2949,
+        "edhrec_rank": 3006,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "frame_effects": [
@@ -10615,22 +10620,22 @@
         "multiverse_ids": [],
         "name": "Wolfwillow Haven",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "7579f57d-c76e-4703-a030-34fb7160cb23",
         "oracle_text": "Enchant land\nWhenever enchanted land is tapped for mana, its controller adds an additional {G}.\n{4}{G}, Sacrifice Wolfwillow Haven: Create a 2/2 green Wolf creature token. Activate only during your turn.",
         "oversized": false,
-        "penny_rank": 2289,
+        "penny_rank": 2349,
         "prices": {
-            "eur": "0.84",
-            "eur_foil": "0.09",
+            "eur": "0.05",
+            "eur_foil": "1.70",
             "tix": null,
-            "usd": "1.03",
+            "usd": "1.13",
             "usd_etched": null,
-            "usd_foil": "3.94"
+            "usd_foil": "5.20"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A7579f57d-c76e-4703-a030-34fb7160cb23&unique=prints",
         "produced_mana": [
             "G"
         ],
         "promo": true,
         "promo_types": [
@@ -10780,20 +10785,20 @@
         ],
         "name": "Who // What // When // Where // Why",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "adfe1b07-dd82-4c39-a7a6-ded0b1c39761",
         "oversized": false,
         "prices": {
-            "eur": "2.99",
-            "eur_foil": "50.00",
+            "eur": "1.37",
+            "eur_foil": "39.00",
             "tix": null,
-            "usd": "1.59",
+            "usd": "1.43",
             "usd_etched": null,
-            "usd_foil": "51.92"
+            "usd_foil": "53.49"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Aadfe1b07-dd82-4c39-a7a6-ded0b1c39761&unique=prints",
         "promo": false,
         "rarity": "rare",
         "related_uris": {
             "edhrec": "https://edhrec.com/route/?cc=Who+%2F%2F+What+%2F%2F+When+%2F%2F+Where+%2F%2F+Why",
             "gatherer": "https://gatherer.wizards.com/Pages/Card/Details.aspx?multiverseid=74358",
@@ -10944,20 +10949,20 @@
         "name": "Very Cryptic Command",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "5d0fd8ee-2cc1-4ed8-9395-1660d15cc9f3",
         "oracle_text": "Choose two \u2014\n\u2022 Switch target creature's power and toughness until end of turn.\n\u2022 Target creature can't be blocked this turn.\n\u2022 Draw a card. If that card's art is by Wayne England, you may reveal it and draw another card.\n\u2022 Assemble a Contraption.",
         "oversized": false,
         "prices": {
-            "eur": "2.99",
+            "eur": "2.46",
             "eur_foil": "25.99",
             "tix": null,
-            "usd": "1.61",
+            "usd": "1.49",
             "usd_etched": null,
-            "usd_foil": "24.99"
+            "usd_foil": "18.49"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A5d0fd8ee-2cc1-4ed8-9395-1660d15cc9f3&unique=prints",
         "promo": false,
         "rarity": "rare",
         "related_uris": {
             "edhrec": "https://edhrec.com/route/?cc=Very+Cryptic+Command",
             "gatherer": "https://gatherer.wizards.com/Pages/Card/Details.aspx?multiverseid=439645",
@@ -11107,20 +11112,20 @@
         "name": "Very Cryptic Command",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "48d94218-a460-4974-82b9-d3a9cba9998e",
         "oracle_text": "Choose two \u2014\n\u2022 Untap two target permanents.\n\u2022 Tap each permanent target player controls with exactly one word in its name.\n\u2022 Discard all the cards in your hand, then draw that many cards.\n\u2022 Return target instant or sorcery card from your graveyard to your hand.",
         "oversized": false,
         "prices": {
-            "eur": "2.50",
+            "eur": "2.40",
             "eur_foil": "7.99",
             "tix": null,
-            "usd": "1.53",
+            "usd": "0.90",
             "usd_etched": null,
-            "usd_foil": "8.94"
+            "usd_foil": "7.31"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A48d94218-a460-4974-82b9-d3a9cba9998e&unique=prints",
         "promo": false,
         "rarity": "rare",
         "related_uris": {
             "edhrec": "https://edhrec.com/route/?cc=Very+Cryptic+Command",
             "gatherer": "https://gatherer.wizards.com/Pages/Card/Details.aspx?multiverseid=439438",
@@ -11278,20 +11283,20 @@
         "name": "Very Cryptic Command",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "5063f840-0aed-4e2d-98d8-65b39e95e3c9",
         "oracle_text": "Choose two \u2014\n\u2022 Draw a card from an opponent's library.\n\u2022 Copy target instant or sorcery spell. You may choose new targets for the copy.\n\u2022 Until end of turn, target creature loses all abilities and becomes a blue Frog with base power and toughness 1/1.\n\u2022 Create a 1/1 colorless Gnome artifact creature token.",
         "oversized": false,
         "prices": {
-            "eur": "3.50",
-            "eur_foil": "9.99",
+            "eur": "2.00",
+            "eur_foil": "9.00",
             "tix": null,
-            "usd": "2.15",
+            "usd": "2.00",
             "usd_etched": null,
-            "usd_foil": "9.00"
+            "usd_foil": "6.21"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A5063f840-0aed-4e2d-98d8-65b39e95e3c9&unique=prints",
         "promo": false,
         "rarity": "rare",
         "related_uris": {
             "edhrec": "https://edhrec.com/route/?cc=Very+Cryptic+Command",
             "gatherer": "https://gatherer.wizards.com/Pages/Card/Details.aspx?multiverseid=439646",
@@ -11441,20 +11446,20 @@
         "name": "Very Cryptic Command",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "9dc00e2b-73a3-42d5-95c9-d86094a6e455",
         "oracle_text": "Choose two \u2014\n\u2022 Return target permanent to its controller's hand.\n\u2022 Draw two cards, then discard a card.\n\u2022 Change the target of target spell with a single target.\n\u2022 Turn over target nontoken creature.",
         "oversized": false,
         "prices": {
-            "eur": "2.75",
+            "eur": "1.50",
             "eur_foil": "26.08",
             "tix": null,
-            "usd": "3.28",
+            "usd": "1.57",
             "usd_etched": null,
-            "usd_foil": "18.95"
+            "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A9dc00e2b-73a3-42d5-95c9-d86094a6e455&unique=prints",
         "promo": false,
         "rarity": "rare",
         "related_uris": {
             "edhrec": "https://edhrec.com/route/?cc=Very+Cryptic+Command",
             "gatherer": "https://gatherer.wizards.com/Pages/Card/Details.aspx?multiverseid=439647",
@@ -11606,20 +11611,20 @@
         "name": "Very Cryptic Command",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "a84f0b11-5c59-4bab-81ef-a84470fb2ade",
         "oracle_text": "Choose two \u2014\n\u2022 Counter target black-bordered spell.\n\u2022 Return target creature to its owner's hand.\n\u2022 Untap each permanent you control with a watermark.\n\u2022 Roll two six-sided dice. Target player mills X cards, where X is the total of those results.",
         "oversized": false,
         "prices": {
-            "eur": "2.75",
-            "eur_foil": "9.99",
+            "eur": "1.49",
+            "eur_foil": "8.89",
             "tix": null,
-            "usd": "3.38",
+            "usd": "3.23",
             "usd_etched": null,
-            "usd_foil": "15.37"
+            "usd_foil": "13.45"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Aa84f0b11-5c59-4bab-81ef-a84470fb2ade&unique=prints",
         "promo": false,
         "rarity": "rare",
         "related_uris": {
             "edhrec": "https://edhrec.com/route/?cc=Very+Cryptic+Command",
             "gatherer": "https://gatherer.wizards.com/Pages/Card/Details.aspx?multiverseid=439648",
@@ -11779,20 +11784,20 @@
         "name": "Very Cryptic Command",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "684dfe99-c957-4b91-bd14-867c20b4b3db",
         "oracle_text": "Choose two \u2014\n\u2022 Scry 3.\n\u2022 Create a 2/2 black Rogue creature token with menace.\n\u2022 Add or subtract 1 or one from a number or number word on target spell or permanent until end of turn.\n\u2022 Return all artifacts target player controls to their owner's hand.",
         "oversized": false,
         "prices": {
-            "eur": "2.47",
-            "eur_foil": "9.00",
+            "eur": "1.95",
+            "eur_foil": "8.49",
             "tix": null,
-            "usd": "1.53",
+            "usd": "1.50",
             "usd_etched": null,
-            "usd_foil": "6.49"
+            "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A684dfe99-c957-4b91-bd14-867c20b4b3db&unique=prints",
         "promo": false,
         "rarity": "rare",
         "related_uris": {
             "edhrec": "https://edhrec.com/route/?cc=Very+Cryptic+Command",
             "gatherer": "https://gatherer.wizards.com/Pages/Card/Details.aspx?multiverseid=439649",
@@ -11832,15 +11837,15 @@
         "color_identity": [
             "U"
         ],
         "colors": [
             "U"
         ],
         "digital": true,
-        "edhrec_rank": 14751,
+        "edhrec_rank": 15293,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "full_art": false,
@@ -11893,15 +11898,15 @@
         ],
         "name": "Academy Elite",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "ba6c3c72-c014-45c6-a0b4-59eb9a65303e",
         "oracle_text": "Academy Elite enters the battlefield with X +1/+1 counters on it, where X is the number of instant and sorcery cards in all graveyards.\n{2}{U}, Remove a +1/+1 counter from Academy Elite: Draw a card, then discard a card.",
         "oversized": false,
-        "penny_rank": 3771,
+        "penny_rank": 3850,
         "power": "0",
         "prices": {
             "eur": null,
             "eur_foil": null,
             "tix": "0.02",
             "usd": null,
             "usd_etched": null,
@@ -11950,15 +11955,15 @@
         "color_identity": [
             "W"
         ],
         "colors": [
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 8442,
+        "edhrec_rank": 8753,
         "finishes": [
             "nonfoil"
         ],
         "flavor_text": "Follow the light. In its absence, follow her.",
         "foil": false,
         "frame": "2015",
         "full_art": false,
@@ -12015,21 +12020,21 @@
         ],
         "name": "Serra Angel",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "4b7ac066-e5c7-43e6-9e7e-2739b24a905d",
         "oracle_text": "Flying, vigilance",
         "oversized": false,
-        "penny_rank": 8528,
+        "penny_rank": 8873,
         "power": "4",
         "prices": {
             "eur": "0.02",
             "eur_foil": null,
             "tix": "0.05",
-            "usd": "0.12",
+            "usd": "0.10",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A4b7ac066-e5c7-43e6-9e7e-2739b24a905d&unique=prints",
         "promo": false,
         "promo_types": [
             "starterdeck"
```

### Comparing `mtg_ssm-2.6.2.dev1/tests/data/migrations.json` & `mtg_ssm-2.6.2.dev2/tests/data/migrations.json`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/tests/data/sets.json` & `mtg_ssm-2.6.2.dev2/tests/data/sets.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9950429940494715%*

 * *Differences: {"'data'": "{0: {'icon_svg_uri': 'https://svgs.scryfall.io/sets/arc.svg?1688961600'}, 1: "*

 * *           "{'icon_svg_uri': 'https://svgs.scryfall.io/sets/bok.svg?1688961600'}, 2: "*

 * *           "{'icon_svg_uri': 'https://svgs.scryfall.io/sets/chk.svg?1688961600'}, 3: "*

 * *           "{'icon_svg_uri': 'https://svgs.scryfall.io/sets/csp.svg?1688961600'}, 4: "*

 * *           "{'icon_svg_uri': 'https://svgs.scryfall.io/sets/fem.svg?1688961600'}, 5: "*

 * *           "{'icon_svg_uri': 'https://svgs.scryfall.io/sets/hml.svg?16889 […]*

```diff
@@ -1,15 +1,15 @@
 {
     "data": [
         {
             "card_count": 1,
             "code": "arc",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/arc.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/arc.svg?1688961600",
             "id": "8bc5ec64-18d5-4c81-96a1-8f619d81a019",
             "name": "Archenemy",
             "nonfoil_only": true,
             "object": "set",
             "released_at": "2010-06-18",
             "scryfall_uri": "https://scryfall.com/sets/arc",
             "search_uri": "https://api.scryfall.com/cards/search?include_extras=true&include_variations=true&order=set&q=e%3Aarc&unique=prints",
@@ -21,15 +21,15 @@
             "arena_code": "bok",
             "block": "Kamigawa",
             "block_code": "chk",
             "card_count": 1,
             "code": "bok",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/bok.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/bok.svg?1688961600",
             "id": "d4b88587-a1f5-4b47-9e24-78ec9e57bd0e",
             "mtgo_code": "bok",
             "name": "Betrayers of Kamigawa",
             "nonfoil_only": false,
             "object": "set",
             "printed_size": 165,
             "released_at": "2005-02-04",
@@ -43,15 +43,15 @@
             "arena_code": "chk",
             "block": "Kamigawa",
             "block_code": "chk",
             "card_count": 2,
             "code": "chk",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/chk.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/chk.svg?1688961600",
             "id": "6183d21f-a0af-4118-ba58-aca1d8719c01",
             "mtgo_code": "chk",
             "name": "Champions of Kamigawa",
             "nonfoil_only": false,
             "object": "set",
             "printed_size": 306,
             "released_at": "2004-10-01",
@@ -65,15 +65,15 @@
             "arena_code": "csp",
             "block": "Ice Age",
             "block_code": "ice",
             "card_count": 1,
             "code": "csp",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/csp.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/csp.svg?1688961600",
             "id": "1f4f105f-73e4-4f03-849e-82a204807847",
             "mtgo_code": "csp",
             "name": "Coldsnap",
             "nonfoil_only": false,
             "object": "set",
             "printed_size": 155,
             "released_at": "2006-07-21",
@@ -84,15 +84,15 @@
             "uri": "https://api.scryfall.com/sets/1f4f105f-73e4-4f03-849e-82a204807847"
         },
         {
             "card_count": 4,
             "code": "fem",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/fem.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/fem.svg?1688961600",
             "id": "cf7390b1-341a-4ae8-a325-da0f5f322f13",
             "name": "Fallen Empires",
             "nonfoil_only": true,
             "object": "set",
             "released_at": "1994-11-01",
             "scryfall_uri": "https://scryfall.com/sets/fem",
             "search_uri": "https://api.scryfall.com/cards/search?include_extras=true&include_variations=true&order=set&q=e%3Afem&unique=prints",
@@ -101,15 +101,15 @@
             "uri": "https://api.scryfall.com/sets/cf7390b1-341a-4ae8-a325-da0f5f322f13"
         },
         {
             "card_count": 2,
             "code": "hml",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/hml.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/hml.svg?1688961600",
             "id": "5ac1f606-e682-46e9-ad0f-122a3783581b",
             "name": "Homelands",
             "nonfoil_only": true,
             "object": "set",
             "released_at": "1995-10-01",
             "scryfall_uri": "https://scryfall.com/sets/hml",
             "search_uri": "https://api.scryfall.com/cards/search?include_extras=true&include_variations=true&order=set&q=e%3Ahml&unique=prints",
@@ -119,15 +119,15 @@
         },
         {
             "arena_code": "pc1",
             "card_count": 2,
             "code": "hop",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/hop.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/hop.svg?1688961600",
             "id": "7137ffeb-eb1d-466c-a0d3-3157f52b1b10",
             "mtgo_code": "pc1",
             "name": "Planechase",
             "nonfoil_only": true,
             "object": "set",
             "released_at": "2009-09-04",
             "scryfall_uri": "https://scryfall.com/sets/hop",
@@ -139,15 +139,15 @@
         {
             "block": "Ice Age",
             "block_code": "ice",
             "card_count": 5,
             "code": "ice",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/ice.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/ice.svg?1688961600",
             "id": "b0e08eea-5c01-4406-a6e2-dcd09c5e5b67",
             "name": "Ice Age",
             "nonfoil_only": true,
             "object": "set",
             "released_at": "1995-06-03",
             "scryfall_uri": "https://scryfall.com/sets/ice",
             "search_uri": "https://api.scryfall.com/cards/search?include_extras=true&include_variations=true&order=set&q=e%3Aice&unique=prints",
@@ -159,15 +159,15 @@
             "arena_code": "isd",
             "block": "Innistrad",
             "block_code": "isd",
             "card_count": 5,
             "code": "isd",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/isd.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/isd.svg?1688961600",
             "id": "d1026945-2969-42b9-be53-f941405a58cb",
             "mtgo_code": "isd",
             "name": "Innistrad",
             "nonfoil_only": false,
             "object": "set",
             "printed_size": 264,
             "released_at": "2011-09-30",
@@ -179,15 +179,15 @@
         },
         {
             "arena_code": "khm",
             "card_count": 3,
             "code": "khm",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/khm.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/khm.svg?1688961600",
             "id": "43057fad-b1c1-437f-bc48-0045bce6d8c9",
             "mtgo_code": "khm",
             "name": "Kaldheim",
             "nonfoil_only": false,
             "object": "set",
             "released_at": "2021-02-05",
             "scryfall_uri": "https://scryfall.com/sets/khm",
@@ -199,15 +199,15 @@
         {
             "block": "Core Set",
             "block_code": "lea",
             "card_count": 4,
             "code": "lea",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/lea.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/lea.svg?1688961600",
             "id": "288bd996-960e-448b-a187-9504c1930c2c",
             "name": "Limited Edition Alpha",
             "nonfoil_only": true,
             "object": "set",
             "released_at": "1993-08-05",
             "scryfall_uri": "https://scryfall.com/sets/lea",
             "search_uri": "https://api.scryfall.com/cards/search?include_extras=true&include_variations=true&order=set&q=e%3Alea&unique=prints",
@@ -219,15 +219,15 @@
             "arena_code": "mbs",
             "block": "Scars of Mirrodin",
             "block_code": "som",
             "card_count": 2,
             "code": "mbs",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/mbs.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/mbs.svg?1688961600",
             "id": "f46c57e3-9301-4006-a6ca-06f3f65961fb",
             "mtgo_code": "mbs",
             "name": "Mirrodin Besieged",
             "nonfoil_only": false,
             "object": "set",
             "printed_size": 155,
             "released_at": "2011-02-04",
@@ -239,15 +239,15 @@
         },
         {
             "arena_code": "mma",
             "card_count": 1,
             "code": "mma",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/mma.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/mma.svg?1688961600",
             "id": "0b7020f2-336d-4706-9ce6-f6710b9ebd5c",
             "mtgo_code": "mma",
             "name": "Modern Masters",
             "nonfoil_only": false,
             "object": "set",
             "printed_size": 229,
             "released_at": "2013-06-07",
@@ -259,15 +259,15 @@
         },
         {
             "arena_code": "neo",
             "card_count": 3,
             "code": "neo",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/neo.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/neo.svg?1688961600",
             "id": "59a2059f-5482-433f-8761-eb2e17859b71",
             "mtgo_code": "neo",
             "name": "Kamigawa: Neon Dynasty",
             "nonfoil_only": false,
             "object": "set",
             "printed_size": 302,
             "released_at": "2022-02-18",
@@ -278,15 +278,15 @@
             "uri": "https://api.scryfall.com/sets/59a2059f-5482-433f-8761-eb2e17859b71"
         },
         {
             "card_count": 1,
             "code": "oarc",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/arc.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/arc.svg?1688961600",
             "id": "238beedf-1d4d-475f-a980-527ba2f55dc6",
             "name": "Archenemy Schemes",
             "nonfoil_only": true,
             "object": "set",
             "parent_set_code": "arc",
             "released_at": "2010-06-18",
             "scryfall_uri": "https://scryfall.com/sets/oarc",
@@ -298,15 +298,15 @@
             "arena_code": "ogw",
             "block": "Battle for Zendikar",
             "block_code": "bfz",
             "card_count": 4,
             "code": "ogw",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/ogw.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/ogw.svg?1688961600",
             "id": "cd51d245-8f95-45b0-ab5f-e2b3a3eb5dfe",
             "mtgo_code": "ogw",
             "name": "Oath of the Gatewatch",
             "nonfoil_only": false,
             "object": "set",
             "printed_size": 184,
             "released_at": "2016-01-22",
@@ -318,15 +318,15 @@
         },
         {
             "arena_code": "ohop",
             "card_count": 1,
             "code": "ohop",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/hop.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/hop.svg?1688961600",
             "id": "7a8b75a9-7c92-4c3f-976a-322e1eb3b6b6",
             "mtgo_code": "ohop",
             "name": "Planechase Planes",
             "nonfoil_only": true,
             "object": "set",
             "parent_set_code": "hop",
             "released_at": "2009-09-04",
@@ -337,15 +337,15 @@
         },
         {
             "arena_code": "opc2",
             "card_count": 2,
             "code": "opc2",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/pc2.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/pc2.svg?1688961600",
             "id": "7079031b-c5b0-4353-87af-a63a0f204f47",
             "mtgo_code": "opc2",
             "name": "Planechase 2012 Planes",
             "nonfoil_only": true,
             "object": "set",
             "parent_set_code": "pc2",
             "released_at": "2012-06-01",
@@ -357,15 +357,15 @@
         {
             "block": "Magic Player Rewards",
             "block_code": "mpr",
             "card_count": 1,
             "code": "p03",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/dci.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/dci.svg?1688961600",
             "id": "dfa906ff-63d8-4065-abef-809988337288",
             "name": "Magic Player Rewards 2003",
             "nonfoil_only": true,
             "object": "set",
             "released_at": "2003-01-01",
             "scryfall_uri": "https://scryfall.com/sets/p03",
             "search_uri": "https://api.scryfall.com/cards/search?include_extras=true&include_variations=true&order=set&q=e%3Ap03&unique=prints",
@@ -374,15 +374,15 @@
         },
         {
             "arena_code": "pc2",
             "card_count": 1,
             "code": "pc2",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/pc2.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/pc2.svg?1688961600",
             "id": "9fb2f83e-7015-4aa9-808f-310ccf0fdb9c",
             "mtgo_code": "pc2",
             "name": "Planechase 2012",
             "nonfoil_only": true,
             "object": "set",
             "released_at": "2012-06-01",
             "scryfall_uri": "https://scryfall.com/sets/pc2",
@@ -392,15 +392,15 @@
             "uri": "https://api.scryfall.com/sets/9fb2f83e-7015-4aa9-808f-310ccf0fdb9c"
         },
         {
             "card_count": 2,
             "code": "pdci",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/dci.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/dci.svg?1688961600",
             "id": "935e91e9-61c2-4b35-a85a-c08fef3b420b",
             "name": "DCI Promos",
             "nonfoil_only": false,
             "object": "set",
             "released_at": "2006-01-01",
             "scryfall_uri": "https://scryfall.com/sets/pdci",
             "search_uri": "https://api.scryfall.com/cards/search?include_extras=true&include_variations=true&order=set&q=e%3Apdci&unique=prints",
@@ -410,15 +410,15 @@
         {
             "block": "Khans of Tarkir",
             "block_code": "ktk",
             "card_count": 2,
             "code": "pfrf",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/frf.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/frf.svg?1688961600",
             "id": "aa9f80e3-8d60-46b7-b91e-eb1736fde866",
             "name": "Fate Reforged Promos",
             "nonfoil_only": false,
             "object": "set",
             "parent_set_code": "frf",
             "released_at": "2015-01-23",
             "scryfall_uri": "https://scryfall.com/sets/pfrf",
@@ -427,15 +427,15 @@
             "uri": "https://api.scryfall.com/sets/aa9f80e3-8d60-46b7-b91e-eb1736fde866"
         },
         {
             "card_count": 1,
             "code": "phop",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/dci.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/dci.svg?1688961600",
             "id": "ef3f6784-a6e8-41ff-8bed-72e0c7121298",
             "name": "Planechase Promos",
             "nonfoil_only": true,
             "object": "set",
             "parent_set_code": "hop",
             "released_at": "2009-09-04",
             "scryfall_uri": "https://scryfall.com/sets/phop",
@@ -444,15 +444,15 @@
             "uri": "https://api.scryfall.com/sets/ef3f6784-a6e8-41ff-8bed-72e0c7121298"
         },
         {
             "card_count": 1,
             "code": "phpr",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/pbook.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/pbook.svg?1688961600",
             "id": "b32cc4a1-1e06-4bec-bab6-89b2691b57a4",
             "name": "HarperPrism Book Promos",
             "nonfoil_only": true,
             "object": "set",
             "released_at": "1994-09-01",
             "scryfall_uri": "https://scryfall.com/sets/phpr",
             "search_uri": "https://api.scryfall.com/cards/search?include_extras=true&include_variations=true&order=set&q=e%3Aphpr&unique=prints",
@@ -463,15 +463,15 @@
             "arena_code": "plc",
             "block": "Time Spiral",
             "block_code": "tsp",
             "card_count": 1,
             "code": "plc",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/plc.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/plc.svg?1688961600",
             "id": "5a1b571c-73e9-4c14-b9d4-a62507d85789",
             "mtgo_code": "plc",
             "name": "Planar Chaos",
             "nonfoil_only": false,
             "object": "set",
             "printed_size": 165,
             "released_at": "2007-02-02",
@@ -485,15 +485,15 @@
             "arena_code": "ps",
             "block": "Invasion",
             "block_code": "inv",
             "card_count": 2,
             "code": "pls",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/pls.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/pls.svg?1688961600",
             "id": "82dc193b-bd5f-4883-a93f-a4155b467ee0",
             "mtgo_code": "ps",
             "name": "Planeshift",
             "nonfoil_only": false,
             "object": "set",
             "printed_size": 143,
             "released_at": "2001-02-05",
@@ -506,15 +506,15 @@
         {
             "block": "Scars of Mirrodin",
             "block_code": "som",
             "card_count": 1,
             "code": "pmbs",
             "digital": false,
             "foil_only": true,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/mbs.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/mbs.svg?1688961600",
             "id": "8a59d98a-4e13-4943-b06c-b35868e954ba",
             "name": "Mirrodin Besieged Promos",
             "nonfoil_only": false,
             "object": "set",
             "parent_set_code": "mbs",
             "released_at": "2011-02-03",
             "scryfall_uri": "https://scryfall.com/sets/pmbs",
@@ -523,15 +523,15 @@
             "uri": "https://api.scryfall.com/sets/8a59d98a-4e13-4943-b06c-b35868e954ba"
         },
         {
             "card_count": 2,
             "code": "pneo",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/neo.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/neo.svg?1688961600",
             "id": "b3161020-d74f-48cc-bc9d-d7233e64e524",
             "name": "Kamigawa: Neon Dynasty Promos",
             "nonfoil_only": false,
             "object": "set",
             "parent_set_code": "neo",
             "released_at": "2022-02-18",
             "scryfall_uri": "https://scryfall.com/sets/pneo",
@@ -542,15 +542,15 @@
         {
             "block": "Guilds of Ravnica",
             "block_code": "grn",
             "card_count": 2,
             "code": "prna",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/rna.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/rna.svg?1688961600",
             "id": "503230ec-81e3-4f92-b847-ff435b1652e0",
             "name": "Ravnica Allegiance Promos",
             "nonfoil_only": false,
             "object": "set",
             "parent_set_code": "rna",
             "released_at": "2019-01-25",
             "scryfall_uri": "https://scryfall.com/sets/prna",
@@ -561,15 +561,15 @@
         {
             "block": "Guilds of Ravnica",
             "block_code": "grn",
             "card_count": 2,
             "code": "prw2",
             "digital": false,
             "foil_only": true,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/rna.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/rna.svg?1688961600",
             "id": "ee3a8eb6-0583-492b-8be5-265795d38038",
             "name": "RNA Ravnica Weekend",
             "nonfoil_only": false,
             "object": "set",
             "parent_set_code": "rna",
             "released_at": "2019-02-16",
             "scryfall_uri": "https://scryfall.com/sets/prw2",
@@ -578,15 +578,15 @@
             "uri": "https://api.scryfall.com/sets/ee3a8eb6-0583-492b-8be5-265795d38038"
         },
         {
             "card_count": 1,
             "code": "ptg",
             "digital": false,
             "foil_only": true,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/ptg.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/ptg.svg?1688961600",
             "id": "d264b61b-bfb3-4388-be42-e34a1eaa00c2",
             "name": "Ponies: The Galloping",
             "nonfoil_only": false,
             "object": "set",
             "released_at": "2019-10-22",
             "scryfall_uri": "https://scryfall.com/sets/ptg",
             "search_uri": "https://api.scryfall.com/cards/search?include_extras=true&include_variations=true&order=set&q=e%3Aptg&unique=prints",
@@ -595,15 +595,15 @@
             "uri": "https://api.scryfall.com/sets/d264b61b-bfb3-4388-be42-e34a1eaa00c2"
         },
         {
             "card_count": 1,
             "code": "ren",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/ren.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/ren.svg?1688961600",
             "id": "bec33d25-cf6f-460f-918d-29b3009686bb",
             "name": "Renaissance",
             "nonfoil_only": true,
             "object": "set",
             "released_at": "1995-08-01",
             "scryfall_uri": "https://scryfall.com/sets/ren",
             "search_uri": "https://api.scryfall.com/cards/search?include_extras=true&include_variations=true&order=set&q=e%3Aren&unique=prints",
@@ -615,15 +615,15 @@
             "arena_code": "rna",
             "block": "Guilds of Ravnica",
             "block_code": "grn",
             "card_count": 1,
             "code": "rna",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/rna.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/rna.svg?1688961600",
             "id": "97a7fd84-8d89-45a3-b48b-c951f6a3f9f1",
             "mtgo_code": "rna",
             "name": "Ravnica Allegiance",
             "nonfoil_only": false,
             "object": "set",
             "printed_size": 259,
             "released_at": "2019-01-25",
@@ -634,15 +634,15 @@
             "uri": "https://api.scryfall.com/sets/97a7fd84-8d89-45a3-b48b-c951f6a3f9f1"
         },
         {
             "card_count": 1,
             "code": "s00",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/s00.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/s00.svg?1688961600",
             "id": "1c105623-2564-40d7-a3aa-4134787fb127",
             "name": "Starter 2000",
             "nonfoil_only": false,
             "object": "set",
             "released_at": "2000-04-01",
             "scryfall_uri": "https://scryfall.com/sets/s00",
             "search_uri": "https://api.scryfall.com/cards/search?include_extras=true&include_variations=true&order=set&q=e%3As00&unique=prints",
@@ -651,15 +651,15 @@
             "uri": "https://api.scryfall.com/sets/1c105623-2564-40d7-a3aa-4134787fb127"
         },
         {
             "card_count": 3,
             "code": "sld",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/star.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/star.svg?1688961600",
             "id": "4d92a8a7-ccb0-437d-abdc-9d70fc5ed672",
             "name": "Secret Lair Drop",
             "nonfoil_only": false,
             "object": "set",
             "released_at": "2019-12-02",
             "scryfall_uri": "https://scryfall.com/sets/sld",
             "search_uri": "https://api.scryfall.com/cards/search?include_extras=true&include_variations=true&order=set&q=e%3Asld&unique=prints",
@@ -671,15 +671,15 @@
             "arena_code": "sok",
             "block": "Kamigawa",
             "block_code": "chk",
             "card_count": 1,
             "code": "sok",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/sok.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/sok.svg?1688961600",
             "id": "4db16ad3-2b95-442f-bb6b-e9aa7fe7f769",
             "mtgo_code": "sok",
             "name": "Saviors of Kamigawa",
             "nonfoil_only": false,
             "object": "set",
             "printed_size": 165,
             "released_at": "2005-06-03",
@@ -690,15 +690,15 @@
             "uri": "https://api.scryfall.com/sets/4db16ad3-2b95-442f-bb6b-e9aa7fe7f769"
         },
         {
             "card_count": 1,
             "code": "sunf",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/unf.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/unf.svg?1688961600",
             "id": "565e3302-2fed-487e-a0f7-7f8037d25030",
             "name": "Unfinity Sticker Sheets",
             "nonfoil_only": true,
             "object": "set",
             "parent_set_code": "unf",
             "released_at": "2022-10-07",
             "scryfall_uri": "https://scryfall.com/sets/sunf",
@@ -708,15 +708,15 @@
         },
         {
             "arena_code": "thb",
             "card_count": 8,
             "code": "thb",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/thb.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/thb.svg?1688961600",
             "id": "5f23a78d-cda1-462a-8be3-a62b40c34913",
             "mtgo_code": "thb",
             "name": "Theros Beyond Death",
             "nonfoil_only": false,
             "object": "set",
             "released_at": "2020-01-24",
             "scryfall_uri": "https://scryfall.com/sets/thb",
@@ -726,15 +726,15 @@
             "uri": "https://api.scryfall.com/sets/5f23a78d-cda1-462a-8be3-a62b40c34913"
         },
         {
             "card_count": 1,
             "code": "unh",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/unh.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/unh.svg?1688961600",
             "id": "4c8bc76a-05a5-43db-aaf0-34deb347b871",
             "name": "Unhinged",
             "nonfoil_only": false,
             "object": "set",
             "printed_size": 141,
             "released_at": "2004-11-19",
             "scryfall_uri": "https://scryfall.com/sets/unh",
@@ -744,15 +744,15 @@
             "uri": "https://api.scryfall.com/sets/4c8bc76a-05a5-43db-aaf0-34deb347b871"
         },
         {
             "card_count": 6,
             "code": "ust",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/ust.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/ust.svg?1688961600",
             "id": "83491685-880d-41dd-a4af-47d2b3b17c10",
             "name": "Unstable",
             "nonfoil_only": false,
             "object": "set",
             "printed_size": 268,
             "released_at": "2017-12-08",
             "scryfall_uri": "https://scryfall.com/sets/ust",
@@ -763,15 +763,15 @@
         },
         {
             "arena_code": "vma",
             "card_count": 1,
             "code": "vma",
             "digital": true,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/vma.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/vma.svg?1688961600",
             "id": "a944551a-73fa-41cd-9159-e8d0e4674403",
             "mtgo_code": "vma",
             "name": "Vintage Masters",
             "nonfoil_only": false,
             "object": "set",
             "printed_size": 325,
             "released_at": "2014-06-16",
@@ -782,15 +782,15 @@
         },
         {
             "arena_code": "w16",
             "card_count": 1,
             "code": "w16",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/w16.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/w16.svg?1688961600",
             "id": "b3a0e4a1-5f2c-44e1-8558-61e6dcd88fda",
             "mtgo_code": "w16",
             "name": "Welcome Deck 2016",
             "nonfoil_only": true,
             "object": "set",
             "released_at": "2016-04-08",
             "scryfall_uri": "https://scryfall.com/sets/w16",
```

### Comparing `mtg_ssm-2.6.2.dev1/tests/data/sets1.json` & `mtg_ssm-2.6.2.dev2/tests/data/sets1.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9963587170979502%*

 * *Differences: {"'data'": "{0: {'icon_svg_uri': 'https://svgs.scryfall.io/sets/arc.svg?1688961600'}, 1: "*

 * *           "{'icon_svg_uri': 'https://svgs.scryfall.io/sets/bok.svg?1688961600'}, 2: "*

 * *           "{'icon_svg_uri': 'https://svgs.scryfall.io/sets/chk.svg?1688961600'}, 3: "*

 * *           "{'icon_svg_uri': 'https://svgs.scryfall.io/sets/csp.svg?1688961600'}, 4: "*

 * *           "{'icon_svg_uri': 'https://svgs.scryfall.io/sets/fem.svg?1688961600'}, 5: "*

 * *           "{'icon_svg_uri': 'https://svgs.scryfall.io/sets/hml.svg?16889 […]*

```diff
@@ -1,15 +1,15 @@
 {
     "data": [
         {
             "card_count": 1,
             "code": "arc",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/arc.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/arc.svg?1688961600",
             "id": "8bc5ec64-18d5-4c81-96a1-8f619d81a019",
             "name": "Archenemy",
             "nonfoil_only": true,
             "object": "set",
             "released_at": "2010-06-18",
             "scryfall_uri": "https://scryfall.com/sets/arc",
             "search_uri": "https://api.scryfall.com/cards/search?include_extras=true&include_variations=true&order=set&q=e%3Aarc&unique=prints",
@@ -21,15 +21,15 @@
             "arena_code": "bok",
             "block": "Kamigawa",
             "block_code": "chk",
             "card_count": 1,
             "code": "bok",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/bok.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/bok.svg?1688961600",
             "id": "d4b88587-a1f5-4b47-9e24-78ec9e57bd0e",
             "mtgo_code": "bok",
             "name": "Betrayers of Kamigawa",
             "nonfoil_only": false,
             "object": "set",
             "printed_size": 165,
             "released_at": "2005-02-04",
@@ -43,15 +43,15 @@
             "arena_code": "chk",
             "block": "Kamigawa",
             "block_code": "chk",
             "card_count": 2,
             "code": "chk",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/chk.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/chk.svg?1688961600",
             "id": "6183d21f-a0af-4118-ba58-aca1d8719c01",
             "mtgo_code": "chk",
             "name": "Champions of Kamigawa",
             "nonfoil_only": false,
             "object": "set",
             "printed_size": 306,
             "released_at": "2004-10-01",
@@ -65,15 +65,15 @@
             "arena_code": "csp",
             "block": "Ice Age",
             "block_code": "ice",
             "card_count": 1,
             "code": "csp",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/csp.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/csp.svg?1688961600",
             "id": "1f4f105f-73e4-4f03-849e-82a204807847",
             "mtgo_code": "csp",
             "name": "Coldsnap",
             "nonfoil_only": false,
             "object": "set",
             "printed_size": 155,
             "released_at": "2006-07-21",
@@ -84,15 +84,15 @@
             "uri": "https://api.scryfall.com/sets/1f4f105f-73e4-4f03-849e-82a204807847"
         },
         {
             "card_count": 4,
             "code": "fem",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/fem.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/fem.svg?1688961600",
             "id": "cf7390b1-341a-4ae8-a325-da0f5f322f13",
             "name": "Fallen Empires",
             "nonfoil_only": true,
             "object": "set",
             "released_at": "1994-11-01",
             "scryfall_uri": "https://scryfall.com/sets/fem",
             "search_uri": "https://api.scryfall.com/cards/search?include_extras=true&include_variations=true&order=set&q=e%3Afem&unique=prints",
@@ -101,15 +101,15 @@
             "uri": "https://api.scryfall.com/sets/cf7390b1-341a-4ae8-a325-da0f5f322f13"
         },
         {
             "card_count": 2,
             "code": "hml",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/hml.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/hml.svg?1688961600",
             "id": "5ac1f606-e682-46e9-ad0f-122a3783581b",
             "name": "Homelands",
             "nonfoil_only": true,
             "object": "set",
             "released_at": "1995-10-01",
             "scryfall_uri": "https://scryfall.com/sets/hml",
             "search_uri": "https://api.scryfall.com/cards/search?include_extras=true&include_variations=true&order=set&q=e%3Ahml&unique=prints",
@@ -119,15 +119,15 @@
         },
         {
             "arena_code": "pc1",
             "card_count": 2,
             "code": "hop",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/hop.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/hop.svg?1688961600",
             "id": "7137ffeb-eb1d-466c-a0d3-3157f52b1b10",
             "mtgo_code": "pc1",
             "name": "Planechase",
             "nonfoil_only": true,
             "object": "set",
             "released_at": "2009-09-04",
             "scryfall_uri": "https://scryfall.com/sets/hop",
@@ -139,15 +139,15 @@
         {
             "block": "Ice Age",
             "block_code": "ice",
             "card_count": 5,
             "code": "ice",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/ice.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/ice.svg?1688961600",
             "id": "b0e08eea-5c01-4406-a6e2-dcd09c5e5b67",
             "name": "Ice Age",
             "nonfoil_only": true,
             "object": "set",
             "released_at": "1995-06-03",
             "scryfall_uri": "https://scryfall.com/sets/ice",
             "search_uri": "https://api.scryfall.com/cards/search?include_extras=true&include_variations=true&order=set&q=e%3Aice&unique=prints",
@@ -159,15 +159,15 @@
             "arena_code": "isd",
             "block": "Innistrad",
             "block_code": "isd",
             "card_count": 5,
             "code": "isd",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/isd.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/isd.svg?1688961600",
             "id": "d1026945-2969-42b9-be53-f941405a58cb",
             "mtgo_code": "isd",
             "name": "Innistrad",
             "nonfoil_only": false,
             "object": "set",
             "printed_size": 264,
             "released_at": "2011-09-30",
@@ -179,15 +179,15 @@
         },
         {
             "arena_code": "khm",
             "card_count": 3,
             "code": "khm",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/khm.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/khm.svg?1688961600",
             "id": "43057fad-b1c1-437f-bc48-0045bce6d8c9",
             "mtgo_code": "khm",
             "name": "Kaldheim",
             "nonfoil_only": false,
             "object": "set",
             "released_at": "2021-02-05",
             "scryfall_uri": "https://scryfall.com/sets/khm",
@@ -199,15 +199,15 @@
         {
             "block": "Core Set",
             "block_code": "lea",
             "card_count": 4,
             "code": "lea",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/lea.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/lea.svg?1688961600",
             "id": "288bd996-960e-448b-a187-9504c1930c2c",
             "name": "Limited Edition Alpha",
             "nonfoil_only": true,
             "object": "set",
             "released_at": "1993-08-05",
             "scryfall_uri": "https://scryfall.com/sets/lea",
             "search_uri": "https://api.scryfall.com/cards/search?include_extras=true&include_variations=true&order=set&q=e%3Alea&unique=prints",
@@ -219,15 +219,15 @@
             "arena_code": "mbs",
             "block": "Scars of Mirrodin",
             "block_code": "som",
             "card_count": 2,
             "code": "mbs",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/mbs.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/mbs.svg?1688961600",
             "id": "f46c57e3-9301-4006-a6ca-06f3f65961fb",
             "mtgo_code": "mbs",
             "name": "Mirrodin Besieged",
             "nonfoil_only": false,
             "object": "set",
             "printed_size": 155,
             "released_at": "2011-02-04",
@@ -239,15 +239,15 @@
         },
         {
             "arena_code": "mma",
             "card_count": 1,
             "code": "mma",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/mma.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/mma.svg?1688961600",
             "id": "0b7020f2-336d-4706-9ce6-f6710b9ebd5c",
             "mtgo_code": "mma",
             "name": "Modern Masters",
             "nonfoil_only": false,
             "object": "set",
             "printed_size": 229,
             "released_at": "2013-06-07",
@@ -259,15 +259,15 @@
         },
         {
             "arena_code": "neo",
             "card_count": 3,
             "code": "neo",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/neo.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/neo.svg?1688961600",
             "id": "59a2059f-5482-433f-8761-eb2e17859b71",
             "mtgo_code": "neo",
             "name": "Kamigawa: Neon Dynasty",
             "nonfoil_only": false,
             "object": "set",
             "printed_size": 302,
             "released_at": "2022-02-18",
@@ -278,15 +278,15 @@
             "uri": "https://api.scryfall.com/sets/59a2059f-5482-433f-8761-eb2e17859b71"
         },
         {
             "card_count": 1,
             "code": "oarc",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/arc.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/arc.svg?1688961600",
             "id": "238beedf-1d4d-475f-a980-527ba2f55dc6",
             "name": "Archenemy Schemes",
             "nonfoil_only": true,
             "object": "set",
             "parent_set_code": "arc",
             "released_at": "2010-06-18",
             "scryfall_uri": "https://scryfall.com/sets/oarc",
@@ -298,15 +298,15 @@
             "arena_code": "ogw",
             "block": "Battle for Zendikar",
             "block_code": "bfz",
             "card_count": 4,
             "code": "ogw",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/ogw.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/ogw.svg?1688961600",
             "id": "cd51d245-8f95-45b0-ab5f-e2b3a3eb5dfe",
             "mtgo_code": "ogw",
             "name": "Oath of the Gatewatch",
             "nonfoil_only": false,
             "object": "set",
             "printed_size": 184,
             "released_at": "2016-01-22",
@@ -318,15 +318,15 @@
         },
         {
             "arena_code": "ohop",
             "card_count": 1,
             "code": "ohop",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/hop.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/hop.svg?1688961600",
             "id": "7a8b75a9-7c92-4c3f-976a-322e1eb3b6b6",
             "mtgo_code": "ohop",
             "name": "Planechase Planes",
             "nonfoil_only": true,
             "object": "set",
             "parent_set_code": "hop",
             "released_at": "2009-09-04",
@@ -337,15 +337,15 @@
         },
         {
             "arena_code": "opc2",
             "card_count": 2,
             "code": "opc2",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/pc2.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/pc2.svg?1688961600",
             "id": "7079031b-c5b0-4353-87af-a63a0f204f47",
             "mtgo_code": "opc2",
             "name": "Planechase 2012 Planes",
             "nonfoil_only": true,
             "object": "set",
             "parent_set_code": "pc2",
             "released_at": "2012-06-01",
@@ -357,15 +357,15 @@
         {
             "block": "Magic Player Rewards",
             "block_code": "mpr",
             "card_count": 1,
             "code": "p03",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/dci.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/dci.svg?1688961600",
             "id": "dfa906ff-63d8-4065-abef-809988337288",
             "name": "Magic Player Rewards 2003",
             "nonfoil_only": true,
             "object": "set",
             "released_at": "2003-01-01",
             "scryfall_uri": "https://scryfall.com/sets/p03",
             "search_uri": "https://api.scryfall.com/cards/search?include_extras=true&include_variations=true&order=set&q=e%3Ap03&unique=prints",
@@ -374,15 +374,15 @@
         },
         {
             "arena_code": "pc2",
             "card_count": 1,
             "code": "pc2",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/pc2.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/pc2.svg?1688961600",
             "id": "9fb2f83e-7015-4aa9-808f-310ccf0fdb9c",
             "mtgo_code": "pc2",
             "name": "Planechase 2012",
             "nonfoil_only": true,
             "object": "set",
             "released_at": "2012-06-01",
             "scryfall_uri": "https://scryfall.com/sets/pc2",
@@ -392,15 +392,15 @@
             "uri": "https://api.scryfall.com/sets/9fb2f83e-7015-4aa9-808f-310ccf0fdb9c"
         },
         {
             "card_count": 2,
             "code": "pdci",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/dci.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/dci.svg?1688961600",
             "id": "935e91e9-61c2-4b35-a85a-c08fef3b420b",
             "name": "DCI Promos",
             "nonfoil_only": false,
             "object": "set",
             "released_at": "2006-01-01",
             "scryfall_uri": "https://scryfall.com/sets/pdci",
             "search_uri": "https://api.scryfall.com/cards/search?include_extras=true&include_variations=true&order=set&q=e%3Apdci&unique=prints",
```

### Comparing `mtg_ssm-2.6.2.dev1/tests/data/sets2.json` & `mtg_ssm-2.6.2.dev2/tests/data/sets2.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9949410319683428%*

 * *Differences: {"'data'": "{0: {'icon_svg_uri': 'https://svgs.scryfall.io/sets/frf.svg?1688961600'}, 1: "*

 * *           "{'icon_svg_uri': 'https://svgs.scryfall.io/sets/dci.svg?1688961600'}, 2: "*

 * *           "{'icon_svg_uri': 'https://svgs.scryfall.io/sets/pbook.svg?1688961600'}, 3: "*

 * *           "{'icon_svg_uri': 'https://svgs.scryfall.io/sets/plc.svg?1688961600'}, 4: "*

 * *           "{'icon_svg_uri': 'https://svgs.scryfall.io/sets/pls.svg?1688961600'}, 5: "*

 * *           "{'icon_svg_uri': 'https://svgs.scryfall.io/sets/mbs.svg?168 […]*

```diff
@@ -3,15 +3,15 @@
         {
             "block": "Khans of Tarkir",
             "block_code": "ktk",
             "card_count": 2,
             "code": "pfrf",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/frf.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/frf.svg?1688961600",
             "id": "aa9f80e3-8d60-46b7-b91e-eb1736fde866",
             "name": "Fate Reforged Promos",
             "nonfoil_only": false,
             "object": "set",
             "parent_set_code": "frf",
             "released_at": "2015-01-23",
             "scryfall_uri": "https://scryfall.com/sets/pfrf",
@@ -20,15 +20,15 @@
             "uri": "https://api.scryfall.com/sets/aa9f80e3-8d60-46b7-b91e-eb1736fde866"
         },
         {
             "card_count": 1,
             "code": "phop",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/dci.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/dci.svg?1688961600",
             "id": "ef3f6784-a6e8-41ff-8bed-72e0c7121298",
             "name": "Planechase Promos",
             "nonfoil_only": true,
             "object": "set",
             "parent_set_code": "hop",
             "released_at": "2009-09-04",
             "scryfall_uri": "https://scryfall.com/sets/phop",
@@ -37,15 +37,15 @@
             "uri": "https://api.scryfall.com/sets/ef3f6784-a6e8-41ff-8bed-72e0c7121298"
         },
         {
             "card_count": 1,
             "code": "phpr",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/pbook.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/pbook.svg?1688961600",
             "id": "b32cc4a1-1e06-4bec-bab6-89b2691b57a4",
             "name": "HarperPrism Book Promos",
             "nonfoil_only": true,
             "object": "set",
             "released_at": "1994-09-01",
             "scryfall_uri": "https://scryfall.com/sets/phpr",
             "search_uri": "https://api.scryfall.com/cards/search?include_extras=true&include_variations=true&order=set&q=e%3Aphpr&unique=prints",
@@ -56,15 +56,15 @@
             "arena_code": "plc",
             "block": "Time Spiral",
             "block_code": "tsp",
             "card_count": 1,
             "code": "plc",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/plc.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/plc.svg?1688961600",
             "id": "5a1b571c-73e9-4c14-b9d4-a62507d85789",
             "mtgo_code": "plc",
             "name": "Planar Chaos",
             "nonfoil_only": false,
             "object": "set",
             "printed_size": 165,
             "released_at": "2007-02-02",
@@ -78,15 +78,15 @@
             "arena_code": "ps",
             "block": "Invasion",
             "block_code": "inv",
             "card_count": 2,
             "code": "pls",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/pls.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/pls.svg?1688961600",
             "id": "82dc193b-bd5f-4883-a93f-a4155b467ee0",
             "mtgo_code": "ps",
             "name": "Planeshift",
             "nonfoil_only": false,
             "object": "set",
             "printed_size": 143,
             "released_at": "2001-02-05",
@@ -99,15 +99,15 @@
         {
             "block": "Scars of Mirrodin",
             "block_code": "som",
             "card_count": 1,
             "code": "pmbs",
             "digital": false,
             "foil_only": true,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/mbs.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/mbs.svg?1688961600",
             "id": "8a59d98a-4e13-4943-b06c-b35868e954ba",
             "name": "Mirrodin Besieged Promos",
             "nonfoil_only": false,
             "object": "set",
             "parent_set_code": "mbs",
             "released_at": "2011-02-03",
             "scryfall_uri": "https://scryfall.com/sets/pmbs",
@@ -116,15 +116,15 @@
             "uri": "https://api.scryfall.com/sets/8a59d98a-4e13-4943-b06c-b35868e954ba"
         },
         {
             "card_count": 2,
             "code": "pneo",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/neo.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/neo.svg?1688961600",
             "id": "b3161020-d74f-48cc-bc9d-d7233e64e524",
             "name": "Kamigawa: Neon Dynasty Promos",
             "nonfoil_only": false,
             "object": "set",
             "parent_set_code": "neo",
             "released_at": "2022-02-18",
             "scryfall_uri": "https://scryfall.com/sets/pneo",
@@ -135,15 +135,15 @@
         {
             "block": "Guilds of Ravnica",
             "block_code": "grn",
             "card_count": 2,
             "code": "prna",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/rna.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/rna.svg?1688961600",
             "id": "503230ec-81e3-4f92-b847-ff435b1652e0",
             "name": "Ravnica Allegiance Promos",
             "nonfoil_only": false,
             "object": "set",
             "parent_set_code": "rna",
             "released_at": "2019-01-25",
             "scryfall_uri": "https://scryfall.com/sets/prna",
@@ -154,15 +154,15 @@
         {
             "block": "Guilds of Ravnica",
             "block_code": "grn",
             "card_count": 2,
             "code": "prw2",
             "digital": false,
             "foil_only": true,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/rna.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/rna.svg?1688961600",
             "id": "ee3a8eb6-0583-492b-8be5-265795d38038",
             "name": "RNA Ravnica Weekend",
             "nonfoil_only": false,
             "object": "set",
             "parent_set_code": "rna",
             "released_at": "2019-02-16",
             "scryfall_uri": "https://scryfall.com/sets/prw2",
@@ -171,15 +171,15 @@
             "uri": "https://api.scryfall.com/sets/ee3a8eb6-0583-492b-8be5-265795d38038"
         },
         {
             "card_count": 1,
             "code": "ptg",
             "digital": false,
             "foil_only": true,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/ptg.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/ptg.svg?1688961600",
             "id": "d264b61b-bfb3-4388-be42-e34a1eaa00c2",
             "name": "Ponies: The Galloping",
             "nonfoil_only": false,
             "object": "set",
             "released_at": "2019-10-22",
             "scryfall_uri": "https://scryfall.com/sets/ptg",
             "search_uri": "https://api.scryfall.com/cards/search?include_extras=true&include_variations=true&order=set&q=e%3Aptg&unique=prints",
@@ -188,15 +188,15 @@
             "uri": "https://api.scryfall.com/sets/d264b61b-bfb3-4388-be42-e34a1eaa00c2"
         },
         {
             "card_count": 1,
             "code": "ren",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/ren.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/ren.svg?1688961600",
             "id": "bec33d25-cf6f-460f-918d-29b3009686bb",
             "name": "Renaissance",
             "nonfoil_only": true,
             "object": "set",
             "released_at": "1995-08-01",
             "scryfall_uri": "https://scryfall.com/sets/ren",
             "search_uri": "https://api.scryfall.com/cards/search?include_extras=true&include_variations=true&order=set&q=e%3Aren&unique=prints",
@@ -208,15 +208,15 @@
             "arena_code": "rna",
             "block": "Guilds of Ravnica",
             "block_code": "grn",
             "card_count": 1,
             "code": "rna",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/rna.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/rna.svg?1688961600",
             "id": "97a7fd84-8d89-45a3-b48b-c951f6a3f9f1",
             "mtgo_code": "rna",
             "name": "Ravnica Allegiance",
             "nonfoil_only": false,
             "object": "set",
             "printed_size": 259,
             "released_at": "2019-01-25",
@@ -227,15 +227,15 @@
             "uri": "https://api.scryfall.com/sets/97a7fd84-8d89-45a3-b48b-c951f6a3f9f1"
         },
         {
             "card_count": 1,
             "code": "s00",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/s00.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/s00.svg?1688961600",
             "id": "1c105623-2564-40d7-a3aa-4134787fb127",
             "name": "Starter 2000",
             "nonfoil_only": false,
             "object": "set",
             "released_at": "2000-04-01",
             "scryfall_uri": "https://scryfall.com/sets/s00",
             "search_uri": "https://api.scryfall.com/cards/search?include_extras=true&include_variations=true&order=set&q=e%3As00&unique=prints",
@@ -244,15 +244,15 @@
             "uri": "https://api.scryfall.com/sets/1c105623-2564-40d7-a3aa-4134787fb127"
         },
         {
             "card_count": 3,
             "code": "sld",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/star.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/star.svg?1688961600",
             "id": "4d92a8a7-ccb0-437d-abdc-9d70fc5ed672",
             "name": "Secret Lair Drop",
             "nonfoil_only": false,
             "object": "set",
             "released_at": "2019-12-02",
             "scryfall_uri": "https://scryfall.com/sets/sld",
             "search_uri": "https://api.scryfall.com/cards/search?include_extras=true&include_variations=true&order=set&q=e%3Asld&unique=prints",
@@ -264,15 +264,15 @@
             "arena_code": "sok",
             "block": "Kamigawa",
             "block_code": "chk",
             "card_count": 1,
             "code": "sok",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/sok.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/sok.svg?1688961600",
             "id": "4db16ad3-2b95-442f-bb6b-e9aa7fe7f769",
             "mtgo_code": "sok",
             "name": "Saviors of Kamigawa",
             "nonfoil_only": false,
             "object": "set",
             "printed_size": 165,
             "released_at": "2005-06-03",
@@ -283,15 +283,15 @@
             "uri": "https://api.scryfall.com/sets/4db16ad3-2b95-442f-bb6b-e9aa7fe7f769"
         },
         {
             "card_count": 1,
             "code": "sunf",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/unf.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/unf.svg?1688961600",
             "id": "565e3302-2fed-487e-a0f7-7f8037d25030",
             "name": "Unfinity Sticker Sheets",
             "nonfoil_only": true,
             "object": "set",
             "parent_set_code": "unf",
             "released_at": "2022-10-07",
             "scryfall_uri": "https://scryfall.com/sets/sunf",
@@ -301,15 +301,15 @@
         },
         {
             "arena_code": "thb",
             "card_count": 8,
             "code": "thb",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/thb.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/thb.svg?1688961600",
             "id": "5f23a78d-cda1-462a-8be3-a62b40c34913",
             "mtgo_code": "thb",
             "name": "Theros Beyond Death",
             "nonfoil_only": false,
             "object": "set",
             "released_at": "2020-01-24",
             "scryfall_uri": "https://scryfall.com/sets/thb",
@@ -319,15 +319,15 @@
             "uri": "https://api.scryfall.com/sets/5f23a78d-cda1-462a-8be3-a62b40c34913"
         },
         {
             "card_count": 1,
             "code": "unh",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/unh.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/unh.svg?1688961600",
             "id": "4c8bc76a-05a5-43db-aaf0-34deb347b871",
             "name": "Unhinged",
             "nonfoil_only": false,
             "object": "set",
             "printed_size": 141,
             "released_at": "2004-11-19",
             "scryfall_uri": "https://scryfall.com/sets/unh",
@@ -337,15 +337,15 @@
             "uri": "https://api.scryfall.com/sets/4c8bc76a-05a5-43db-aaf0-34deb347b871"
         },
         {
             "card_count": 6,
             "code": "ust",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/ust.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/ust.svg?1688961600",
             "id": "83491685-880d-41dd-a4af-47d2b3b17c10",
             "name": "Unstable",
             "nonfoil_only": false,
             "object": "set",
             "printed_size": 268,
             "released_at": "2017-12-08",
             "scryfall_uri": "https://scryfall.com/sets/ust",
@@ -356,15 +356,15 @@
         },
         {
             "arena_code": "vma",
             "card_count": 1,
             "code": "vma",
             "digital": true,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/vma.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/vma.svg?1688961600",
             "id": "a944551a-73fa-41cd-9159-e8d0e4674403",
             "mtgo_code": "vma",
             "name": "Vintage Masters",
             "nonfoil_only": false,
             "object": "set",
             "printed_size": 325,
             "released_at": "2014-06-16",
@@ -375,15 +375,15 @@
         },
         {
             "arena_code": "w16",
             "card_count": 1,
             "code": "w16",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/w16.svg?1678680000",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/w16.svg?1688961600",
             "id": "b3a0e4a1-5f2c-44e1-8558-61e6dcd88fda",
             "mtgo_code": "w16",
             "name": "Welcome Deck 2016",
             "nonfoil_only": true,
             "object": "set",
             "released_at": "2016-04-08",
             "scryfall_uri": "https://scryfall.com/sets/w16",
```

### Comparing `mtg_ssm-2.6.2.dev1/tests/gen_testdata.py` & `mtg_ssm-2.6.2.dev2/tests/gen_testdata.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/tests/mtg/test_util.py` & `mtg_ssm-2.6.2.dev2/tests/mtg/test_util.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/tests/scryfall/test_fetcher.py` & `mtg_ssm-2.6.2.dev2/tests/scryfall/test_fetcher.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/tests/serialization/__snapshots__/test_csv.ambr` & `mtg_ssm-2.6.2.dev2/tests/serialization/__snapshots__/test_csv.ambr`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/tests/serialization/__snapshots__/test_xlsx.ambr` & `mtg_ssm-2.6.2.dev2/tests/serialization/__snapshots__/test_xlsx.ambr`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/tests/serialization/test_csv.py` & `mtg_ssm-2.6.2.dev2/tests/serialization/test_csv.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/tests/serialization/test_interface.py` & `mtg_ssm-2.6.2.dev2/tests/serialization/test_interface.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/tests/serialization/test_xlsx.py` & `mtg_ssm-2.6.2.dev2/tests/serialization/test_xlsx.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev1/tests/test_ssm.py` & `mtg_ssm-2.6.2.dev2/tests/test_ssm.py`

 * *Files identical despite different names*

