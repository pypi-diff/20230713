# Comparing `tmp/napari-spatialdata-0.2.4.tar.gz` & `tmp/napari-spatialdata-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-spatialdata-0.2.4.tar", last modified: Tue May 23 16:22:43 2023, max compression
+gzip compressed data, was "napari-spatialdata-0.2.5.tar", last modified: Thu Jul 13 15:16:32 2023, max compression
```

## Comparing `napari-spatialdata-0.2.4.tar` & `napari-spatialdata-0.2.5.tar`

### file list

```diff
@@ -1,78 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.373450 napari-spatialdata-0.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.345449 napari-spatialdata-0.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.349449 napari-spatialdata-0.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/.mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.349449 napari-spatialdata-0.2.4/.napari/
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/.napari/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-05-23 16:22:43.373450 napari-spatialdata-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.353449 napari-spatialdata-0.2.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.353449 napari-spatialdata-0.2.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.353449 napari-spatialdata-0.2.4/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/_templates/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.353449 napari-spatialdata-0.2.4/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.353449 napari-spatialdata-0.2.4/docs/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/extensions/typed_returns.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.361449 napari-spatialdata-0.2.4/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)  2807648 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/notebooks/mibitof_analysis.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  3449197 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/notebooks/nanostring_analysis.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   250844 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/notebooks/scatterwidget.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  5522494 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/notebooks/spatialdata.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/references.bib
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/references.md
--rw-r--r--   0 runner    (1001) docker     (123)    16450 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/docs/template_usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.369449 napari-spatialdata-0.2.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/examples/spatialdata_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/examples/spatialdata_visium.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-23 16:22:43.373450 napari-spatialdata-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.345449 napari-spatialdata-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.369449 napari-spatialdata-0.2.4/src/napari_spatialdata/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/_categoricals_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.373450 napari-spatialdata-0.2.4/src/napari_spatialdata/_constants/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/_constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/_constants/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/_constants/_pkg_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/_constants/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/_interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/_scatterwidgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-23 16:22:43.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/_view.py
--rw-r--r--   0 runner    (1001) docker     (123)    18152 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/src/napari_spatialdata/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.373450 napari-spatialdata-0.2.4/src/napari_spatialdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-05-23 16:22:43.000000 napari-spatialdata-0.2.4/src/napari_spatialdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-23 16:22:43.000000 napari-spatialdata-0.2.4/src/napari_spatialdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 16:22:43.000000 napari-spatialdata-0.2.4/src/napari_spatialdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-23 16:22:43.000000 napari-spatialdata-0.2.4/src/napari_spatialdata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-23 16:22:43.000000 napari-spatialdata-0.2.4/src/napari_spatialdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-23 16:22:43.000000 napari-spatialdata-0.2.4/src/napari_spatialdata.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:43.373450 napari-spatialdata-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/tests/test_interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/tests/test_scatterwidgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/tests/test_spatialdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-23 16:22:17.000000 napari-spatialdata-0.2.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.487995 napari-spatialdata-0.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.455994 napari-spatialdata-0.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.467994 napari-spatialdata-0.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/.mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.467994 napari-spatialdata-0.2.5/.napari/
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/.napari/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-07-13 15:16:32.487995 napari-spatialdata-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.467994 napari-spatialdata-0.2.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.467994 napari-spatialdata-0.2.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.467994 napari-spatialdata-0.2.5/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/_templates/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.467994 napari-spatialdata-0.2.5/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.467994 napari-spatialdata-0.2.5/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/extensions/typed_returns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.475994 napari-spatialdata-0.2.5/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)  2807648 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/notebooks/mibitof_analysis.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  3449197 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/notebooks/nanostring_analysis.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   250844 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/notebooks/scatterwidget.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  5522494 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/notebooks/spatialdata.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/references.bib
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/references.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16450 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/docs/template_usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.479994 napari-spatialdata-0.2.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/examples/spatialdata_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/examples/spatialdata_visium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-13 15:16:32.491995 napari-spatialdata-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.459994 napari-spatialdata-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.487995 napari-spatialdata-0.2.5/src/napari_spatialdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.487995 napari-spatialdata-0.2.5/src/napari_spatialdata/_constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/_constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/_constants/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/_constants/_pkg_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/_constants/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/_scatterwidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/_sdata_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 15:16:32.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18158 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.487995 napari-spatialdata-0.2.5/src/napari_spatialdata/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/utils/_categoricals_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/utils/_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10180 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/src/napari_spatialdata/utils/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.487995 napari-spatialdata-0.2.5/src/napari_spatialdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-07-13 15:16:32.000000 napari-spatialdata-0.2.5/src/napari_spatialdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-13 15:16:32.000000 napari-spatialdata-0.2.5/src/napari_spatialdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:16:32.000000 napari-spatialdata-0.2.5/src/napari_spatialdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-13 15:16:32.000000 napari-spatialdata-0.2.5/src/napari_spatialdata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-13 15:16:32.000000 napari-spatialdata-0.2.5/src/napari_spatialdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 15:16:32.000000 napari-spatialdata-0.2.5/src/napari_spatialdata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:32.487995 napari-spatialdata-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/tests/test_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/tests/test_scatterwidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/tests/test_spatialdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/tests/test_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-13 15:16:14.000000 napari-spatialdata-0.2.5/tox.ini
```

### Comparing `napari-spatialdata-0.2.4/.github/workflows/test_and_deploy.yml` & `napari-spatialdata-0.2.5/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.4/.gitignore` & `napari-spatialdata-0.2.5/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -103,7 +103,10 @@
 
 # docs
 /docs/generated/
 /docs/_build/
 
 # Tutorial data
 docs/notebooks/tutorial_data/
