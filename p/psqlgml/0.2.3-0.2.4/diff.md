# Comparing `tmp/psqlgml-0.2.3.tar.gz` & `tmp/psqlgml-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psqlgml-0.2.3.tar", last modified: Wed Dec 14 18:52:12 2022, max compression
+gzip compressed data, was "psqlgml-0.2.4.tar", last modified: Thu Jul 13 13:54:38 2023, max compression
```

## Comparing `psqlgml-0.2.3.tar` & `psqlgml-0.2.4.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:12.865683 psqlgml-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2022-12-14 18:51:47.000000 psqlgml-0.2.3/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:12.849683 psqlgml-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:12.853683 psqlgml-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2022-12-14 18:51:47.000000 psqlgml-0.2.3/.github/workflows/psqlgml.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2022-12-14 18:51:47.000000 psqlgml-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2022-12-14 18:51:47.000000 psqlgml-0.2.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2022-12-14 18:51:47.000000 psqlgml-0.2.3/.secrets.baseline
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2022-12-14 18:51:47.000000 psqlgml-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2022-12-14 18:51:47.000000 psqlgml-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2022-12-14 18:52:12.865683 psqlgml-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2022-12-14 18:51:47.000000 psqlgml-0.2.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:12.853683 psqlgml-0.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2022-12-14 18:51:47.000000 psqlgml-0.2.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      799 2022-12-14 18:51:47.000000 psqlgml-0.2.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:12.853683 psqlgml-0.2.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2022-12-14 18:51:47.000000 psqlgml-0.2.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2022-12-14 18:51:47.000000 psqlgml-0.2.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       54 2022-12-14 18:51:47.000000 psqlgml-0.2.3/mypy
--rw-r--r--   0 runner    (1001) docker     (123)      891 2022-12-14 18:51:47.000000 psqlgml-0.2.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:12.849683 psqlgml-0.2.3/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:12.849683 psqlgml-0.2.3/schemas/gdcdictionary/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:12.853683 psqlgml-0.2.3/schemas/gdcdictionary/2.4.1-rc.1/
--rw-r--r--   0 runner    (1001) docker     (123)  1807634 2022-12-14 18:51:47.000000 psqlgml-0.2.3/schemas/gdcdictionary/2.4.1-rc.1/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)  1527166 2022-12-14 18:51:47.000000 psqlgml-0.2.3/schemas/gdcdictionary/2.4.1-rc.1/schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2022-12-14 18:52:12.865683 psqlgml-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:12.849683 psqlgml-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:12.857683 psqlgml-0.2.3/src/psqlgml/
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2022-12-14 18:51:47.000000 psqlgml-0.2.3/src/psqlgml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2022-12-14 18:51:47.000000 psqlgml-0.2.3/src/psqlgml/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:12.857683 psqlgml-0.2.3/src/psqlgml/dictionaries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:51:47.000000 psqlgml-0.2.3/src/psqlgml/dictionaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2022-12-14 18:51:47.000000 psqlgml-0.2.3/src/psqlgml/dictionaries/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2022-12-14 18:51:47.000000 psqlgml-0.2.3/src/psqlgml/dictionaries/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2022-12-14 18:51:47.000000 psqlgml-0.2.3/src/psqlgml/dictionaries/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2022-12-14 18:51:47.000000 psqlgml-0.2.3/src/psqlgml/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2022-12-14 18:51:47.000000 psqlgml-0.2.3/src/psqlgml/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2022-12-14 18:51:47.000000 psqlgml-0.2.3/src/psqlgml/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:12.857683 psqlgml-0.2.3/src/psqlgml/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2022-12-14 18:51:47.000000 psqlgml-0.2.3/src/psqlgml/templates/schema.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2022-12-14 18:51:47.000000 psqlgml-0.2.3/src/psqlgml/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2022-12-14 18:51:47.000000 psqlgml-0.2.3/src/psqlgml/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)    10827 2022-12-14 18:51:47.000000 psqlgml-0.2.3/src/psqlgml/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2022-12-14 18:51:47.000000 psqlgml-0.2.3/src/psqlgml/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:12.857683 psqlgml-0.2.3/src/psqlgml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2022-12-14 18:52:12.000000 psqlgml-0.2.3/src/psqlgml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2022-12-14 18:52:12.000000 psqlgml-0.2.3/src/psqlgml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-14 18:52:12.000000 psqlgml-0.2.3/src/psqlgml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2022-12-14 18:52:12.000000 psqlgml-0.2.3/src/psqlgml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      252 2022-12-14 18:52:12.000000 psqlgml-0.2.3/src/psqlgml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-14 18:52:12.000000 psqlgml-0.2.3/src/psqlgml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-14 18:52:00.000000 psqlgml-0.2.3/src/psqlgml.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:12.857683 psqlgml-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:12.857683 psqlgml-0.2.3/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:12.857683 psqlgml-0.2.3/tests/data/dictionary/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:12.861683 psqlgml-0.2.3/tests/data/dictionary/0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/data/dictionary/0.1.0/_definitions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/data/dictionary/0.1.0/_terms.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/data/dictionary/0.1.0/_terms_enum.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/data/dictionary/0.1.0/case.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/data/dictionary/0.1.0/metaschema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/data/dictionary/0.1.0/program.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      586 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/data/dictionary/0.1.0/project.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/data/dictionary/mini.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:12.861683 psqlgml-0.2.3/tests/data/invalid/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/data/invalid/association.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/data/invalid/duplicated_def.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      244 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/data/invalid/invalid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/data/invalid/undefined_link.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      456 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/data/simple_valid.json
--rw-r--r--   0 runner    (1001) docker     (123)      192 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/data/simple_valid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      606 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:12.861683 psqlgml-0.2.3/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/integration/test_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/integration/test_git_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/integration/test_public_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/integration/test_script.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 18:52:12.865683 psqlgml-0.2.3/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/unit/test_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/unit/test_git_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/unit/test_local_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/unit/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/unit/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/unit/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tests/unit/test_visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2022-12-14 18:51:47.000000 psqlgml-0.2.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:54:38.260434 psqlgml-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-13 13:54:10.000000 psqlgml-0.2.4/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:54:38.248433 psqlgml-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:54:38.252433 psqlgml-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-13 13:54:10.000000 psqlgml-0.2.4/.github/workflows/psqlgml.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-13 13:54:10.000000 psqlgml-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-13 13:54:10.000000 psqlgml-0.2.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-13 13:54:10.000000 psqlgml-0.2.4/.secrets.baseline
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-07-13 13:54:10.000000 psqlgml-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-13 13:54:10.000000 psqlgml-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-13 13:54:38.264434 psqlgml-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-13 13:54:10.000000 psqlgml-0.2.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:54:38.252433 psqlgml-0.2.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-13 13:54:10.000000 psqlgml-0.2.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-13 13:54:10.000000 psqlgml-0.2.4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:54:38.252433 psqlgml-0.2.4/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-13 13:54:10.000000 psqlgml-0.2.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-13 13:54:10.000000 psqlgml-0.2.4/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-13 13:54:10.000000 psqlgml-0.2.4/mypy
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-13 13:54:10.000000 psqlgml-0.2.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:54:38.248433 psqlgml-0.2.4/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:54:38.248433 psqlgml-0.2.4/schemas/gdcdictionary/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:54:38.256433 psqlgml-0.2.4/schemas/gdcdictionary/2.4.1-rc.1/
+-rw-r--r--   0 runner    (1001) docker     (123)  1807634 2023-07-13 13:54:10.000000 psqlgml-0.2.4/schemas/gdcdictionary/2.4.1-rc.1/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1527166 2023-07-13 13:54:10.000000 psqlgml-0.2.4/schemas/gdcdictionary/2.4.1-rc.1/schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-13 13:54:38.264434 psqlgml-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:54:38.248433 psqlgml-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:54:38.256433 psqlgml-0.2.4/src/psqlgml/
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-13 13:54:10.000000 psqlgml-0.2.4/src/psqlgml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-07-13 13:54:10.000000 psqlgml-0.2.4/src/psqlgml/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:54:38.260434 psqlgml-0.2.4/src/psqlgml/dictionaries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 13:54:10.000000 psqlgml-0.2.4/src/psqlgml/dictionaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-07-13 13:54:10.000000 psqlgml-0.2.4/src/psqlgml/dictionaries/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-07-13 13:54:10.000000 psqlgml-0.2.4/src/psqlgml/dictionaries/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-07-13 13:54:10.000000 psqlgml-0.2.4/src/psqlgml/dictionaries/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-13 13:54:10.000000 psqlgml-0.2.4/src/psqlgml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-13 13:54:10.000000 psqlgml-0.2.4/src/psqlgml/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-13 13:54:10.000000 psqlgml-0.2.4/src/psqlgml/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:54:38.260434 psqlgml-0.2.4/src/psqlgml/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-13 13:54:10.000000 psqlgml-0.2.4/src/psqlgml/templates/schema.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-07-13 13:54:10.000000 psqlgml-0.2.4/src/psqlgml/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-13 13:54:10.000000 psqlgml-0.2.4/src/psqlgml/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10824 2023-07-13 13:54:10.000000 psqlgml-0.2.4/src/psqlgml/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-13 13:54:10.000000 psqlgml-0.2.4/src/psqlgml/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:54:38.256433 psqlgml-0.2.4/src/psqlgml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-13 13:54:38.000000 psqlgml-0.2.4/src/psqlgml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-13 13:54:38.000000 psqlgml-0.2.4/src/psqlgml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 13:54:38.000000 psqlgml-0.2.4/src/psqlgml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 13:54:38.000000 psqlgml-0.2.4/src/psqlgml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-13 13:54:38.000000 psqlgml-0.2.4/src/psqlgml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 13:54:38.000000 psqlgml-0.2.4/src/psqlgml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 13:54:25.000000 psqlgml-0.2.4/src/psqlgml.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:54:38.260434 psqlgml-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:54:38.260434 psqlgml-0.2.4/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:54:38.260434 psqlgml-0.2.4/tests/data/dictionary/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:54:38.260434 psqlgml-0.2.4/tests/data/dictionary/0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/data/dictionary/0.1.0/_definitions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/data/dictionary/0.1.0/_terms.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/data/dictionary/0.1.0/_terms_enum.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/data/dictionary/0.1.0/case.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/data/dictionary/0.1.0/metaschema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/data/dictionary/0.1.0/program.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/data/dictionary/0.1.0/project.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/data/dictionary/mini.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:54:38.260434 psqlgml-0.2.4/tests/data/invalid/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/data/invalid/association.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/data/invalid/duplicated_def.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/data/invalid/invalid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/data/invalid/undefined_link.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/data/simple_valid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/data/simple_valid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:54:38.260434 psqlgml-0.2.4/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/integration/test_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/integration/test_git_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/integration/test_public_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/integration/test_script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:54:38.260434 psqlgml-0.2.4/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/unit/test_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/unit/test_git_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/unit/test_local_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/unit/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/unit/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/unit/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tests/unit/test_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-13 13:54:10.000000 psqlgml-0.2.4/tox.ini
```

### Comparing `psqlgml-0.2.3/.github/workflows/psqlgml.yaml` & `psqlgml-0.2.4/.github/workflows/psqlgml.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 name: psqlgml-ci
 
 on:
   - push
 jobs:
   tests:
-    runs-on: ubuntu-18.04
+    runs-on: ubuntu-20.04
     strategy:
       matrix:
         python:
           - 3.6
           - 3.7
           - 3.8
           - 3.9
```

### Comparing `psqlgml-0.2.3/.gitignore` & `psqlgml-0.2.4/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 ipython_config.py
 .python-version
 celerybeat-schedule
 *.sage.py
 .env
 .venv
 env/
+venv
 venv/
 ENV/
 env.bak/
 venv.bak/
 .spyderproject
 .spyproject
 .ropeproject
```

### Comparing `psqlgml-0.2.3/.pre-commit-config.yaml` & `psqlgml-0.2.4/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.1.0
+    rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: fix-encoding-pragma
         args: [--remove]
       - id: check-yaml
   - repo: https://github.com/psf/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/pycqa/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
         name: isort (python)
       - id: isort
         name: isort (cython)
         types: [ cython ]
       - id: isort
         name: isort (pyi)
         types: [ pyi ]
   - repo: https://github.com/Yelp/detect-secrets
-    rev: v1.2.0
+    rev: v1.4.0
     hooks:
       - id: detect-secrets
         args: [ '--baseline', '.secrets.baseline' ]
   - repo: https://github.com/pycqa/flake8
-    rev: 4.0.1
+    rev: 6.0.0
     hooks:
       - id: flake8
   - repo: https://github.com/pre-commit/pygrep-hooks
