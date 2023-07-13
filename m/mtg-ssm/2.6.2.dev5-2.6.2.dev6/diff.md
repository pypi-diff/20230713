# Comparing `tmp/mtg_ssm-2.6.2.dev5.tar.gz` & `tmp/mtg_ssm-2.6.2.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtg_ssm-2.6.2.dev5.tar", last modified: Thu Jul 13 08:32:37 2023, max compression
+gzip compressed data, was "mtg_ssm-2.6.2.dev6.tar", last modified: Thu Jul 13 09:05:24 2023, max compression
```

## Comparing `mtg_ssm-2.6.2.dev5.tar` & `mtg_ssm-2.6.2.dev6.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:32:37.054699 mtg_ssm-2.6.2.dev5/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:32:37.030698 mtg_ssm-2.6.2.dev5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:32:37.034698 mtg_ssm-2.6.2.dev5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/.github/workflows/integration.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-07-13 08:32:37.054699 mtg_ssm-2.6.2.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/TODO.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:32:37.034698 mtg_ssm-2.6.2.dev5/mtg_ssm/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/mtg_ssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-13 08:32:36.000000 mtg_ssm-2.6.2.dev5/mtg_ssm/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:32:37.034698 mtg_ssm-2.6.2.dev5/mtg_ssm/containers/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/mtg_ssm/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/mtg_ssm/containers/bundles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/mtg_ssm/containers/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/mtg_ssm/containers/counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/mtg_ssm/containers/indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/mtg_ssm/containers/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:32:37.038698 mtg_ssm-2.6.2.dev5/mtg_ssm/mtg/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/mtg_ssm/mtg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/mtg_ssm/mtg/util.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/mtg_ssm/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:32:37.038698 mtg_ssm-2.6.2.dev5/mtg_ssm/scryfall/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/mtg_ssm/scryfall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/mtg_ssm/scryfall/fetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/mtg_ssm/scryfall/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:32:37.038698 mtg_ssm-2.6.2.dev5/mtg_ssm/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/mtg_ssm/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/mtg_ssm/serialization/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/mtg_ssm/serialization/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/mtg_ssm/serialization/xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)    10331 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/mtg_ssm/ssm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:32:37.034698 mtg_ssm-2.6.2.dev5/mtg_ssm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-07-13 08:32:36.000000 mtg_ssm-2.6.2.dev5/mtg_ssm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-13 08:32:37.000000 mtg_ssm-2.6.2.dev5/mtg_ssm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 08:32:36.000000 mtg_ssm-2.6.2.dev5/mtg_ssm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 08:32:36.000000 mtg_ssm-2.6.2.dev5/mtg_ssm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-13 08:32:36.000000 mtg_ssm-2.6.2.dev5/mtg_ssm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 08:32:36.000000 mtg_ssm-2.6.2.dev5/mtg_ssm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 08:32:37.054699 mtg_ssm-2.6.2.dev5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:32:37.038698 mtg_ssm-2.6.2.dev5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:32:37.042698 mtg_ssm-2.6.2.dev5/tests/containers/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/tests/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/tests/containers/test_bundles.py
--rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/tests/containers/test_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/tests/containers/test_indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/tests/containers/test_legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:32:37.046698 mtg_ssm-2.6.2.dev5/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/tests/data/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/tests/data/bulk_data.json
--rw-r--r--   0 runner    (1001) docker     (123)   456765 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/tests/data/cards.json
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/tests/data/migrations.json
--rw-r--r--   0 runner    (1001) docker     (123)    31317 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/tests/data/sets.json
--rw-r--r--   0 runner    (1001) docker     (123)    15912 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/tests/data/sets1.json
--rw-r--r--   0 runner    (1001) docker     (123)    15519 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/tests/data/sets2.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     6683 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/tests/gen_testdata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:32:37.046698 mtg_ssm-2.6.2.dev5/tests/mtg/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/tests/mtg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/tests/mtg/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:32:37.050699 mtg_ssm-2.6.2.dev5/tests/scryfall/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/tests/scryfall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/tests/scryfall/test_fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:32:37.054699 mtg_ssm-2.6.2.dev5/tests/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/tests/serialization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:32:37.054699 mtg_ssm-2.6.2.dev5/tests/serialization/__snapshots__/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/tests/serialization/__snapshots__/test_csv.ambr
--rw-r--r--   0 runner    (1001) docker     (123)    22101 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/tests/serialization/__snapshots__/test_xlsx.ambr
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/tests/serialization/test_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/tests/serialization/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/tests/serialization/test_xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)    16267 2023-07-13 08:32:26.000000 mtg_ssm-2.6.2.dev5/tests/test_ssm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.403107 mtg_ssm-2.6.2.dev6/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.391107 mtg_ssm-2.6.2.dev6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.391107 mtg_ssm-2.6.2.dev6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/.github/workflows/integration.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-07-13 09:05:24.403107 mtg_ssm-2.6.2.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/TODO.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.395107 mtg_ssm-2.6.2.dev6/mtg_ssm/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-13 09:05:24.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.395107 mtg_ssm-2.6.2.dev6/mtg_ssm/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/containers/bundles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/containers/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/containers/counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/containers/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/containers/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.395107 mtg_ssm-2.6.2.dev6/mtg_ssm/mtg/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/mtg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/mtg/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.395107 mtg_ssm-2.6.2.dev6/mtg_ssm/scryfall/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/scryfall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/scryfall/fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11606 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/scryfall/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.399107 mtg_ssm-2.6.2.dev6/mtg_ssm/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/serialization/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/serialization/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/serialization/xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10331 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/mtg_ssm/ssm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.395107 mtg_ssm-2.6.2.dev6/mtg_ssm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-07-13 09:05:24.000000 mtg_ssm-2.6.2.dev6/mtg_ssm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-13 09:05:24.000000 mtg_ssm-2.6.2.dev6/mtg_ssm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:05:24.000000 mtg_ssm-2.6.2.dev6/mtg_ssm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 09:05:24.000000 mtg_ssm-2.6.2.dev6/mtg_ssm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-13 09:05:24.000000 mtg_ssm-2.6.2.dev6/mtg_ssm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 09:05:24.000000 mtg_ssm-2.6.2.dev6/mtg_ssm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 09:05:24.403107 mtg_ssm-2.6.2.dev6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.399107 mtg_ssm-2.6.2.dev6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.399107 mtg_ssm-2.6.2.dev6/tests/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/containers/test_bundles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/containers/test_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/containers/test_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/containers/test_legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.399107 mtg_ssm-2.6.2.dev6/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/data/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/data/bulk_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)   456765 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/data/cards.json
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/data/migrations.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31317 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/data/sets.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15912 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/data/sets1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15519 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/data/sets2.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6650 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/gen_testdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.399107 mtg_ssm-2.6.2.dev6/tests/mtg/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/mtg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/mtg/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.403107 mtg_ssm-2.6.2.dev6/tests/scryfall/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/scryfall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/scryfall/test_fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.403107 mtg_ssm-2.6.2.dev6/tests/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/serialization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:05:24.403107 mtg_ssm-2.6.2.dev6/tests/serialization/__snapshots__/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/serialization/__snapshots__/test_csv.ambr
+-rw-r--r--   0 runner    (1001) docker     (123)    22101 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/serialization/__snapshots__/test_xlsx.ambr
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/serialization/test_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/serialization/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/serialization/test_xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16267 2023-07-13 09:05:14.000000 mtg_ssm-2.6.2.dev6/tests/test_ssm.py
```

### Comparing `mtg_ssm-2.6.2.dev5/.github/workflows/integration.yml` & `mtg_ssm-2.6.2.dev6/.github/workflows/integration.yml`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/.github/workflows/publish.yml` & `mtg_ssm-2.6.2.dev6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/.github/workflows/run-tests.yml` & `mtg_ssm-2.6.2.dev6/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/.gitignore` & `mtg_ssm-2.6.2.dev6/.gitignore`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/.pre-commit-config.yaml` & `mtg_ssm-2.6.2.dev6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/LICENSE.txt` & `mtg_ssm-2.6.2.dev6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/PKG-INFO` & `mtg_ssm-2.6.2.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtg_ssm
-Version: 2.6.2.dev5
+Version: 2.6.2.dev6
 Summary: A tool to manage Magic: the Gathering collection spreadsheets
 Author-email: George Leslie-Waksman <waksman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/gwax/mtg_ssm
 Project-URL: Bug Tracker, https://github.com/gwax/mtg_ssm/issues
 Keywords: mtg,magic,collection,tracking,spreadsheet
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mtg_ssm-2.6.2.dev5/README.rst` & `mtg_ssm-2.6.2.dev6/README.rst`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/mtg_ssm/containers/bundles.py` & `mtg_ssm-2.6.2.dev6/mtg_ssm/containers/bundles.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/mtg_ssm/containers/collection.py` & `mtg_ssm-2.6.2.dev6/mtg_ssm/containers/collection.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/mtg_ssm/containers/counts.py` & `mtg_ssm-2.6.2.dev6/mtg_ssm/containers/counts.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/mtg_ssm/containers/indexes.py` & `mtg_ssm-2.6.2.dev6/mtg_ssm/containers/indexes.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/mtg_ssm/containers/legacy.py` & `mtg_ssm-2.6.2.dev6/mtg_ssm/containers/legacy.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/mtg_ssm/mtg/util.py` & `mtg_ssm-2.6.2.dev6/mtg_ssm/mtg/util.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/mtg_ssm/scryfall/fetcher.py` & `mtg_ssm-2.6.2.dev6/mtg_ssm/scryfall/fetcher.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Scryfall data fetcher."""
 
 import gzip
 import os
-from typing import List, cast
+from typing import List
 
 import appdirs
 import msgspec
 from requests_cache import CachedSession, SerializerPipeline, Stage, pickle_serializer
 
 from mtg_ssm.containers.bundles import ScryfallDataSet
 from mtg_ssm.scryfall.models import (
@@ -50,32 +50,35 @@
     print(f'Fetched {endpoint}{" [CACHED]" if cached_response else ""}')
     return response.content
 
 
 def scryfetch() -> ScryfallDataSet:  # pylint: disable=too-many-locals
     """Retrieve and deserialize Scryfall object data."""
     print("Reading data from scryfall")
-    scrylist_decoder = msgspec.json.Decoder(ScryList)
-
-    bulk_data_list = scrylist_decoder.decode(_fetch_endpoint(BULK_DATA_ENDPOINT))
-    bulk_data = cast(List[ScryBulkData], bulk_data_list.data)
-
-    sets_list = scrylist_decoder.decode(_fetch_endpoint(SETS_ENDPOINT))
-    sets_data = cast(List[ScrySet], sets_list.data)
+    bulk_data = msgspec.json.decode(
+        _fetch_endpoint(BULK_DATA_ENDPOINT), type=ScryList[ScryBulkData]
+    ).data
+
+    scrylistset_decoder = msgspec.json.Decoder(ScryList[ScrySet])
+    sets_list = scrylistset_decoder.decode(_fetch_endpoint(SETS_ENDPOINT))
+    sets_data = sets_list.data
     while sets_list.has_more and sets_list.next_page is not None:
-        sets_list = scrylist_decoder.decode(_fetch_endpoint(sets_list.next_page))
-        sets_data += cast(List[ScrySet], sets_list.data)
+        sets_list = scrylistset_decoder.decode(_fetch_endpoint(sets_list.next_page))
+        sets_data += sets_list.data
 
-    migrations_list = scrylist_decoder.decode(_fetch_endpoint(MIGRATIONS_ENDPOINT))
-    migrations_data = cast(List[ScryMigration], migrations_list.data)
+    scrylistmigration_decoder = msgspec.json.Decoder(ScryList[ScryMigration])
+    migrations_list = scrylistmigration_decoder.decode(
+        _fetch_endpoint(MIGRATIONS_ENDPOINT)
+    )
+    migrations_data = migrations_list.data
     while migrations_list.has_more and migrations_list.next_page is not None:
-        migrations_list = scrylist_decoder.decode(
+        migrations_list = scrylistmigration_decoder.decode(
             _fetch_endpoint(migrations_list.next_page)
         )
-        migrations_data += cast(List[ScryMigration], migrations_list.data)
+        migrations_data += migrations_list.data
 
     [cards_endpoint] = [bd.download_uri for bd in bulk_data if bd.type == BULK_TYPE]
     cards_data = msgspec.json.decode(
         _fetch_endpoint(cards_endpoint), type=List[ScryCard]
     )
 
     scryfall_data = ScryfallDataSet(
```