+
+# Other data
+spatialdata-sandbox
```

### Comparing `napari-spatialdata-0.2.4/.mypy.ini` & `napari-spatialdata-0.2.5/.mypy.ini`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.4/.napari/DESCRIPTION.md` & `napari-spatialdata-0.2.5/.napari/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.4/.pre-commit-config.yaml` & `napari-spatialdata-0.2.5/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -3,26 +3,26 @@
   python: python3
 default_stages:
   - commit
   - push
 minimum_pre_commit_version: 2.9.3
 repos:
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.3.0
+    rev: v1.4.1
     hooks:
       - id: mypy
         additional_dependencies: [numpy>=1.23]
         exclude: docs
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
         additional_dependencies: [toml]
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.0-alpha.9-for-vscode
+    rev: v3.0.0
     hooks:
       - id: prettier
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: detect-private-key
       - id: check-merge-conflict
@@ -41,15 +41,15 @@
         args: [--django]
       - id: check-case-conflict
       - id: check-docstring-first
       - id: check-yaml
       - id: check-toml
       - id: requirements-txt-fixer
   - repo: https://github.com/asottile/blacken-docs
-    rev: 1.13.0
+    rev: 1.15.0
     hooks:
       - id: blacken-docs
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.269
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.0.277
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
```

### Comparing `napari-spatialdata-0.2.4/LICENSE` & `napari-spatialdata-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.4/PKG-INFO` & `napari-spatialdata-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-spatialdata
-Version: 0.2.4
+Version: 0.2.5
 Summary: Interactive visualization of spatial omics data with napari
 Home-page: https://github.com/scverse/napari-spatialdata.git
 Author: giovanni palla
 Author-email: giov.pll@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/scverse/napari-spatialdata/issues
 Project-URL: Documentation, https://github.com/scverse/napari-spatialdata#README.md
```

### Comparing `napari-spatialdata-0.2.4/README.md` & `napari-spatialdata-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.4/docs/Makefile` & `napari-spatialdata-0.2.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.4/docs/_templates/autosummary/class.rst` & `napari-spatialdata-0.2.5/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.4/docs/conf.py` & `napari-spatialdata-0.2.5/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
     # ("py:obj", "napari_spatialdata.QtAdataScatterWidget.scroll"),
     # ("py:obj", "napari_spatialdata.QtAdataScatterWidget.insertAction"),
     # If building the documentation fails because of a missing link that is outside your control,
     # you can add an exception to this list.
     # ("py:class", "igraph.Graph"),
 ]
 
-qt_documentation = "PyQt6"
+qt_documentation = "PyQt5"
 
 suppress_warnings = [
     "myst.header",  # https://github.com/executablebooks/MyST-Parser/issues/262
 ]
 
 
 def setup(app):
