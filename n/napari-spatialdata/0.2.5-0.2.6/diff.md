# Comparing `tmp/napari-spatialdata-0.2.5.tar.gz` & `tmp/napari-spatialdata-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-spatialdata-0.2.5.tar", last modified: Thu Jul 13 15:16:32 2023, max compression
+gzip compressed data, was "napari-spatialdata-0.2.6.tar", last modified: Thu Jul 13 15:54:28 2023, max compression
```

## Comparing `napari-spatialdata-0.2.5.tar` & `napari-spatialdata-0.2.6.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.487995 napari-spatialdata-0.2.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.455994 napari-spatialdata-0.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.467994 napari-spatialdata-0.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/.mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.467994 napari-spatialdata-0.2.5/.napari/
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/.napari/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-07-13 15:16:32.487995 napari-spatialdata-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.467994 napari-spatialdata-0.2.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.467994 napari-spatialdata-0.2.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.467994 napari-spatialdata-0.2.5/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/_templates/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.467994 napari-spatialdata-0.2.5/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.467994 napari-spatialdata-0.2.5/docs/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/extensions/typed_returns.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.475994 napari-spatialdata-0.2.5/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)  2807648 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/notebooks/mibitof_analysis.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  3449197 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/notebooks/nanostring_analysis.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   250844 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/notebooks/scatterwidget.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  5522494 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/notebooks/spatialdata.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/references.bib
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/references.md
--rw-r--r--   0 runner    (1001) docker     (123)    16450 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/template_usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.479994 napari-spatialdata-0.2.5/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/examples/spatialdata_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/examples/spatialdata_visium.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-13 15:16:32.491995 napari-spatialdata-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.459994 napari-spatialdata-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.487995 napari-spatialdata-0.2.5/src/napari_spatialdata/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.487995 napari-spatialdata-0.2.5/src/napari_spatialdata/_constants/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/_constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/_constants/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/_constants/_pkg_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/_constants/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/_interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/_scatterwidgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/_sdata_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 15:16:32.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18158 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.487995 napari-spatialdata-0.2.5/src/napari_spatialdata/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/utils/_categoricals_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/utils/_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10180 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/utils/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.487995 napari-spatialdata-0.2.5/src/napari_spatialdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-07-13 15:16:32.000000 napari-spatialdata-0.2.5/src/napari_spatialdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-13 15:16:32.000000 napari-spatialdata-0.2.5/src/napari_spatialdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:16:32.000000 napari-spatialdata-0.2.5/src/napari_spatialdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-13 15:16:32.000000 napari-spatialdata-0.2.5/src/napari_spatialdata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-13 15:16:32.000000 napari-spatialdata-0.2.5/src/napari_spatialdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 15:16:32.000000 napari-spatialdata-0.2.5/src/napari_spatialdata.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.487995 napari-spatialdata-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/tests/test_interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/tests/test_scatterwidgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/tests/test_spatialdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/tests/test_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:54:28.365569 napari-spatialdata-0.2.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:54:28.329569 napari-spatialdata-0.2.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:54:28.337569 napari-spatialdata-0.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/.mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:54:28.337569 napari-spatialdata-0.2.6/.napari/
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/.napari/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-07-13 15:54:28.365569 napari-spatialdata-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:54:28.341569 napari-spatialdata-0.2.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:54:28.341569 napari-spatialdata-0.2.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:54:28.341569 napari-spatialdata-0.2.6/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/docs/_templates/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:54:28.341569 napari-spatialdata-0.2.6/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:54:28.341569 napari-spatialdata-0.2.6/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/docs/extensions/typed_returns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:54:28.349569 napari-spatialdata-0.2.6/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)  2807648 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/docs/notebooks/mibitof_analysis.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  3449197 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/docs/notebooks/nanostring_analysis.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   250844 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/docs/notebooks/scatterwidget.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  5522494 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/docs/notebooks/spatialdata.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/docs/references.bib
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/docs/references.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16450 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/docs/template_usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:54:28.353569 napari-spatialdata-0.2.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/examples/spatialdata_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/examples/spatialdata_visium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-13 15:54:28.365569 napari-spatialdata-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:54:28.333569 napari-spatialdata-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:54:28.357569 napari-spatialdata-0.2.6/src/napari_spatialdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/src/napari_spatialdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/src/napari_spatialdata/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:54:28.361569 napari-spatialdata-0.2.6/src/napari_spatialdata/_constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/src/napari_spatialdata/_constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/src/napari_spatialdata/_constants/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/src/napari_spatialdata/_constants/_pkg_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/src/napari_spatialdata/_constants/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/src/napari_spatialdata/_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/src/napari_spatialdata/_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/src/napari_spatialdata/_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/src/napari_spatialdata/_scatterwidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/src/napari_spatialdata/_sdata_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 15:54:28.000000 napari-spatialdata-0.2.6/src/napari_spatialdata/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/src/napari_spatialdata/_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/src/napari_spatialdata/_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18158 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/src/napari_spatialdata/_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/src/napari_spatialdata/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:54:28.361569 napari-spatialdata-0.2.6/src/napari_spatialdata/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/src/napari_spatialdata/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/src/napari_spatialdata/utils/_categoricals_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/src/napari_spatialdata/utils/_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10180 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/src/napari_spatialdata/utils/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:54:28.361569 napari-spatialdata-0.2.6/src/napari_spatialdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-07-13 15:54:28.000000 napari-spatialdata-0.2.6/src/napari_spatialdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-13 15:54:28.000000 napari-spatialdata-0.2.6/src/napari_spatialdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:54:28.000000 napari-spatialdata-0.2.6/src/napari_spatialdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-13 15:54:28.000000 napari-spatialdata-0.2.6/src/napari_spatialdata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-13 15:54:28.000000 napari-spatialdata-0.2.6/src/napari_spatialdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 15:54:28.000000 napari-spatialdata-0.2.6/src/napari_spatialdata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:54:28.365569 napari-spatialdata-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/tests/test_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/tests/test_scatterwidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/tests/test_spatialdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/tests/test_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-13 15:54:00.000000 napari-spatialdata-0.2.6/tox.ini
```

### Comparing `napari-spatialdata-0.2.5/.github/workflows/test_and_deploy.yml` & `napari-spatialdata-0.2.6/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/.gitignore` & `napari-spatialdata-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/.mypy.ini` & `napari-spatialdata-0.2.6/.mypy.ini`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/.napari/DESCRIPTION.md` & `napari-spatialdata-0.2.6/.napari/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/.pre-commit-config.yaml` & `napari-spatialdata-0.2.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/LICENSE` & `napari-spatialdata-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/PKG-INFO` & `napari-spatialdata-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-spatialdata
-Version: 0.2.5
+Version: 0.2.6
 Summary: Interactive visualization of spatial omics data with napari
 Home-page: https://github.com/scverse/napari-spatialdata.git
 Author: giovanni palla
 Author-email: giov.pll@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/scverse/napari-spatialdata/issues
 Project-URL: Documentation, https://github.com/scverse/napari-spatialdata#README.md
```