### Comparing `mtg_ssm-2.6.2.dev5/mtg_ssm/scryfall/models.py` & `mtg_ssm-2.6.2.dev6/mtg_ssm/scryfall/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Scryfall object models."""
 
 import datetime as dt
 from decimal import Decimal
 from enum import Enum
-from typing import Dict, List, Literal, Optional, Union
+from typing import Dict, Generic, List, Literal, Optional, TypeVar, Union
 from uuid import UUID
 
 from msgspec import Struct
+from typing_extensions import TypeAlias
 
 
 class ScryColor(str, Enum):
     """Enum for https://scryfall.com/docs/api/colors#color-arrays"""
 
     WHITE = "W"
     BLUE = "U"
@@ -447,21 +448,32 @@
     performed_at: dt.date
     migration_strategy: ScryMigrationStrategy
     old_scryfall_id: UUID
     new_scryfall_id: Optional[UUID] = None
     note: Optional[str] = None
 
 
+ScryListable: TypeAlias = Union[
+    ScryBulkData,
+    ScryCard,
+    ScryMigration,
+    ScrySet,
+]
+
+_ScryListableT = TypeVar("_ScryListableT", bound=ScryListable)
+
+
 class ScryList(
     Struct,
+    Generic[_ScryListableT],
     tag_field="object",
     tag="list",
     kw_only=True,
     omit_defaults=True,
 ):
     """Model for https://scryfall.com/docs/api/lists"""
 
