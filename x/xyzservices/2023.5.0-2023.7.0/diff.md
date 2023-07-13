# Comparing `tmp/xyzservices-2023.5.0.tar.gz` & `tmp/xyzservices-2023.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xyzservices-2023.5.0.tar", last modified: Fri May 19 20:50:17 2023, max compression
+gzip compressed data, was "xyzservices-2023.7.0.tar", last modified: Thu Jul 13 20:07:04 2023, max compression
```

## Comparing `xyzservices-2023.5.0.tar` & `xyzservices-2023.7.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:17.321644 xyzservices-2023.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:17.317644 xyzservices-2023.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:17.317644 xyzservices-2023.5.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/.github/PULL_REQUEST_TEMPLATE/community_contribution.md
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:17.317644 xyzservices-2023.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/.github/workflows/release_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/.github/workflows/update_providers.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-05-19 20:50:17.321644 xyzservices-2023.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:17.317644 xyzservices-2023.5.0/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/ci/latest.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/ci/update_providers.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:17.317644 xyzservices-2023.5.0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/doc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:17.317644 xyzservices-2023.5.0/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:17.317644 xyzservices-2023.5.0/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/doc/source/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    10052 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/doc/source/_static/generate_gallery.js
--rw-r--r--   0 runner    (1001) docker     (123)   380575 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/doc/source/_static/xyzmaps.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/doc/source/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/doc/source/gallery.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/doc/source/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    35770 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/doc/source/introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/doc/source/registration.md
--rw-r--r--   0 runner    (1001) docker     (123)   663316 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/doc/source/tiles.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:17.317644 xyzservices-2023.5.0/provider_sources/
--rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/provider_sources/_compress_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/provider_sources/_parse_leaflet_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)   144374 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/provider_sources/leaflet-providers-parsed.json
--rw-r--r--   0 runner    (1001) docker     (123)    25567 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/provider_sources/xyzservices-providers.json
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 20:50:17.321644 xyzservices-2023.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:17.317644 xyzservices-2023.5.0/xyzservices/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/xyzservices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:17.321644 xyzservices-2023.5.0/xyzservices/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/xyzservices/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   430664 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/xyzservices/data/providers.json
--rw-r--r--   0 runner    (1001) docker     (123)    21475 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/xyzservices/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/xyzservices/providers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:17.321644 xyzservices-2023.5.0/xyzservices/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/xyzservices/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/xyzservices/tests/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-05-19 20:50:10.000000 xyzservices-2023.5.0/xyzservices/tests/test_providers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 20:50:17.317644 xyzservices-2023.5.0/xyzservices.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-05-19 20:50:17.000000 xyzservices-2023.5.0/xyzservices.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-19 20:50:17.000000 xyzservices-2023.5.0/xyzservices.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 20:50:17.000000 xyzservices-2023.5.0/xyzservices.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-19 20:50:17.000000 xyzservices-2023.5.0/xyzservices.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:07:04.443049 xyzservices-2023.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:07:04.435048 xyzservices-2023.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:07:04.435048 xyzservices-2023.7.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/.github/PULL_REQUEST_TEMPLATE/community_contribution.md
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:07:04.435048 xyzservices-2023.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/.github/workflows/release_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/.github/workflows/update_providers.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-07-13 20:07:04.443049 xyzservices-2023.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:07:04.435048 xyzservices-2023.7.0/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/ci/latest.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/ci/update_providers.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:07:04.435048 xyzservices-2023.7.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:07:04.439048 xyzservices-2023.7.0/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:07:04.439048 xyzservices-2023.7.0/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/doc/source/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10052 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/doc/source/_static/generate_gallery.js
+-rw-r--r--   0 runner    (1001) docker     (123)   380575 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/doc/source/_static/xyzmaps.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/doc/source/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/doc/source/gallery.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/doc/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35770 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/doc/source/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/doc/source/registration.md
+-rw-r--r--   0 runner    (1001) docker     (123)   663316 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/doc/source/tiles.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:07:04.439048 xyzservices-2023.7.0/provider_sources/
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/provider_sources/_compress_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/provider_sources/_parse_leaflet_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)   143871 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/provider_sources/leaflet-providers-parsed.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25567 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/provider_sources/xyzservices-providers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 20:07:04.443049 xyzservices-2023.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:07:04.439048 xyzservices-2023.7.0/xyzservices/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/xyzservices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:07:04.439048 xyzservices-2023.7.0/xyzservices/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/xyzservices/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   432759 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/xyzservices/data/providers.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21475 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/xyzservices/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/xyzservices/providers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:07:04.443049 xyzservices-2023.7.0/xyzservices/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/xyzservices/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/xyzservices/tests/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/xyzservices/tests/test_providers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:07:04.439048 xyzservices-2023.7.0/xyzservices.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-07-13 20:07:04.000000 xyzservices-2023.7.0/xyzservices.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-13 20:07:04.000000 xyzservices-2023.7.0/xyzservices.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 20:07:04.000000 xyzservices-2023.7.0/xyzservices.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 20:07:04.000000 xyzservices-2023.7.0/xyzservices.egg-info/top_level.txt
```

### Comparing `xyzservices-2023.5.0/.github/PULL_REQUEST_TEMPLATE/community_contribution.md` & `xyzservices-2023.7.0/.github/PULL_REQUEST_TEMPLATE/community_contribution.md`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.5.0/.github/workflows/release_to_pypi.yml` & `xyzservices-2023.7.0/.github/workflows/release_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.5.0/.github/workflows/tests.yaml` & `xyzservices-2023.7.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.5.0/.github/workflows/update_providers.yaml` & `xyzservices-2023.7.0/.github/workflows/update_providers.yaml`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.5.0/.gitignore` & `xyzservices-2023.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.5.0/CHANGELOG.md` & `xyzservices-2023.7.0/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changelog
 =========
 
