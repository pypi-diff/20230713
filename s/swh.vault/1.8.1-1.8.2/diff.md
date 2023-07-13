# Comparing `tmp/swh.vault-1.8.1.tar.gz` & `tmp/swh.vault-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.vault-1.8.1.tar", last modified: Mon Nov  7 14:29:37 2022, max compression
+gzip compressed data, was "swh.vault-1.8.2.tar", last modified: Thu Jul 13 14:22:05 2023, max compression
```

## Comparing `swh.vault-1.8.1.tar` & `swh.vault-1.8.2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-07 14:29:37.000000 swh.vault-1.8.1/
--rw-r--r--   0 jenkins    (115) docker     (999)      140 2022-11-07 14:29:36.000000 swh.vault-1.8.1/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      113 2022-11-07 14:29:36.000000 swh.vault-1.8.1/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      848 2022-11-07 14:29:36.000000 swh.vault-1.8.1/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2022-11-07 14:29:36.000000 swh.vault-1.8.1/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2022-11-07 14:29:36.000000 swh.vault-1.8.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)       15 2022-11-07 14:29:36.000000 swh.vault-1.8.1/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2022-11-07 14:29:36.000000 swh.vault-1.8.1/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      248 2022-11-07 14:29:36.000000 swh.vault-1.8.1/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2022-11-07 14:29:36.000000 swh.vault-1.8.1/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     1338 2022-11-07 14:29:37.000000 swh.vault-1.8.1/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)      412 2022-11-07 14:29:36.000000 swh.vault-1.8.1/README.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      332 2022-11-07 14:29:36.000000 swh.vault-1.8.1/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-07 14:29:37.000000 swh.vault-1.8.1/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2022-11-07 14:29:36.000000 swh.vault-1.8.1/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2022-11-07 14:29:36.000000 swh.vault-1.8.1/docs/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)      412 2022-11-07 14:29:36.000000 swh.vault-1.8.1/docs/README.rst
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-07 14:29:37.000000 swh.vault-1.8.1/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-11-07 14:29:36.000000 swh.vault-1.8.1/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-07 14:29:37.000000 swh.vault-1.8.1/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-11-07 14:29:36.000000 swh.vault-1.8.1/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)     5190 2022-11-07 14:29:36.000000 swh.vault-1.8.1/docs/api.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      133 2022-11-07 14:29:36.000000 swh.vault-1.8.1/docs/cli.rst
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2022-11-07 14:29:36.000000 swh.vault-1.8.1/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1791 2022-11-07 14:29:36.000000 swh.vault-1.8.1/docs/getting-started.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     1486 2022-11-07 14:29:36.000000 swh.vault-1.8.1/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      458 2022-11-07 14:29:36.000000 swh.vault-1.8.1/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2022-11-07 14:29:36.000000 swh.vault-1.8.1/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)      122 2022-11-07 14:29:36.000000 swh.vault-1.8.1/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)       15 2022-11-07 14:29:36.000000 swh.vault-1.8.1/requirements-swh-graph.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       98 2022-11-07 14:29:36.000000 swh.vault-1.8.1/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      164 2022-11-07 14:29:36.000000 swh.vault-1.8.1/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       77 2022-11-07 14:29:36.000000 swh.vault-1.8.1/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2022-11-07 14:29:37.000000 swh.vault-1.8.1/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2369 2022-11-07 14:29:36.000000 swh.vault-1.8.1/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-07 14:29:37.000000 swh.vault-1.8.1/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-07 14:29:37.000000 swh.vault-1.8.1/swh/vault/
--rw-r--r--   0 jenkins    (115) docker     (999)     1672 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-07 14:29:37.000000 swh.vault-1.8.1/swh/vault/api/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/api/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      655 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/api/client.py
--rw-r--r--   0 jenkins    (115) docker     (999)      499 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/api/serializers.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3346 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/api/server.py
--rw-r--r--   0 jenkins    (115) docker     (999)    18015 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/backend.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1562 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/cache.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5317 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/cli.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-07 14:29:37.000000 swh.vault-1.8.1/swh/vault/cookers/
--rw-r--r--   0 jenkins    (115) docker     (999)     4144 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/cookers/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5429 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/cookers/base.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1046 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/cookers/directory.py
--rw-r--r--   0 jenkins    (115) docker     (999)    29817 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/cookers/git_bare.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1435 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/cookers/revision_flat.py
--rw-r--r--   0 jenkins    (115) docker     (999)     9075 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/cookers/revision_gitfast.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1869 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/cookers/utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)      821 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/cooking_tasks.py
--rw-r--r--   0 jenkins    (115) docker     (999)      287 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/exc.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1653 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/in_memory_backend.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2287 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/interface.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/py.typed
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-07 14:29:37.000000 swh.vault-1.8.1/swh/vault/sql/
--rw-r--r--   0 jenkins    (115) docker     (999)     1728 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/sql/30-schema.sql
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-07 14:29:37.000000 swh.vault-1.8.1/swh/vault/sql/upgrades/
--rw-r--r--   0 jenkins    (115) docker     (999)      975 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/sql/upgrades/002.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      879 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/sql/upgrades/003.sql
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-07 14:29:37.000000 swh.vault-1.8.1/swh/vault/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)      100 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1993 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/tests/conftest.py
--rw-r--r--   0 jenkins    (115) docker     (999)    14421 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/tests/test_backend.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2585 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/tests/test_cache.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5143 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) docker     (999)    45106 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/tests/test_cookers.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2929 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/tests/test_cookers_base.py
--rw-r--r--   0 jenkins    (115) docker     (999)    20267 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/tests/test_git_bare_cooker.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1848 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/tests/test_init.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3560 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/tests/test_init_cookers.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6196 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/tests/test_server.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5132 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/tests/test_to_disk.py
--rw-r--r--   0 jenkins    (115) docker     (999)      586 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/tests/vault_testing.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5470 2022-11-07 14:29:36.000000 swh.vault-1.8.1/swh/vault/to_disk.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-11-07 14:29:37.000000 swh.vault-1.8.1/swh.vault.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     1338 2022-11-07 14:29:37.000000 swh.vault-1.8.1/swh.vault.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     1770 2022-11-07 14:29:37.000000 swh.vault-1.8.1/swh.vault.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2022-11-07 14:29:37.000000 swh.vault-1.8.1/swh.vault.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       44 2022-11-07 14:29:37.000000 swh.vault-1.8.1/swh.vault.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2022-11-07 14:29:37.000000 swh.vault-1.8.1/swh.vault.egg-info/not-zip-safe
--rw-r--r--   0 jenkins    (115) docker     (999)      358 2022-11-07 14:29:37.000000 swh.vault-1.8.1/swh.vault.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2022-11-07 14:29:37.000000 swh.vault-1.8.1/swh.vault.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1486 2022-11-07 14:29:36.000000 swh.vault-1.8.1/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-13 14:22:05.796317 swh.vault-1.8.2/
+-rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-07-13 14:22:00.000000 swh.vault-1.8.2/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      113 2023-07-13 14:22:00.000000 swh.vault-1.8.2/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-07-13 14:22:00.000000 swh.vault-1.8.2/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-07-13 14:22:00.000000 swh.vault-1.8.2/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-07-13 14:22:00.000000 swh.vault-1.8.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)       15 2023-07-13 14:22:00.000000 swh.vault-1.8.2/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-07-13 14:22:00.000000 swh.vault-1.8.2/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      248 2023-07-13 14:22:00.000000 swh.vault-1.8.2/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-07-13 14:22:00.000000 swh.vault-1.8.2/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     1338 2023-07-13 14:22:05.796317 swh.vault-1.8.2/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)      412 2023-07-13 14:22:00.000000 swh.vault-1.8.2/README.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      332 2023-07-13 14:22:00.000000 swh.vault-1.8.2/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-13 14:22:05.792317 swh.vault-1.8.2/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-07-13 14:22:00.000000 swh.vault-1.8.2/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-07-13 14:22:00.000000 swh.vault-1.8.2/docs/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)      412 2023-07-13 14:22:00.000000 swh.vault-1.8.2/docs/README.rst
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-13 14:22:05.792317 swh.vault-1.8.2/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-13 14:22:00.000000 swh.vault-1.8.2/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-13 14:22:05.792317 swh.vault-1.8.2/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-13 14:22:00.000000 swh.vault-1.8.2/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)     5190 2023-07-13 14:22:00.000000 swh.vault-1.8.2/docs/api.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      133 2023-07-13 14:22:00.000000 swh.vault-1.8.2/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-07-13 14:22:00.000000 swh.vault-1.8.2/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1791 2023-07-13 14:22:00.000000 swh.vault-1.8.2/docs/getting-started.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     1606 2023-07-13 14:22:00.000000 swh.vault-1.8.2/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      458 2023-07-13 14:22:00.000000 swh.vault-1.8.2/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-07-13 14:22:00.000000 swh.vault-1.8.2/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)      122 2023-07-13 14:22:00.000000 swh.vault-1.8.2/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)       15 2023-07-13 14:22:00.000000 swh.vault-1.8.2/requirements-swh-graph.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       98 2023-07-13 14:22:00.000000 swh.vault-1.8.2/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      182 2023-07-13 14:22:00.000000 swh.vault-1.8.2/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       77 2023-07-13 14:22:00.000000 swh.vault-1.8.2/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-07-13 14:22:05.800317 swh.vault-1.8.2/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2369 2023-07-13 14:22:00.000000 swh.vault-1.8.2/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-13 14:22:05.792317 swh.vault-1.8.2/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-13 14:22:05.796317 swh.vault-1.8.2/swh/vault/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1709 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-13 14:22:05.796317 swh.vault-1.8.2/swh/vault/api/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/api/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      655 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/api/client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      499 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/api/serializers.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3312 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/api/server.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    18537 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/backend.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1562 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/cache.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5322 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/cli.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-13 14:22:05.796317 swh.vault-1.8.2/swh/vault/cookers/
+-rw-r--r--   0 jenkins    (115) docker     (999)     4154 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/cookers/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5429 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/cookers/base.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1046 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/cookers/directory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    30066 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/cookers/git_bare.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1435 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/cookers/revision_flat.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9075 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/cookers/revision_gitfast.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1869 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/cookers/utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      821 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/cooking_tasks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      287 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/exc.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1658 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/in_memory_backend.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2287 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/interface.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/py.typed
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-13 14:22:05.796317 swh.vault-1.8.2/swh/vault/sql/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1728 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/sql/30-schema.sql
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-13 14:22:05.796317 swh.vault-1.8.2/swh/vault/sql/upgrades/
+-rw-r--r--   0 jenkins    (115) docker     (999)      975 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/sql/upgrades/002.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      879 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/sql/upgrades/003.sql
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-13 14:22:05.796317 swh.vault-1.8.2/swh/vault/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)      100 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1988 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/tests/conftest.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    14447 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/tests/test_backend.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2585 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/tests/test_cache.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5143 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    44997 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/tests/test_cookers.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2929 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/tests/test_cookers_base.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    20291 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/tests/test_git_bare_cooker.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1848 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/tests/test_init.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3403 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/tests/test_init_cookers.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6196 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/tests/test_server.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5132 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/tests/test_to_disk.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      586 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/tests/vault_testing.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5586 2023-07-13 14:22:00.000000 swh.vault-1.8.2/swh/vault/to_disk.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-13 14:22:05.792317 swh.vault-1.8.2/swh.vault.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1338 2023-07-13 14:22:05.000000 swh.vault-1.8.2/swh.vault.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     1770 2023-07-13 14:22:05.000000 swh.vault-1.8.2/swh.vault.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-07-13 14:22:05.000000 swh.vault-1.8.2/swh.vault.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       44 2023-07-13 14:22:05.000000 swh.vault-1.8.2/swh.vault.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-07-13 14:22:05.000000 swh.vault-1.8.2/swh.vault.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins    (115) docker     (999)      376 2023-07-13 14:22:05.000000 swh.vault-1.8.2/swh.vault.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-07-13 14:22:05.000000 swh.vault-1.8.2/swh.vault.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1507 2023-07-13 14:22:00.000000 swh.vault-1.8.2/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `swh.vault-1.8.1/.pre-commit-config.yaml` & `swh.vault-1.8.2/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         entry: mypy
         args: [swh]
         pass_filenames: false
         language: system
         types: [python]
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.11.5
     hooks:
       - id: isort
 
   - repo: https://github.com/python/black
     rev: 22.10.0
     hooks:
       - id: black
```