-    data: List[Union[ScrySet, ScryCard, ScryBulkData, ScryMigration]]
+    data: List[_ScryListableT]
     has_more: bool
     next_page: Optional[str] = None
     total_cards: Optional[int] = None
     warnings: Optional[List[str]] = None
```

### Comparing `mtg_ssm-2.6.2.dev5/mtg_ssm/serialization/csv.py` & `mtg_ssm-2.6.2.dev6/mtg_ssm/serialization/csv.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/mtg_ssm/serialization/interface.py` & `mtg_ssm-2.6.2.dev6/mtg_ssm/serialization/interface.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/mtg_ssm/serialization/xlsx.py` & `mtg_ssm-2.6.2.dev6/mtg_ssm/serialization/xlsx.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/mtg_ssm/ssm.py` & `mtg_ssm-2.6.2.dev6/mtg_ssm/ssm.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/mtg_ssm.egg-info/PKG-INFO` & `mtg_ssm-2.6.2.dev6/mtg_ssm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtg-ssm
-Version: 2.6.2.dev5
+Version: 2.6.2.dev6
 Summary: A tool to manage Magic: the Gathering collection spreadsheets
 Author-email: George Leslie-Waksman <waksman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/gwax/mtg_ssm
 Project-URL: Bug Tracker, https://github.com/gwax/mtg_ssm/issues
 Keywords: mtg,magic,collection,tracking,spreadsheet
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mtg_ssm-2.6.2.dev5/mtg_ssm.egg-info/SOURCES.txt` & `mtg_ssm-2.6.2.dev6/mtg_ssm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/pylintrc` & `mtg_ssm-2.6.2.dev6/pylintrc`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/pyproject.toml` & `mtg_ssm-2.6.2.dev6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Games/Entertainment",
 ]
 
 dependencies = [
     "appdirs~=1.4",
-    "msgspec~=0.13",
+    "msgspec~=0.15",
     "openpyxl~=3.0",
     "requests~=2.27",
     'requests-cache~=0.9.8',
 ]
 dynamic = ["version"]
 
 [project.urls]
```