+xyzservices 2023.7.0 (July 13, 2023)
+------------------------------------
+
+Providers:
+
+- Added ``GeoportailFrance`` ``Orthoimagery_Orthophotos_Irc_express_2023`` and
+  ``Orthoimagery_Orthophotos_Ortho_express_2023`` layers
+- Updated domain for ``OpenStreetMap.DE``
+- Marked ``GeoportailFrance.Orthoimagery_Orthophotos_1980_1995`` as possibly broken
+
 xyzservices 2023.5.0 (May 19, 2023)
 -----------------------------------
 
 Providers:
 
 - Added ``OrdnanceSurvey`` layers
```

### Comparing `xyzservices-2023.5.0/CONTRIBUTING.md` & `xyzservices-2023.7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.5.0/LICENSE` & `xyzservices-2023.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.5.0/PKG-INFO` & `xyzservices-2023.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xyzservices
-Version: 2023.5.0
+Version: 2023.7.0
 Summary: Source of XYZ tiles providers
 Home-page: https://github.com/geopandas/xyzservices
 Author: Dani Arribas-Bel, Martin Fleischmann
 Author-email: daniel.arribas.bel@gmail.com, martin@martinfleischmann.net
 License: 3-Clause BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `xyzservices-2023.5.0/README.md` & `xyzservices-2023.7.0/README.md`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.5.0/doc/Makefile` & `xyzservices-2023.7.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.5.0/doc/make.bat` & `xyzservices-2023.7.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.5.0/doc/source/_static/custom.css` & `xyzservices-2023.7.0/doc/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.5.0/doc/source/_static/generate_gallery.js` & `xyzservices-2023.7.0/doc/source/_static/generate_gallery.js`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.5.0/doc/source/_static/xyzmaps.jpg` & `xyzservices-2023.7.0/doc/source/_static/xyzmaps.jpg`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.5.0/doc/source/api.rst` & `xyzservices-2023.7.0/doc/source/api.rst`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.5.0/doc/source/conf.py` & `xyzservices-2023.7.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.5.0/doc/source/contributing.md` & `xyzservices-2023.7.0/doc/source/contributing.md`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.5.0/doc/source/gallery.rst` & `xyzservices-2023.7.0/doc/source/gallery.rst`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.5.0/doc/source/index.md` & `xyzservices-2023.7.0/doc/source/index.md`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.5.0/doc/source/introduction.ipynb` & `xyzservices-2023.7.0/doc/source/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.5.0/doc/source/registration.md` & `xyzservices-2023.7.0/doc/source/registration.md`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.5.0/doc/source/tiles.png` & `xyzservices-2023.7.0/doc/source/tiles.png`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.5.0/provider_sources/_compress_providers.py` & `xyzservices-2023.7.0/provider_sources/_compress_providers.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,14 +188,15 @@
                 "Ocsge_Couverture_2002",
                 "Ocsge_Couverture_2014",
                 "Ocsge_Usage_2002",
                 "Ocsge_Usage_2014",
                 "Orthoimagery_Orthophotos_Coast2000",
                 "Pcrs_Lamb93",
                 "Orthoimagery_Ortho_sat_Spot_2013",