### Comparing `swh.vault-1.8.1/CODE_OF_CONDUCT.md` & `swh.vault-1.8.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.vault-1.8.1/LICENSE` & `swh.vault-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.vault-1.8.1/PKG-INFO` & `swh.vault-1.8.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.vault
-Version: 1.8.1
+Version: 1.8.2
 Summary: Software Heritage vault
 Home-page: https://forge.softwareheritage.org/diffusion/DVAU/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-vault
```

### Comparing `swh.vault-1.8.1/docs/api.rst` & `swh.vault-1.8.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `swh.vault-1.8.1/docs/getting-started.rst` & `swh.vault-1.8.2/docs/getting-started.rst`

 * *Files identical despite different names*

### Comparing `swh.vault-1.8.1/docs/index.rst` & `swh.vault-1.8.2/docs/index.rst`

 * *Files 9% similar despite different names*

```diff
@@ -42,8 +42,16 @@
 Reference Documentation
 -----------------------
 
 .. toctree::
    :maxdepth: 2
 
    cli
-   /apidoc/swh.vault
+
+.. only:: standalone_package_doc
+
+   Indices and tables
+   ------------------
+
+   * :ref:`genindex`
+   * :ref:`modindex`
+   * :ref:`search`
```

### Comparing `swh.vault-1.8.1/setup.py` & `swh.vault-1.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.8.1/swh/vault/__init__.py` & `swh.vault-1.8.2/swh/vault/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from __future__ import annotations
 
 import importlib
 import logging
 from typing import Dict
 import warnings
 