```

### Comparing `napari-spatialdata-0.2.4/docs/contributing.md` & `napari-spatialdata-0.2.5/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.4/docs/extensions/typed_returns.py` & `napari-spatialdata-0.2.5/docs/extensions/typed_returns.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.4/docs/make.bat` & `napari-spatialdata-0.2.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.4/docs/notebooks/mibitof_analysis.ipynb` & `napari-spatialdata-0.2.5/docs/notebooks/mibitof_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.4/docs/notebooks/nanostring_analysis.ipynb` & `napari-spatialdata-0.2.5/docs/notebooks/nanostring_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.4/docs/notebooks/scatterwidget.ipynb` & `napari-spatialdata-0.2.5/docs/notebooks/scatterwidget.ipynb`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.4/docs/notebooks/spatialdata.ipynb` & `napari-spatialdata-0.2.5/docs/notebooks/spatialdata.ipynb`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.4/docs/references.bib` & `napari-spatialdata-0.2.5/docs/references.bib`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.4/docs/template_usage.md` & `napari-spatialdata-0.2.5/docs/template_usage.md`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.4/pyproject.toml` & `napari-spatialdata-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.4/setup.cfg` & `napari-spatialdata-0.2.5/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 	scanpydoc
 	ipykernel
 	ipython
 	sphinx-copybutton
 	sphinx-qt-documentation
 	myst-nb
 all = 
-	PyQt6
+	PyQt5
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 napari_spatiadata = napari.yaml
 
@@ -81,13 +81,13 @@
 console_scripts = 
 	spatialdata = napari_spatialdata.__main__:main
 
 [tool:pytest]
 python_files = test_*.py
 testpaths = tests/
 xfail_strict = true
-qt_api = pyqt6
+qt_api = pyqt5
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `napari-spatialdata-0.2.4/src/napari_spatialdata/__init__.py` & `napari-spatialdata-0.2.5/src/napari_spatialdata/__init__.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.4/src/napari_spatialdata/__main__.py` & `napari-spatialdata-0.2.5/src/napari_spatialdata/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,29 +12,36 @@
 
 def main() -> None:
     """Run the napari-spatialdata CLI."""
     cli()
 
 
 @cli.command(help="Interactive visualization of SpatialData datasets with napari")
-@click.argument("path", nargs=-1, type=tuple, required=True)
-def view(paths: tuple[str]) -> None:
+@click.argument("path", nargs=-1, type=str, required=True)
+@click.option(
+    "--headless",
+    "-h",
+    is_flag=True,
+    default=False,
+    help="Run napari in headless mode. Used for testing.",
+)
+def view(path: tuple[str], headless: bool) -> None:
     """Interactive visualization of SpatialData datasets with napari.
 
     :param path: Path to the SpatialData dataset
     """
-    assert type(paths) == tuple
+    assert type(path) == tuple
 
     import spatialdata as sd
 
     from napari_spatialdata import Interactive
 
     sdatas = []
-    for path in paths:
-        p = Path(path).resolve()
+    for p_str in path:
+        p = Path(p_str).resolve()
         assert p.exists(), f"Error: {p} does not exist"
         logger.info(f"Reading {p}")
         if not p.is_dir():
             logger.error(
                 f"Error: .zarr storage not found at {p}. Please specify a valid OME-NGFF spatial data (.zarr) file. "
                 "Example "
                 '"python -m '
@@ -42,12 +49,13 @@
             )
             return
         sdata = sd.SpatialData.read(p)
         sdatas.append(sdata)
 
     # TODO: support multiple spatial data
     interactive = Interactive(sdata=sdatas[0])
-    interactive.run()
+    if not headless:
+        interactive.run()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `napari-spatialdata-0.2.4/src/napari_spatialdata/_categoricals_utils.py` & `napari-spatialdata-0.2.5/src/napari_spatialdata/utils/_categoricals_utils.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.4/src/napari_spatialdata/_constants/_pkg_constants.py` & `napari-spatialdata-0.2.5/src/napari_spatialdata/_constants/_pkg_constants.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.4/src/napari_spatialdata/_constants/_utils.py` & `napari-spatialdata-0.2.5/src/napari_spatialdata/_constants/_utils.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.4/src/napari_spatialdata/_model.py` & `napari-spatialdata-0.2.5/src/napari_spatialdata/_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pandas as pd
 from anndata import AnnData
 from napari.layers import Layer
 from napari.utils.events import EmitterGroup, Event
 
 from napari_spatialdata._constants._constants import Symbol
 from napari_spatialdata._constants._pkg_constants import Key