### Comparing `napari-spatialdata-0.2.5/README.md` & `napari-spatialdata-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/docs/Makefile` & `napari-spatialdata-0.2.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/docs/_templates/autosummary/class.rst` & `napari-spatialdata-0.2.6/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/docs/conf.py` & `napari-spatialdata-0.2.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/docs/contributing.md` & `napari-spatialdata-0.2.6/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/docs/extensions/typed_returns.py` & `napari-spatialdata-0.2.6/docs/extensions/typed_returns.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/docs/make.bat` & `napari-spatialdata-0.2.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/docs/notebooks/mibitof_analysis.ipynb` & `napari-spatialdata-0.2.6/docs/notebooks/mibitof_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/docs/notebooks/nanostring_analysis.ipynb` & `napari-spatialdata-0.2.6/docs/notebooks/nanostring_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/docs/notebooks/scatterwidget.ipynb` & `napari-spatialdata-0.2.6/docs/notebooks/scatterwidget.ipynb`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/docs/notebooks/spatialdata.ipynb` & `napari-spatialdata-0.2.6/docs/notebooks/spatialdata.ipynb`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/docs/references.bib` & `napari-spatialdata-0.2.6/docs/references.bib`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/docs/template_usage.md` & `napari-spatialdata-0.2.6/docs/template_usage.md`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/pyproject.toml` & `napari-spatialdata-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/setup.cfg` & `napari-spatialdata-0.2.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/src/napari_spatialdata/__init__.py` & `napari-spatialdata-0.2.6/src/napari_spatialdata/__init__.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/src/napari_spatialdata/__main__.py` & `napari-spatialdata-0.2.6/src/napari_spatialdata/__main__.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/src/napari_spatialdata/_constants/_pkg_constants.py` & `napari-spatialdata-0.2.6/src/napari_spatialdata/_constants/_pkg_constants.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/src/napari_spatialdata/_constants/_utils.py` & `napari-spatialdata-0.2.6/src/napari_spatialdata/_constants/_utils.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/src/napari_spatialdata/_interactive.py` & `napari-spatialdata-0.2.6/src/napari_spatialdata/_interactive.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/src/napari_spatialdata/_model.py` & `napari-spatialdata-0.2.6/src/napari_spatialdata/_model.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/src/napari_spatialdata/_reader.py` & `napari-spatialdata-0.2.6/src/napari_spatialdata/_reader.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/src/napari_spatialdata/_scatterwidgets.py` & `napari-spatialdata-0.2.6/src/napari_spatialdata/_scatterwidgets.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/src/napari_spatialdata/_sdata_widgets.py` & `napari-spatialdata-0.2.6/src/napari_spatialdata/_sdata_widgets.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/src/napari_spatialdata/_view.py` & `napari-spatialdata-0.2.6/src/napari_spatialdata/_view.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/src/napari_spatialdata/_viewer.py` & `napari-spatialdata-0.2.6/src/napari_spatialdata/_viewer.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/src/napari_spatialdata/_widgets.py` & `napari-spatialdata-0.2.6/src/napari_spatialdata/_widgets.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/src/napari_spatialdata/napari.yaml` & `napari-spatialdata-0.2.6/src/napari_spatialdata/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/src/napari_spatialdata/utils/_categoricals_utils.py` & `napari-spatialdata-0.2.6/src/napari_spatialdata/utils/_categoricals_utils.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/src/napari_spatialdata/utils/_test_utils.py` & `napari-spatialdata-0.2.6/src/napari_spatialdata/utils/_test_utils.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/src/napari_spatialdata/utils/_utils.py` & `napari-spatialdata-0.2.6/src/napari_spatialdata/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/src/napari_spatialdata.egg-info/PKG-INFO` & `napari-spatialdata-0.2.6/src/napari_spatialdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-spatialdata
-Version: 0.2.5
+Version: 0.2.6
 Summary: Interactive visualization of spatial omics data with napari
 Home-page: https://github.com/scverse/napari-spatialdata.git
 Author: giovanni palla
 Author-email: giov.pll@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/scverse/napari-spatialdata/issues
 Project-URL: Documentation, https://github.com/scverse/napari-spatialdata#README.md
```

### Comparing `napari-spatialdata-0.2.5/src/napari_spatialdata.egg-info/SOURCES.txt` & `napari-spatialdata-0.2.6/src/napari_spatialdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/tests/conftest.py` & `napari-spatialdata-0.2.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/tests/test_cli.py` & `napari-spatialdata-0.2.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/tests/test_interactive.py` & `napari-spatialdata-0.2.6/tests/test_interactive.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/tests/test_scatterwidgets.py` & `napari-spatialdata-0.2.6/tests/test_scatterwidgets.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/tests/test_spatialdata.py` & `napari-spatialdata-0.2.6/tests/test_spatialdata.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/tests/test_utils.py` & `napari-spatialdata-0.2.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/tests/test_viewer.py` & `napari-spatialdata-0.2.6/tests/test_viewer.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.5/tox.ini` & `napari-spatialdata-0.2.6/tox.ini`

 * *Files identical despite different names*