+from swh.vault.backend import VaultDB
+
 logger = logging.getLogger(__name__)
 
 
 BACKEND_TYPES: Dict[str, str] = {
     "remote": ".api.client.RemoteVaultClient",
     "postgresql": ".backend.VaultBackend",
     "memory": ".in_memory_backend.InMemoryVaultBackend",
@@ -53,8 +55,8 @@
 
     (module_path, class_name) = class_path.rsplit(".", 1)
     module = importlib.import_module(module_path, package=__package__)
     Vault = getattr(module, class_name)
     return Vault(**kwargs)
 
 
-get_datastore = get_vault
+get_datastore = VaultDB
```

### Comparing `swh.vault-1.8.1/swh/vault/api/client.py` & `swh.vault-1.8.2/swh/vault/api/client.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.8.1/swh/vault/api/server.py` & `swh.vault-1.8.2/swh/vault/api/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# Copyright (C) 2016-2022  The Software Heritage developers
+# Copyright (C) 2016-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from __future__ import annotations
 
 import os
 from typing import Any, Dict, Optional
 
 from swh.core.api import RPCServerApp
 from swh.core.api import encode_data_server as encode_data
 from swh.core.api import error_handler
-from swh.core.config import config_basepath, merge_configs, read_raw_config
+from swh.core.config import merge_configs, read_raw_config
 from swh.vault import get_vault as get_swhvault
 from swh.vault.backend import NotFoundExc
 from swh.vault.interface import VaultInterface
 
 from .serializers import DECODERS, ENCODERS
 
 # do not define default services here
@@ -106,15 +106,15 @@
     """
     config_path = os.environ.get("SWH_CONFIG_FILENAME", config_path)
     if not config_path:
         raise ValueError("Missing configuration path.")
     if not os.path.isfile(config_path):
         raise ValueError(f"Configuration path {config_path} should exist.")
 
-    app_config = read_raw_config(config_basepath(config_path))
+    app_config = read_raw_config(config_path)
     app_config["vault"] = check_config(app_config)
     app.config.update(merge_configs(DEFAULT_CONFIG, app_config))
 
     return app
 
 
 if __name__ == "__main__":
```

### Comparing `swh.vault-1.8.1/swh/vault/backend.py` & `swh.vault-1.8.2/swh/vault/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,26 +62,23 @@
 We apologize for the inconvenience.
 
 --\x20
 The Software Heritage Developers
 """
 
 
-class VaultBackend:
+class VaultDB:
     """
-    Backend for the Software Heritage Vault.
+    PostgreSQL backend for the Software Heritage Vault.
     """
 
     current_version = 4
 
     def __init__(self, **config):
         self.config = config
-        self.cache = VaultCache(**config["cache"])
-        self.scheduler = get_scheduler(**config["scheduler"])
-        self.storage = get_storage(**config["storage"])
 
         if "db" not in self.config:
             raise ValueError(
                 "The 'db' configuration entry is missing "
                 "in the vault configuration file"
             )
         db_conn = config["db"]
@@ -98,14 +95,26 @@
             return self._db
         return BaseDb.from_pool(self._pool)
 
     def put_db(self, db):
         if db is not self._db:
             db.put_conn()
 
+
+class VaultBackend(VaultDB):
+    """
+    Backend for the Software Heritage Vault.
+    """
+
+    def __init__(self, **config):
+        super().__init__(**config)
+        self.cache = VaultCache(**config["cache"])
+        self.scheduler = get_scheduler(**config["scheduler"])
+        self.storage = get_storage(**config["storage"])
+
     @db_transaction()
     def progress(
         self,
         bundle_type: str,
         swhid: CoreSWHID,
         raise_notfound: bool = True,
         db=None,
@@ -488,34 +497,40 @@
                 (n_id,),
             )
 
     def _smtp_send(self, msg: MIMEText):
         smtp_server = smtplib.SMTP(**self.config.get("smtp", {}))
         try:
             status = smtp_server.noop()[0]
-        except smtplib.SMTPException:
-            status = -1
-        if status != 250:
+        except smtplib.SMTPException as e:
             error_message = (
                 f"Unable to send SMTP message '{msg['Subject']}' to "
-                f"{msg['To']}: cannot connect to server"
+                f"{msg['To']}: cannot connect to server ({e})"
             )
             logger.error(error_message)
             sentry_sdk.capture_message(error_message, "error")
         else:
-            try:
-                # Send the message
-                smtp_server.send_message(msg)
-            except smtplib.SMTPException as exc:
-                logger.exception(exc)
+            if status != 250:
                 error_message = (
                     f"Unable to send SMTP message '{msg['Subject']}' to "
-                    f"{msg['To']}: {exc}"
+                    f"{msg['To']}: server returned status {status}"
                 )
+                logger.error(error_message)
                 sentry_sdk.capture_message(error_message, "error")
+            else:
+                try:
+                    # Send the message
+                    smtp_server.send_message(msg)
+                except smtplib.SMTPException as exc:
+                    logger.exception(exc)
+                    error_message = (
+                        f"Unable to send SMTP message '{msg['Subject']}' to "
+                        f"{msg['To']}: {exc}"
+                    )
+                    sentry_sdk.capture_message(error_message, "error")
 
     @db_transaction()
     def _cache_expire(self, cond, *args, db=None, cur=None) -> None:
         """Low-level expiration method, used by cache_expire_* methods"""
         # Embedded SELECT query to be able to use ORDER BY and LIMIT
         cur.execute(
             """
```

### Comparing `swh.vault-1.8.1/swh/vault/cache.py` & `swh.vault-1.8.2/swh/vault/cache.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.8.1/swh/vault/cli.py` & `swh.vault-1.8.2/swh/vault/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
     from .cookers import get_cooker_cls
     from .in_memory_backend import InMemoryVaultBackend
 
     conf = config.read(config_file)
 
     try:
-        from swh.graph.client import RemoteGraphClient  # optional dependency
+        from swh.graph.http_client import RemoteGraphClient  # optional dependency
 
         graph = RemoteGraphClient(**conf["graph"]) if conf.get("graph") else None
     except ModuleNotFoundError:
         if conf.get("graph"):
             raise EnvironmentError(
                 "Graph configuration required but module is not installed."
             )
```

### Comparing `swh.vault-1.8.1/swh/vault/cookers/__init__.py` & `swh.vault-1.8.2/swh/vault/cookers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import os
 from typing import Any, Dict, List, Type
 
 from swh.core.config import load_named_config
 from swh.core.config import read as read_config
 from swh.model.swhids import CoreSWHID, ObjectType
 from swh.storage import get_storage
-from swh.vault import get_vault
 from swh.vault.cookers.base import DEFAULT_CONFIG, DEFAULT_CONFIG_PATH, BaseVaultCooker
 from swh.vault.cookers.directory import DirectoryCooker
 from swh.vault.cookers.git_bare import GitBareCooker
 from swh.vault.cookers.revision_flat import RevisionFlatCooker
 from swh.vault.cookers.revision_gitfast import RevisionGitfastCooker
 
 _COOKER_CLS: List[Type[BaseVaultCooker]] = [
@@ -94,28 +93,30 @@
 
     Raises:
         ValueError in case of a missing top-level vault key configuration or a storage
           key.
         EnvironmentError in case the vault configuration reference a non remote class.
 
     """
+    from swh.vault import get_vault
+
     if "SWH_CONFIG_FILENAME" in os.environ:
         cfg = read_config(os.environ["SWH_CONFIG_FILENAME"], DEFAULT_CONFIG)
     else:
         cfg = load_named_config(DEFAULT_CONFIG_PATH, DEFAULT_CONFIG)
     cooker_cls = get_cooker_cls(bundle_type, swhid.object_type)
 
     cfg = check_config(cfg)
     vcfg = cfg["vault"]
 
     storage = get_storage(**vcfg.pop("storage"))
     backend = get_vault(**vcfg)
 
     try:
-        from swh.graph.client import RemoteGraphClient  # optional dependency
+        from swh.graph.http_client import RemoteGraphClient  # optional dependency
 
         graph = RemoteGraphClient(**vcfg["graph"]) if vcfg.get("graph") else None
     except ModuleNotFoundError:
         if vcfg.get("graph"):
             raise EnvironmentError(
                 "Graph configuration required but module is not installed."
             )
```

### Comparing `swh.vault-1.8.1/swh/vault/cookers/base.py` & `swh.vault-1.8.2/swh/vault/cookers/base.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.8.1/swh/vault/cookers/directory.py` & `swh.vault-1.8.2/swh/vault/cookers/directory.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.8.1/swh/vault/cookers/git_bare.py` & `swh.vault-1.8.2/swh/vault/cookers/git_bare.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,26 @@
 import logging
 import multiprocessing.dummy
 import os.path
 import re
 import subprocess
 import tarfile
 import tempfile
-from typing import Any, Dict, Iterable, Iterator, List, NoReturn, Optional, Set, Tuple
+from typing import (
+    Any,
+    Dict,
+    Iterable,
+    Iterator,
+    List,
+    NoReturn,
+    Optional,
+    Set,
+    Tuple,
+    cast,
+)
 import zlib
 
 import sentry_sdk
 
 from swh.core.api.classes import stream_results_optional
 from swh.model import git_objects
 from swh.model.hashutil import hash_to_bytehex, hash_to_hex
@@ -59,14 +70,15 @@
     TimestampWithTimezone,
 )
 from swh.model.model import Content, Directory, DirectoryEntry
 from swh.model.model import ObjectType as ModelObjectType
 from swh.model.swhids import CoreSWHID, ObjectType
 from swh.storage.algos.revisions_walker import DFSRevisionsWalker
 from swh.storage.algos.snapshot import snapshot_get_all_branches
+from swh.storage.interface import HashDict
 from swh.vault.cookers.base import BaseVaultCooker
 from swh.vault.to_disk import HIDDEN_MESSAGE, SKIPPED_MESSAGE
 
 RELEASE_BATCH_SIZE = 10000
 REVISION_BATCH_SIZE = 10000
 DIRECTORY_BATCH_SIZE = 10000
 CONTENT_BATCH_SIZE = 100
@@ -127,29 +139,29 @@
 
     def _pop(self, stack: List[Sha1Git], n: int) -> List[Sha1Git]:
         """Removes ``n`` object from the ``stack`` and returns them."""
         obj_ids = stack[-n:]
         stack[-n:] = []
         return obj_ids
 
-    def prepare_bundle(self):
+    def prepare_bundle(self) -> None:
         """Main entry point. Initializes the state, creates the bundle, and
         sends it to the backend."""
         # Objects we will visit soon (aka. "todo-lists"):
         self._rel_stack: List[Sha1Git] = []
         self._rev_stack: List[Sha1Git] = []
         self._dir_stack: List[Sha1Git] = []
         self._cnt_stack: List[Sha1Git] = []
 
         # Set of objects already in any of the stacks:
         self._seen: Set[Sha1Git] = set()
         self._walker_state: Optional[Any] = None
 
         # Set of errors we expect git-fsck to raise at the end:
-        self._expected_fsck_errors = set()
+        self._expected_fsck_errors: Set[str] = set()
 
         with tempfile.TemporaryDirectory(prefix="swh-vault-gitbare-") as workdir:
             # Initialize a Git directory
             self.workdir = workdir
             self.gitdir = os.path.join(workdir, "clone.git")
             os.mkdir(self.gitdir)
             self.init_git()
@@ -260,28 +272,29 @@
             directory=self.obj_id,
             synthetic=True,
         )
         self.write_revision_node(revision)
 
         return revision.id
 