-    rev: v1.9.0
+    rev: v1.10.0
     hooks:
       - id: python-use-type-annotations
   - repo: https://github.com/Lucas-C/pre-commit-hooks-markup
     rev: v1.0.1
     hooks:
       - id: rst-linter
```

### Comparing `psqlgml-0.2.3/.secrets.baseline` & `psqlgml-0.2.4/.secrets.baseline`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'version'": "'1.4.0'"}*

```diff
@@ -123,9 +123,9 @@
                 "hashed_secret": "4a9e2768850629c1bc1a0f9fac1fba06d6f549c9",
                 "is_verified": false,
                 "line_number": 21,
                 "type": "Hex High Entropy String"
             }
         ]
     },
-    "version": "1.2.0"
+    "version": "1.4.0"
 }
```

### Comparing `psqlgml-0.2.3/LICENSE` & `psqlgml-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `psqlgml-0.2.3/PKG-INFO` & `psqlgml-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psqlgml
-Version: 0.2.3
+Version: 0.2.4
 Home-page: https://github.com/kulgan/psqlgml
 Author: Rowland Ogwara
 Author-email: r.ogwara@gmail.com
 License: Apache Software License 2.0
 Keywords: gdcdictionary,psqlgraph,graphml,mocks,testing
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `psqlgml-0.2.3/README.rst` & `psqlgml-0.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `psqlgml-0.2.3/docs/Makefile` & `psqlgml-0.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `psqlgml-0.2.3/docs/make.bat` & `psqlgml-0.2.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `psqlgml-0.2.3/docs/source/conf.py` & `psqlgml-0.2.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `psqlgml-0.2.3/pyproject.toml` & `psqlgml-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `psqlgml-0.2.3/schemas/gdcdictionary/2.4.1-rc.1/schema.json` & `psqlgml-0.2.4/schemas/gdcdictionary/2.4.1-rc.1/schema.json`

 * *Files identical despite different names*