+                "Orthoimagery_Orthophotos_1980_1995",
             ]
 
             if name in possibly_broken:
                 leaflet["GeoportailFrance"][name]["status"] = "broken"
 
 with open("../xyzservices/data/providers.json", "w") as f:
     json.dump(leaflet, f, indent=4)
```

### Comparing `xyzservices-2023.5.0/provider_sources/_parse_leaflet_providers.py` & `xyzservices-2023.7.0/provider_sources/_parse_leaflet_providers.py`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.5.0/provider_sources/leaflet-providers-parsed.json` & `xyzservices-2023.7.0/provider_sources/leaflet-providers-parsed.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9955043859649124%*

 * *Differences: {"'OpenStreetMap'": "{'DE': {'url': 'https://tile.openstreetmap.de/{z}/{x}/{y}.png'}}",*

 * * "'_meta'": "{'date_of_creation': '2023-07-13', 'commit': 'commit "*

 * *            "15b5c38a104a6e71f69b4ab48ea5b0b13835d5d2 (openstreetmap.de)'}"}*

```diff
@@ -2269,15 +2269,15 @@
             "url": "https://tile.osm.ch/switzerland/{z}/{x}/{y}.png"
         },
         "DE": {
             "attribution": "(C) OpenStreetMap contributors",
             "html_attribution": "&copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
             "max_zoom": 18,
             "name": "OpenStreetMap.DE",
-            "url": "https://{s}.tile.openstreetmap.de/{z}/{x}/{y}.png"
+            "url": "https://tile.openstreetmap.de/{z}/{x}/{y}.png"
         },
         "France": {
             "attribution": "(C) OpenStreetMap France | (C) OpenStreetMap contributors",
             "html_attribution": "&copy; OpenStreetMap France | &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
             "max_zoom": 20,
             "name": "OpenStreetMap.France",
             "url": "https://{s}.tile.openstreetmap.fr/osmfr/{z}/{x}/{y}.png"
@@ -2858,16 +2858,16 @@
             "max_zoom": 18,
             "name": "WaymarkedTrails.slopes",
             "url": "https://tile.waymarkedtrails.org/{variant}/{z}/{x}/{y}.png",
             "variant": "slopes"
         }
     },
     "_meta": {
-        "commit": "commit 79c2a213e6373d6871d2edabf69ecae25dc9e0f7 (Bump eslint from 8.38.0 to 8.39.0\n\nBumps [eslint](https://github.com/eslint/eslint) from 8.38.0 to 8.39.0.\n- [Release notes](https://github.com/eslint/eslint/releases)\n- [Changelog](https://github.com/eslint/eslint/blob/main/CHANGELOG.md)\n- [Commits](https://github.com/eslint/eslint/compare/v8.38.0...v8.39.0)\n\n---\nupdated-dependencies:\n- dependency-name: eslint\n  dependency-type: direct:development\n  update-type: version-update:semver-minor\n...\n\nSigned-off-by: dependabot[bot] <support@github.com>)",
-        "date_of_creation": "2023-05-15",
+        "commit": "commit 15b5c38a104a6e71f69b4ab48ea5b0b13835d5d2 (openstreetmap.de)",
+        "date_of_creation": "2023-07-13",
         "description": "JSON representation of the leaflet providers defined by the leaflet-providers.js extension to Leaflet (https://github.com/leaflet-extras/leaflet-providers)"
     },
     "nlmaps": {
         "grijs": {
             "attribution": "Kaartgegevens (C) Kadaster",
             "bounds": [
                 [
```

### Comparing `xyzservices-2023.5.0/provider_sources/xyzservices-providers.json` & `xyzservices-2023.7.0/provider_sources/xyzservices-providers.json`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.5.0/setup.py` & `xyzservices-2023.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.5.0/xyzservices/data/providers.json` & `xyzservices-2023.7.0/xyzservices/data/providers.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999811071462363%*

 * *Differences: {"'GeoportailFrance'": "{'Orthoimagery_Orthophotos_Irc_express_2022': {'apikey': 'orthohisto'}, "*

 * *                       "'Orthoimagery_Orthophotos_Ortho_express_2022': {'apikey': 'orthohisto'}, "*

 * *                       "'Orthoimagery_Orthophotos_1980_1995': {'bounds': [[41.3125, -2.37153], "*

 * *                       "[49.7785, 9.67536]], 'style': 'BDORTHOHISTORIQUE', 'status': 'broken'}, "*

 * *                       "'Orthoimagery_Ortho_sat_Pleiades_2022': {'bounds': {0: {insert: [(1, "*

 * *                       '- […]*

```diff
@@ -668,15 +668,15 @@
         },
         "Bdcarto_etat_major_Niveau3": {
             "TileMatrixSet": "PM",
             "apikey": "sol",
             "attribution": "Geoportail France",
             "bounds": [
                 [
-                    43.151,
+                    42.6423,
                     -5.15012
                 ],
                 [
                     51.0938,
                     7.19384
                 ]
             ],
@@ -4194,24 +4194,24 @@
         "Orthoimagery_Ortho_sat_Pleiades_2022": {
             "TileMatrixSet": "PM",
             "apikey": "satellite",
             "attribution": "Geoportail France",
             "bounds": [
                 [
                     -21.3733,
-                    -61.6648
+                    -67.7132
                 ],
                 [
-                    51.1117,
+                    69.3108,
                     55.7216
                 ]
             ],
             "format": "image/png",
             "html_attribution": "<a target=\"_blank\"href=\"https://www.geoportail.gouv.fr/\">Geoportail France</a>",
-            "max_zoom": 19,
+            "max_zoom": 18,
             "min_zoom": 0,
             "name": "GeoportailFrance.Orthoimagery_Ortho_sat_Pleiades_2022",
             "style": "normal",
             "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
             "variant": "ORTHOIMAGERY.ORTHO-SAT.PLEIADES.2022"
         },
         "Orthoimagery_Ortho_sat_Rapideye_2010": {
@@ -5068,28 +5068,29 @@
         },
         "Orthoimagery_Orthophotos_1980_1995": {
             "TileMatrixSet": "PM",
             "apikey": "orthohisto",
             "attribution": "Geoportail France",
             "bounds": [
                 [
-                    41.2761,
-                    8.37634
+                    41.3125,
+                    -2.37153
                 ],
                 [
-                    43.0899,
-                    9.72525
+                    49.7785,
+                    9.67536
                 ]
             ],
             "format": "image/png",
             "html_attribution": "<a target=\"_blank\"href=\"https://www.geoportail.gouv.fr/\">Geoportail France</a>",
             "max_zoom": 18,
             "min_zoom": 3,
             "name": "GeoportailFrance.Orthoimagery_Orthophotos_1980_1995",
-            "style": "normal",
+            "status": "broken",
+            "style": "BDORTHOHISTORIQUE",
             "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
             "variant": "ORTHOIMAGERY.ORTHOPHOTOS.1980-1995"
         },
         "Orthoimagery_Orthophotos_Bdortho": {
             "TileMatrixSet": "PM",
             "apikey": "ortho",
             "attribution": "Geoportail France",
@@ -5387,15 +5388,15 @@
             "name": "GeoportailFrance.Orthoimagery_Orthophotos_Irc_express_2021",
             "style": "normal",
             "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
             "variant": "ORTHOIMAGERY.ORTHOPHOTOS.IRC-EXPRESS.2021"
         },
         "Orthoimagery_Orthophotos_Irc_express_2022": {
             "TileMatrixSet": "PM",
-            "apikey": "ortho",
+            "apikey": "orthohisto",
             "attribution": "Geoportail France",
             "bounds": [
                 [
                     -75.0,
                     -179.5
                 ],
                 [
@@ -5408,14 +5409,37 @@
             "max_zoom": 19,
             "min_zoom": 0,
             "name": "GeoportailFrance.Orthoimagery_Orthophotos_Irc_express_2022",
             "style": "normal",
             "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
             "variant": "ORTHOIMAGERY.ORTHOPHOTOS.IRC-EXPRESS.2022"
         },
+        "Orthoimagery_Orthophotos_Irc_express_2023": {
+            "TileMatrixSet": "PM",
+            "apikey": "ortho",
+            "attribution": "Geoportail France",
+            "bounds": [
+                [
+                    47.4719,
+                    1.48832
+                ],
+                [
+                    48.3543,
+                    3.13499
+                ]
+            ],
+            "format": "image/jpeg",
+            "html_attribution": "<a target=\"_blank\"href=\"https://www.geoportail.gouv.fr/\">Geoportail France</a>",
+            "max_zoom": 19,
+            "min_zoom": 0,
+            "name": "GeoportailFrance.Orthoimagery_Orthophotos_Irc_express_2023",
+            "style": "normal",
+            "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
+            "variant": "ORTHOIMAGERY.ORTHOPHOTOS.IRC-EXPRESS.2023"
+        },
         "Orthoimagery_Orthophotos_Ortho_asp_pac2020": {
             "TileMatrixSet": "PM",
             "apikey": "orthohisto",
             "attribution": "Geoportail France",
             "bounds": [
                 [
                     -75.0,
@@ -5525,15 +5549,15 @@
             "name": "GeoportailFrance.Orthoimagery_Orthophotos_Ortho_express_2021",
             "style": "normal",
             "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
             "variant": "ORTHOIMAGERY.ORTHOPHOTOS.ORTHO-EXPRESS.2021"
         },
         "Orthoimagery_Orthophotos_Ortho_express_2022": {
             "TileMatrixSet": "PM",
-            "apikey": "ortho",
+            "apikey": "orthohisto",
             "attribution": "Geoportail France",
             "bounds": [
                 [
                     -75.0,
                     -179.5
                 ],
                 [
@@ -5546,14 +5570,37 @@
             "max_zoom": 19,
             "min_zoom": 0,
             "name": "GeoportailFrance.Orthoimagery_Orthophotos_Ortho_express_2022",
             "style": "normal",
             "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
             "variant": "ORTHOIMAGERY.ORTHOPHOTOS.ORTHO-EXPRESS.2022"
         },
+        "Orthoimagery_Orthophotos_Ortho_express_2023": {
+            "TileMatrixSet": "PM",
+            "apikey": "ortho",
+            "attribution": "Geoportail France",
+            "bounds": [
+                [
+                    47.4719,
+                    1.48832
+                ],
+                [
+                    48.3543,
+                    3.13499
+                ]
+            ],
+            "format": "image/jpeg",
+            "html_attribution": "<a target=\"_blank\"href=\"https://www.geoportail.gouv.fr/\">Geoportail France</a>",
+            "max_zoom": 19,
+            "min_zoom": 0,
+            "name": "GeoportailFrance.Orthoimagery_Orthophotos_Ortho_express_2023",
+            "style": "normal",
+            "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
+            "variant": "ORTHOIMAGERY.ORTHOPHOTOS.ORTHO-EXPRESS.2023"
+        },
         "Orthoimagery_Orthophotos_Socle_asp_2018": {
             "TileMatrixSet": "PM",
             "apikey": "orthohisto",
             "attribution": "Geoportail France",
             "bounds": [
                 [
                     -75.0,
@@ -8654,15 +8701,15 @@
             "url": "https://tile.osm.ch/switzerland/{z}/{x}/{y}.png"
         },
         "DE": {
             "attribution": "(C) OpenStreetMap contributors",
             "html_attribution": "&copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
             "max_zoom": 18,
             "name": "OpenStreetMap.DE",
-            "url": "https://{s}.tile.openstreetmap.de/{z}/{x}/{y}.png"
+            "url": "https://tile.openstreetmap.de/{z}/{x}/{y}.png"
         },
         "France": {
             "attribution": "(C) OpenStreetMap France | (C) OpenStreetMap contributors",
             "html_attribution": "&copy; OpenStreetMap France | &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
             "max_zoom": 20,
             "name": "OpenStreetMap.France",
             "url": "https://{s}.tile.openstreetmap.fr/osmfr/{z}/{x}/{y}.png"
```

### Comparing `xyzservices-2023.5.0/xyzservices/lib.py` & `xyzservices-2023.7.0/xyzservices/lib.py`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.5.0/xyzservices/tests/test_lib.py` & `xyzservices-2023.7.0/xyzservices/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.5.0/xyzservices/tests/test_providers.py` & `xyzservices-2023.7.0/xyzservices/tests/test_providers.py`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.5.0/xyzservices.egg-info/PKG-INFO` & `xyzservices-2023.7.0/xyzservices.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xyzservices
-Version: 2023.5.0
+Version: 2023.7.0
 Summary: Source of XYZ tiles providers
 Home-page: https://github.com/geopandas/xyzservices
 Author: Dani Arribas-Bel, Martin Fleischmann
 Author-email: daniel.arribas.bel@gmail.com, martin@martinfleischmann.net
 License: 3-Clause BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `xyzservices-2023.5.0/xyzservices.egg-info/SOURCES.txt` & `xyzservices-2023.7.0/xyzservices.egg-info/SOURCES.txt`

 * *Files identical despite different names*