-    def write_refs(self, snapshot=None):
+    def write_refs(self, snapshot=None) -> None:
         """Writes all files in :file:`.git/refs/`.
 
         For non-snapshot objects, this is only ``master``."""
         refs: Dict[bytes, bytes]  # ref name -> target
-        if self.obj_type == RootObjectType.DIRECTORY:
+        if self.obj_type is RootObjectType.DIRECTORY:
             # We need a synthetic revision pointing to the directory
             rev_id = self._make_stub_directory_revision(self.obj_id)
 
             refs = {b"refs/heads/master": hash_to_bytehex(rev_id)}
-        elif self.obj_type == RootObjectType.REVISION:
+        elif self.obj_type is RootObjectType.REVISION:
             refs = {b"refs/heads/master": hash_to_bytehex(self.obj_id)}
-        elif self.obj_type == RootObjectType.RELEASE:
+        elif self.obj_type is RootObjectType.RELEASE:
             (release,) = self.storage.release_get([self.obj_id])
+            assert release, self.obj_id
 
             if release.name and re.match(rb"^[a-zA-Z0-9_.-]+$", release.name):
                 release_name = release.name
             else:
                 release_name = b"release"
 
             refs = {
@@ -289,15 +302,15 @@
             }
 
             if release.target_type.value == ModelObjectType.REVISION:
                 # Not necessary, but makes it easier to browse
                 refs[b"ref/heads/master"] = hash_to_bytehex(release.target)
             # TODO: synthesize a master branch for other target types
 
