# Comparing `tmp/mtg_ssm-2.6.1.dev1.tar.gz` & `tmp/mtg_ssm-2.6.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtg_ssm-2.6.1.dev1.tar", last modified: Thu Mar 16 18:56:57 2023, max compression
+gzip compressed data, was "mtg_ssm-2.6.2.dev1.tar", last modified: Thu Jul 13 08:16:06 2023, max compression
```

## Comparing `mtg_ssm-2.6.1.dev1.tar` & `mtg_ssm-2.6.2.dev1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:56:57.740095 mtg_ssm-2.6.1.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:56:57.732094 mtg_ssm-2.6.1.dev1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:56:57.732094 mtg_ssm-2.6.1.dev1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/.github/workflows/integration.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11823 2023-03-16 18:56:57.740095 mtg_ssm-2.6.1.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10531 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/TODO.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:56:57.732094 mtg_ssm-2.6.1.dev1/mtg_ssm/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/mtg_ssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-16 18:56:57.000000 mtg_ssm-2.6.1.dev1/mtg_ssm/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:56:57.736094 mtg_ssm-2.6.1.dev1/mtg_ssm/containers/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/mtg_ssm/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/mtg_ssm/containers/bundles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/mtg_ssm/containers/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/mtg_ssm/containers/counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/mtg_ssm/containers/indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/mtg_ssm/containers/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:56:57.736094 mtg_ssm-2.6.1.dev1/mtg_ssm/mtg/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/mtg_ssm/mtg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/mtg_ssm/mtg/util.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/mtg_ssm/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:56:57.736094 mtg_ssm-2.6.1.dev1/mtg_ssm/scryfall/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/mtg_ssm/scryfall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/mtg_ssm/scryfall/fetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    11261 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/mtg_ssm/scryfall/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:56:57.736094 mtg_ssm-2.6.1.dev1/mtg_ssm/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/mtg_ssm/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/mtg_ssm/serialization/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/mtg_ssm/serialization/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/mtg_ssm/serialization/xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)    10331 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/mtg_ssm/ssm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:56:57.732094 mtg_ssm-2.6.1.dev1/mtg_ssm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11823 2023-03-16 18:56:57.000000 mtg_ssm-2.6.1.dev1/mtg_ssm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-03-16 18:56:57.000000 mtg_ssm-2.6.1.dev1/mtg_ssm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 18:56:57.000000 mtg_ssm-2.6.1.dev1/mtg_ssm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-16 18:56:57.000000 mtg_ssm-2.6.1.dev1/mtg_ssm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-03-16 18:56:57.000000 mtg_ssm-2.6.1.dev1/mtg_ssm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-16 18:56:57.000000 mtg_ssm-2.6.1.dev1/mtg_ssm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 18:56:57.740095 mtg_ssm-2.6.1.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:56:57.736094 mtg_ssm-2.6.1.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:56:57.736094 mtg_ssm-2.6.1.dev1/tests/containers/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/tests/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/tests/containers/test_bundles.py
--rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/tests/containers/test_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/tests/containers/test_indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/tests/containers/test_legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:56:57.740095 mtg_ssm-2.6.1.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/tests/data/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/tests/data/bulk_data.json
--rw-r--r--   0 runner    (1001) docker     (123)   453985 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/tests/data/cards.json
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/tests/data/migrations.json
--rw-r--r--   0 runner    (1001) docker     (123)    31317 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/tests/data/sets.json
--rw-r--r--   0 runner    (1001) docker     (123)    15912 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/tests/data/sets1.json
--rw-r--r--   0 runner    (1001) docker     (123)    15519 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/tests/data/sets2.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     6683 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/tests/gen_testdata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:56:57.740095 mtg_ssm-2.6.1.dev1/tests/mtg/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/tests/mtg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/tests/mtg/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:56:57.740095 mtg_ssm-2.6.1.dev1/tests/scryfall/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/tests/scryfall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/tests/scryfall/test_fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:56:57.740095 mtg_ssm-2.6.1.dev1/tests/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/tests/serialization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 18:56:57.740095 mtg_ssm-2.6.1.dev1/tests/serialization/__snapshots__/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/tests/serialization/__snapshots__/test_csv.ambr
--rw-r--r--   0 runner    (1001) docker     (123)    22100 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/tests/serialization/__snapshots__/test_xlsx.ambr
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/tests/serialization/test_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/tests/serialization/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/tests/serialization/test_xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)    16267 2023-03-16 18:56:41.000000 mtg_ssm-2.6.1.dev1/tests/test_ssm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.377427 mtg_ssm-2.6.2.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.369427 mtg_ssm-2.6.2.dev1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.369427 mtg_ssm-2.6.2.dev1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/.github/workflows/integration.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-07-13 08:16:06.377427 mtg_ssm-2.6.2.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/TODO.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.369427 mtg_ssm-2.6.2.dev1/mtg_ssm/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-13 08:16:06.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.369427 mtg_ssm-2.6.2.dev1/mtg_ssm/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/containers/bundles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/containers/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/containers/counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/containers/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/containers/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.369427 mtg_ssm-2.6.2.dev1/mtg_ssm/mtg/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/mtg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/mtg/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.373427 mtg_ssm-2.6.2.dev1/mtg_ssm/scryfall/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/scryfall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/scryfall/fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/scryfall/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.373427 mtg_ssm-2.6.2.dev1/mtg_ssm/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/serialization/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/serialization/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/serialization/xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10331 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/mtg_ssm/ssm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.369427 mtg_ssm-2.6.2.dev1/mtg_ssm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-07-13 08:16:06.000000 mtg_ssm-2.6.2.dev1/mtg_ssm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-13 08:16:06.000000 mtg_ssm-2.6.2.dev1/mtg_ssm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 08:16:06.000000 mtg_ssm-2.6.2.dev1/mtg_ssm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 08:16:06.000000 mtg_ssm-2.6.2.dev1/mtg_ssm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-13 08:16:06.000000 mtg_ssm-2.6.2.dev1/mtg_ssm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 08:16:06.000000 mtg_ssm-2.6.2.dev1/mtg_ssm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 08:16:06.377427 mtg_ssm-2.6.2.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.373427 mtg_ssm-2.6.2.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.373427 mtg_ssm-2.6.2.dev1/tests/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/containers/test_bundles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/containers/test_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/containers/test_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/containers/test_legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.373427 mtg_ssm-2.6.2.dev1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/data/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/data/bulk_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)   456696 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/data/cards.json
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/data/migrations.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31317 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/data/sets.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15912 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/data/sets1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15519 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/data/sets2.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6683 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/gen_testdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.373427 mtg_ssm-2.6.2.dev1/tests/mtg/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/mtg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/mtg/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.373427 mtg_ssm-2.6.2.dev1/tests/scryfall/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/scryfall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/scryfall/test_fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.377427 mtg_ssm-2.6.2.dev1/tests/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/serialization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:16:06.377427 mtg_ssm-2.6.2.dev1/tests/serialization/__snapshots__/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/serialization/__snapshots__/test_csv.ambr
+-rw-r--r--   0 runner    (1001) docker     (123)    22102 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/serialization/__snapshots__/test_xlsx.ambr
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/serialization/test_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/serialization/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/serialization/test_xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16267 2023-07-13 08:15:57.000000 mtg_ssm-2.6.2.dev1/tests/test_ssm.py
```

### Comparing `mtg_ssm-2.6.1.dev1/.github/workflows/integration.yml` & `mtg_ssm-2.6.2.dev1/.github/workflows/integration.yml`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/.github/workflows/run-tests.yml` & `mtg_ssm-2.6.2.dev1/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/.gitignore` & `mtg_ssm-2.6.2.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/.pre-commit-config.yaml` & `mtg_ssm-2.6.2.dev1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/LICENSE.txt` & `mtg_ssm-2.6.2.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/PKG-INFO` & `mtg_ssm-2.6.2.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtg_ssm
-Version: 2.6.1.dev1
+Version: 2.6.2.dev1
 Summary: A tool to manage Magic: the Gathering collection spreadsheets
 Author-email: George Leslie-Waksman <waksman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/gwax/mtg_ssm
 Project-URL: Bug Tracker, https://github.com/gwax/mtg_ssm/issues
 Keywords: mtg,magic,collection,tracking,spreadsheet
 Classifier: Development Status :: 5 - Production/Stable
@@ -196,14 +196,19 @@
 =========
 
 Development
 -----------
 
 -   ...
 
+2.6.1
+-----
+
+-   Minor Scryfall data changes.
+
 2.6.0
 -----
 
 -   Fix a bunch of tests for scryfall data changes, which change a number of
     promo set card assignments.
 -   Add "minigame" to scryfall set type.
 -   Improved scryfall caching performance and decreased cache folder size
```

### Comparing `mtg_ssm-2.6.1.dev1/README.rst` & `mtg_ssm-2.6.2.dev1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -164,14 +164,19 @@
 =========
 
 Development
 -----------
 
 -   ...
 
+2.6.1
+-----
+
+-   Minor Scryfall data changes.
+
 2.6.0
 -----
 
 -   Fix a bunch of tests for scryfall data changes, which change a number of
     promo set card assignments.
 -   Add "minigame" to scryfall set type.
 -   Improved scryfall caching performance and decreased cache folder size
```

### Comparing `mtg_ssm-2.6.1.dev1/mtg_ssm/containers/bundles.py` & `mtg_ssm-2.6.2.dev1/mtg_ssm/containers/bundles.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/mtg_ssm/containers/collection.py` & `mtg_ssm-2.6.2.dev1/mtg_ssm/containers/collection.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/mtg_ssm/containers/counts.py` & `mtg_ssm-2.6.2.dev1/mtg_ssm/containers/counts.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/mtg_ssm/containers/indexes.py` & `mtg_ssm-2.6.2.dev1/mtg_ssm/containers/indexes.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/mtg_ssm/containers/legacy.py` & `mtg_ssm-2.6.2.dev1/mtg_ssm/containers/legacy.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/mtg_ssm/mtg/util.py` & `mtg_ssm-2.6.2.dev1/mtg_ssm/mtg/util.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/mtg_ssm/scryfall/fetcher.py` & `mtg_ssm-2.6.2.dev1/mtg_ssm/scryfall/fetcher.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/mtg_ssm/scryfall/models.py` & `mtg_ssm-2.6.2.dev1/mtg_ssm/scryfall/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,14 +199,15 @@
     GLADIATOR = "gladiator"
     EXPLORER = "explorer"
     HISTORICBRAWL = "historicbrawl"
     ALCHEMY = "alchemy"
     PAUPERCOMMANDER = "paupercommander"
     PREMODERN = "premodern"
     PREDH = "predh"
+    OATHBREAKER = "oathbreaker"
 
 
 class ScryLegality(str, Enum):
     """Enum for card legalities values"""
 
     LEGAL = "legal"
     NOT_LEGAL = "not_legal"
```

### Comparing `mtg_ssm-2.6.1.dev1/mtg_ssm/serialization/csv.py` & `mtg_ssm-2.6.2.dev1/mtg_ssm/serialization/csv.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/mtg_ssm/serialization/interface.py` & `mtg_ssm-2.6.2.dev1/mtg_ssm/serialization/interface.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/mtg_ssm/serialization/xlsx.py` & `mtg_ssm-2.6.2.dev1/mtg_ssm/serialization/xlsx.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/mtg_ssm/ssm.py` & `mtg_ssm-2.6.2.dev1/mtg_ssm/ssm.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/mtg_ssm.egg-info/PKG-INFO` & `mtg_ssm-2.6.2.dev1/mtg_ssm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtg-ssm
-Version: 2.6.1.dev1
+Version: 2.6.2.dev1
 Summary: A tool to manage Magic: the Gathering collection spreadsheets
 Author-email: George Leslie-Waksman <waksman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/gwax/mtg_ssm
 Project-URL: Bug Tracker, https://github.com/gwax/mtg_ssm/issues
 Keywords: mtg,magic,collection,tracking,spreadsheet
 Classifier: Development Status :: 5 - Production/Stable
@@ -196,14 +196,19 @@
 =========
 
 Development
 -----------
 
 -   ...
 
+2.6.1
+-----
+
+-   Minor Scryfall data changes.
+
 2.6.0
 -----
 
 -   Fix a bunch of tests for scryfall data changes, which change a number of
     promo set card assignments.
 -   Add "minigame" to scryfall set type.
 -   Improved scryfall caching performance and decreased cache folder size
```

### Comparing `mtg_ssm-2.6.1.dev1/mtg_ssm.egg-info/SOURCES.txt` & `mtg_ssm-2.6.2.dev1/mtg_ssm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/pylintrc` & `mtg_ssm-2.6.2.dev1/pylintrc`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/pyproject.toml` & `mtg_ssm-2.6.2.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/tests/conftest.py` & `mtg_ssm-2.6.2.dev1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/tests/containers/test_bundles.py` & `mtg_ssm-2.6.2.dev1/tests/containers/test_bundles.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/tests/containers/test_counts.py` & `mtg_ssm-2.6.2.dev1/tests/containers/test_counts.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/tests/containers/test_indexes.py` & `mtg_ssm-2.6.2.dev1/tests/containers/test_indexes.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/tests/containers/test_legacy.py` & `mtg_ssm-2.6.2.dev1/tests/containers/test_legacy.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/tests/data/bulk_data.json` & `mtg_ssm-2.6.2.dev1/tests/data/bulk_data.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333334%*

 * *Differences: {"'data'": "{0: {'download_uri': "*

 * *           "'https://data.scryfall.io/default-cards/default-cards-20230316210924.json', "*

 * *           "'updated_at': '2023-03-16T21:09:24.643000Z'}}"}*

```diff
@@ -1,18 +1,18 @@
 {
     "data": [
         {
             "content_encoding": "gzip",
             "content_type": "application/json",
             "description": "A JSON file containing every card object on Scryfall in English or the printed language if the card is only available in one language.",
-            "download_uri": "https://data.scryfall.io/default-cards/default-cards-20230310220757.json",
+            "download_uri": "https://data.scryfall.io/default-cards/default-cards-20230316210924.json",
             "id": "e2ef41e3-5778-4bc2-af3f-78eca4dd9c23",
             "name": "Default Cards",
             "object": "bulk_data",
             "type": "default_cards",
-            "updated_at": "2023-03-10T22:07:57.155000Z",
+            "updated_at": "2023-03-16T21:09:24.643000Z",
             "uri": "https://api.scryfall.com/bulk-data/e2ef41e3-5778-4bc2-af3f-78eca4dd9c23"
         }
     ],
     "has_more": false,
     "object": "list"
 }