### Comparing `mtg_ssm-2.6.2.dev5/tests/conftest.py` & `mtg_ssm-2.6.2.dev6/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """pytest test configuration file."""
 # pylint: disable=redefined-outer-name
 
 from pathlib import Path
-from typing import Dict, Generator, List, cast
+from typing import Dict, Generator, List
 from uuid import UUID
 
 import msgspec
 import pytest
 import responses
 
 from mtg_ssm.containers.bundles import ScryfallDataSet
@@ -40,26 +40,26 @@
         return msgspec.json.decode(card_data_file.read(), type=List[ScryCard])
 
 
 @pytest.fixture(scope="session")
 def sets_data() -> List[ScrySet]:
     """Fixture containing all test set data."""
     with SETS_DATA_FILE.open("rb") as sets_data_file:
-        sets_list = msgspec.json.decode(sets_data_file.read(), type=ScryList)
-    return cast(List[ScrySet], sets_list.data)
+        sets_list = msgspec.json.decode(sets_data_file.read(), type=ScryList[ScrySet])
+    return sets_list.data
 
 
 @pytest.fixture(scope="session")
 def migrations_data() -> List[ScryMigration]:
     """Fixture containing all test migrations data."""
     with MIGRATIONS_DATA_FILE.open("rb") as migrations_data_file:
         migrations_list = msgspec.json.decode(
-            migrations_data_file.read(), type=ScryList
+            migrations_data_file.read(), type=ScryList[ScryMigration]
         )