-        elif self.obj_type == RootObjectType.SNAPSHOT:
+        elif self.obj_type is RootObjectType.SNAPSHOT:
             if snapshot is None:
                 # refs were already written in a previous step
                 return
             branches = []
             for (branch_name, branch) in snapshot.branches.items():
                 if branch is None:
                     logging.error(
@@ -421,15 +434,15 @@
         them to ``self._rev_stack``.
 
         If swh-graph is not available, this requires fetching the revisions themselves,
         so they are directly loaded instead."""
         loaded_from_graph = False
 
         if self.graph:
-            from swh.graph.client import GraphArgumentException
+            from swh.graph.http_client import GraphArgumentException
 
             # First, try to cook using swh-graph, as it is more efficient than
             # swh-storage for querying the history
             obj_swhid = CoreSWHID(
                 object_type=ObjectType.REVISION,
                 object_id=obj_id,
             )
@@ -478,15 +491,15 @@
 
         if self.graph:
             revision_ids = []
             release_ids = []
             directory_ids = []
             content_ids = []
 
-            from swh.graph.client import GraphArgumentException
+            from swh.graph.http_client import GraphArgumentException
 
             # First, try to cook using swh-graph, as it is more efficient than
             # swh-storage for querying the history
             obj_swhid = CoreSWHID(
                 object_type=ObjectType.SNAPSHOT,
                 object_id=obj_id,
             )
@@ -685,15 +698,18 @@
                 # TODO: When content.status will have type Literal, replace this with
                 # assert_never
                 assert False, f"{content.swhid} has status: {content.status!r}"
 
         contents_and_data: Iterator[Tuple[Content, Optional[bytes]]]
         if self.objstorage is None:
             contents_and_data = (
-                (content, self.storage.content_get_data(content.sha1))
+                (
+                    content,
+                    self.storage.content_get_data(cast(HashDict, content.hashes())),
+                )
                 for content in visible_contents
             )
         else:
             contents_and_data = zip(
                 visible_contents,
                 self.objstorage.get_batch(c.hashes() for c in visible_contents),
             )
```

### Comparing `swh.vault-1.8.1/swh/vault/cookers/revision_flat.py` & `swh.vault-1.8.2/swh/vault/cookers/revision_flat.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.8.1/swh/vault/cookers/revision_gitfast.py` & `swh.vault-1.8.2/swh/vault/cookers/revision_gitfast.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.8.1/swh/vault/cookers/utils.py` & `swh.vault-1.8.2/swh/vault/cookers/utils.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.8.1/swh/vault/cooking_tasks.py` & `swh.vault-1.8.2/swh/vault/cooking_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.8.1/swh/vault/in_memory_backend.py` & `swh.vault-1.8.2/swh/vault/in_memory_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,8 +44,8 @@
 
     # Batch endpoints
 
     def batch_cook(self, batch: List[Tuple[str, str]]) -> int:
         raise NotImplementedError("InMemoryVaultBackend.batch_cook()")
 
     def batch_progress(self, batch_id: int) -> Dict[str, Any]:
-        pass
+        return {}
```

### Comparing `swh.vault-1.8.1/swh/vault/interface.py` & `swh.vault-1.8.2/swh/vault/interface.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.8.1/swh/vault/sql/30-schema.sql` & `swh.vault-1.8.2/swh/vault/sql/30-schema.sql`

 * *Files identical despite different names*

### Comparing `swh.vault-1.8.1/swh/vault/sql/upgrades/002.sql` & `swh.vault-1.8.2/swh/vault/sql/upgrades/002.sql`

 * *Files identical despite different names*

### Comparing `swh.vault-1.8.1/swh/vault/sql/upgrades/003.sql` & `swh.vault-1.8.2/swh/vault/sql/upgrades/003.sql`

 * *Files identical despite different names*

### Comparing `swh.vault-1.8.1/swh/vault/tests/conftest.py` & `swh.vault-1.8.2/swh/vault/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 from typing import Any, Dict
 
 import pkg_resources.extern.packaging.version
 import pytest
 from pytest_postgresql import factories
 
-from swh.core.db.pytest_plugin import initialize_database_for_module
+from swh.core.db.db_utils import initialize_database_for_module
 from swh.vault import get_vault
 from swh.vault.backend import VaultBackend
 
 os.environ["LC_ALL"] = "C.UTF-8"
 
 # needed for directory tests on git-cloned repositories
 # 022 is usually the default value, but some environments (eg. Debian builds) have
```

### Comparing `swh.vault-1.8.1/swh/vault/tests/test_backend.py` & `swh.vault-1.8.2/swh/vault/tests/test_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 
 from swh.core.sentry import init_sentry
 from swh.model.model import Content
 from swh.model.swhids import CoreSWHID
 from swh.vault.exc import NotFoundExc
 from swh.vault.tests.vault_testing import hash_content
 
+SENTRY_DSN = "https://user@example.org/1234"
+
 
 @contextlib.contextmanager
 def mock_cooking(vault_backend):
     with patch.object(vault_backend, "_send_task") as mt:
         mt.return_value = 42
         with patch("swh.vault.backend.get_cooker_cls") as mg:
             mcc = MagicMock()
@@ -240,15 +242,15 @@
         m.reset_mock()
         swh_vault.send_notif(TEST_TYPE, TEST_SWHID)
         m.assert_not_called()
 
 
 def test_send_email_error_no_smtp(swh_vault):
     reports = []
-    init_sentry("http://example.org", extra_kwargs={"transport": reports.append})
+    init_sentry(SENTRY_DSN, extra_kwargs={"transport": reports.append})
 
     emails = ("a@example.com", "billg@example.com", "test+42@example.org")
     with mock_cooking(swh_vault):
         for email in emails:
             swh_vault.cook(TEST_TYPE, TEST_SWHID, email=email)
     swh_vault.set_status(TEST_TYPE, TEST_SWHID, "done")
     swh_vault.send_notif(TEST_TYPE, TEST_SWHID)
@@ -266,15 +268,15 @@
         # second is the sentry_sdk.capture_message
         assert reports[2 * i + 1]["level"] == "error"
         assert reg.match(reports[2 * i + 1]["message"])
 
 
 def test_send_email_error_send_failed(swh_vault):
     reports = []
-    init_sentry("http://example.org", extra_kwargs={"transport": reports.append})
+    init_sentry(SENTRY_DSN, extra_kwargs={"transport": reports.append})
 
     emails = ("a@example.com", "billg@example.com", "test+42@example.org")
     with mock_cooking(swh_vault):
         for email in emails:
             swh_vault.cook(TEST_TYPE, TEST_SWHID, email=email)
     swh_vault.set_status(TEST_TYPE, TEST_SWHID, "done")
```

### Comparing `swh.vault-1.8.1/swh/vault/tests/test_cache.py` & `swh.vault-1.8.2/swh/vault/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.8.1/swh/vault/tests/test_cli.py` & `swh.vault-1.8.2/swh/vault/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.8.1/swh/vault/tests/test_cookers.py` & `swh.vault-1.8.2/swh/vault/tests/test_cookers.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import dulwich.fastexport
 import dulwich.index
 import dulwich.objects
 import dulwich.porcelain
 import dulwich.repo
 import pytest
 
-from swh.loader.git.from_disk import GitLoaderFromDisk
+from swh.loader.git.loader import GitLoader
 from swh.model import from_disk, hashutil
 from swh.model.model import (
     Person,
     Release,
     Revision,
     RevisionType,
     SkippedContent,
@@ -43,15 +43,15 @@
 from swh.model.model import ObjectType as ModelObjectType
 from swh.model.swhids import CoreSWHID, ObjectType
 from swh.vault.cookers import DirectoryCooker, GitBareCooker, RevisionGitfastCooker
 from swh.vault.tests.vault_testing import hash_content
 from swh.vault.to_disk import HIDDEN_MESSAGE, SKIPPED_MESSAGE
 
 
-class TestRepo:
+class _TestRepo:
     """A tiny context manager for a test git repository, with some utility
     functions to perform basic git stuff.
     """
 
     def __init__(self, repo_dir=None):
         self.repo_dir = repo_dir
 
@@ -165,19 +165,17 @@
 @pytest.fixture
 def git_loader(
     swh_storage,
 ):
     """Instantiate a Git Loader using the storage instance as storage."""
 
     def _create_loader(directory):
-        return GitLoaderFromDisk(
+        return GitLoader(
             swh_storage,
-            "fake_origin",
-            directory=directory,
-            visit_date=datetime.datetime.now(datetime.timezone.utc),
+            directory,
         )
 
     return _create_loader
 
 
 @contextlib.contextmanager
 def cook_extract_directory_dircooker(storage, swhid, fsck=True):
@@ -196,15 +194,15 @@
     cooker.storage = None
 
 
 @contextlib.contextmanager
 def cook_extract_directory_gitfast(storage, swhid, fsck=True):
     """Context manager that cooks a revision containing a directory and extract it,
     using RevisionGitfastCooker"""
-    test_repo = TestRepo()
+    test_repo = _TestRepo()
     with test_repo as p:
         date = TimestampWithTimezone.from_datetime(
             datetime.datetime.now(datetime.timezone.utc)
         )
         revision = Revision(
             directory=swhid.object_id,
             message=b"dummy message",
@@ -296,15 +294,15 @@
     cooker.storage = None
 
 
 @contextlib.contextmanager
 def cook_extract_revision_gitfast(storage, swhid, fsck=True):
     """Context manager that cooks a revision and extract it,
     using RevisionGitfastCooker"""
-    test_repo = TestRepo()
+    test_repo = _TestRepo()
     with cook_stream_revision_gitfast(storage, swhid) as stream, test_repo as p:
         processor = dulwich.fastexport.GitImportProcessor(test_repo.repo)
         processor.import_stream(stream)
         yield test_repo, p
 
 
 @contextlib.contextmanager
@@ -334,15 +332,15 @@
                 [
                     "git",
                     "clone",
                     os.path.join(td, f"{swhid}.git"),
                     clone_dir,
                 ]
             )
-            test_repo = TestRepo(clone_dir)
+            test_repo = _TestRepo(clone_dir)
             with test_repo:
                 yield test_repo, clone_dir
 
 
 @contextlib.contextmanager
 def cook_extract_revision_git_bare(storage, swhid, fsck=True):
     with cook_extract_git_bare(
@@ -387,15 +385,15 @@
     "   test content\n" "and unicode \N{BLACK HEART SUIT}\n" " and trailing spaces   "
 )
 TEST_EXECUTABLE = b"\x42\x40\x00\x00\x05"
 
 
 class TestDirectoryCooker:
     def test_directory_simple(self, git_loader, cook_extract_directory):
-        repo = TestRepo()
+        repo = _TestRepo()
         with repo as rp:
             (rp / "file").write_text(TEST_CONTENT)
             (rp / "executable").write_bytes(TEST_EXECUTABLE)
             (rp / "executable").chmod(0o755)
             (rp / "link").symlink_to("file")
             (rp / "dir1/dir2").mkdir(parents=True)
             (rp / "dir1/dir2/file").write_text(TEST_CONTENT)
@@ -417,15 +415,15 @@
             assert (p / "dir1/dir2/file").stat().st_mode == 0o100644
             assert (p / "dir1/dir2/file").read_text() == TEST_CONTENT
 
             directory = from_disk.Directory.from_disk(path=bytes(p))
             assert obj_id_hex == hashutil.hash_to_hex(directory.hash)
 
     def test_directory_filtered_objects(self, git_loader, cook_extract_directory):
-        repo = TestRepo()
+        repo = _TestRepo()
         with repo as rp:
             file_1, id_1 = hash_content(b"test1")
             file_2, id_2 = hash_content(b"test2")
             file_3, id_3 = hash_content(b"test3")
 
             (rp / "file").write_bytes(file_1)
             (rp / "hidden_file").write_bytes(file_2)
@@ -464,15 +462,15 @@
             assert (p / "hidden_file").read_bytes() == HIDDEN_MESSAGE
             assert (p / "absent_file").read_bytes() == SKIPPED_MESSAGE
 
     def test_directory_bogus_perms(self, git_loader, cook_extract_directory):
         # Some early git repositories have 664/775 permissions... let's check
         # if all the weird modes are properly normalized in the directory
         # cooker.
-        repo = TestRepo()
+        repo = _TestRepo()
         with repo as rp:
             (rp / "file").write_text(TEST_CONTENT)
             (rp / "file").chmod(0o664)
             (rp / "executable").write_bytes(TEST_EXECUTABLE)
             (rp / "executable").chmod(0o775)
             (rp / "wat").write_text(TEST_CONTENT)
             (rp / "wat").chmod(0o604)
@@ -514,15 +512,15 @@
 
     @pytest.mark.parametrize("direct_objstorage", [True, False])
     def test_directory_objstorage(
         self, swh_storage, git_loader, mocker, direct_objstorage
     ):
         """Like test_directory_simple, but using swh_objstorage directly, without
         going through swh_storage.content_get_data()"""
-        repo = TestRepo()
+        repo = _TestRepo()
         with repo as rp:
             (rp / "file").write_text(TEST_CONTENT)
             (rp / "executable").write_bytes(TEST_EXECUTABLE)
             (rp / "executable").chmod(0o755)
             (rp / "link").symlink_to("file")
             (rp / "dir1/dir2").mkdir(parents=True)
             (rp / "dir1/dir2/file").write_text(TEST_CONTENT)
@@ -590,15 +588,15 @@
     """Shared loading and checking methods that can be reused by different types
     of tests."""
 
     def load_repo_simple(self, git_loader):
         #
         #     1--2--3--4--5--6--7
         #
-        repo = TestRepo()
+        repo = _TestRepo()
         with repo as rp:
             (rp / "file1").write_text(TEST_CONTENT)
             repo.commit("add file1")
             (rp / "file2").write_text(TEST_CONTENT)
             repo.commit("add file2")
             (rp / "dir1/dir2").mkdir(parents=True)
             (rp / "dir1/dir2/file").write_text(TEST_CONTENT)
@@ -633,15 +631,15 @@
 
     def load_repo_two_roots(self, git_loader):
         #
         #    1----3---4
         #        /
         #   2----
         #
-        repo = TestRepo()
+        repo = _TestRepo()
         with repo as rp:
             (rp / "file1").write_text(TEST_CONTENT)
             c1 = repo.commit("Add file1")
             del repo.repo.refs[b"refs/heads/master"]  # git update-ref -d HEAD
             (rp / "file2").write_text(TEST_CONTENT)
             repo.commit("Add file2")
             repo.merge([c1])
@@ -662,15 +660,15 @@
 
     def load_repo_two_heads(self, git_loader):
         #
         #    1---2----4      <-- master and b1
         #         \
         #          ----3     <-- b2
         #
-        repo = TestRepo()
+        repo = _TestRepo()
         with repo as rp:
             (rp / "file1").write_text(TEST_CONTENT)
             repo.commit("Add file1")
 
             (rp / "file2").write_text(TEST_CONTENT)
             c2 = repo.commit("Add file2")
 
@@ -707,15 +705,15 @@
 
     def load_repo_two_double_fork_merge(self, git_loader):
         #
         #     2---4---6
         #    /   /   /
         #   1---3---5
         #
-        repo = TestRepo()
+        repo = _TestRepo()
         with repo as rp:
             (rp / "file1").write_text(TEST_CONTENT)
             c1 = repo.commit("Add file1")  # create commit 1
             repo.repo.refs[b"refs/heads/c1"] = c1  # branch c1 from master
 
             (rp / "file2").write_text(TEST_CONTENT)
             repo.commit("Add file2")  # create commit 2
@@ -760,15 +758,15 @@
         #
         #       .---.---5
         #      /   /   /
         #     2   3   4
         #    /   /   /
         #   1---.---.
         #
-        repo = TestRepo()
+        repo = _TestRepo()
         with repo as rp:
             (rp / "file1").write_text(TEST_CONTENT)
             c1 = repo.commit("Commit 1")
             repo.repo.refs[b"refs/heads/b1"] = c1
             repo.repo.refs[b"refs/heads/b2"] = c1
 
             repo.commit("Commit 2")
@@ -802,15 +800,15 @@
         assert (
             ert.repo[c2_id].parents
             == ert.repo[c3_id].parents
             == ert.repo[c4_id].parents
         )
 
     def load_repo_filtered_objects(self, git_loader):
-        repo = TestRepo()
+        repo = _TestRepo()
         with repo as rp:
             file_1, id_1 = hash_content(b"test1")
             file_2, id_2 = hash_content(b"test2")
             file_3, id_3 = hash_content(b"test3")
 
             (rp / "file").write_bytes(file_1)
             (rp / "hidden_file").write_bytes(file_2)
@@ -850,15 +848,15 @@
         assert (p / "file").read_bytes() == b"test1"
         assert (p / "hidden_file").read_bytes() == HIDDEN_MESSAGE
         assert (p / "absent_file").read_bytes() == SKIPPED_MESSAGE
 
     def load_repo_null_fields(self, git_loader):
         # Our schema doesn't enforce a lot of non-null revision fields. We need
         # to check these cases don't break the cooker.
-        repo = TestRepo()
+        repo = _TestRepo()
         with repo as rp:
             (rp / "file").write_text(TEST_CONTENT)
             c = repo.commit("initial commit")
             loader = git_loader(str(rp))
             loader.load()
             repo.repo.refs[b"HEAD"].decode()
             dir_id_hex = repo.repo[c].tree.decode()
@@ -888,15 +886,15 @@
     def load_repo_tags(self, git_loader):
         #        v-- t2
         #
         #    1---2----5      <-- master, t5, and t5a (annotated)
         #         \
         #          ----3----4     <-- t4a (annotated)
         #
-        repo = TestRepo()
+        repo = _TestRepo()
         with repo as rp:
             (rp / "file1").write_text(TEST_CONTENT)
             repo.commit("Add file1")
 
             (rp / "file2").write_text(TEST_CONTENT)
             repo.commit("Add file2")  # create c2
```

### Comparing `swh.vault-1.8.1/swh/vault/tests/test_cookers_base.py` & `swh.vault-1.8.2/swh/vault/tests/test_cookers_base.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.8.1/swh/vault/tests/test_git_bare_cooker.py` & `swh.vault-1.8.2/swh/vault/tests/test_git_bare_cooker.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import attr
 import dulwich.repo
 import pytest
 from pytest import param
 from pytest_postgresql import factories
 
-from swh.core.db.pytest_plugin import initialize_database_for_module
+from swh.core.db.db_utils import initialize_database_for_module
 from swh.model.from_disk import DentryPerms
 from swh.model.model import (
     Content,
     Directory,
     DirectoryEntry,
     ObjectType,
     Person,
@@ -51,15 +51,17 @@
 )
 
 storage_postgresql = factories.postgresql("storage_postgresql_proc")
 
 
 @pytest.fixture
 def swh_storage(storage_postgresql):
-    return get_storage("local", db=storage_postgresql.dsn, objstorage={"cls": "memory"})
+    return get_storage(
+        "postgresql", db=storage_postgresql.dsn, objstorage={"cls": "memory"}
+    )
 
 
 class RootObjects(enum.Enum):
     REVISION = enum.auto()
     SNAPSHOT = enum.auto()
     RELEASE = enum.auto()
     WEIRD_RELEASE = enum.auto()  # has a : in the name + points to another release
@@ -171,15 +173,15 @@
     If up_to_date_graph is true, then swh-graph contains all objects.
     Else, cnt4, cnt5, dir4, rev2, rel2, rel3, and snp are missing from the graph.
 
     If tag is False, rel2 is excluded.
 
     If weird_branches is False, dir4, cnt4, rel3, rel4, and cnt5 are excluded.
     """
-    from swh.graph.naive_client import NaiveClient as GraphClient
+    from swh.graph.http_naive_client import NaiveClient as GraphClient
 
     # Create objects:
 
     date = TimestampWithTimezone.from_datetime(
         datetime.datetime(2021, 5, 7, 8, 43, 59, tzinfo=datetime.timezone.utc)
     )
     author = Person.from_fullname(b"Foo <foo@example.org>")
@@ -627,15 +629,15 @@
             ),
         }
     )
     swh_storage.snapshot_add([snapshot])
 
     # Add all objects to graph
     if use_graph:
-        from swh.graph.naive_client import NaiveClient as GraphClient
+        from swh.graph.http_naive_client import NaiveClient as GraphClient
 
         nodes = [
             str(x.swhid()) for x in [content, directory, revision, release, snapshot]
         ]
         edges = [
             (str(x.swhid()), str(y.swhid()))
             for (x, y) in [
```

### Comparing `swh.vault-1.8.1/swh/vault/tests/test_init.py` & `swh.vault-1.8.2/swh/vault/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.8.1/swh/vault/tests/test_init_cookers.py` & `swh.vault-1.8.2/swh/vault/tests/test_init_cookers.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,18 +14,16 @@
 
 
 @pytest.fixture
 def swh_cooker_config():
     return {
         "vault": {
             "cls": "remote",
-            "args": {
-                "url": "mock://vault-backend",
-                "storage": {"cls": "remote", "url": "mock://storage-url"},
-            },
+            "url": "mock://vault-backend",
+            "storage": {"cls": "remote", "url": "mock://storage-url"},
         }
     }
 
 
 def write_config_to_env(config: Dict, tmp_path, monkeypatch) -> str:
     """Write the configuration dict into a temporary file, then reference that path to
     SWH_CONFIG_FILENAME environment variable.
@@ -55,15 +53,15 @@
         ({}, ValueError, "missing 'vault' configuration"),
         (
             {"vault": {"cls": "local"}},
             EnvironmentError,
             "This vault backend can only be a 'remote' configuration",
         ),
         (
-            {"vault": {"cls": "remote", "args": {"missing-storage-key": ""}}},
+            {"vault": {"cls": "remote", "missing-storage-key": ""}},
             ValueError,
             "invalid configuration: missing 'storage' config entry",
         ),
     ],
 )
 def test_get_cooker_config_ko(
     config_ko, exception_class, exception_msg, monkeypatch, tmp_path
@@ -77,26 +75,22 @@
 
 @pytest.mark.parametrize(
     "config_ok",
     [
         {
             "vault": {
                 "cls": "remote",
-                "args": {
-                    "url": "mock://vault-backend",
-                    "storage": {"cls": "remote", "url": "mock://storage-url"},
-                },
+                "url": "mock://vault-backend",
+                "storage": {"cls": "remote", "url": "mock://storage-url"},
             }
         },
         {
             "vault": {
                 "cls": "remote",
-                "args": {
-                    "url": "mock://vault-backend",
-                },
+                "url": "mock://vault-backend",
             },
             "storage": {"cls": "remote", "url": "mock://storage-url"},
         },
         {
             "vault": {
                 "cls": "remote",
                 "url": "mock://vault-backend",
```

### Comparing `swh.vault-1.8.1/swh/vault/tests/test_server.py` & `swh.vault-1.8.2/swh/vault/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.8.1/swh/vault/tests/test_to_disk.py` & `swh.vault-1.8.2/swh/vault/tests/test_to_disk.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.8.1/swh/vault/tests/vault_testing.py` & `swh.vault-1.8.2/swh/vault/tests/vault_testing.py`

 * *Files identical despite different names*

### Comparing `swh.vault-1.8.1/swh/vault/to_disk.py` & `swh.vault-1.8.2/swh/vault/to_disk.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import functools
 import os
 from typing import Any, Dict, Iterator, List
 
 from swh.model import hashutil
 from swh.model.from_disk import DentryPerms, mode_to_perms
 from swh.storage.algos.dir_iterators import dir_iterator
-from swh.storage.interface import StorageInterface
+from swh.storage.interface import HashDict, StorageInterface
 
 MISSING_MESSAGE = (
     b"This content is missing from the Software Heritage archive "
     b"(or from the mirror used while retrieving it)."
 )
 
 SKIPPED_MESSAGE = (
@@ -44,16 +44,19 @@
         they could not be retrieved (either due to privacy policy or because
         their sizes were too big for us to archive it).
 
     """
     for file_data in files_data:
         status = file_data["status"]
         if status == "visible":
-            sha1 = file_data["sha1"]
-            data = storage.content_get_data(sha1)
+            hashes: HashDict = {
+                "sha1": file_data["sha1"],
+                "sha1_git": file_data["sha1_git"],
+            }
+            data = storage.content_get_data(hashes)
             if data is None:
                 content = SKIPPED_MESSAGE
             else:
                 content = data
         elif status == "absent":
             content = SKIPPED_MESSAGE
         elif status == "hidden":
```

### Comparing `swh.vault-1.8.1/swh.vault.egg-info/PKG-INFO` & `swh.vault-1.8.2/swh.vault.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.vault
-Version: 1.8.1
+Version: 1.8.2
 Summary: Software Heritage vault
 Home-page: https://forge.softwareheritage.org/diffusion/DVAU/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-vault
```

### Comparing `swh.vault-1.8.1/swh.vault.egg-info/SOURCES.txt` & `swh.vault-1.8.2/swh.vault.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.vault-1.8.1/tox.ini` & `swh.vault-1.8.2/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 [tox]
+requires =
+  tox>4
 envlist=black,flake8,mypy,py3
 
 [testenv]
 extras =
   testing
   graph
 deps =
@@ -29,50 +31,47 @@
   {envpython} -m flake8
 
 [testenv:mypy]
 extras =
   testing
   graph
 deps =
-  mypy==0.942
+  mypy==1.0.1
 commands =
   mypy swh
 
 # build documentation outside swh-environment using the current
 # git HEAD of swh-docs, is executed on CI for each diff to prevent
 # breaking doc build
 [testenv:sphinx]
-whitelist_externals = make
+allowlist_externals = make
 usedevelop = true
 extras =
   testing
   graph
 deps =
   # fetch and install swh-docs in develop mode
-  -e git+https://forge.softwareheritage.org/source/swh-docs#egg=swh.docs
-
+  -e git+https://forge.softwareheritage.org/source/swh-docs.git\#egg=swh.docs
 setenv =
   SWH_PACKAGE_DOC_TOX_BUILD = 1
   # turn warnings into errors
   SPHINXOPTS = -W
 commands =
   make -I ../.tox/sphinx/src/swh-docs/swh/ -C docs
 
-
 # build documentation only inside swh-environment using local state
 # of swh-docs package
 [testenv:sphinx-dev]
-whitelist_externals = make
+allowlist_externals = make
 usedevelop = true
 extras =
   testing
   graph
 deps =
   # install swh-docs in develop mode
   -e ../swh-docs
-
 setenv =
   SWH_PACKAGE_DOC_TOX_BUILD = 1
   # turn warnings into errors
   SPHINXOPTS = -W
 commands =
   make -I ../.tox/sphinx-dev/src/swh-docs/swh/ -C docs
```