-from napari_spatialdata._utils import NDArrayA, _ensure_dense_vector
+from napari_spatialdata.utils._utils import NDArrayA, _ensure_dense_vector
 
 __all__ = ["ImageModel"]
 
 
 @dataclass
 class ImageModel:
     """Model which holds the data for interactive visualization."""
```

### Comparing `napari-spatialdata-0.2.4/src/napari_spatialdata/_reader.py` & `napari-spatialdata-0.2.5/src/napari_spatialdata/_reader.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.4/src/napari_spatialdata/_scatterwidgets.py` & `napari-spatialdata-0.2.5/src/napari_spatialdata/_scatterwidgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 from napari.layers import Layer
 from napari.viewer import Viewer
 from napari_matplotlib.base import NapariMPLWidget
 from pandas.api.types import is_categorical_dtype
 from qtpy import QtWidgets
 from qtpy.QtCore import Signal
 
-from napari_spatialdata._categoricals_utils import _add_categorical_legend
 from napari_spatialdata._model import ImageModel
-from napari_spatialdata._utils import NDArrayA, _get_categorical, _set_palette
 from napari_spatialdata._widgets import AListWidget, ComponentWidget
+from napari_spatialdata.utils._categoricals_utils import _add_categorical_legend
+from napari_spatialdata.utils._utils import NDArrayA, _get_categorical, _set_palette
 
 __all__ = [
     "MatplotlibWidget",
     "AxisWidgets",
 ]
```

### Comparing `napari-spatialdata-0.2.4/src/napari_spatialdata/_utils.py` & `napari-spatialdata-0.2.5/src/napari_spatialdata/utils/_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from functools import wraps
 from typing import TYPE_CHECKING, Any, Callable, Optional, Sequence, Union
 
 import numpy as np
 import pandas as pd
 from anndata import AnnData
 from dask.dataframe.core import DataFrame as DaskDataFrame
+from datatree import DataTree
 from geopandas import GeoDataFrame
 from loguru import logger
 from matplotlib.colors import is_color_like, to_rgb
 from multiscale_spatial_image.multiscale_spatial_image import MultiscaleSpatialImage
 from numba import njit, prange
 from pandas.api.types import infer_dtype, is_categorical_dtype
 from pandas.core.dtypes.common import (
@@ -19,21 +20,24 @@
     is_numeric_dtype,
     is_object_dtype,
     is_string_dtype,
 )
 from scipy.sparse import issparse, spmatrix
 from scipy.spatial import KDTree
 from spatial_image import SpatialImage
-from spatialdata.models import SpatialElement
+from spatialdata.models import SpatialElement, get_axes_names
 from spatialdata.transformations import get_transformation
 
-from napari_spatialdata._categoricals_utils import (
+from napari_spatialdata._constants._pkg_constants import Key
+from napari_spatialdata.utils._categoricals_utils import (
     add_colors_for_categorical_sample_annotation,
 )
-from napari_spatialdata._constants._pkg_constants import Key
+
+if TYPE_CHECKING:
+    from xarray import DataArray
 
 try:
     from numpy.typing import NDArray
 
     NDArrayA = NDArray[Any]
 except (ImportError, TypeError):
     NDArray = np.ndarray  # type: ignore[misc]
@@ -217,7 +221,61 @@
         ),
         dtype=np.bool_,
     )
     for i in prange(len(out)):
         out[i] = _point_inside_triangles(triangles - points[i])
 
     return out