### Comparing `psqlgml-0.2.3/schemas/gdcdictionary/2.4.1-rc.1/schema.yaml` & `psqlgml-0.2.4/schemas/gdcdictionary/2.4.1-rc.1/schema.yaml`

 * *Files identical despite different names*

### Comparing `psqlgml-0.2.3/setup.cfg` & `psqlgml-0.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `psqlgml-0.2.3/src/psqlgml/__init__.py` & `psqlgml-0.2.4/src/psqlgml/__init__.py`

 * *Files identical despite different names*

### Comparing `psqlgml-0.2.3/src/psqlgml/cli.py` & `psqlgml-0.2.4/src/psqlgml/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,14 @@
 def visualize_data(
     output_dir: str,
     data_dir: str,
     data_file: str,
     output_format: psqlgml.RenderFormat,
     show: bool,
 ) -> None:
-
     psqlgml.draw(data_dir, data_file, output_dir, output_format, show_rendered=show)
 
 
 def configure_logger(cfg: LoggingConfig) -> None:
     lcfg = yaml.safe_load(
         f"""
         version: 1
```

### Comparing `psqlgml-0.2.3/src/psqlgml/dictionaries/readers.py` & `psqlgml-0.2.4/src/psqlgml/dictionaries/readers.py`

 * *Files identical despite different names*

### Comparing `psqlgml-0.2.3/src/psqlgml/dictionaries/repository.py` & `psqlgml-0.2.4/src/psqlgml/dictionaries/repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,14 @@
         dictionary_dir.mkdir(parents=True, exist_ok=True)
         commit_tree: objects.Tree = porcelain.get_object_by_path(
             self.repo, self.schema_path, committish=commit_id
         )
 
         # dump schema files to dump location
         for entry in commit_tree.items():
-
             file_name = entry.path.decode()
             blob = self.repo.get_object(entry.sha)
 
             # skip sub folders
             if not isinstance(blob, objects.Blob):
                 logger.debug(f"Skipping extra folders in schema directory {file_name}")
                 continue
@@ -132,15 +131,14 @@
         if isinstance(obj, objects.Commit):
             return obj.id
         if isinstance(obj, objects.Tag):
             return obj.object[1]
         raise ValueError(f"Unrecognized commit {commit_ref}")
 
     def clone(self) -> None:
-
         if self.repo:
             return
 
         if not self.is_cloned:
             logger.debug(f"cloning new repository {self.url} into {self.local_directory}")
 
             self.repo = porcelain.clone(
```

### Comparing `psqlgml-0.2.3/src/psqlgml/dictionaries/schemas.py` & `psqlgml-0.2.4/src/psqlgml/dictionaries/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,14 @@
 
 
 def load_schemas(
     schema_path: str,
     meta_schema: str = DEFAULT_META_SCHEMA,
     definitions: FrozenSet[str] = DEFAULT_DEFINITIONS,
 ) -> Dict[str, DictionarySchema]:
-
     excludes: FrozenSet[str] = frozenset([meta_schema] + list(definitions))
     raw_schemas: List[types.DictionarySchemaDict] = []
 
     definitions_paths = Path(schema_path)
     for definition in definitions_paths.iterdir():
         # skip non yaml files and directories
         if (
@@ -160,15 +159,14 @@
         if path not in excludes:
             raw_schemas.append(cast(types.DictionarySchemaDict, schema))
 
     return _load_schema(raw_schemas)
 
 
 def resolve_schema(entry: T, resolver: Optional[Resolver] = None) -> T:
-
     # unit entries
     if not isinstance(entry, (list, dict)):
         return entry
 
     # handle list
     if isinstance(entry, list):
         return cast(T, [resolve_schema(e, resolver) for e in entry])
```

### Comparing `psqlgml-0.2.3/src/psqlgml/resources.py` & `psqlgml-0.2.4/src/psqlgml/resources.py`

 * *Files identical despite different names*

### Comparing `psqlgml-0.2.3/src/psqlgml/schema.py` & `psqlgml-0.2.4/src/psqlgml/schema.py`

 * *Files identical despite different names*

### Comparing `psqlgml-0.2.3/src/psqlgml/templates/schema.jinja2` & `psqlgml-0.2.4/src/psqlgml/templates/schema.jinja2`

 * *Files identical despite different names*

### Comparing `psqlgml-0.2.3/src/psqlgml/types.py` & `psqlgml-0.2.4/src/psqlgml/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
 
     @property
     def links(self) -> List[SubGroupedLink]:
         return self.raw.get("links") or []
 
     @property
     def required(self) -> List[str]:
-        return self.raw["required"]
+        return self.raw.get("required") or []
 
     @property
     def unique_keys(self) -> List[List[str]]:
         return self.raw["uniqueKeys"]
 
     @property
     def properties(self) -> Dict[str, Any]:
```

### Comparing `psqlgml-0.2.3/src/psqlgml/validators.py` & `psqlgml-0.2.4/src/psqlgml/validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,23 +101,21 @@
     def validator(self) -> Draft7Validator:
         if self.dictionary_tag not in SCHEMA:
             gml_schema = self.request.schema
             SCHEMA[self.dictionary_tag] = Draft7Validator(schema=gml_schema)
         return SCHEMA[self.dictionary_tag]
 
     def validate_schema(self, obj: types.GmlData) -> Set[DataViolation]:
-
         violations: Set[DataViolation] = set()
         for e in self.validator.iter_errors(obj):
             str_path = ".".join([str(entry) for entry in e.path])
             violations.add(self.report_violation(str_path, e.message))
         return violations
 
     def validate(self) -> Dict[str, Set[DataViolation]]:
-
         payload = self.request.payload
         violations: Dict[str, Set[DataViolation]] = {}
 
         for resource, schema_data in payload.items():
             schema_violations = self.validate_schema(schema_data)
             violations[resource] = schema_violations
         return violations
@@ -197,15 +195,14 @@
         for resource, schema in payload.items():
             unique_field: types.UniqueFieldType = schema.get("unique_field", "submitter_id")
             for node in schema["nodes"]:
                 unique_id = node[unique_field]
                 node_types[unique_id] = node["label"]
 
         for resource, schema in payload.items():
-
             sub_violations: Set[DataViolation] = set()
             for index, edge in enumerate(schema["edges"]):
                 src = edge["src"]
                 dst = edge["dst"]
                 edge_label = edge.get("label")
                 src_label = node_types[src]
                 dst_label = node_types[dst]
```

### Comparing `psqlgml-0.2.3/src/psqlgml/visualization.py` & `psqlgml-0.2.4/src/psqlgml/visualization.py`

 * *Files identical despite different names*

### Comparing `psqlgml-0.2.3/src/psqlgml.egg-info/PKG-INFO` & `psqlgml-0.2.4/src/psqlgml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psqlgml
-Version: 0.2.3
+Version: 0.2.4
 Home-page: https://github.com/kulgan/psqlgml
 Author: Rowland Ogwara
 Author-email: r.ogwara@gmail.com
 License: Apache Software License 2.0
 Keywords: gdcdictionary,psqlgraph,graphml,mocks,testing
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `psqlgml-0.2.3/src/psqlgml.egg-info/SOURCES.txt` & `psqlgml-0.2.4/src/psqlgml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psqlgml-0.2.3/tests/conftest.py` & `psqlgml-0.2.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `psqlgml-0.2.3/tests/data/dictionary/0.1.0/_definitions.yaml` & `psqlgml-0.2.4/tests/data/dictionary/0.1.0/_definitions.yaml`

 * *Files identical despite different names*

### Comparing `psqlgml-0.2.3/tests/data/dictionary/0.1.0/_terms.yaml` & `psqlgml-0.2.4/tests/data/dictionary/0.1.0/_terms.yaml`

 * *Files identical despite different names*

### Comparing `psqlgml-0.2.3/tests/data/dictionary/0.1.0/_terms_enum.yaml` & `psqlgml-0.2.4/tests/data/dictionary/0.1.0/_terms_enum.yaml`

 * *Files identical despite different names*

### Comparing `psqlgml-0.2.3/tests/data/dictionary/0.1.0/case.yaml` & `psqlgml-0.2.4/tests/data/dictionary/0.1.0/case.yaml`

 * *Files identical despite different names*

### Comparing `psqlgml-0.2.3/tests/data/dictionary/0.1.0/metaschema.yaml` & `psqlgml-0.2.4/tests/data/dictionary/0.1.0/metaschema.yaml`

 * *Files identical despite different names*

### Comparing `psqlgml-0.2.3/tests/data/dictionary/0.1.0/program.yaml` & `psqlgml-0.2.4/tests/data/dictionary/0.1.0/program.yaml`

 * *Files identical despite different names*

### Comparing `psqlgml-0.2.3/tests/data/dictionary/0.1.0/project.yaml` & `psqlgml-0.2.4/tests/data/dictionary/0.1.0/project.yaml`

 * *Files identical despite different names*

### Comparing `psqlgml-0.2.3/tests/data/dictionary/mini.yaml` & `psqlgml-0.2.4/tests/data/dictionary/mini.yaml`

 * *Files identical despite different names*

### Comparing `psqlgml-0.2.3/tests/helpers.py` & `psqlgml-0.2.4/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `psqlgml-0.2.3/tests/integration/test_dictionary.py` & `psqlgml-0.2.4/tests/integration/test_dictionary.py`

 * *Files identical despite different names*

### Comparing `psqlgml-0.2.3/tests/integration/test_git_repository.py` & `psqlgml-0.2.4/tests/integration/test_git_repository.py`

 * *Files identical despite different names*

### Comparing `psqlgml-0.2.3/tests/integration/test_script.py` & `psqlgml-0.2.4/tests/integration/test_script.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
         ymo = yaml.safe_load(y)
         assert "properties" in ymo
         assert jso["url"] == REMOTE_GIT_URL
         assert jso["version"] == version
 
 
 def test_schema_generate_local(cli_runner: CliRunner, data_dir: str, tmpdir: Path) -> None:
-
     name = "dictionary"
 
     with mock.patch.dict(os.environ, {"GML_DICTIONARY_HOME": data_dir}):
         result = cli_runner.invoke(
             cli.app,
             ["generate", "-n", name, "-v", "0.1.0", "-o", tmpdir],
         )
```

### Comparing `psqlgml-0.2.3/tests/unit/test_dictionary.py` & `psqlgml-0.2.4/tests/unit/test_dictionary.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,11 +40,10 @@
 
     assert a1 == a2
     assert a1 != a3
     assert a3 != a4
 
 
 def test_from_objects() -> None:
-
     d = schemas.from_object(helpers.MiniDictionary.schema, name="mini", version="1.0.0")
     assert {"cases", "projects", "portions", "samples", "centers", "programs"} == d.links
     assert len(d.schema) == 6
```

### Comparing `psqlgml-0.2.3/tests/unit/test_git_repository.py` & `psqlgml-0.2.4/tests/unit/test_git_repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     ],
 )
 def test_get_dictionary_dir(data_dir: str, default_base: str, expectation) -> None:
     """Tests dictionary directory is set properly with and without env variables"""
 
     gml_dir = f"{Path.home()}/.gml/dictionaries" if default_base else data_dir
     with mock.patch.dict(os.environ, {"GML_DICTIONARY_HOME": gml_dir}):
-
         repo = repository.GitRepository(name="dictionary", url=REMOTE_GIT_URL, lazy_load=True)
         assert repo.name == "dictionary"
         assert Path(expectation) == repo.get_dictionary_directory("0.1.0")
 
 
 @pytest.mark.parametrize(
     "local_git_home",
@@ -35,15 +34,14 @@
         f"{pkg_resources.resource_filename('tests', 'data')}",
     ],
 )
 def test_get_local_git_dir(local_git_home: str) -> None:
     """Tests dictionary directory is set properly with and without env variables"""
 
     with mock.patch.dict(os.environ, {"GML_GIT_HOME": local_git_home}):
-
         repo = repository.GitRepository(name="dictionary", url=REMOTE_GIT_URL, lazy_load=True)
         assert repo.name == "dictionary"
         assert Path(f"{local_git_home}/dictionary/master") == repo.local_directory
 
 
 def test_lazy_load_no_clone(tmpdir: Path) -> None:
     with mock.patch.dict(os.environ, {"GML_GIT_HOME": str(tmpdir)}):
```

### Comparing `psqlgml-0.2.3/tests/unit/test_local_repository.py` & `psqlgml-0.2.4/tests/unit/test_local_repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,25 +20,23 @@
     repo = repository.LocalRepository(name="dictionary", base_directory=base_dir)
 
     assert repo.name == "dictionary"
     assert Path(expectation) == repo.get_dictionary_directory("0.1.0")
 
 
 def test_load_local_dictionary(data_dir: str) -> None:
-
     base_dir = Path(data_dir)
     repo = repository.LocalRepository(name="dictionary", base_directory=base_dir)
     dictionary = repo.read("0.1.0")
     assert dictionary
     assert dictionary.name == "dictionary"
     assert dictionary.version == "0.1.0"
 
 
 def test_load_invalid_local_dictionary(data_dir: str) -> None:
-
     base_dir = Path(data_dir)
     repo = repository.LocalRepository(name="dictionary", base_directory=base_dir)
     with pytest.raises(IOError) as exc_info:
         repo.read("0.2.0")
     assert exc_info.type == IOError
     assert (
         exc_info.value.args[0]
```

### Comparing `psqlgml-0.2.3/tests/unit/test_resources.py` & `psqlgml-0.2.4/tests/unit/test_resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from psqlgml import resources as r
 from psqlgml.types import GmlData
 
 JSON_PAYLOAD = "simple_valid.json"
 
 
 def test_merge_resource(data_dir):
-
     merged = r.load_resource(data_dir, JSON_PAYLOAD)
     assert "extends" not in merged
 
     nodes = merged["nodes"]
     assert len(nodes) == 5
 
     edges = merged["edges"]
```

### Comparing `psqlgml-0.2.3/tests/unit/test_schema.py` & `psqlgml-0.2.4/tests/unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `psqlgml-0.2.3/tests/unit/test_validators.py` & `psqlgml-0.2.4/tests/unit/test_validators.py`

 * *Files identical despite different names*

### Comparing `psqlgml-0.2.3/tests/unit/test_visualization.py` & `psqlgml-0.2.4/tests/unit/test_visualization.py`

 * *Files identical despite different names*

### Comparing `psqlgml-0.2.3/tox.ini` & `psqlgml-0.2.4/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 commands =
     python3 -m pytest --cov-report xml --cov-report html {posargs: }
 
 [testenv:lint]
 skip_install = True
 commands_pre =
 deps =
+    attrs
     mypy
     pre-commit
 allowlist_externals =
     bash
 
 commands =
     pre-commit run --all-files --show-diff-on-failure {posargs: }
```