```

### Comparing `mtg_ssm-2.6.1.dev1/tests/data/cards.json` & `mtg_ssm-2.6.2.dev1/tests/data/cards.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9915584126466814%*

 * *Differences: {'0': "{'edhrec_rank': 4168, 'legalities': {'oathbreaker': 'legal'}, 'penny_rank': 8902, 'prices': "*

 * *      "{'eur': '0.40'}}",*

 * * '1': "{'edhrec_rank': 20524, 'legalities': {'oathbreaker': 'legal'}, 'prices': {'eur': '0.09'}}",*

 * * '10': "{'edhrec_rank': 18712, 'legalities': {'oathbreaker': 'legal'}, 'prices': {'eur': '0.05'}}",*

 * * '11': "{'edhrec_rank': 2592, 'legalities': {'oathbreaker': 'legal'}}",*

 * * '12': "{'legalities': {'oathbreaker': 'banned'}}",*

 * * '13': "{'legalities': {'oathbreaker': 'banned'}, 'prices': {' […]*

```diff
@@ -13,15 +13,15 @@
         "color_identity": [
             "W"
         ],
         "colors": [
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 4159,
+        "edhrec_rank": 4168,
         "finishes": [
             "nonfoil"
         ],
         "flavor_text": "Only leonin clerics who can survive the Razor Fields for one turning of the suns can stand in the Cave of Light.",
         "foil": false,
         "frame": "2003",
         "full_art": false,
@@ -51,14 +51,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "legal",
             "pioneer": "not_legal",
             "predh": "legal",
             "premodern": "not_legal",
@@ -71,18 +72,18 @@
         ],
         "name": "Leonin Abunas",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "10064324-34a0-47eb-a58e-01db10234ed9",
         "oracle_text": "Artifacts you control have hexproof. (They can't be the targets of spells or abilities your opponents control.)",
         "oversized": false,
-        "penny_rank": 8836,
+        "penny_rank": 8902,
         "power": "2",
         "prices": {
-            "eur": "0.74",
+            "eur": "0.40",
             "eur_foil": null,
             "tix": null,
             "usd": "0.77",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A10064324-34a0-47eb-a58e-01db10234ed9&unique=prints",
@@ -154,15 +155,15 @@
         "color_identity": [
             "W"
         ],
         "colors": [
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 20541,
+        "edhrec_rank": 20524,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2003",
         "full_art": false,
@@ -195,14 +196,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "restricted",
             "penny": "legal",
             "pioneer": "not_legal",
             "predh": "legal",
             "premodern": "not_legal",
@@ -218,15 +220,15 @@
         "name": "Faithful Squire // Kaiso, Memory of Loyalty",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "2358ffc2-6663-4ef3-b3a4-b036a4733ac6",
         "oversized": false,
         "power": "2",
         "prices": {
-            "eur": "0.05",
+            "eur": "0.09",
             "eur_foil": "0.59",
             "tix": "0.02",
             "usd": "0.11",
             "usd_etched": null,
             "usd_foil": "0.28"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A2358ffc2-6663-4ef3-b3a4-b036a4733ac6&unique=prints",
@@ -268,15 +270,15 @@
         "card_back_id": "0aeebaf5-8c7d-4636-9e82-8c27447861f7",
         "cardmarket_id": 11972,
         "cmc": 0.0,
         "collector_number": "273",
         "color_identity": [],
         "colors": [],
         "digital": false,
-        "edhrec_rank": 1976,
+        "edhrec_rank": 1979,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2003",
         "full_art": false,
@@ -307,14 +309,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "not_legal",
             "predh": "legal",
             "premodern": "not_legal",
@@ -330,18 +333,18 @@
         "name": "Boseiju, Who Shelters All",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "36937483-30cb-449a-8028-75017a124922",
         "oracle_text": "Boseiju, Who Shelters All enters the battlefield tapped.\n{T}, Pay 2 life: Add {C}. If that mana is spent on an instant or sorcery spell, that spell can't be countered.",
         "oversized": false,
         "prices": {
-            "eur": "9.50",
-            "eur_foil": "67.00",
-            "tix": "0.20",
-            "usd": "22.91",
+            "eur": "15.90",
+            "eur_foil": "37.50",
+            "tix": "0.22",
+            "usd": "22.68",
             "usd_etched": null,
             "usd_foil": "108.88"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A36937483-30cb-449a-8028-75017a124922&unique=prints",
         "produced_mana": [
             "C"
         ],
@@ -412,15 +415,15 @@
         "color_identity": [
             "W"
         ],
         "colors": [
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 12440,
+        "edhrec_rank": 12469,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2003",
         "full_art": false,
@@ -454,14 +457,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "restricted",
             "penny": "legal",
             "pioneer": "not_legal",
             "predh": "legal",
             "premodern": "not_legal",
@@ -475,21 +479,21 @@
             78600
         ],
         "name": "Bushi Tenderfoot // Kenzo the Hardhearted",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "82959ca2-cd96-4cca-9ce0-afb8db209860",
         "oversized": false,
-        "penny_rank": 9462,
+        "penny_rank": 9564,
         "power": "1",
         "prices": {
-            "eur": "0.02",
+            "eur": "0.05",
             "eur_foil": "4.95",
             "tix": "0.02",
-            "usd": "0.23",
+            "usd": "0.24",
             "usd_etched": null,
             "usd_foil": "6.85"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A82959ca2-cd96-4cca-9ce0-afb8db209860&unique=prints",
         "promo": false,
         "rarity": "uncommon",
         "related_uris": {
@@ -532,15 +536,15 @@
         "color_identity": [
             "W"
         ],
         "colors": [
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 16801,
+        "edhrec_rank": 16876,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2003",
         "full_art": false,
@@ -573,14 +577,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "restricted",
             "penny": "legal",
             "pioneer": "not_legal",
             "predh": "legal",
             "premodern": "not_legal",
@@ -595,15 +600,15 @@
         ],
         "name": "J\u00f6tun Grunt",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "43fbfeec-bcaf-48b8-befe-b7346fec5a3a",
         "oracle_text": "Cumulative upkeep\u2014Put two cards from a single graveyard on the bottom of their owner's library. (At the beginning of your upkeep, put an age counter on this permanent, then sacrifice it unless you pay its upkeep cost for each age counter on it.)",
         "oversized": false,
-        "penny_rank": 10706,
+        "penny_rank": 10808,
         "power": "4",
         "prices": {
             "eur": "0.10",
             "eur_foil": "0.99",
             "tix": "0.02",
             "usd": "0.17",
             "usd_etched": null,
@@ -670,15 +675,15 @@
         "color_identity": [
             "G"
         ],
         "colors": [
             "G"
         ],
         "digital": false,
-        "edhrec_rank": 6571,
+        "edhrec_rank": 6581,
         "finishes": [
             "nonfoil"
         ],
         "foil": false,
         "frame": "1993",
         "full_art": false,
         "games": [
@@ -707,14 +712,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "legal",
             "pauper": "legal",
             "paupercommander": "legal",
             "penny": "legal",
             "pioneer": "not_legal",
             "predh": "legal",
             "premodern": "not_legal",
@@ -727,18 +733,18 @@
         ],
         "name": "Thallid",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "46abaabe-7015-4d82-a5aa-2706b1f51bed",
         "oracle_text": "At the beginning of your upkeep, put a spore counter on Thallid.\nRemove three spore counters from Thallid: Create a 1/1 green Saproling creature token.",
         "oversized": false,
-        "penny_rank": 8874,
+        "penny_rank": 8836,
         "power": "1",
         "prices": {
-            "eur": "0.12",
+            "eur": "0.05",
             "eur_foil": null,
             "tix": null,
             "usd": "0.20",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A46abaabe-7015-4d82-a5aa-2706b1f51bed&unique=prints",
@@ -802,15 +808,15 @@
         "color_identity": [
             "G"
         ],
         "colors": [
             "G"
         ],
         "digital": false,
-        "edhrec_rank": 6571,
+        "edhrec_rank": 6581,
         "finishes": [
             "nonfoil"
         ],
         "foil": false,
         "frame": "1993",
         "full_art": false,
         "games": [
@@ -839,14 +845,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "legal",
             "pauper": "legal",
             "paupercommander": "legal",
             "penny": "legal",
             "pioneer": "not_legal",
             "predh": "legal",
             "premodern": "not_legal",
@@ -859,18 +866,18 @@
         ],
         "name": "Thallid",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "46abaabe-7015-4d82-a5aa-2706b1f51bed",
         "oracle_text": "At the beginning of your upkeep, put a spore counter on Thallid.\nRemove three spore counters from Thallid: Create a 1/1 green Saproling creature token.",
         "oversized": false,
-        "penny_rank": 8874,
+        "penny_rank": 8836,
         "power": "1",
         "prices": {
-            "eur": "0.04",
+            "eur": "0.05",
             "eur_foil": null,
             "tix": null,
             "usd": "0.18",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A46abaabe-7015-4d82-a5aa-2706b1f51bed&unique=prints",
@@ -934,15 +941,15 @@
         "color_identity": [
             "G"
         ],
         "colors": [
             "G"
         ],
         "digital": false,
-        "edhrec_rank": 6571,
+        "edhrec_rank": 6581,
         "finishes": [
             "nonfoil"
         ],
         "foil": false,
         "frame": "1993",
         "full_art": false,
         "games": [
@@ -971,14 +978,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "legal",
             "pauper": "legal",
             "paupercommander": "legal",
             "penny": "legal",
             "pioneer": "not_legal",
             "predh": "legal",
             "premodern": "not_legal",
@@ -991,18 +999,18 @@
         ],
         "name": "Thallid",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "46abaabe-7015-4d82-a5aa-2706b1f51bed",
         "oracle_text": "At the beginning of your upkeep, put a spore counter on Thallid.\nRemove three spore counters from Thallid: Create a 1/1 green Saproling creature token.",
         "oversized": false,
-        "penny_rank": 8874,
+        "penny_rank": 8836,
         "power": "1",
         "prices": {
-            "eur": "0.10",
+            "eur": "0.05",
             "eur_foil": null,
             "tix": null,
             "usd": "0.21",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A46abaabe-7015-4d82-a5aa-2706b1f51bed&unique=prints",
@@ -1066,15 +1074,15 @@
         "color_identity": [
             "G"
         ],
         "colors": [
             "G"
         ],
         "digital": false,
-        "edhrec_rank": 6571,
+        "edhrec_rank": 6581,
         "finishes": [
             "nonfoil"
         ],
         "foil": false,
         "frame": "1993",
         "full_art": false,
         "games": [
@@ -1103,14 +1111,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "legal",
             "pauper": "legal",
             "paupercommander": "legal",
             "penny": "legal",
             "pioneer": "not_legal",
             "predh": "legal",
             "premodern": "not_legal",
@@ -1123,18 +1132,18 @@
         ],
         "name": "Thallid",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "46abaabe-7015-4d82-a5aa-2706b1f51bed",
         "oracle_text": "At the beginning of your upkeep, put a spore counter on Thallid.\nRemove three spore counters from Thallid: Create a 1/1 green Saproling creature token.",
         "oversized": false,
-        "penny_rank": 8874,
+        "penny_rank": 8836,
         "power": "1",
         "prices": {
-            "eur": "0.10",
+            "eur": "0.15",
             "eur_foil": null,
             "tix": null,
             "usd": "0.19",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A46abaabe-7015-4d82-a5aa-2706b1f51bed&unique=prints",
@@ -1180,15 +1189,15 @@
         "color_identity": [
             "B"
         ],
         "colors": [
             "B"
         ],
         "digital": false,
-        "edhrec_rank": 18662,
+        "edhrec_rank": 18712,
         "finishes": [
             "nonfoil"
         ],
         "flavor_text": "\"It keeps some out, yes. It also keeps others in!\"\n\u2014Grandmother Sengir",
         "foil": false,
         "frame": "1993",
         "full_art": false,
@@ -1221,14 +1230,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "not_legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "legal",
             "paupercommander": "legal",
             "penny": "not_legal",
             "pioneer": "not_legal",
             "predh": "legal",
             "premodern": "legal",
@@ -1243,15 +1253,15 @@
         "nonfoil": true,
         "object": "card",
         "oracle_id": "443f8dd1-333d-42c4-a286-302a9496209a",
         "oracle_text": "Defender (This creature can't attack.)\nProtection from black",
         "oversized": false,
         "power": "0",
         "prices": {
-            "eur": "0.02",
+            "eur": "0.15",
             "eur_foil": null,
             "tix": null,
             "usd": "0.18",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A443f8dd1-333d-42c4-a286-302a9496209a&unique=prints",
@@ -1297,15 +1307,15 @@
         "color_identity": [
             "B"
         ],
         "colors": [
             "B"
         ],
         "digital": false,
-        "edhrec_rank": 18662,
+        "edhrec_rank": 18712,
         "finishes": [
             "nonfoil"
         ],
         "flavor_text": "\"Just the place for a picnic.\"\n\u2014Murat, Death Speaker",
         "foil": false,
         "frame": "1993",
         "full_art": false,
@@ -1338,14 +1348,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "not_legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "legal",
             "paupercommander": "legal",
             "penny": "not_legal",
             "pioneer": "not_legal",
             "predh": "legal",
             "premodern": "legal",
@@ -1360,15 +1371,15 @@
         "nonfoil": true,
         "object": "card",
         "oracle_id": "443f8dd1-333d-42c4-a286-302a9496209a",
         "oracle_text": "Defender (This creature can't attack.)\nProtection from black",
         "oversized": false,
         "power": "0",
         "prices": {
-            "eur": "0.03",
+            "eur": "0.05",
             "eur_foil": null,
             "tix": null,
             "usd": "0.18",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A443f8dd1-333d-42c4-a286-302a9496209a&unique=prints",
@@ -1415,15 +1426,15 @@
         "color_identity": [
             "W"
         ],
         "colors": [
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 2581,
+        "edhrec_rank": 2592,
         "finishes": [
             "nonfoil"
         ],
         "flavor_text": "Ixidor had only to imagine their ruin and Akroma made it so.",
         "foil": false,
         "frame": "2003",
         "full_art": false,
@@ -1456,14 +1467,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "not_legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "not_legal",
             "predh": "legal",
             "premodern": "legal",
@@ -1572,14 +1584,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "legal",
             "historic": "banned",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "not_legal",
+            "oathbreaker": "banned",
             "oldschool": "not_legal",
             "pauper": "legal",
             "paupercommander": "legal",
             "penny": "legal",
             "pioneer": "not_legal",
             "predh": "legal",
             "premodern": "legal",
@@ -1691,14 +1704,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "legal",
             "historic": "banned",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "not_legal",
+            "oathbreaker": "banned",
             "oldschool": "not_legal",
             "pauper": "legal",
             "paupercommander": "legal",
             "penny": "legal",
             "pioneer": "not_legal",
             "predh": "legal",
             "premodern": "legal",
@@ -1714,18 +1728,18 @@
         "nonfoil": true,
         "object": "card",
         "oracle_id": "53f7c868-b03e-4fc2-8dcf-a75bbfa3272b",
         "oracle_text": "Add {B}{B}{B}.",
         "oversized": false,
         "penny_rank": 27,
         "prices": {
-            "eur": "0.76",
+            "eur": "0.46",
             "eur_foil": null,
-            "tix": "1.46",
-            "usd": "1.03",
+            "tix": "1.85",
+            "usd": "1.04",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A53f7c868-b03e-4fc2-8dcf-a75bbfa3272b&unique=prints",
         "produced_mana": [
             "B"
         ],
@@ -1805,14 +1819,15 @@
             "explorer": "legal",
             "future": "legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "legal",
             "paupercommander": "legal",
             "penny": "legal",
             "pioneer": "legal",
             "predh": "legal",
             "premodern": "legal",
@@ -1827,15 +1842,15 @@
         "name": "Forest",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "b34bb2dc-c1af-4d77-b0b3-a0fb342a5fc6",
         "oracle_text": "({T}: Add {G}.)",
         "oversized": false,
         "prices": {
-            "eur": "0.45",
+            "eur": "0.20",
             "eur_foil": null,
             "tix": "0.11",
             "usd": "0.91",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ab34bb2dc-c1af-4d77-b0b3-a0fb342a5fc6&unique=prints",
@@ -1918,14 +1933,15 @@
             "explorer": "legal",
             "future": "legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "legal",
             "paupercommander": "legal",
             "penny": "legal",
             "pioneer": "legal",
             "predh": "legal",
             "premodern": "legal",
@@ -1940,18 +1956,18 @@
         "name": "Forest",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "b34bb2dc-c1af-4d77-b0b3-a0fb342a5fc6",
         "oracle_text": "({T}: Add {G}.)",
         "oversized": false,
         "prices": {
-            "eur": "0.15",
+            "eur": "0.30",
             "eur_foil": null,
             "tix": "0.80",
-            "usd": "1.03",
+            "usd": "1.01",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ab34bb2dc-c1af-4d77-b0b3-a0fb342a5fc6&unique=prints",
         "produced_mana": [
             "G"
         ],
@@ -2031,14 +2047,15 @@
             "explorer": "legal",
             "future": "legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "legal",
             "paupercommander": "legal",
             "penny": "legal",
             "pioneer": "legal",
             "predh": "legal",
             "premodern": "legal",
@@ -2053,18 +2070,18 @@
         "name": "Forest",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "b34bb2dc-c1af-4d77-b0b3-a0fb342a5fc6",
         "oracle_text": "({T}: Add {G}.)",
         "oversized": false,
         "prices": {
-            "eur": "0.37",
+            "eur": "0.19",
             "eur_foil": null,
             "tix": "2.85",
-            "usd": "0.45",
+            "usd": "0.48",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ab34bb2dc-c1af-4d77-b0b3-a0fb342a5fc6&unique=prints",
         "produced_mana": [
             "G"
         ],
@@ -2144,14 +2161,15 @@
             "explorer": "legal",
             "future": "not_legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "legal",
             "paupercommander": "legal",
             "penny": "not_legal",
             "pioneer": "legal",
             "predh": "legal",
             "premodern": "legal",
@@ -2166,18 +2184,18 @@
         "name": "Snow-Covered Forest",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "5f0d3be8-e63e-4ade-ae58-6b0c14f2ce6d",
         "oracle_text": "({T}: Add {G}.)",
         "oversized": false,
         "prices": {
-            "eur": "1.11",
+            "eur": "2.75",
             "eur_foil": null,
-            "tix": "2.25",
-            "usd": "2.00",
+            "tix": "2.09",
+            "usd": "2.07",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A5f0d3be8-e63e-4ade-ae58-6b0c14f2ce6d&unique=prints",
         "produced_mana": [
             "G"
         ],
@@ -2222,15 +2240,15 @@
         "color_identity": [
             "B"
         ],
         "colors": [
             "B"
         ],
         "digital": false,
-        "edhrec_rank": 15642,
+        "edhrec_rank": 15621,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "flavor_text": "Death took his humanity but not his skill with the knife.",
         "foil": true,
         "frame": "2003",
@@ -2264,14 +2282,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "restricted",
             "penny": "legal",
             "pioneer": "not_legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -2286,15 +2305,15 @@
         ],
         "name": "Abattoir Ghoul",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "2b211adb-de44-4468-b65d-907a09aa7e9d",
         "oracle_text": "First strike\nWhenever a creature dealt damage by Abattoir Ghoul this turn dies, you gain life equal to that creature's toughness.",
         "oversized": false,
-        "penny_rank": 4728,
+        "penny_rank": 4727,
         "power": "3",
         "prices": {
             "eur": "0.05",
             "eur_foil": "0.15",
             "tix": "0.04",
             "usd": "0.05",
             "usd_etched": null,
@@ -2392,15 +2411,15 @@
         "cardmarket_id": 250620,
         "cmc": 1.0,
         "collector_number": "51",
         "color_identity": [
             "U"
         ],
         "digital": false,
-        "edhrec_rank": 11715,
+        "edhrec_rank": 11722,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2003",
         "frame_effects": [
@@ -2428,14 +2447,15 @@
             "explorer": "legal",
             "future": "legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "legal",
             "paupercommander": "legal",
             "penny": "legal",
             "pioneer": "legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -2451,18 +2471,18 @@
         "name": "Delver of Secrets // Insectile Aberration",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "edd531b9-f615-4399-8c8c-1c5e18c4acbf",
         "oversized": false,
         "penny_rank": 102,
         "prices": {
-            "eur": "0.91",
-            "eur_foil": "4.65",
+            "eur": "0.53",
+            "eur_foil": "5.75",
             "tix": "0.02",
-            "usd": "0.56",
+            "usd": "0.61",
             "usd_etched": null,
             "usd_foil": "6.68"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Aedd531b9-f615-4399-8c8c-1c5e18c4acbf&unique=prints",
         "promo": false,
         "rarity": "common",
         "related_uris": {
@@ -2540,14 +2560,15 @@
             "explorer": "legal",
             "future": "legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "legal",
             "paupercommander": "legal",
             "penny": "legal",
             "pioneer": "legal",
             "predh": "legal",
             "premodern": "legal",
@@ -2563,16 +2584,16 @@
         "name": "Forest",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "b34bb2dc-c1af-4d77-b0b3-a0fb342a5fc6",
         "oracle_text": "({T}: Add {G}.)",
         "oversized": false,
         "prices": {
-            "eur": "0.10",
-            "eur_foil": "0.39",
+            "eur": "0.09",
+            "eur_foil": "1.00",
             "tix": "0.02",
             "usd": "0.17",
             "usd_etched": null,
             "usd_foil": "1.44"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ab34bb2dc-c1af-4d77-b0b3-a0fb342a5fc6&unique=prints",
         "produced_mana": [
@@ -2655,14 +2676,15 @@
             "explorer": "legal",
             "future": "legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "legal",
             "paupercommander": "legal",
             "penny": "legal",
             "pioneer": "legal",
             "predh": "legal",
             "premodern": "legal",
@@ -2678,16 +2700,16 @@
         "name": "Forest",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "b34bb2dc-c1af-4d77-b0b3-a0fb342a5fc6",
         "oracle_text": "({T}: Add {G}.)",
         "oversized": false,
         "prices": {
-            "eur": "0.10",
-            "eur_foil": "0.30",
+            "eur": "0.09",
+            "eur_foil": "0.80",
             "tix": "0.03",
             "usd": "0.18",
             "usd_etched": null,
             "usd_foil": "1.37"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ab34bb2dc-c1af-4d77-b0b3-a0fb342a5fc6&unique=prints",
         "produced_mana": [
@@ -2770,14 +2792,15 @@
             "explorer": "legal",
             "future": "legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "legal",
             "paupercommander": "legal",
             "penny": "legal",
             "pioneer": "legal",
             "predh": "legal",
             "premodern": "legal",
@@ -2793,15 +2816,15 @@
         "name": "Forest",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "b34bb2dc-c1af-4d77-b0b3-a0fb342a5fc6",
         "oracle_text": "({T}: Add {G}.)",
         "oversized": false,
         "prices": {
-            "eur": "0.15",
+            "eur": "0.09",
             "eur_foil": "0.99",
             "tix": "0.03",
             "usd": "0.20",
             "usd_etched": null,
             "usd_foil": "0.61"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ab34bb2dc-c1af-4d77-b0b3-a0fb342a5fc6&unique=prints",
@@ -2900,14 +2923,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "not_legal",
             "modern": "not_legal",
+            "oathbreaker": "not_legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "not_legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -2990,15 +3014,15 @@
         "card_back_id": "0aeebaf5-8c7d-4636-9e82-8c27447861f7",
         "cardmarket_id": 532177,
         "cmc": 4.0,
         "collector_number": "237",
         "color_identity": [],
         "colors": [],
         "digital": false,
-        "edhrec_rank": 1388,
+        "edhrec_rank": 1393,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "flavor_text": "The Skoti owe their immortality to the elixir, and the manner of its creation is their most closely guarded secret.",
         "foil": true,
         "frame": "2015",
@@ -3031,14 +3055,15 @@
             "explorer": "legal",
             "future": "not_legal",
             "gladiator": "legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "legal",
             "pioneer": "legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -3059,20 +3084,20 @@
         "penny_rank": 770,
         "preview": {
             "previewed_at": "2021-01-16",
             "source": "Luca Van Deun",
             "source_uri": "https://twitter.com/LegenVD/status/1350493142966013952"
         },
         "prices": {
-            "eur": "0.85",
-            "eur_foil": "1.43",
+            "eur": "0.94",
+            "eur_foil": "1.50",
             "tix": "0.02",
-            "usd": "1.83",
+            "usd": "1.66",
             "usd_etched": null,
-            "usd_foil": "2.06"
+            "usd_foil": "1.97"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Aed7300f4-831a-4ba4-b5e6-ceba8d079eaa&unique=prints",
         "promo": false,
         "rarity": "rare",
         "related_uris": {
             "edhrec": "https://edhrec.com/route/?cc=Cosmos+Elixir",
             "gatherer": "https://gatherer.wizards.com/Pages/Card/Details.aspx?multiverseid=503853",
@@ -3127,15 +3152,15 @@
         "card_back_id": "0aeebaf5-8c7d-4636-9e82-8c27447861f7",
         "cardmarket_id": 532412,
         "cmc": 4.0,
         "collector_number": "368",
         "color_identity": [],
         "colors": [],
         "digital": false,
-        "edhrec_rank": 1388,
+        "edhrec_rank": 1393,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "frame_effects": [
@@ -3170,14 +3195,15 @@
             "explorer": "legal",
             "future": "not_legal",
             "gladiator": "legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "legal",
             "pioneer": "legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -3197,20 +3223,20 @@
         "penny_rank": 770,
         "preview": {
             "previewed_at": "2021-01-20",
             "source": "Luca Van Deun",
             "source_uri": "https://twitter.com/LegenVD/status/1350493142966013952"
         },
         "prices": {
-            "eur": "2.00",
+            "eur": "1.90",
             "eur_foil": "1.80",
             "tix": null,
-            "usd": "1.33",
+            "usd": "1.42",
             "usd_etched": null,
-            "usd_foil": "1.67"
+            "usd_foil": "1.73"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Aed7300f4-831a-4ba4-b5e6-ceba8d079eaa&unique=prints",
         "promo": false,
         "promo_types": [
             "boosterfun"
         ],
         "rarity": "rare",
@@ -3254,15 +3280,15 @@
         "color_identity": [
             "U"
         ],
         "colors": [
             "U"
         ],
         "digital": false,
-        "edhrec_rank": 17640,
+        "edhrec_rank": 17698,
         "finishes": [
             "nonfoil"
         ],
         "flavor_text": "These spirits of the air are winsome and wild, and cannot be truly contained. Only marginally intelligent, they often substitute whimsy for strategy, delighting in mischief and mayhem.",
         "foil": false,
         "frame": "1993",
         "full_art": false,
@@ -3294,14 +3320,15 @@
             "explorer": "legal",
             "future": "not_legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "legal",
             "pauper": "not_legal",
             "paupercommander": "restricted",
             "penny": "legal",
             "pioneer": "legal",
             "predh": "legal",
             "premodern": "legal",
@@ -3314,15 +3341,15 @@
         ],
         "name": "Air Elemental",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "7744bae4-a8b7-44a5-9b4c-0048ad4cc448",
         "oracle_text": "Flying",
         "oversized": false,
-        "penny_rank": 6504,
+        "penny_rank": 6499,
         "power": "4",
         "prices": {
             "eur": "369.00",
             "eur_foil": null,
             "tix": null,
             "usd": null,
             "usd_etched": null,
@@ -3408,14 +3435,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "legal",
             "historic": "banned",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "not_legal",
+            "oathbreaker": "banned",
             "oldschool": "legal",
             "pauper": "legal",
             "paupercommander": "legal",
             "penny": "legal",
             "pioneer": "not_legal",
             "predh": "legal",
             "premodern": "legal",
@@ -3520,14 +3548,15 @@
             "explorer": "legal",
             "future": "legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "legal",
             "pauper": "legal",
             "paupercommander": "legal",
             "penny": "legal",
             "pioneer": "legal",
             "predh": "legal",
             "premodern": "legal",
@@ -3631,14 +3660,15 @@
             "explorer": "legal",
             "future": "legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "legal",
             "pauper": "legal",
             "paupercommander": "legal",
             "penny": "legal",
             "pioneer": "legal",
             "predh": "legal",
             "premodern": "legal",
@@ -3655,15 +3685,15 @@
         "oracle_id": "b34bb2dc-c1af-4d77-b0b3-a0fb342a5fc6",
         "oracle_text": "({T}: Add {G}.)",
         "oversized": false,
         "prices": {
             "eur": "29.99",
             "eur_foil": null,
             "tix": null,
-            "usd": "78.29",
+            "usd": "76.63",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ab34bb2dc-c1af-4d77-b0b3-a0fb342a5fc6&unique=prints",
         "produced_mana": [
             "G"
         ],
@@ -3708,15 +3738,15 @@
         "color_identity": [
             "B"
         ],
         "colors": [
             "B"
         ],
         "digital": false,
-        "edhrec_rank": 1635,
+        "edhrec_rank": 1638,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "flavor_text": "\"Under the suns, Mirrodin kneels and begs us for perfection.\"\n\u2014Geth, Lord of the Vault",
         "foil": true,
         "frame": "2003",
@@ -3748,14 +3778,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "legal",
             "pioneer": "not_legal",
             "predh": "legal",
             "premodern": "not_legal",
@@ -3772,20 +3803,20 @@
         "nonfoil": true,
         "object": "card",
         "oracle_id": "038c0165-32b6-4e81-8180-604b49905207",
         "oracle_text": "Put X -1/-1 counters on each creature. Shuffle Black Sun's Zenith into its owner's library.",
         "oversized": false,
         "penny_rank": 1796,
         "prices": {
-            "eur": "5.06",
-            "eur_foil": "3.95",
+            "eur": "4.61",
+            "eur_foil": "9.49",
             "tix": "0.02",
-            "usd": "5.45",
+            "usd": "5.58",
             "usd_etched": null,
-            "usd_foil": "11.56"
+            "usd_foil": "11.92"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A038c0165-32b6-4e81-8180-604b49905207&unique=prints",
         "promo": false,
         "rarity": "rare",
         "related_uris": {
             "edhrec": "https://edhrec.com/route/?cc=Black+Sun%27s+Zenith",
             "gatherer": "https://gatherer.wizards.com/Pages/Card/Details.aspx?multiverseid=214061",
@@ -3844,15 +3875,15 @@
         "color_identity": [
             "W"
         ],
         "colors": [
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 2265,
+        "edhrec_rank": 2268,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2003",
         "full_art": false,
@@ -3885,14 +3916,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "not_legal",
             "predh": "legal",
             "premodern": "not_legal",
@@ -3909,20 +3941,20 @@
         "nonfoil": true,
         "object": "card",
         "oracle_id": "454a8902-8120-4373-96ee-bbf352b04e8d",
         "oracle_text": "Battle cry (Whenever this creature attacks, each other attacking creature gets +1/+0 until end of turn.)\nWhenever Hero of Bladehold attacks, create two 1/1 white Soldier creature tokens that are tapped and attacking.",
         "oversized": false,
         "power": "3",
         "prices": {
-            "eur": "6.31",
+            "eur": "8.15",
             "eur_foil": "11.00",
-            "tix": "0.09",
-            "usd": "15.61",
+            "tix": "0.10",
+            "usd": "15.49",
             "usd_etched": null,
-            "usd_foil": "25.93"
+            "usd_foil": "26.66"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A454a8902-8120-4373-96ee-bbf352b04e8d&unique=prints",
         "promo": false,
         "rarity": "mythic",
         "related_uris": {
             "edhrec": "https://edhrec.com/route/?cc=Hero+of+Bladehold",
             "gatherer": "https://gatherer.wizards.com/Pages/Card/Details.aspx?multiverseid=214064",
@@ -3982,15 +4014,15 @@
         "color_identity": [
             "G"
         ],
         "colors": [
             "G"
         ],
         "digital": false,
-        "edhrec_rank": 6571,
+        "edhrec_rank": 6581,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2003",
         "full_art": false,
@@ -4021,14 +4053,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "legal",
             "paupercommander": "legal",
             "penny": "legal",
             "pioneer": "not_legal",
             "predh": "legal",
             "premodern": "not_legal",
@@ -4043,23 +4076,23 @@
         ],
         "name": "Thallid",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "46abaabe-7015-4d82-a5aa-2706b1f51bed",
         "oracle_text": "At the beginning of your upkeep, put a spore counter on Thallid.\nRemove three spore counters from Thallid: Create a 1/1 green Saproling creature token.",
         "oversized": false,
-        "penny_rank": 8874,
+        "penny_rank": 8836,
         "power": "1",
         "prices": {
             "eur": "0.15",
-            "eur_foil": "0.98",
+            "eur_foil": "1.27",
             "tix": "0.03",
             "usd": "0.28",
             "usd_etched": null,
-            "usd_foil": "0.50"
+            "usd_foil": "0.51"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A46abaabe-7015-4d82-a5aa-2706b1f51bed&unique=prints",
         "promo": false,
         "rarity": "common",
         "related_uris": {
             "edhrec": "https://edhrec.com/route/?cc=Thallid",
             "gatherer": "https://gatherer.wizards.com/Pages/Card/Details.aspx?multiverseid=370352",
@@ -4099,15 +4132,15 @@
         "cmc": 0.0,
         "collector_number": "266",
         "color_identity": [
             "G"
         ],
         "colors": [],
         "digital": false,
-        "edhrec_rank": 129,
+        "edhrec_rank": 127,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "frame_effects": [
@@ -4144,14 +4177,15 @@
             "explorer": "legal",
             "future": "legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -4171,20 +4205,20 @@
         "oversized": false,
         "preview": {
             "previewed_at": "2022-01-27",
             "source": "Wizards of the Coast",
             "source_uri": "https://www.twitch.tv/videos/1277767538"
         },
         "prices": {
-            "eur": "38.23",
-            "eur_foil": "38.43",
-            "tix": "59.90",
-            "usd": "39.26",
+            "eur": "38.97",
+            "eur_foil": "37.72",
+            "tix": "54.84",
+            "usd": "37.02",
             "usd_etched": null,
-            "usd_foil": "38.71"
+            "usd_foil": "40.06"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Abf1341dd-41a3-49f6-87ec-63170dde4324&unique=prints",
         "produced_mana": [
             "G"
         ],
         "promo": false,
         "rarity": "rare",
@@ -4227,15 +4261,15 @@
         "cmc": 0.0,
         "collector_number": "412",
         "color_identity": [
             "G"
         ],
         "colors": [],
         "digital": false,
-        "edhrec_rank": 129,
+        "edhrec_rank": 127,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "frame_effects": [
@@ -4272,14 +4306,15 @@
             "explorer": "legal",
             "future": "legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -4298,20 +4333,20 @@
         "oversized": false,
         "preview": {
             "previewed_at": "2022-01-27",
             "source": "Wizards of the Coast",
             "source_uri": "https://www.twitch.tv/videos/1277767538"
         },
         "prices": {
-            "eur": "46.54",
-            "eur_foil": "64.45",
+            "eur": "48.97",
+            "eur_foil": "69.00",
             "tix": null,
-            "usd": "44.99",
+            "usd": "42.43",
             "usd_etched": null,
-            "usd_foil": "73.69"
+            "usd_foil": "73.67"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Abf1341dd-41a3-49f6-87ec-63170dde4324&unique=prints",
         "produced_mana": [
             "G"
         ],
         "promo": false,
         "promo_types": [
@@ -4356,15 +4391,15 @@
         "cmc": 0.0,
         "collector_number": "501",
         "color_identity": [
             "G"
         ],
         "colors": [],
         "digital": false,
-        "edhrec_rank": 129,
+        "edhrec_rank": 127,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "frame_effects": [
@@ -4402,14 +4437,15 @@
             "explorer": "legal",
             "future": "legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -4428,20 +4464,20 @@
         "oversized": false,
         "preview": {
             "previewed_at": "2022-01-28",
             "source": "Wizards of the Coast",
             "source_uri": "https://www.twitch.tv/videos/1277767538"
         },
         "prices": {
-            "eur": "44.88",
-            "eur_foil": "49.94",
+            "eur": "41.65",
+            "eur_foil": "54.67",
             "tix": null,
-            "usd": "39.76",
+            "usd": "40.90",
             "usd_etched": null,
-            "usd_foil": "44.39"
+            "usd_foil": "45.41"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Abf1341dd-41a3-49f6-87ec-63170dde4324&unique=prints",
         "produced_mana": [
             "G"
         ],
         "promo": false,
         "promo_types": [
@@ -4521,14 +4557,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "not_legal",
             "modern": "not_legal",
+            "oathbreaker": "not_legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "not_legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -4542,18 +4579,18 @@
         "name": "All in Good Time",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "402ba90d-6c41-49ee-ab50-7f0a466f66fe",
         "oracle_text": "When you set this scheme in motion, take an extra turn after this one. Schemes can't be set in motion that turn.",
         "oversized": true,
         "prices": {
-            "eur": "13.91",
+            "eur": "15.00",
             "eur_foil": null,
             "tix": null,
-            "usd": "20.61",
+            "usd": "18.08",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A402ba90d-6c41-49ee-ab50-7f0a466f66fe&unique=prints",
         "promo": false,
         "rarity": "common",
         "related_uris": {
@@ -4629,14 +4666,15 @@
             "explorer": "legal",
             "future": "not_legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "legal",
             "paupercommander": "legal",
             "penny": "legal",
             "pioneer": "legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -4652,20 +4690,20 @@
         "name": "Wastes",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "05d24b0c-904a-46b6-b42a-96a4d91a0dd4",
         "oracle_text": "{T}: Add {C}.",
         "oversized": false,
         "prices": {
-            "eur": "0.34",
-            "eur_foil": "4.99",
+            "eur": "0.28",
+            "eur_foil": "6.20",
             "tix": "0.02",
-            "usd": "1.05",
+            "usd": "1.04",
             "usd_etched": null,
-            "usd_foil": "7.64"
+            "usd_foil": "7.66"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A05d24b0c-904a-46b6-b42a-96a4d91a0dd4&unique=prints",
         "produced_mana": [
             "C"
         ],
         "promo": false,
         "rarity": "common",
@@ -4741,14 +4779,15 @@
             "explorer": "legal",
             "future": "not_legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "legal",
             "paupercommander": "legal",
             "penny": "legal",
             "pioneer": "legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -4762,15 +4801,15 @@
         "name": "Wastes",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "05d24b0c-904a-46b6-b42a-96a4d91a0dd4",
         "oracle_text": "{T}: Add {C}.",
         "oversized": false,
         "prices": {
-            "eur": "0.99",
+            "eur": "1.24",
             "eur_foil": null,
             "tix": null,
             "usd": "2.69",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A05d24b0c-904a-46b6-b42a-96a4d91a0dd4&unique=prints",
@@ -4852,14 +4891,15 @@
             "explorer": "legal",
             "future": "not_legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "legal",
             "paupercommander": "legal",
             "penny": "legal",
             "pioneer": "legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -4875,17 +4915,17 @@
         "name": "Wastes",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "05d24b0c-904a-46b6-b42a-96a4d91a0dd4",
         "oracle_text": "{T}: Add {C}.",
         "oversized": false,
         "prices": {
-            "eur": "0.34",
-            "eur_foil": "10.98",
-            "tix": "0.02",
+            "eur": "0.26",
+            "eur_foil": "10.99",
+            "tix": "0.03",
             "usd": "1.10",
             "usd_etched": null,
             "usd_foil": "10.49"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A05d24b0c-904a-46b6-b42a-96a4d91a0dd4&unique=prints",
         "produced_mana": [
             "C"
@@ -4964,14 +5004,15 @@
             "explorer": "legal",
             "future": "not_legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "legal",
             "paupercommander": "legal",
             "penny": "legal",
             "pioneer": "legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -4985,18 +5026,18 @@
         "name": "Wastes",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "05d24b0c-904a-46b6-b42a-96a4d91a0dd4",
         "oracle_text": "{T}: Add {C}.",
         "oversized": false,
         "prices": {
-            "eur": "1.50",
+            "eur": "0.55",
             "eur_foil": null,
             "tix": null,
-            "usd": "1.29",
+            "usd": "1.28",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A05d24b0c-904a-46b6-b42a-96a4d91a0dd4&unique=prints",
         "produced_mana": [
             "C"
         ],
@@ -5074,14 +5115,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "not_legal",
             "modern": "not_legal",
+            "oathbreaker": "not_legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "not_legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -5181,14 +5223,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "not_legal",
             "modern": "not_legal",
+            "oathbreaker": "not_legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "not_legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -5203,18 +5246,18 @@
         "name": "Akoum",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "25650a32-4014-4065-ad01-7357c3ad3995",
         "oracle_text": "Players may cast enchantment spells as though they had flash.\nWhenever you roll {CHAOS}, destroy target creature that isn't enchanted.",
         "oversized": true,
         "prices": {
-            "eur": "0.75",
+            "eur": "1.04",
             "eur_foil": null,
             "tix": "0.03",
-            "usd": "1.18",
+            "usd": "1.22",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A25650a32-4014-4065-ad01-7357c3ad3995&unique=prints",
         "promo": false,
         "rarity": "common",
         "related_uris": {
@@ -5289,14 +5332,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "not_legal",
             "modern": "not_legal",
+            "oathbreaker": "not_legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "not_legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -5310,18 +5354,18 @@
         "name": "Chaotic Aether",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "6dc67a65-31bf-4535-9e02-8f6d6ecefde5",
         "oracle_text": "When you encounter Chaotic Aether, each blank roll of the planar die is a {CHAOS} roll until a player planeswalks away from a plane. (Then planeswalk away from this phenomenon.)",
         "oversized": true,
         "prices": {
-            "eur": "0.75",
+            "eur": "1.02",
             "eur_foil": null,
             "tix": null,
-            "usd": "4.75",
+            "usd": "3.24",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A6dc67a65-31bf-4535-9e02-8f6d6ecefde5&unique=prints",
         "promo": false,
         "rarity": "common",
         "related_uris": {
@@ -5825,14 +5869,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "not_legal",
             "modern": "not_legal",
+            "oathbreaker": "not_legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "not_legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -5901,15 +5946,15 @@
         "color_identity": [
             "W"
         ],
         "colors": [
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 16624,
+        "edhrec_rank": 16532,
         "finishes": [
             "nonfoil"
         ],
         "flavor_text": "When an order for griffin barding comes in, blacksmiths prepare their forges for months of exacting work. They know griffins always detect imperfections and never haggle.",
         "foil": false,
         "frame": "2003",
         "full_art": false,
@@ -5943,14 +5988,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "not_legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "legal",
             "paupercommander": "legal",
             "penny": "legal",
             "pioneer": "not_legal",
             "predh": "legal",
             "premodern": "not_legal",
@@ -5967,15 +6013,15 @@
         "nonfoil": true,
         "object": "card",
         "oracle_id": "ad3d6003-66d3-486d-aa54-ddce1adb5ff1",
         "oracle_text": "Flying, vigilance",
         "oversized": false,
         "power": "2",
         "prices": {
-            "eur": "0.29",
+            "eur": "0.15",
             "eur_foil": null,
             "tix": "0.05",
             "usd": "0.22",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Aad3d6003-66d3-486d-aa54-ddce1adb5ff1&unique=prints",
@@ -6021,15 +6067,15 @@
         "color_identity": [
             "B"
         ],
         "colors": [
             "B"
         ],
         "digital": false,
-        "edhrec_rank": 1635,
+        "edhrec_rank": 1638,
         "finishes": [
             "foil"
         ],
         "foil": true,
         "frame": "2003",
         "full_art": true,
         "games": [
@@ -6058,14 +6104,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "legal",
             "pioneer": "not_legal",
             "predh": "legal",
             "premodern": "not_legal",
@@ -6083,15 +6130,15 @@
         "penny_rank": 1796,
         "prices": {
             "eur": null,
             "eur_foil": "13.99",
             "tix": null,
             "usd": null,
             "usd_etched": null,
-            "usd_foil": "28.58"
+            "usd_foil": "28.73"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A038c0165-32b6-4e81-8180-604b49905207&unique=prints",
         "promo": true,
         "promo_types": [
             "gameday"
         ],
         "rarity": "rare",
@@ -6165,14 +6212,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "not_legal",
             "modern": "not_legal",
+            "oathbreaker": "not_legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "not_legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -6189,15 +6237,15 @@
         "oracle_id": "97f708de-9271-4137-a9fe-dda25b922900",
         "oracle_text": "Creatures can't block.\nWhenever you roll {CHAOS}, draw a card for each land you control.",
         "oversized": true,
         "prices": {
             "eur": "15.00",
             "eur_foil": null,
             "tix": null,
-            "usd": "7.90",
+            "usd": "8.47",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A97f708de-9271-4137-a9fe-dda25b922900&unique=prints",
         "promo": true,
         "rarity": "rare",
         "related_uris": {
@@ -6239,15 +6287,15 @@
         "color_identity": [
             "W"
         ],
         "colors": [
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 10535,
+        "edhrec_rank": 10559,
         "finishes": [
             "foil"
         ],
         "flavor_text": "\"Dragons seek war. I bring it to them.\"",
         "foil": true,
         "frame": "2015",
         "full_art": false,
@@ -6279,14 +6327,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "legal",
             "pioneer": "legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -6297,15 +6346,15 @@
         "multiverse_ids": [],
         "name": "Dragonscale General",
         "nonfoil": false,
         "object": "card",
         "oracle_id": "9fc6e1db-cf09-4b8c-be4f-bb02ffe7a188",
         "oracle_text": "At the beginning of your end step, bolster X, where X is the number of tapped creatures you control. (Choose a creature with the least toughness among creatures you control and put X +1/+1 counters on it.)",
         "oversized": false,
-        "penny_rank": 5088,
+        "penny_rank": 5110,
         "power": "2",
         "prices": {
             "eur": null,
             "eur_foil": "0.29",
             "tix": null,
             "usd": null,
             "usd_etched": null,
@@ -6359,15 +6408,15 @@
         "color_identity": [
             "W"
         ],
         "colors": [
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 10535,
+        "edhrec_rank": 10559,
         "finishes": [
             "foil"
         ],
         "flavor_text": "\"Dragons seek war. I bring it to them.\"",
         "foil": true,
         "frame": "2015",
         "full_art": false,
@@ -6399,14 +6448,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "legal",
             "pioneer": "legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -6417,23 +6467,23 @@
         "multiverse_ids": [],
         "name": "Dragonscale General",
         "nonfoil": false,
         "object": "card",
         "oracle_id": "9fc6e1db-cf09-4b8c-be4f-bb02ffe7a188",
         "oracle_text": "At the beginning of your end step, bolster X, where X is the number of tapped creatures you control. (Choose a creature with the least toughness among creatures you control and put X +1/+1 counters on it.)",
         "oversized": false,
-        "penny_rank": 5088,
+        "penny_rank": 5110,
         "power": "2",
         "prices": {
             "eur": null,
             "eur_foil": "0.95",
             "tix": null,
             "usd": null,
             "usd_etched": null,
-            "usd_foil": "0.51"
+            "usd_foil": "0.44"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A9fc6e1db-cf09-4b8c-be4f-bb02ffe7a188&unique=prints",
         "promo": true,
         "promo_types": [
             "setpromo",
             "prerelease",
             "datestamped"
@@ -6513,14 +6563,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "not_legal",
             "modern": "not_legal",
+            "oathbreaker": "not_legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "not_legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -6534,18 +6585,18 @@
         "name": "Stairs to Infinity",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "7a425df4-7010-462e-9cb5-20389bac721c",
         "oracle_text": "Players have no maximum hand size.\nWhenever you roll the planar die, draw a card.\nWhenever you roll {CHAOS}, reveal the top card of your planar deck. You may put it on the bottom of your planar deck.",
         "oversized": true,
         "prices": {
-            "eur": "0.75",
+            "eur": "1.99",
             "eur_foil": null,
             "tix": null,
-            "usd": "3.80",
+            "usd": "3.70",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A7a425df4-7010-462e-9cb5-20389bac721c&unique=prints",
         "promo": true,
         "promo_types": [
             "instore"
@@ -6586,15 +6637,15 @@
         "card_back_id": "0aeebaf5-8c7d-4636-9e82-8c27447861f7",
         "cardmarket_id": 15173,
         "cmc": 0.0,
         "collector_number": "1",
         "color_identity": [],
         "colors": [],
         "digital": false,
-        "edhrec_rank": 8319,
+        "edhrec_rank": 8334,
         "finishes": [
             "nonfoil"
         ],
         "foil": false,
         "frame": "1993",
         "full_art": false,
         "games": [
@@ -6625,14 +6676,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "not_legal",
             "predh": "legal",
             "premodern": "not_legal",
@@ -6645,20 +6697,20 @@
         ],
         "name": "Arena",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "12326d23-1fb5-4084-a23a-d6e2c90ea36c",
         "oracle_text": "{3}, {T}: Tap target creature you control and target creature of an opponent's choice they control. Those creatures fight each other. (Each deals damage equal to its power to the other.)",
         "oversized": false,
-        "penny_rank": 5142,
+        "penny_rank": 5125,
         "prices": {
-            "eur": "4.50",
+            "eur": "5.00",
             "eur_foil": null,
             "tix": null,
-            "usd": "8.46",
+            "usd": "8.48",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A12326d23-1fb5-4084-a23a-d6e2c90ea36c&unique=prints",
         "promo": true,
         "promo_types": [
             "mediainsert"
@@ -6725,15 +6777,15 @@
         "color_identity": [
             "R"
         ],
         "colors": [
             "R"
         ],
         "digital": false,
-        "edhrec_rank": 8405,
+        "edhrec_rank": 8392,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2003",
         "full_art": false,
@@ -6764,14 +6816,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "not_legal",
             "predh": "legal",
             "premodern": "not_legal",
@@ -6786,17 +6839,17 @@
         "name": "Boom // Bust",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "514fdac0-95f4-4034-b891-283fe0fb6da6",
         "oversized": false,
         "penny_rank": 786,
         "prices": {
-            "eur": "0.50",
+            "eur": "0.20",
             "eur_foil": "2.45",
-            "tix": "0.15",
+            "tix": "0.16",
             "usd": "1.64",
             "usd_etched": null,
             "usd_foil": "13.05"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A514fdac0-95f4-4034-b891-283fe0fb6da6&unique=prints",
         "promo": false,
         "rarity": "rare",
@@ -6843,15 +6896,15 @@
         ],
         "colors": [
             "B",
             "U",
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 11385,
+        "edhrec_rank": 11400,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "flavor_text": "Altered by Phyrexian science, corrupted by black mana, and twisted by rage, Ertai still looked in the mirror and saw only glory.",
         "foil": true,
         "frame": "1997",
@@ -6883,14 +6936,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "not_legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "not_legal",
             "predh": "legal",
             "premodern": "legal",
@@ -6905,21 +6959,21 @@
         ],
         "name": "Ertai, the Corrupted",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "36934bd0-b275-4222-926c-b5a74cf0967d",
         "oracle_text": "{U}, {T}, Sacrifice a creature or enchantment: Counter target spell.",
         "oversized": false,
-        "penny_rank": 11155,
+        "penny_rank": 11108,
         "power": "3",
         "prices": {
-            "eur": "1.76",
+            "eur": "1.28",
             "eur_foil": "45.97",
             "tix": "0.14",
-            "usd": "4.01",
+            "usd": "3.92",
             "usd_etched": null,
             "usd_foil": "106.39"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A36934bd0-b275-4222-926c-b5a74cf0967d&unique=prints",
         "promo": false,
         "rarity": "rare",
         "related_uris": {
@@ -6966,15 +7020,15 @@
         ],
         "colors": [
             "B",
             "U",
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 11385,
+        "edhrec_rank": 11400,
         "finishes": [
             "foil"
         ],
         "flavor_text": "Altered by Phyrexian science, corrupted by black mana, and twisted by rage, Ertai still looked in the mirror and saw only glory.",
         "foil": true,
         "frame": "1997",
         "full_art": false,
@@ -7005,14 +7059,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "not_legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "not_legal",
             "predh": "legal",
             "premodern": "legal",
@@ -7025,19 +7080,19 @@
         ],
         "name": "Ertai, the Corrupted",
         "nonfoil": false,
         "object": "card",
         "oracle_id": "36934bd0-b275-4222-926c-b5a74cf0967d",
         "oracle_text": "{U}, {T}, Sacrifice a creature or enchantment: Counter target spell.",
         "oversized": false,
-        "penny_rank": 11155,
+        "penny_rank": 11108,
         "power": "3",
         "prices": {
             "eur": null,
-            "eur_foil": "115.00",
+            "eur_foil": "434.99",
             "tix": null,
             "usd": null,
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A36934bd0-b275-4222-926c-b5a74cf0967d&unique=prints",
         "promo": false,
@@ -7100,15 +7155,15 @@
         "color_identity": [
             "W"
         ],
         "colors": [
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 2265,
+        "edhrec_rank": 2268,
         "finishes": [
             "foil"
         ],
         "foil": true,
         "frame": "2003",
         "full_art": false,
         "games": [
@@ -7139,14 +7194,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "not_legal",
             "predh": "legal",
             "premodern": "not_legal",
@@ -7160,19 +7216,19 @@
         "object": "card",
         "oracle_id": "454a8902-8120-4373-96ee-bbf352b04e8d",
         "oracle_text": "Battle cry (Whenever this creature attacks, each other attacking creature gets +1/+0 until end of turn.)\nWhenever Hero of Bladehold attacks, create two 1/1 white Soldier creature tokens that are tapped and attacking.",
         "oversized": false,
         "power": "3",
         "prices": {
             "eur": null,
-            "eur_foil": "1.50",
+            "eur_foil": "5.12",
             "tix": null,
             "usd": null,
             "usd_etched": null,
-            "usd_foil": "16.36"
+            "usd_foil": "16.62"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A454a8902-8120-4373-96ee-bbf352b04e8d&unique=prints",
         "promo": true,
         "promo_types": [
             "setpromo",
             "datestamped",
             "prerelease"
@@ -7216,15 +7272,15 @@
         "cmc": 0.0,
         "collector_number": "266p",
         "color_identity": [
             "G"
         ],
         "colors": [],
         "digital": false,
-        "edhrec_rank": 129,
+        "edhrec_rank": 127,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "frame_effects": [
@@ -7259,14 +7315,15 @@
             "explorer": "legal",
             "future": "legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -7278,20 +7335,20 @@
         "name": "Boseiju, Who Endures",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "bf1341dd-41a3-49f6-87ec-63170dde4324",
         "oracle_text": "{T}: Add {G}.\nChannel \u2014 {1}{G}, Discard Boseiju, Who Endures: Destroy target artifact, enchantment, or nonbasic land an opponent controls. That player may search their library for a land card with a basic land type, put it onto the battlefield, then shuffle. This ability costs {1} less to activate for each legendary creature you control.",
         "oversized": false,
         "prices": {
-            "eur": "33.00",
-            "eur_foil": "34.50",
+            "eur": "31.67",
+            "eur_foil": "40.00",
             "tix": null,
-            "usd": "32.95",
+            "usd": "34.25",
             "usd_etched": null,
-            "usd_foil": "31.24"
+            "usd_foil": "32.17"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Abf1341dd-41a3-49f6-87ec-63170dde4324&unique=prints",
         "produced_mana": [
             "G"
         ],
         "promo": true,
         "promo_types": [
@@ -7336,15 +7393,15 @@
         "cmc": 0.0,
         "collector_number": "266s",
         "color_identity": [
             "G"
         ],
         "colors": [],
         "digital": false,
-        "edhrec_rank": 129,
+        "edhrec_rank": 127,
         "finishes": [
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "frame_effects": [
             "legendary"
@@ -7378,14 +7435,15 @@
             "explorer": "legal",
             "future": "legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -7398,15 +7456,15 @@
         "nonfoil": false,
         "object": "card",
         "oracle_id": "bf1341dd-41a3-49f6-87ec-63170dde4324",
         "oracle_text": "{T}: Add {G}.\nChannel \u2014 {1}{G}, Discard Boseiju, Who Endures: Destroy target artifact, enchantment, or nonbasic land an opponent controls. That player may search their library for a land card with a basic land type, put it onto the battlefield, then shuffle. This ability costs {1} less to activate for each legendary creature you control.",
         "oversized": false,
         "prices": {
             "eur": null,
-            "eur_foil": "33.99",
+            "eur_foil": "40.00",
             "tix": null,
             "usd": null,
             "usd_etched": null,
             "usd_foil": "33.84"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Abf1341dd-41a3-49f6-87ec-63170dde4324&unique=prints",
         "produced_mana": [
@@ -7475,15 +7533,15 @@
         "color_identity": [
             "W"
         ],
         "colors": [
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 3899,
+        "edhrec_rank": 3910,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "full_art": false,
@@ -7515,14 +7573,15 @@
             "explorer": "legal",
             "future": "not_legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "legal",
             "pioneer": "legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -7533,23 +7592,23 @@
         "multiverse_ids": [],
         "name": "Tithe Taker",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "c916b81f-700e-4a1a-8c8e-c4685ceaecd2",
         "oracle_text": "During your turn, spells your opponents cast cost {1} more to cast and abilities your opponents activate cost {1} more to activate unless they're mana abilities.\nAfterlife 1 (When this creature dies, create a 1/1 white and black Spirit creature token with flying.)",
         "oversized": false,
-        "penny_rank": 1662,
+        "penny_rank": 1661,
         "power": "2",
         "prices": {
-            "eur": "0.58",
-            "eur_foil": "1.40",
+            "eur": "0.50",
+            "eur_foil": "1.25",
             "tix": null,
             "usd": "0.79",
             "usd_etched": null,
-            "usd_foil": "1.44"
+            "usd_foil": "1.43"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ac916b81f-700e-4a1a-8c8e-c4685ceaecd2&unique=prints",
         "promo": true,
         "promo_types": [
             "setpromo",
             "promopack",
             "stamped"
@@ -7614,15 +7673,15 @@
         "color_identity": [
             "W"
         ],
         "colors": [
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 3899,
+        "edhrec_rank": 3910,
         "finishes": [
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "full_art": false,
         "games": [
@@ -7653,14 +7712,15 @@
             "explorer": "legal",
             "future": "not_legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "legal",
             "pioneer": "legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -7671,15 +7731,15 @@
         "multiverse_ids": [],
         "name": "Tithe Taker",
         "nonfoil": false,
         "object": "card",
         "oracle_id": "c916b81f-700e-4a1a-8c8e-c4685ceaecd2",
         "oracle_text": "During your turn, spells your opponents cast cost {1} more to cast and abilities your opponents activate cost {1} more to activate unless they're mana abilities.\nAfterlife 1 (When this creature dies, create a 1/1 white and black Spirit creature token with flying.)",
         "oversized": false,
-        "penny_rank": 1662,
+        "penny_rank": 1661,
         "power": "2",
         "prices": {
             "eur": null,
             "eur_foil": "1.40",
             "tix": null,
             "usd": null,
             "usd_etched": null,
@@ -7768,14 +7828,15 @@
             "explorer": "legal",
             "future": "legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "legal",
             "paupercommander": "legal",
             "penny": "legal",
             "pioneer": "legal",
             "predh": "legal",
             "premodern": "legal",
@@ -7882,14 +7943,15 @@
             "explorer": "legal",
             "future": "legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "legal",
             "paupercommander": "legal",
             "penny": "legal",
             "pioneer": "legal",
             "predh": "legal",
             "premodern": "legal",
@@ -7907,15 +7969,15 @@
         "preview": {
             "previewed_at": "2018-12-17",
             "source": "Wizards of the Coast",
             "source_uri": "https://magic.wizards.com/en/articles/archive/feature/magic-gathering-chandra-preview-2018-12-05"
         },
         "prices": {
             "eur": null,
-            "eur_foil": "1.96",
+            "eur_foil": "1.58",
             "tix": null,
             "usd": null,
             "usd_etched": null,
             "usd_foil": "3.44"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Abc71ebf6-2056-41f7-be35-b2e5c34afa99&unique=prints",
         "produced_mana": [
@@ -8046,14 +8108,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "not_legal",
             "modern": "not_legal",
+            "oathbreaker": "not_legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "not_legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -8153,14 +8216,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "not_legal",
+            "oathbreaker": "legal",
             "oldschool": "legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "legal",
             "pioneer": "not_legal",
             "predh": "legal",
             "premodern": "legal",
@@ -8173,15 +8237,15 @@
         "nonfoil": true,
         "object": "card",
         "oracle_id": "92eed395-62ca-4293-882b-8565c40daab5",
         "oracle_text": "At the beginning of your draw step, you may draw two additional cards. If you do, choose two cards in your hand drawn this turn. For each of those cards, pay 4 life or put the card on top of your library.",
         "oversized": false,
         "penny_rank": 80,
         "prices": {
-            "eur": "32.00",
+            "eur": "22.90",
             "eur_foil": null,
             "tix": null,
             "usd": "140.40",
             "usd_etched": null,
             "usd_foil": null
         },
         "printed_name": "Biblioth\u00e8que sylvestre",
@@ -8245,15 +8309,15 @@
         "color_identity": [
             "W"
         ],
         "colors": [
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 3899,
+        "edhrec_rank": 3910,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "full_art": false,
@@ -8287,14 +8351,15 @@
             "explorer": "legal",
             "future": "not_legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "legal",
             "pioneer": "legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -8308,26 +8373,26 @@
         ],
         "name": "Tithe Taker",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "c916b81f-700e-4a1a-8c8e-c4685ceaecd2",
         "oracle_text": "During your turn, spells your opponents cast cost {1} more to cast and abilities your opponents activate cost {1} more to activate unless they're mana abilities.\nAfterlife 1 (When this creature dies, create a 1/1 white and black Spirit creature token with flying.)",
         "oversized": false,
-        "penny_rank": 1662,
+        "penny_rank": 1661,
         "power": "2",
         "preview": {
             "previewed_at": "2018-12-17",
             "source": "Wizards of the Coast",
             "source_uri": "https://magic.wizards.com/en/articles/archive/feature/ravnica-allegiance-mechanics-2018-12-17"
         },
         "prices": {
-            "eur": "0.43",
-            "eur_foil": "0.70",
+            "eur": "0.42",
+            "eur_foil": "1.00",
             "tix": "0.02",
-            "usd": "0.74",
+            "usd": "0.70",
             "usd_etched": null,
             "usd_foil": "1.77"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ac916b81f-700e-4a1a-8c8e-c4685ceaecd2&unique=prints",
         "promo": false,
         "rarity": "rare",
         "related_uris": {
@@ -8372,15 +8437,15 @@
         "color_identity": [
             "G"
         ],
         "colors": [
             "G"
         ],
         "digital": false,
-        "edhrec_rank": 14823,
+        "edhrec_rank": 14847,
         "finishes": [
             "foil"
         ],
         "foil": true,
         "frame": "1997",
         "full_art": false,
         "games": [
@@ -8409,14 +8474,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "legal",
             "pioneer": "not_legal",
             "predh": "legal",
             "premodern": "legal",
@@ -8427,15 +8493,15 @@
         "multiverse_ids": [],
         "name": "Rhox",
         "nonfoil": false,
         "object": "card",
         "oracle_id": "f6f4c684-2915-4a58-9c4b-487387f7cf73",
         "oracle_text": "You may have Rhox assign its combat damage as though it weren't blocked.\n{2}{G}: Regenerate Rhox. (The next time this creature would be destroyed this turn, it isn't. Instead tap it, remove all damage from it, and remove it from combat.)",
         "oversized": false,
-        "penny_rank": 10329,
+        "penny_rank": 10455,
         "power": "5",
         "prices": {
             "eur": null,
             "eur_foil": "1.19",
             "tix": null,
             "usd": null,
             "usd_etched": null,
@@ -8525,15 +8591,15 @@
                 "oracle_text": "{3}, {T}: Double the amount of each type of unspent mana you have.",
                 "type_line": "Artifact"
             }
         ],
         "collector_number": "1080",
         "color_identity": [],
         "digital": false,
-        "edhrec_rank": 3160,
+        "edhrec_rank": 3149,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "full_art": false,
@@ -8554,14 +8620,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "legal",
             "pioneer": "not_legal",
             "predh": "legal",
             "premodern": "not_legal",
@@ -8569,22 +8636,22 @@
             "vintage": "legal"
         },
         "multiverse_ids": [],
         "name": "Doubling Cube // Doubling Cube",
         "nonfoil": true,
         "object": "card",
         "oversized": false,
-        "penny_rank": 11392,
+        "penny_rank": 11549,
         "prices": {
             "eur": null,
             "eur_foil": null,
             "tix": null,
-            "usd": "7.15",
+            "usd": "7.13",
             "usd_etched": null,
-            "usd_foil": "7.43"
+            "usd_foil": "7.37"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A9afd8f12-0796-4500-aaa3-10b4a46ef6ec&unique=prints",
         "promo": false,
         "rarity": "rare",
         "related_uris": {
             "edhrec": "https://edhrec.com/route/?cc=Doubling+Cube+%2F%2F+Doubling+Cube",
             "tcgplayer_infinite_articles": "https://infinite.tcgplayer.com/search?contentMode=article&game=magic&partner=scryfall&q=Doubling+Cube+%2F%2F+Doubling+Cube&utm_campaign=affiliate&utm_medium=api&utm_source=scryfall",
@@ -9086,14 +9153,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "not_legal",
             "modern": "not_legal",
+            "oathbreaker": "not_legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "not_legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -9108,16 +9176,16 @@
         "nonfoil": true,
         "object": "card",
         "oracle_id": "4465eff4-5851-4721-a248-866c686c2ab8",
         "oracle_text": "",
         "oversized": false,
         "power": "1",
         "prices": {
-            "eur": "0.74",
-            "eur_foil": "1.25",
+            "eur": "0.75",
+            "eur_foil": "1.50",
             "tix": null,
             "usd": "1.72",
             "usd_etched": null,
             "usd_foil": "1.75"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A4465eff4-5851-4721-a248-866c686c2ab8&unique=prints",
         "promo": false,
@@ -9201,14 +9269,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "legal",
             "paupercommander": "legal",
             "penny": "legal",
             "pioneer": "not_legal",
             "predh": "legal",
             "premodern": "not_legal",
@@ -9339,14 +9408,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "legal",
             "pioneer": "not_legal",
             "predh": "banned",
             "premodern": "not_legal",
@@ -9360,21 +9430,21 @@
             87599
         ],
         "name": "Erayo, Soratami Ascendant // Erayo's Essence",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "d83bb32d-f409-421a-9d93-bd7ea3240b47",
         "oversized": false,
-        "penny_rank": 2358,
+        "penny_rank": 2357,
         "power": "1",
         "prices": {
-            "eur": "4.70",
+            "eur": "3.99",
             "eur_foil": "25.00",
-            "tix": "0.01",
-            "usd": "5.77",
+            "tix": "0.02",
+            "usd": "5.76",
             "usd_etched": null,
             "usd_foil": "40.28"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ad83bb32d-f409-421a-9d93-bd7ea3240b47&unique=prints",
         "promo": false,
         "rarity": "rare",
         "related_uris": {
@@ -9450,14 +9520,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "not_legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "legal",
             "paupercommander": "legal",
             "penny": "not_legal",
             "pioneer": "not_legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -9474,15 +9545,15 @@
         "oracle_id": "c3e5d355-fbfb-4489-aeea-8b0ea5de6fcd",
         "oracle_text": "{TK}{TK} \u2014 {T}: Add {C}{C}. Spend this mana only to cast noncreature spells.\n{TK}{TK}{TK} \u2014 Infect (This permanent deals damage to creatures in the form of -1/-1 counters and to players in the form of poison counters.)\n{TK}{TK} \u2014 3/2\n{TK}{TK}{TK}{TK} \u2014 4/7",
         "oversized": false,
         "prices": {
             "eur": "0.19",
             "eur_foil": null,
             "tix": null,
-            "usd": "0.18",
+            "usd": "0.21",
             "usd_etched": null,
             "usd_foil": null
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ac3e5d355-fbfb-4489-aeea-8b0ea5de6fcd&unique=prints",
         "produced_mana": [
             "C"
         ],
@@ -9530,15 +9601,15 @@
             "R"
         ],
         "colors": [
             "G",
             "R"
         ],
         "digital": false,
-        "edhrec_rank": 3026,
+        "edhrec_rank": 3035,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "frame_effects": [
@@ -9576,14 +9647,15 @@
             "explorer": "legal",
             "future": "not_legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -9604,18 +9676,18 @@
         "power": "4",
         "preview": {
             "previewed_at": "2019-12-24",
             "source": "Wizards of the Coast",
             "source_uri": "https://twitter.com/MTG_Arena/status/1209549655878422529"
         },
         "prices": {
-            "eur": "6.88",
-            "eur_foil": "8.90",
-            "tix": "1.42",
-            "usd": "4.10",
+            "eur": "7.22",
+            "eur_foil": "6.00",
+            "tix": "1.50",
+            "usd": "4.12",
             "usd_etched": null,
             "usd_foil": "5.42"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ae8473969-195f-41ee-a84d-463cc8c0ef02&unique=prints",
         "produced_mana": [
             "G",
             "R"
@@ -9666,15 +9738,15 @@
             "R"
         ],
         "colors": [
             "G",
             "R"
         ],
         "digital": false,
-        "edhrec_rank": 3026,
+        "edhrec_rank": 3035,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "frame_effects": [
@@ -9714,14 +9786,15 @@
             "explorer": "legal",
             "future": "not_legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -9739,20 +9812,20 @@
         "power": "4",
         "preview": {
             "previewed_at": "2020-01-02",
             "source": "Wizards of the Coast",
             "source_uri": "https://magic.wizards.com/en/articles/archive/card-image-gallery/theros-beyond-death-variants"
         },
         "prices": {
-            "eur": "5.50",
-            "eur_foil": "14.99",
+            "eur": "6.98",
+            "eur_foil": "9.90",
             "tix": null,
-            "usd": "2.98",
+            "usd": "3.00",
             "usd_etched": null,
-            "usd_foil": "3.94"
+            "usd_foil": "4.06"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ae8473969-195f-41ee-a84d-463cc8c0ef02&unique=prints",
         "produced_mana": [
             "G",
             "R"
         ],
         "promo": false,
@@ -9801,15 +9874,15 @@
         "color_identity": [
             "G"
         ],
         "colors": [
             "G"
         ],
         "digital": false,
-        "edhrec_rank": 725,
+        "edhrec_rank": 727,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "flavor_text": "Ancient yet ever-young, it is wise and subtle\u2014and cruel and reckless as the spring itself.",
         "foil": true,
         "frame": "2015",
@@ -9847,14 +9920,15 @@
             "explorer": "legal",
             "future": "not_legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -9875,20 +9949,20 @@
         "power": "5",
         "preview": {
             "previewed_at": "2020-01-09",
             "source": "The Command Zone",
             "source_uri": "https://www.youtube.com/watch?v=FrSbBMp45rg"
         },
         "prices": {
-            "eur": "9.98",
+            "eur": "9.11",
             "eur_foil": "14.45",
-            "tix": "0.37",
-            "usd": "19.68",
+            "tix": "0.45",
+            "usd": "19.34",
             "usd_etched": null,
-            "usd_foil": "22.09"
+            "usd_foil": "22.35"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A8b610f8f-c8dd-4eeb-bc6e-3bc706d5f63e&unique=prints",
         "promo": false,
         "rarity": "mythic",
         "related_uris": {
             "edhrec": "https://edhrec.com/route/?cc=Nyxbloom+Ancient",
             "gatherer": "https://gatherer.wizards.com/Pages/Card/Details.aspx?multiverseid=476441",
@@ -9930,15 +10004,15 @@
         "color_identity": [
             "G"
         ],
         "colors": [
             "G"
         ],
         "digital": false,
-        "edhrec_rank": 725,
+        "edhrec_rank": 727,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "frame_effects": [
@@ -9976,14 +10050,15 @@
             "explorer": "legal",
             "future": "not_legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -9996,20 +10071,20 @@
         "nonfoil": true,
         "object": "card",
         "oracle_id": "8b610f8f-c8dd-4eeb-bc6e-3bc706d5f63e",
         "oracle_text": "Trample\nIf you tap a permanent for mana, it produces three times as much of that mana instead.",
         "oversized": false,
         "power": "5",
         "prices": {
-            "eur": "17.50",
-            "eur_foil": "57.35",
+            "eur": "15.46",
+            "eur_foil": "55.00",
             "tix": null,
-            "usd": "27.35",
+            "usd": "27.06",
             "usd_etched": null,
-            "usd_foil": "70.20"
+            "usd_foil": "70.43"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A8b610f8f-c8dd-4eeb-bc6e-3bc706d5f63e&unique=prints",
         "promo": false,
         "promo_types": [
             "boosterfun"
         ],
         "rarity": "mythic",
@@ -10095,14 +10170,15 @@
             "explorer": "legal",
             "future": "not_legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "legal",
             "pioneer": "legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -10116,27 +10192,27 @@
         ],
         "name": "Temple of Plenty",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "e521322b-0e83-458c-8936-7021a80ee279",
         "oracle_text": "Temple of Plenty enters the battlefield tapped.\nWhen Temple of Plenty enters the battlefield, scry 1.\n{T}: Add {G} or {W}.",
         "oversized": false,
-        "penny_rank": 974,
+        "penny_rank": 976,
         "preview": {
             "previewed_at": "2019-12-30",
             "source": "ChannelFireball",
             "source_uri": "https://www.channelfireball.com/all-strategy/articles/3-point/theros-beyond-death-exclusive-preview/"
         },
         "prices": {
-            "eur": "0.32",
-            "eur_foil": "1.49",
+            "eur": "0.23",
+            "eur_foil": "0.30",
             "tix": "0.02",
-            "usd": "0.70",
+            "usd": "0.65",
             "usd_etched": null,
-            "usd_foil": "0.93"
+            "usd_foil": "0.94"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ae521322b-0e83-458c-8936-7021a80ee279&unique=prints",
         "produced_mana": [
             "G",
             "W"
         ],
         "promo": false,
@@ -10225,14 +10301,15 @@
             "explorer": "legal",
             "future": "not_legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "legal",
             "pioneer": "legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -10243,25 +10320,25 @@
         "multiverse_ids": [],
         "name": "Temple of Plenty",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "e521322b-0e83-458c-8936-7021a80ee279",
         "oracle_text": "Temple of Plenty enters the battlefield tapped.\nWhen Temple of Plenty enters the battlefield, scry 1.\n{T}: Add {G} or {W}.",
         "oversized": false,
-        "penny_rank": 974,
+        "penny_rank": 976,
         "preview": {
             "previewed_at": "2019-12-30",
             "source": "ChannelFireball",
             "source_uri": "https://www.channelfireball.com/all-strategy/articles/3-point/theros-beyond-death-exclusive-preview/"
         },
         "prices": {
-            "eur": "2.10",
+            "eur": "2.99",
             "eur_foil": "3.40",
             "tix": null,
-            "usd": "2.23",
+            "usd": "2.21",
             "usd_etched": null,
             "usd_foil": "10.28"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Ae521322b-0e83-458c-8936-7021a80ee279&unique=prints",
         "produced_mana": [
             "G",
             "W"
@@ -10329,15 +10406,15 @@
         "color_identity": [
             "G"
         ],
         "colors": [
             "G"
         ],
         "digital": false,
-        "edhrec_rank": 2945,
+        "edhrec_rank": 2949,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "full_art": false,
@@ -10371,14 +10448,15 @@
             "explorer": "legal",
             "future": "not_legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -10392,27 +10470,27 @@
         ],
         "name": "Wolfwillow Haven",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "7579f57d-c76e-4703-a030-34fb7160cb23",
         "oracle_text": "Enchant land\nWhenever enchanted land is tapped for mana, its controller adds an additional {G}.\n{4}{G}, Sacrifice Wolfwillow Haven: Create a 2/2 green Wolf creature token. Activate only during your turn.",
         "oversized": false,
-        "penny_rank": 2290,
+        "penny_rank": 2289,
         "preview": {
             "previewed_at": "2020-01-09",
             "source": "Drawza",
             "source_uri": "https://www.twitch.tv/drawza"
         },
         "prices": {
-            "eur": "0.14",
-            "eur_foil": "0.75",
+            "eur": "0.21",
+            "eur_foil": "0.49",
             "tix": "0.03",
-            "usd": "0.35",
+            "usd": "0.36",
             "usd_etched": null,
-            "usd_foil": "0.51"
+            "usd_foil": "0.50"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A7579f57d-c76e-4703-a030-34fb7160cb23&unique=prints",
         "produced_mana": [
             "G"
         ],
         "promo": false,
         "rarity": "uncommon",
@@ -10473,15 +10551,15 @@
         "color_identity": [
             "G"
         ],
         "colors": [
             "G"
         ],
         "digital": false,
-        "edhrec_rank": 2945,
+        "edhrec_rank": 2949,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "frame_effects": [
@@ -10518,14 +10596,15 @@
             "explorer": "legal",
             "future": "not_legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -10536,22 +10615,22 @@
         "multiverse_ids": [],
         "name": "Wolfwillow Haven",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "7579f57d-c76e-4703-a030-34fb7160cb23",
         "oracle_text": "Enchant land\nWhenever enchanted land is tapped for mana, its controller adds an additional {G}.\n{4}{G}, Sacrifice Wolfwillow Haven: Create a 2/2 green Wolf creature token. Activate only during your turn.",
         "oversized": false,
-        "penny_rank": 2290,
+        "penny_rank": 2289,
         "prices": {
-            "eur": "0.05",
-            "eur_foil": "0.40",
+            "eur": "0.84",
+            "eur_foil": "0.09",
             "tix": null,
-            "usd": "1.07",
+            "usd": "1.03",
             "usd_etched": null,
-            "usd_foil": "3.73"
+            "usd_foil": "3.94"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A7579f57d-c76e-4703-a030-34fb7160cb23&unique=prints",
         "produced_mana": [
             "G"
         ],
         "promo": true,
         "promo_types": [
@@ -10680,14 +10759,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "not_legal",
             "modern": "not_legal",
+            "oathbreaker": "not_legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "not_legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -10700,18 +10780,18 @@
         ],
         "name": "Who // What // When // Where // Why",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "adfe1b07-dd82-4c39-a7a6-ded0b1c39761",
         "oversized": false,
         "prices": {
-            "eur": "1.95",
+            "eur": "2.99",
             "eur_foil": "50.00",
             "tix": null,
-            "usd": "1.60",
+            "usd": "1.59",
             "usd_etched": null,
             "usd_foil": "51.92"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Aadfe1b07-dd82-4c39-a7a6-ded0b1c39761&unique=prints",
         "promo": false,
         "rarity": "rare",
         "related_uris": {
@@ -10842,14 +10922,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "not_legal",
             "modern": "not_legal",
+            "oathbreaker": "not_legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "not_legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -10863,15 +10944,15 @@
         "name": "Very Cryptic Command",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "5d0fd8ee-2cc1-4ed8-9395-1660d15cc9f3",
         "oracle_text": "Choose two \u2014\n\u2022 Switch target creature's power and toughness until end of turn.\n\u2022 Target creature can't be blocked this turn.\n\u2022 Draw a card. If that card's art is by Wayne England, you may reveal it and draw another card.\n\u2022 Assemble a Contraption.",
         "oversized": false,
         "prices": {
-            "eur": "1.85",
+            "eur": "2.99",
             "eur_foil": "25.99",
             "tix": null,
             "usd": "1.61",
             "usd_etched": null,
             "usd_foil": "24.99"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A5d0fd8ee-2cc1-4ed8-9395-1660d15cc9f3&unique=prints",
@@ -11004,14 +11085,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "not_legal",
             "modern": "not_legal",
+            "oathbreaker": "not_legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "not_legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -11025,15 +11107,15 @@
         "name": "Very Cryptic Command",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "48d94218-a460-4974-82b9-d3a9cba9998e",
         "oracle_text": "Choose two \u2014\n\u2022 Untap two target permanents.\n\u2022 Tap each permanent target player controls with exactly one word in its name.\n\u2022 Discard all the cards in your hand, then draw that many cards.\n\u2022 Return target instant or sorcery card from your graveyard to your hand.",
         "oversized": false,
         "prices": {
-            "eur": "1.75",
+            "eur": "2.50",
             "eur_foil": "7.99",
             "tix": null,
             "usd": "1.53",
             "usd_etched": null,
             "usd_foil": "8.94"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A48d94218-a460-4974-82b9-d3a9cba9998e&unique=prints",
@@ -11174,14 +11256,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "not_legal",
             "modern": "not_legal",
+            "oathbreaker": "not_legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "not_legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -11195,18 +11278,18 @@
         "name": "Very Cryptic Command",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "5063f840-0aed-4e2d-98d8-65b39e95e3c9",
         "oracle_text": "Choose two \u2014\n\u2022 Draw a card from an opponent's library.\n\u2022 Copy target instant or sorcery spell. You may choose new targets for the copy.\n\u2022 Until end of turn, target creature loses all abilities and becomes a blue Frog with base power and toughness 1/1.\n\u2022 Create a 1/1 colorless Gnome artifact creature token.",
         "oversized": false,
         "prices": {
-            "eur": "2.90",
+            "eur": "3.50",
             "eur_foil": "9.99",
             "tix": null,
-            "usd": "2.16",
+            "usd": "2.15",
             "usd_etched": null,
             "usd_foil": "9.00"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A5063f840-0aed-4e2d-98d8-65b39e95e3c9&unique=prints",
         "promo": false,
         "rarity": "rare",
         "related_uris": {
@@ -11336,14 +11419,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "not_legal",
             "modern": "not_legal",
+            "oathbreaker": "not_legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "not_legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -11357,18 +11441,18 @@
         "name": "Very Cryptic Command",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "9dc00e2b-73a3-42d5-95c9-d86094a6e455",
         "oracle_text": "Choose two \u2014\n\u2022 Return target permanent to its controller's hand.\n\u2022 Draw two cards, then discard a card.\n\u2022 Change the target of target spell with a single target.\n\u2022 Turn over target nontoken creature.",
         "oversized": false,
         "prices": {
-            "eur": "2.49",
+            "eur": "2.75",
             "eur_foil": "26.08",
             "tix": null,
-            "usd": "3.32",
+            "usd": "3.28",
             "usd_etched": null,
             "usd_foil": "18.95"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A9dc00e2b-73a3-42d5-95c9-d86094a6e455&unique=prints",
         "promo": false,
         "rarity": "rare",
         "related_uris": {
@@ -11500,14 +11584,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "not_legal",
             "modern": "not_legal",
+            "oathbreaker": "not_legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "not_legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -11521,18 +11606,18 @@
         "name": "Very Cryptic Command",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "a84f0b11-5c59-4bab-81ef-a84470fb2ade",
         "oracle_text": "Choose two \u2014\n\u2022 Counter target black-bordered spell.\n\u2022 Return target creature to its owner's hand.\n\u2022 Untap each permanent you control with a watermark.\n\u2022 Roll two six-sided dice. Target player mills X cards, where X is the total of those results.",
         "oversized": false,
         "prices": {
-            "eur": "2.01",
+            "eur": "2.75",
             "eur_foil": "9.99",
             "tix": null,
-            "usd": "3.36",
+            "usd": "3.38",
             "usd_etched": null,
             "usd_foil": "15.37"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3Aa84f0b11-5c59-4bab-81ef-a84470fb2ade&unique=prints",
         "promo": false,
         "rarity": "rare",
         "related_uris": {
@@ -11672,14 +11757,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "not_legal",
             "modern": "not_legal",
+            "oathbreaker": "not_legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "not_legal",
             "pioneer": "not_legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -11693,15 +11779,15 @@
         "name": "Very Cryptic Command",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "684dfe99-c957-4b91-bd14-867c20b4b3db",
         "oracle_text": "Choose two \u2014\n\u2022 Scry 3.\n\u2022 Create a 2/2 black Rogue creature token with menace.\n\u2022 Add or subtract 1 or one from a number or number word on target spell or permanent until end of turn.\n\u2022 Return all artifacts target player controls to their owner's hand.",
         "oversized": false,
         "prices": {
-            "eur": "2.49",
+            "eur": "2.47",
             "eur_foil": "9.00",
             "tix": null,
             "usd": "1.53",
             "usd_etched": null,
             "usd_foil": "6.49"
         },
         "prints_search_uri": "https://api.scryfall.com/cards/search?order=released&q=oracleid%3A684dfe99-c957-4b91-bd14-867c20b4b3db&unique=prints",
@@ -11746,15 +11832,15 @@
         "color_identity": [
             "U"
         ],
         "colors": [
             "U"
         ],
         "digital": true,
-        "edhrec_rank": 14697,
+        "edhrec_rank": 14751,
         "finishes": [
             "nonfoil",
             "foil"
         ],
         "foil": true,
         "frame": "2015",
         "full_art": false,
@@ -11784,14 +11870,15 @@
             "explorer": "not_legal",
             "future": "not_legal",
             "gladiator": "not_legal",
             "historic": "not_legal",
             "historicbrawl": "not_legal",
             "legacy": "legal",
             "modern": "not_legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "not_legal",
             "penny": "legal",
             "pioneer": "not_legal",
             "predh": "not_legal",
             "premodern": "not_legal",
@@ -11806,15 +11893,15 @@
         ],
         "name": "Academy Elite",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "ba6c3c72-c014-45c6-a0b4-59eb9a65303e",
         "oracle_text": "Academy Elite enters the battlefield with X +1/+1 counters on it, where X is the number of instant and sorcery cards in all graveyards.\n{2}{U}, Remove a +1/+1 counter from Academy Elite: Draw a card, then discard a card.",
         "oversized": false,
-        "penny_rank": 3774,
+        "penny_rank": 3771,
         "power": "0",
         "prices": {
             "eur": null,
             "eur_foil": null,
             "tix": "0.02",
             "usd": null,
             "usd_etched": null,
@@ -11863,15 +11950,15 @@
         "color_identity": [
             "W"
         ],
         "colors": [
             "W"
         ],
         "digital": false,
-        "edhrec_rank": 8454,
+        "edhrec_rank": 8442,
         "finishes": [
             "nonfoil"
         ],
         "flavor_text": "Follow the light. In its absence, follow her.",
         "foil": false,
         "frame": "2015",
         "full_art": false,
@@ -11905,14 +11992,15 @@
             "explorer": "legal",
             "future": "not_legal",
             "gladiator": "legal",
             "historic": "legal",
             "historicbrawl": "legal",
             "legacy": "legal",
             "modern": "legal",
+            "oathbreaker": "legal",
             "oldschool": "not_legal",
             "pauper": "not_legal",
             "paupercommander": "restricted",
             "penny": "legal",
             "pioneer": "legal",
             "predh": "legal",
             "premodern": "legal",
@@ -11927,15 +12015,15 @@
         ],
         "name": "Serra Angel",
         "nonfoil": true,
         "object": "card",
         "oracle_id": "4b7ac066-e5c7-43e6-9e7e-2739b24a905d",
         "oracle_text": "Flying, vigilance",
         "oversized": false,
-        "penny_rank": 8569,
+        "penny_rank": 8528,
         "power": "4",
         "prices": {
             "eur": "0.02",
             "eur_foil": null,
             "tix": "0.05",
             "usd": "0.12",
             "usd_etched": null,
```

### Comparing `mtg_ssm-2.6.1.dev1/tests/data/migrations.json` & `mtg_ssm-2.6.2.dev1/tests/data/migrations.json`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/tests/data/sets.json` & `mtg_ssm-2.6.2.dev1/tests/data/sets.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9950429940494715%*

 * *Differences: {"'data'": "{0: {'icon_svg_uri': 'https://svgs.scryfall.io/sets/arc.svg?1678680000'}, 1: "*

 * *           "{'icon_svg_uri': 'https://svgs.scryfall.io/sets/bok.svg?1678680000'}, 2: "*

 * *           "{'icon_svg_uri': 'https://svgs.scryfall.io/sets/chk.svg?1678680000'}, 3: "*

 * *           "{'icon_svg_uri': 'https://svgs.scryfall.io/sets/csp.svg?1678680000'}, 4: "*

 * *           "{'icon_svg_uri': 'https://svgs.scryfall.io/sets/fem.svg?1678680000'}, 5: "*

 * *           "{'icon_svg_uri': 'https://svgs.scryfall.io/sets/hml.svg?16786 […]*

```diff
@@ -1,15 +1,15 @@
 {
     "data": [
         {
             "card_count": 1,
             "code": "arc",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/arc.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/arc.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/bok.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/bok.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/chk.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/chk.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/csp.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/csp.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/fem.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/fem.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/hml.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/hml.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/hop.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/hop.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/ice.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/ice.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/isd.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/isd.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/khm.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/khm.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/lea.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/lea.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/mbs.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/mbs.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/mma.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/mma.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/neo.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/neo.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/arc.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/arc.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/ogw.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/ogw.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/hop.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/hop.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/pc2.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/pc2.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/dci.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/dci.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/pc2.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/pc2.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/dci.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/dci.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/frf.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/frf.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/dci.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/dci.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/pbook.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/pbook.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/plc.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/plc.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/pls.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/pls.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/mbs.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/mbs.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/neo.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/neo.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/rna.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/rna.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/rna.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/rna.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/ptg.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/ptg.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/ren.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/ren.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/rna.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/rna.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/s00.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/s00.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/star.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/star.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/sok.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/sok.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/unf.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/unf.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/thb.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/thb.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/unh.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/unh.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/ust.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/ust.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/vma.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/vma.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/w16.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/w16.svg?1678680000",
             "id": "b3a0e4a1-5f2c-44e1-8558-61e6dcd88fda",
             "mtgo_code": "w16",
             "name": "Welcome Deck 2016",
             "nonfoil_only": true,
             "object": "set",
             "released_at": "2016-04-08",
             "scryfall_uri": "https://scryfall.com/sets/w16",
```

### Comparing `mtg_ssm-2.6.1.dev1/tests/data/sets1.json` & `mtg_ssm-2.6.2.dev1/tests/data/sets1.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9963587170979502%*

 * *Differences: {"'data'": "{0: {'icon_svg_uri': 'https://svgs.scryfall.io/sets/arc.svg?1678680000'}, 1: "*

 * *           "{'icon_svg_uri': 'https://svgs.scryfall.io/sets/bok.svg?1678680000'}, 2: "*

 * *           "{'icon_svg_uri': 'https://svgs.scryfall.io/sets/chk.svg?1678680000'}, 3: "*

 * *           "{'icon_svg_uri': 'https://svgs.scryfall.io/sets/csp.svg?1678680000'}, 4: "*

 * *           "{'icon_svg_uri': 'https://svgs.scryfall.io/sets/fem.svg?1678680000'}, 5: "*

 * *           "{'icon_svg_uri': 'https://svgs.scryfall.io/sets/hml.svg?16786 […]*

```diff
@@ -1,15 +1,15 @@
 {
     "data": [
         {
             "card_count": 1,
             "code": "arc",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/arc.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/arc.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/bok.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/bok.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/chk.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/chk.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/csp.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/csp.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/fem.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/fem.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/hml.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/hml.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/hop.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/hop.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/ice.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/ice.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/isd.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/isd.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/khm.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/khm.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/lea.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/lea.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/mbs.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/mbs.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/mma.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/mma.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/neo.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/neo.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/arc.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/arc.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/ogw.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/ogw.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/hop.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/hop.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/pc2.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/pc2.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/dci.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/dci.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/pc2.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/pc2.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/dci.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/dci.svg?1678680000",
             "id": "935e91e9-61c2-4b35-a85a-c08fef3b420b",
             "name": "DCI Promos",
             "nonfoil_only": false,
             "object": "set",
             "released_at": "2006-01-01",
             "scryfall_uri": "https://scryfall.com/sets/pdci",
             "search_uri": "https://api.scryfall.com/cards/search?include_extras=true&include_variations=true&order=set&q=e%3Apdci&unique=prints",
```

### Comparing `mtg_ssm-2.6.1.dev1/tests/data/sets2.json` & `mtg_ssm-2.6.2.dev1/tests/data/sets2.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9949410319683428%*

 * *Differences: {"'data'": "{0: {'icon_svg_uri': 'https://svgs.scryfall.io/sets/frf.svg?1678680000'}, 1: "*

 * *           "{'icon_svg_uri': 'https://svgs.scryfall.io/sets/dci.svg?1678680000'}, 2: "*

 * *           "{'icon_svg_uri': 'https://svgs.scryfall.io/sets/pbook.svg?1678680000'}, 3: "*

 * *           "{'icon_svg_uri': 'https://svgs.scryfall.io/sets/plc.svg?1678680000'}, 4: "*

 * *           "{'icon_svg_uri': 'https://svgs.scryfall.io/sets/pls.svg?1678680000'}, 5: "*

 * *           "{'icon_svg_uri': 'https://svgs.scryfall.io/sets/mbs.svg?167 […]*

```diff
@@ -3,15 +3,15 @@
         {
             "block": "Khans of Tarkir",
             "block_code": "ktk",
             "card_count": 2,
             "code": "pfrf",
             "digital": false,
             "foil_only": false,
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/frf.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/frf.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/dci.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/dci.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/pbook.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/pbook.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/plc.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/plc.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/pls.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/pls.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/mbs.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/mbs.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/neo.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/neo.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/rna.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/rna.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/rna.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/rna.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/ptg.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/ptg.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/ren.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/ren.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/rna.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/rna.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/s00.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/s00.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/star.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/star.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/sok.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/sok.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/unf.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/unf.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/thb.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/thb.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/unh.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/unh.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/ust.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/ust.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/vma.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/vma.svg?1678680000",
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
-            "icon_svg_uri": "https://svgs.scryfall.io/sets/w16.svg?1678078800",
+            "icon_svg_uri": "https://svgs.scryfall.io/sets/w16.svg?1678680000",
             "id": "b3a0e4a1-5f2c-44e1-8558-61e6dcd88fda",
             "mtgo_code": "w16",
             "name": "Welcome Deck 2016",
             "nonfoil_only": true,
             "object": "set",
             "released_at": "2016-04-08",
             "scryfall_uri": "https://scryfall.com/sets/w16",
```

### Comparing `mtg_ssm-2.6.1.dev1/tests/gen_testdata.py` & `mtg_ssm-2.6.2.dev1/tests/gen_testdata.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/tests/mtg/test_util.py` & `mtg_ssm-2.6.2.dev1/tests/mtg/test_util.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/tests/scryfall/test_fetcher.py` & `mtg_ssm-2.6.2.dev1/tests/scryfall/test_fetcher.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/tests/serialization/__snapshots__/test_csv.ambr` & `mtg_ssm-2.6.2.dev1/tests/serialization/__snapshots__/test_csv.ambr`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/tests/serialization/__snapshots__/test_xlsx.ambr` & `mtg_ssm-2.6.2.dev1/tests/serialization/__snapshots__/test_xlsx.ambr`

 * *Files 0% similar despite different names*

```diff
@@ -253,15 +253,15 @@
     list([
       '=I2+J2',
       '=I2*G2+J2*H2',
       'Dark Ritual',
       '120',
       '4ebcd681-1871-4914-bcd7-6bd95829f6e0',
       'Justin Hampton',
-      Decimal('1.03'),
+      Decimal('1.04'),
       None,
       None,
       None,
       '=_xlfn.TEXTJOIN(", ",1,IF(\'LEA\'!A3>0,"LEA:"&\'LEA\'!A3,""),IF(\'HOP\'!A3>0,"HOP:"&\'HOP\'!A3,""))',
     ]),
     list([
       '=I3+J3',
@@ -279,41 +279,41 @@
     list([
       '=I4+J4',
       '=I4*G4+J4*H4',
       'Forest',
       '381',
       'b346b784-7bde-49d0-bfa9-56236cbe19d9',
       'Pat Morrissey',
-      Decimal('1.03'),
+      Decimal('1.01'),
       None,
       None,
       2,
       None,
     ]),
     list([
       '=I5+J5',
       '=I5*G5+J5*H5',
       'Forest',
       '382',
       '768c4d8f-5700-4f0a-9ff2-58422aeb1dac',
       'Pat Morrissey',
-      Decimal('0.45'),
+      Decimal('0.48'),
       None,
       3,
       4,
       None,
     ]),
     list([
       '=I6+J6',
       '=I6*G6+J6*H6',
       'Snow-Covered Forest',
       '383',
       '4c0ad95c-d62c-4138-ada0-fa39a63a449e',
       'Pat Morrissey',
-      Decimal('2.00'),
+      Decimal('2.07'),
       None,
       None,
       None,
       None,
     ]),
   ])
 # ---
@@ -610,15 +610,15 @@
     list([
       '=I5+J5',
       '=I5*G5+J5*H5',
       'Forest',
       '295',
       'f20c89d9-71c9-45f5-a9cb-6e253b0a7cca',
       'Christopher Rush',
-      78.29,
+      76.63,
       None,
       None,
       None,
       None,
     ]),
   ])
 # ---
@@ -709,15 +709,15 @@
     list([
       '=I2+J2',
       '=I2*G2+J2*H2',
       'Dark Ritual',
       '120',
       '4ebcd681-1871-4914-bcd7-6bd95829f6e0',
       'Justin Hampton',
-      1.03,
+      1.04,
       None,
       None,
       None,
       '=_xlfn.TEXTJOIN(", ",1,IF(\'LEA\'!A3>0,"LEA:"&\'LEA\'!A3,""),IF(\'HOP\'!A3>0,"HOP:"&\'HOP\'!A3,""))',
     ]),
     list([
       '=I3+J3',
@@ -735,41 +735,41 @@
     list([
       '=I4+J4',
       '=I4*G4+J4*H4',
       'Forest',
       '381',
       'b346b784-7bde-49d0-bfa9-56236cbe19d9',
       'Pat Morrissey',
-      1.03,
+      1.01,
       None,
       None,
       None,
       None,
     ]),
     list([
       '=I5+J5',
       '=I5*G5+J5*H5',
       'Forest',
       '382',
       '768c4d8f-5700-4f0a-9ff2-58422aeb1dac',
       'Pat Morrissey',
-      0.45,
+      0.48,
       None,
       None,
       None,
       None,
     ]),
     list([
       '=I6+J6',
       '=I6*G6+J6*H6',
       'Snow-Covered Forest',
       '383',
       '4c0ad95c-d62c-4138-ada0-fa39a63a449e',
       'Pat Morrissey',
-      2,
+      2.07,
       None,
       None,
       None,
       None,
     ]),
   ])
 # ---
@@ -821,28 +821,28 @@
     list([
       '=I2+J2',
       '=I2*G2+J2*H2',
       'Bushi Tenderfoot // Kenzo the Hardhearted',
       '2',
       '864ad989-19a6-4930-8efc-bbc077a18c32',
       'Mark Zug',
-      0.23,
+      0.24,
       6.85,
       None,
       None,
       None,
     ]),
     list([
       '=I3+J3',
       '=I3*G3+J3*H3',
       'Boseiju, Who Shelters All',
       '273',
       '0180d9a8-992c-4d55-8ac4-33a587786993',
       'Ralph Horsley',
-      22.91,
+      22.68,
       108.88,
       None,
       None,
       None,
     ]),
   ])
 # ---
@@ -894,15 +894,15 @@
     list([
       '=I2+J2',
       '=I2*G2+J2*H2',
       "Erayo, Soratami Ascendant // Erayo's Essence",
       '35',
       '0b61d772-2d8b-4acf-9dd2-b2e8b03538c8',
       'Matt Cavotta',
-      5.77,
+      5.76,
       40.28,
       None,
       None,
       None,
     ]),
   ])
 # ---
@@ -968,15 +968,15 @@
       '=I2+J2',
       '=I2*G2+J2*H2',
       'Hero of Bladehold',
       '8★',
       '8829efa0-498a-43ca-91aa-f9caeeafe298',
       'Scott Chou',
       None,
-      16.36,
+      16.62,
       None,
       None,
       '=IF(\'MBS\'!A2>0,"MBS:"&\'MBS\'!A2,"")',
     ]),
   ])
 # ---
 # name: test_write[11 - MBS]
@@ -997,29 +997,29 @@
     list([
       '=I2+J2',
       '=I2*G2+J2*H2',
       'Hero of Bladehold',
       '8',
       '8a3853ec-e307-46e0-96d7-0706b5c45c5e',
       'Austin Hsu',
-      15.61,
-      25.93,
+      15.49,
+      26.66,
       None,
       None,
       '=IF(\'PMBS\'!A2>0,"PMBS:"&\'PMBS\'!A2,"")',
     ]),
     list([
       '=I3+J3',
       '=I3*G3+J3*H3',
       "Black Sun's Zenith",
       '39',
       '03bdcf52-50b8-42c0-9665-931d83f5f314',
       'Daniel Ljunggren',
-      5.45,
-      11.56,
+      5.58,
+      11.92,
       None,
       None,
       None,
     ]),
   ])
 # ---
 # name: test_write[12 - NEO]
@@ -1040,42 +1040,42 @@
     list([
       '=I2+J2',
       '=I2*G2+J2*H2',
       'Boseiju, Who Endures',
       '266',
       '2135ac5a-187b-4dc9-8f82-34e8d1603416',
       'Chris Ostrowski',
-      39.26,
-      38.71,
+      37.02,
+      40.06,
       None,
       None,
       '=IF(SUM(\'PNEO\'!A2:A3)>0,"PNEO:"&SUM(\'PNEO\'!A2:A3),"")',
     ]),
     list([
       '=I3+J3',
       '=I3*G3+J3*H3',
       'Boseiju, Who Endures',
       '412',
       '0055ea30-20fb-4324-a632-8fed87628f05',
       'Esuthio',
-      44.99,
-      73.69,
+      42.43,
+      73.67,
       None,
       None,
       '=IF(SUM(\'PNEO\'!A2:A3)>0,"PNEO:"&SUM(\'PNEO\'!A2:A3),"")',
     ]),
     list([
       '=I4+J4',
       '=I4*G4+J4*H4',
       'Boseiju, Who Endures',
       '501',
       '2488a80b-6882-4b59-8232-f02f800204a9',
       'Chris Ostrowski',
-      39.76,
-      44.39,
+      40.9,
+      45.41,
       None,
       None,
       '=IF(SUM(\'PNEO\'!A2:A3)>0,"PNEO:"&SUM(\'PNEO\'!A2:A3),"")',
     ]),
   ])
 # ---
 # name: test_write[13 - PNEO]
@@ -1096,16 +1096,16 @@
     list([
       '=I2+J2',
       '=I2*G2+J2*H2',
       'Boseiju, Who Endures',
       '266p',
       'dda82840-1f3f-4be7-9bc7-66ff551ef5c0',
       'Chris Ostrowski',
-      32.95,
-      31.24,
+      34.25,
+      32.17,
       None,
       None,
       '=IF(SUM(\'NEO\'!A2:A4)>0,"NEO:"&SUM(\'NEO\'!A2:A4),"")',
     ]),
     list([
       '=I3+J3',
       '=I3*G3+J3*H3',
```

### Comparing `mtg_ssm-2.6.1.dev1/tests/serialization/test_csv.py` & `mtg_ssm-2.6.2.dev1/tests/serialization/test_csv.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/tests/serialization/test_interface.py` & `mtg_ssm-2.6.2.dev1/tests/serialization/test_interface.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/tests/serialization/test_xlsx.py` & `mtg_ssm-2.6.2.dev1/tests/serialization/test_xlsx.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.1.dev1/tests/test_ssm.py` & `mtg_ssm-2.6.2.dev1/tests/test_ssm.py`

 * *Files identical despite different names*