+
+
+def _adjust_channels_order(element: SpatialImage | MultiscaleSpatialImage) -> tuple[DataArray, bool]:
+    """Swap the axes to y, x, c and check if an image supports rgb(a) visualization.
+
+    Checks whether c dim is present in the axes and if so, transposes the dimensions to have c last.
+    If the dimension of c is 3 or 4, it is assumed that the image is suitable for rgb(a) visualization.
+
+    Parameters
+    ----------
+    element: SpatialImage | MultiScaleSpatialImage
+        Element in sdata.images
+
+    Returns
+    -------
+    new_raster: DataArray
+        The image in shape of (c, y, x)
+    rgb: bool
+        Flag indicating suitability for rgb(a) visualization.
+    """
+    axes = get_axes_names(element)
+
+    if "c" in axes:
+        assert axes.index("c") == 0
+        if isinstance(element, SpatialImage):
+            n_channels = element.shape[0]
+        elif isinstance(element, MultiscaleSpatialImage):
+            v = element["scale0"].values()
+            assert len(v) == 1
+            n_channels = v.__iter__().__next__().shape[0]
+        else:
+            raise TypeError(f"Unsupported type for images or labels: {type(element)}")
+    else:
+        n_channels = 0
+
+    if n_channels in [3, 4]:
+        rgb = True
+        new_raster = element.transpose("y", "x", "c")
+    else:
+        rgb = False
+        new_raster = element
+
+    # TODO: after we call .transpose() on a MultiscaleSpatialImage object we get a DataTree object. We should look at
+    # this better and either cast somehow back to MultiscaleSpatialImage or fix/report this
+    if isinstance(new_raster, (MultiscaleSpatialImage, DataTree)):
+        list_of_xdata = []
+        for k in new_raster:
+            v = new_raster[k].values()
+            assert len(v) == 1
+            xdata = v.__iter__().__next__()
+            list_of_xdata.append(xdata)
+        new_raster = list_of_xdata
+
+    return new_raster, rgb
```

### Comparing `napari-spatialdata-0.2.4/src/napari_spatialdata/_view.py` & `napari-spatialdata-0.2.5/src/napari_spatialdata/_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,25 +18,25 @@
     QVBoxLayout,
     QWidget,
 )
 
 from napari_spatialdata._constants._pkg_constants import Key
 from napari_spatialdata._model import ImageModel
 from napari_spatialdata._scatterwidgets import AxisWidgets, MatplotlibWidget
-from napari_spatialdata._utils import (
-    NDArrayA,
-    _get_categorical,
-    _points_inside_triangles,
-)
 from napari_spatialdata._widgets import (
     AListWidget,
     CBarWidget,
     ComponentWidget,
     RangeSliderWidget,
 )
+from napari_spatialdata.utils._utils import (
+    NDArrayA,
+    _get_categorical,
+    _points_inside_triangles,
+)
 
 __all__ = ["QtAdataViewWidget", "QtAdataScatterWidget"]
 
 
 class QtAdataScatterWidget(QWidget):
     """Adata viewer widget."""
 
@@ -256,15 +256,15 @@
             # TODO: Check if this can be removed
             self.model.points_coordinates = layer.metadata["points"].X
             self.model.points_var = layer.metadata["points"].obs["gene"]
             self.model.point_diameter = np.array([0.0] + [layer.metadata["point_diameter"]] * 2) * self.model.scale
 
         self.model.spot_diameter = np.array([0.0, 10.0, 10.0])
         self.model.labels_key = layer.metadata["labels_key"] if isinstance(layer, Labels) else None
-        self.model.system_name = self.model.layer.name
+        self.model.system_name = layer.metadata["name"] if "name" in layer.metadata else None
 
         if "colormap" in layer.metadata:
             self.model.cmap = layer.metadata["colormap"]
         if hasattr(
             self, "obs_widget"
         ):  # to check if the widget has been already initialized, layer update should only be called on layer change
             self._on_layer_update()
```

### Comparing `napari-spatialdata-0.2.4/src/napari_spatialdata/_widgets.py` & `napari-spatialdata-0.2.5/src/napari_spatialdata/_widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from sklearn.preprocessing import MinMaxScaler
 from superqt import QRangeSlider
 from vispy import scene
 from vispy.color.colormap import Colormap, MatplotlibColormap
 from vispy.scene.widgets import ColorBarWidget
 
 from napari_spatialdata._model import ImageModel