-    return cast(List[ScryMigration], migrations_list.data)
+    return migrations_list.data
 
 
 @pytest.fixture(scope="session")
 def id_to_card(cards_data: List[ScryCard]) -> Dict[UUID, ScryCard]:
     """Fixture returning scryfall id to card object for all test card data."""
     return {card.id: card for card in cards_data}
```

### Comparing `mtg_ssm-2.6.2.dev5/tests/containers/test_bundles.py` & `mtg_ssm-2.6.2.dev6/tests/containers/test_bundles.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/tests/containers/test_counts.py` & `mtg_ssm-2.6.2.dev6/tests/containers/test_counts.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/tests/containers/test_indexes.py` & `mtg_ssm-2.6.2.dev6/tests/containers/test_indexes.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/tests/containers/test_legacy.py` & `mtg_ssm-2.6.2.dev6/tests/containers/test_legacy.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/tests/data/bulk_data.json` & `mtg_ssm-2.6.2.dev6/tests/data/bulk_data.json`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/tests/data/cards.json` & `mtg_ssm-2.6.2.dev6/tests/data/cards.json`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/tests/data/migrations.json` & `mtg_ssm-2.6.2.dev6/tests/data/migrations.json`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/tests/data/sets.json` & `mtg_ssm-2.6.2.dev6/tests/data/sets.json`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/tests/data/sets1.json` & `mtg_ssm-2.6.2.dev6/tests/data/sets1.json`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/tests/data/sets2.json` & `mtg_ssm-2.6.2.dev6/tests/data/sets2.json`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/tests/gen_testdata.py` & `mtg_ssm-2.6.2.dev6/tests/gen_testdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python3
 """Script to build mtgjson testdata."""
 # pylint: disable=protected-access
 
 import copy
 from pathlib import Path
-from typing import List, cast
 
 import msgspec
 
 from mtg_ssm.scryfall import fetcher, models
 
 
 class Error(Exception):
@@ -81,17 +80,18 @@
 
 
 def main() -> None:  # pylint: disable=too-many-locals,too-many-statements
     """Read scryfall data and write a subset for use as test data."""
     print("Fetching scryfall data")
     scrydata = fetcher.scryfetch()
     bulk_data_list = msgspec.json.decode(
-        fetcher._fetch_endpoint(fetcher.BULK_DATA_ENDPOINT), type=models.ScryList
+        fetcher._fetch_endpoint(fetcher.BULK_DATA_ENDPOINT),
+        type=models.ScryList[models.ScryBulkData],
     )
-    bulk_data = cast(List[models.ScryBulkData], bulk_data_list.data)
+    bulk_data = bulk_data_list.data
 
     print("Selecting sets")
     accepted_sets = sorted(
         (s for s in scrydata.sets if s.code in TEST_SETS_TO_CARDS),
         key=lambda sset: sset.code,
     )
     missing_sets = set(TEST_SETS_TO_CARDS.keys()) - {s.code for s in accepted_sets}
```

### Comparing `mtg_ssm-2.6.2.dev5/tests/mtg/test_util.py` & `mtg_ssm-2.6.2.dev6/tests/mtg/test_util.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/tests/scryfall/test_fetcher.py` & `mtg_ssm-2.6.2.dev6/tests/scryfall/test_fetcher.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/tests/serialization/__snapshots__/test_csv.ambr` & `mtg_ssm-2.6.2.dev6/tests/serialization/__snapshots__/test_csv.ambr`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/tests/serialization/__snapshots__/test_xlsx.ambr` & `mtg_ssm-2.6.2.dev6/tests/serialization/__snapshots__/test_xlsx.ambr`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/tests/serialization/test_csv.py` & `mtg_ssm-2.6.2.dev6/tests/serialization/test_csv.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/tests/serialization/test_interface.py` & `mtg_ssm-2.6.2.dev6/tests/serialization/test_interface.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/tests/serialization/test_xlsx.py` & `mtg_ssm-2.6.2.dev6/tests/serialization/test_xlsx.py`

 * *Files identical despite different names*

### Comparing `mtg_ssm-2.6.2.dev5/tests/test_ssm.py` & `mtg_ssm-2.6.2.dev6/tests/test_ssm.py`

 * *Files identical despite different names*