-from napari_spatialdata._utils import (
+from napari_spatialdata.utils._utils import (
     NDArrayA,
     _get_categorical,
     _min_max_norm,
     _position_cluster_labels,
     _set_palette,
 )
```

### Comparing `napari-spatialdata-0.2.4/src/napari_spatialdata/napari.yaml` & `napari-spatialdata-0.2.5/src/napari_spatialdata/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.4/src/napari_spatialdata.egg-info/PKG-INFO` & `napari-spatialdata-0.2.5/src/napari_spatialdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-spatialdata
-Version: 0.2.4
+Version: 0.2.5
 Summary: Interactive visualization of spatial omics data with napari
 Home-page: https://github.com/scverse/napari-spatialdata.git
 Author: giovanni palla
 Author-email: giov.pll@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/scverse/napari-spatialdata/issues
 Project-URL: Documentation, https://github.com/scverse/napari-spatialdata#README.md
```

### Comparing `napari-spatialdata-0.2.4/src/napari_spatialdata.egg-info/SOURCES.txt` & `napari-spatialdata-0.2.5/src/napari_spatialdata.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -29,33 +29,39 @@
 docs/notebooks/nanostring_analysis.ipynb
 docs/notebooks/scatterwidget.ipynb
 docs/notebooks/spatialdata.ipynb
 examples/spatialdata_empty.py
 examples/spatialdata_visium.py
 src/napari_spatialdata/__init__.py
 src/napari_spatialdata/__main__.py
-src/napari_spatialdata/_categoricals_utils.py
 src/napari_spatialdata/_interactive.py
 src/napari_spatialdata/_model.py
 src/napari_spatialdata/_reader.py
 src/napari_spatialdata/_scatterwidgets.py
-src/napari_spatialdata/_utils.py
+src/napari_spatialdata/_sdata_widgets.py
 src/napari_spatialdata/_version.py
 src/napari_spatialdata/_view.py
+src/napari_spatialdata/_viewer.py
 src/napari_spatialdata/_widgets.py
 src/napari_spatialdata/napari.yaml
 src/napari_spatialdata.egg-info/PKG-INFO
 src/napari_spatialdata.egg-info/SOURCES.txt
 src/napari_spatialdata.egg-info/dependency_links.txt
 src/napari_spatialdata.egg-info/entry_points.txt
 src/napari_spatialdata.egg-info/requires.txt
 src/napari_spatialdata.egg-info/top_level.txt
 src/napari_spatialdata/_constants/__init__.py
 src/napari_spatialdata/_constants/_constants.py
 src/napari_spatialdata/_constants/_pkg_constants.py
 src/napari_spatialdata/_constants/_utils.py
+src/napari_spatialdata/utils/__init__.py
+src/napari_spatialdata/utils/_categoricals_utils.py
+src/napari_spatialdata/utils/_test_utils.py
+src/napari_spatialdata/utils/_utils.py
 tests/__init__.py
 tests/conftest.py
+tests/test_cli.py
 tests/test_interactive.py
 tests/test_scatterwidgets.py
 tests/test_spatialdata.py
-tests/test_utils.py
+tests/test_utils.py
+tests/test_viewer.py
```

### Comparing `napari-spatialdata-0.2.4/tests/conftest.py` & `napari-spatialdata-0.2.5/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import pytest
 from anndata import AnnData
 from loguru import logger
 from matplotlib.testing.compare import compare_images
-from napari_spatialdata._utils import NDArrayA
+from napari_spatialdata.utils._utils import NDArrayA
 from scipy import ndimage as ndi
 from skimage import data
 
 HERE: Path = Path(__file__).parent
 
 SEED = 42
```

### Comparing `napari-spatialdata-0.2.4/tests/test_interactive.py` & `napari-spatialdata-0.2.5/tests/test_interactive.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import numpy as np
 import pandas as pd
 import pytest
 from anndata import AnnData
 from napari.layers import Image, Labels
 from napari_spatialdata._model import ImageModel
-from napari_spatialdata._utils import NDArrayA
 from napari_spatialdata._view import QtAdataScatterWidget, QtAdataViewWidget
+from napari_spatialdata.utils._utils import NDArrayA
 
 
 # make_napari_viewer is a pytest fixture that returns a napari viewer object
 @pytest.mark.parametrize("widget", [QtAdataViewWidget, QtAdataScatterWidget])
 def test_creating_widget_with_data(
     make_napari_viewer: Any,
     widget: Any,
```

### Comparing `napari-spatialdata-0.2.4/tests/test_scatterwidgets.py` & `napari-spatialdata-0.2.5/tests/test_scatterwidgets.py`

 * *Files identical despite different names*

### Comparing `napari-spatialdata-0.2.4/tox.ini` & `napari-spatialdata-0.2.5/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     windows: win32
 deps =
     pytest
     pytest-xdist
     pytest-cov
     pytest-qt
     pytest-mock
-    PyQt6
+    PyQt5
 passenv =
     CI
     GITHUB_ACTIONS
     DISPLAY
     XAUTHORITY
     NUMPY_EXPERIMENTAL_ARRAY_FUNCTION
     PYVISTA_OFF_SCREEN
```

