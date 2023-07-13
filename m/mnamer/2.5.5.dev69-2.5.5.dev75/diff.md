# Comparing `tmp/mnamer-2.5.5.dev69.tar.gz` & `tmp/mnamer-2.5.5.dev75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnamer-2.5.5.dev69.tar", last modified: Thu Jan 12 18:03:03 2023, max compression
+gzip compressed data, was "mnamer-2.5.5.dev75.tar", last modified: Thu Jul 13 17:06:14 2023, max compression
```

## Comparing `mnamer-2.5.5.dev69.tar` & `mnamer-2.5.5.dev75.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 18:03:03.651792 mnamer-2.5.5.dev69/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 18:03:03.627792 mnamer-2.5.5.dev69/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 18:03:03.623792 mnamer-2.5.5.dev69/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 18:03:03.627792 mnamer-2.5.5.dev69/.github/actions/init/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/.github/actions/init/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 18:03:03.627792 mnamer-2.5.5.dev69/.github/actions/lint/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/.github/actions/lint/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 18:03:03.627792 mnamer-2.5.5.dev69/.github/actions/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/.github/actions/test/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 18:03:03.627792 mnamer-2.5.5.dev69/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/.github/workflows/pull_request.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/.python-version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 18:03:03.627792 mnamer-2.5.5.dev69/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-01-12 18:03:03.651792 mnamer-2.5.5.dev69/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 18:03:03.639792 mnamer-2.5.5.dev69/assets/
--rw-r--r--   0 runner    (1001) docker     (123)  1074066 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/assets/design.eps
--rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/assets/logo-2.png
--rw-r--r--   0 runner    (1001) docker     (123)    11154 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/assets/logo-3.png
--rw-r--r--   0 runner    (1001) docker     (123)    15178 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/assets/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)  4765533 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/assets/recording.mov
--rw-r--r--   0 runner    (1001) docker     (123)  3269286 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/assets/screenshot.eps
--rw-r--r--   0 runner    (1001) docker     (123)    42324 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/assets/screenshot.png
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 18:03:03.643792 mnamer-2.5.5.dev69/mnamer/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/mnamer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/mnamer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-01-12 18:03:03.000000 mnamer-2.5.5.dev69/mnamer/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/mnamer/argument.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/mnamer/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    19376 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/mnamer/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/mnamer/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/mnamer/frontends.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/mnamer/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/mnamer/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    17562 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/mnamer/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/mnamer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/mnamer/setting_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    16022 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/mnamer/setting_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     9206 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/mnamer/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/mnamer/tty.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/mnamer/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    14824 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/mnamer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 18:03:03.647792 mnamer-2.5.5.dev69/mnamer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-01-12 18:03:03.000000 mnamer-2.5.5.dev69/mnamer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-01-12 18:03:03.000000 mnamer-2.5.5.dev69/mnamer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 18:03:03.000000 mnamer-2.5.5.dev69/mnamer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-12 18:03:03.000000 mnamer-2.5.5.dev69/mnamer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-01-12 18:03:03.000000 mnamer-2.5.5.dev69/mnamer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-12 18:03:03.000000 mnamer-2.5.5.dev69/mnamer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 18:03:03.651792 mnamer-2.5.5.dev69/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 18:03:03.647792 mnamer-2.5.5.dev69/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 18:03:03.647792 mnamer-2.5.5.dev69/tests/e2e/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/tests/e2e/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/tests/e2e/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/tests/e2e/test_directives.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/tests/e2e/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/tests/e2e/test_moving.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 18:03:03.647792 mnamer-2.5.5.dev69/tests/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/tests/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/tests/local/test_argument.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/tests/local/test_language.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/tests/local/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/tests/local/test_setting_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/tests/local/test_setting_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/tests/local/test_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/tests/local/test_tty.py
--rw-r--r--   0 runner    (1001) docker     (123)    25741 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/tests/local/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 18:03:03.651792 mnamer-2.5.5.dev69/tests/network/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/tests/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/tests/network/test_endpoints__omdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/tests/network/test_endpoints__tmdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/tests/network/test_endpoints__tvdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/tests/network/test_endpoints__tvmaze.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/tests/network/test_providers__omdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/tests/network/test_providers__tmdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/tests/network/test_providers__tvdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-01-12 18:02:35.000000 mnamer-2.5.5.dev69/tests/network/test_providers__tvmaze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:14.466650 mnamer-2.5.5.dev75/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:14.450650 mnamer-2.5.5.dev75/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:14.446650 mnamer-2.5.5.dev75/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:14.450650 mnamer-2.5.5.dev75/.github/actions/init/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/.github/actions/init/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:14.450650 mnamer-2.5.5.dev75/.github/actions/lint/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/.github/actions/lint/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:14.450650 mnamer-2.5.5.dev75/.github/actions/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/.github/actions/test/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:14.450650 mnamer-2.5.5.dev75/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/.github/workflows/pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/.python-version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:14.450650 mnamer-2.5.5.dev75/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-07-13 17:06:14.466650 mnamer-2.5.5.dev75/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:14.458650 mnamer-2.5.5.dev75/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)  1074066 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/assets/design.eps
+-rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/assets/logo-2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11154 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/assets/logo-3.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15178 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/assets/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)  4765533 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/assets/recording.mov
+-rw-r--r--   0 runner    (1001) docker     (123)  3269286 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/assets/screenshot.eps
+-rw-r--r--   0 runner    (1001) docker     (123)    42324 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/assets/screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:14.462650 mnamer-2.5.5.dev75/mnamer/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/mnamer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/mnamer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-13 17:06:14.000000 mnamer-2.5.5.dev75/mnamer/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/mnamer/argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/mnamer/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19376 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/mnamer/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/mnamer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/mnamer/frontends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/mnamer/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/mnamer/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17416 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/mnamer/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/mnamer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/mnamer/setting_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16022 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/mnamer/setting_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9206 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/mnamer/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/mnamer/tty.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/mnamer/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14824 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/mnamer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:14.462650 mnamer-2.5.5.dev75/mnamer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-07-13 17:06:14.000000 mnamer-2.5.5.dev75/mnamer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-13 17:06:14.000000 mnamer-2.5.5.dev75/mnamer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:06:14.000000 mnamer-2.5.5.dev75/mnamer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-13 17:06:14.000000 mnamer-2.5.5.dev75/mnamer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-13 17:06:14.000000 mnamer-2.5.5.dev75/mnamer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-13 17:06:14.000000 mnamer-2.5.5.dev75/mnamer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 17:06:14.466650 mnamer-2.5.5.dev75/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:14.462650 mnamer-2.5.5.dev75/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:14.462650 mnamer-2.5.5.dev75/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/tests/e2e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/tests/e2e/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/tests/e2e/test_directives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/tests/e2e/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/tests/e2e/test_moving.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:14.466650 mnamer-2.5.5.dev75/tests/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/tests/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/tests/local/test_argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/tests/local/test_language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/tests/local/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/tests/local/test_setting_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/tests/local/test_setting_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/tests/local/test_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/tests/local/test_tty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25741 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/tests/local/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:06:14.466650 mnamer-2.5.5.dev75/tests/network/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/tests/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/tests/network/test_endpoints__omdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/tests/network/test_endpoints__tmdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/tests/network/test_endpoints__tvdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/tests/network/test_endpoints__tvmaze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/tests/network/test_providers__omdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/tests/network/test_providers__tmdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/tests/network/test_providers__tvdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-07-13 17:05:52.000000 mnamer-2.5.5.dev75/tests/network/test_providers__tvmaze.py
```

### Comparing `mnamer-2.5.5.dev69/.github/actions/lint/action.yml` & `mnamer-2.5.5.dev75/.github/actions/lint/action.yml`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/.github/actions/test/action.yml` & `mnamer-2.5.5.dev75/.github/actions/test/action.yml`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/.github/workflows/pull_request.yml` & `mnamer-2.5.5.dev75/.github/workflows/pull_request.yml`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/.github/workflows/push.yml` & `mnamer-2.5.5.dev75/.github/workflows/push.yml`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/LICENSE.txt` & `mnamer-2.5.5.dev75/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/PKG-INFO` & `mnamer-2.5.5.dev75/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnamer
-Version: 2.5.5.dev69
+Version: 2.5.5.dev75
 Summary: A command-line utility for organizing media files.
 Author-email: Jessy Williams <jessy@jessywilliams.com>
 Maintainer-email: Jessy Williams <jessy@jessywilliams.com>
 License: MIT License
         
         Copyright (c) 2017 Jessy Williams
```

### Comparing `mnamer-2.5.5.dev69/README.md` & `mnamer-2.5.5.dev75/README.md`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/assets/design.eps` & `mnamer-2.5.5.dev75/assets/design.eps`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/assets/logo-2.png` & `mnamer-2.5.5.dev75/assets/logo-2.png`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/assets/logo-3.png` & `mnamer-2.5.5.dev75/assets/logo-3.png`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/assets/logo.png` & `mnamer-2.5.5.dev75/assets/logo.png`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/assets/recording.mov` & `mnamer-2.5.5.dev75/assets/recording.mov`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/assets/screenshot.eps` & `mnamer-2.5.5.dev75/assets/screenshot.eps`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/assets/screenshot.png` & `mnamer-2.5.5.dev75/assets/screenshot.png`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/makefile` & `mnamer-2.5.5.dev75/makefile`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/mnamer/__main__.py` & `mnamer-2.5.5.dev75/mnamer/__main__.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/mnamer/argument.py` & `mnamer-2.5.5.dev75/mnamer/argument.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/mnamer/const.py` & `mnamer-2.5.5.dev75/mnamer/const.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/mnamer/endpoints.py` & `mnamer-2.5.5.dev75/mnamer/endpoints.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/mnamer/exceptions.py` & `mnamer-2.5.5.dev75/mnamer/exceptions.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/mnamer/frontends.py` & `mnamer-2.5.5.dev75/mnamer/frontends.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/mnamer/language.py` & `mnamer-2.5.5.dev75/mnamer/language.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/mnamer/metadata.py` & `mnamer-2.5.5.dev75/mnamer/metadata.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/mnamer/providers.py` & `mnamer-2.5.5.dev75/mnamer/providers.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,23 +170,22 @@
             synopsis=response["overview"],
             id_tmdb=response["id"],
             id_imdb=response["imdb_id"],
         )
 
     def _search_name(self, name: str, year: str | None, language: Language | None):
         assert self.api_key
-        year_from, year_to = year_range_parse(year, 5)
         page = 1
         page_max = 5  # each page yields a maximum of 20 results
         found = False
         while True:
             response = tmdb_search_movies(
                 self.api_key,
                 name,
-                f"{year_from}-{year_to}",
+                year,
                 language,
                 page=page,
                 cache=self.cache,
             )
             for entry in response["results"]:
                 try:
                     meta = MetadataMovie(
@@ -194,17 +193,16 @@
                         name=entry["title"],
                         language=language,
                         synopsis=entry["overview"],
                         year=entry["release_date"],
                     )
                     if not meta.year:
                         continue
-                    if year_from <= int(meta.year) <= year_to:
-                        yield meta
-                        found = True
+                    yield meta
+                    found = True
                 except (AttributeError, KeyError, TypeError, ValueError):
                     continue
             if page == response["total_pages"]:
                 break
             elif page >= page_max:
                 break
             page += 1
```

### Comparing `mnamer-2.5.5.dev69/mnamer/setting_spec.py` & `mnamer-2.5.5.dev75/mnamer/setting_spec.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/mnamer/setting_store.py` & `mnamer-2.5.5.dev75/mnamer/setting_store.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/mnamer/target.py` & `mnamer-2.5.5.dev75/mnamer/target.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/mnamer/tty.py` & `mnamer-2.5.5.dev75/mnamer/tty.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/mnamer/types.py` & `mnamer-2.5.5.dev75/mnamer/types.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/mnamer/utils.py` & `mnamer-2.5.5.dev75/mnamer/utils.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/mnamer.egg-info/PKG-INFO` & `mnamer-2.5.5.dev75/mnamer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnamer
-Version: 2.5.5.dev69
+Version: 2.5.5.dev75
 Summary: A command-line utility for organizing media files.
 Author-email: Jessy Williams <jessy@jessywilliams.com>
 Maintainer-email: Jessy Williams <jessy@jessywilliams.com>
 License: MIT License
         
         Copyright (c) 2017 Jessy Williams
```

### Comparing `mnamer-2.5.5.dev69/mnamer.egg-info/SOURCES.txt` & `mnamer-2.5.5.dev75/mnamer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/pyproject.toml` & `mnamer-2.5.5.dev75/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/tests/__init__.py` & `mnamer-2.5.5.dev75/tests/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,20 +74,20 @@
         "season": 2,
         "series": "Fargo",
         "title": "Before the Law",
     },
 }
 
 MOVIE_META = {
-    "The Goonies": {
-        "id_imdb": "tt0089218",
-        "id_tmdb": 9340,
+    "Idiocracy": {
+        "id_imdb": "tt0387808",
+        "id_tmdb": 7512,
         "media": "movie",
-        "name": "The Goonies",
-        "year": 1985,
+        "name": "Idiocracy",
+        "year": 2006,
     },
     "Citizen Kane": {
         "id_imdb": "tt0033467",
         "id_tmdb": 15,
         "media": "movie",
         "name": "Citizen Kane",
         "year": 1941,
```

### Comparing `mnamer-2.5.5.dev69/tests/conftest.py` & `mnamer-2.5.5.dev75/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/tests/e2e/conftest.py` & `mnamer-2.5.5.dev75/tests/e2e/conftest.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/tests/e2e/test_directives.py` & `mnamer-2.5.5.dev75/tests/e2e/test_directives.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/tests/e2e/test_errors.py` & `mnamer-2.5.5.dev75/tests/e2e/test_errors.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/tests/e2e/test_moving.py` & `mnamer-2.5.5.dev75/tests/e2e/test_moving.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,25 +7,14 @@
 pytestmark = [
     pytest.mark.e2e,
     pytest.mark.flaky(reruns=2, reruns_delay=5),
 ]
 
 
 @pytest.mark.usefixtures("setup_test_dir")
-def test_complex_metadata(e2e_run, setup_test_files):
-    setup_test_files(
-        "Quien a hierro mata [MicroHD 1080p][DTS 5.1-Castellano-AC3 5.1-Castellano+Subs][ES-EN].mkv"
-    )
-    result = e2e_run("--batch", "--media=movie", ".")
-    assert result.code == 0
-    assert "Quien a Hierro Mata (2019).mkv" in result.out
-    assert "1 out of 1 files processed successfully" in result.out
-
-
-@pytest.mark.usefixtures("setup_test_dir")
 def test_absolute_path(e2e_run, setup_test_files):
     setup_test_files("kill.bill.vol.1.mkv")
     result = e2e_run("--batch", "--media=movie", "kill.bill.vol.1.mkv")
     assert result.code == 0
     assert "Kill Bill Vol. 1 (2003).mkv" in result.out
     assert "1 out of 1 files processed successfully" in result.out
```

### Comparing `mnamer-2.5.5.dev69/tests/local/test_argument.py` & `mnamer-2.5.5.dev75/tests/local/test_argument.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/tests/local/test_language.py` & `mnamer-2.5.5.dev75/tests/local/test_language.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/tests/local/test_metadata.py` & `mnamer-2.5.5.dev75/tests/local/test_metadata.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/tests/local/test_setting_spec.py` & `mnamer-2.5.5.dev75/tests/local/test_setting_spec.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/tests/local/test_setting_store.py` & `mnamer-2.5.5.dev75/tests/local/test_setting_store.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/tests/local/test_target.py` & `mnamer-2.5.5.dev75/tests/local/test_target.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/tests/local/test_tty.py` & `mnamer-2.5.5.dev75/tests/local/test_tty.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/tests/local/test_utils.py` & `mnamer-2.5.5.dev75/tests/local/test_utils.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/tests/network/test_endpoints__omdb.py` & `mnamer-2.5.5.dev75/tests/network/test_endpoints__omdb.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/tests/network/test_endpoints__tmdb.py` & `mnamer-2.5.5.dev75/tests/network/test_endpoints__tmdb.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/tests/network/test_endpoints__tvdb.py` & `mnamer-2.5.5.dev75/tests/network/test_endpoints__tvdb.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/tests/network/test_endpoints__tvmaze.py` & `mnamer-2.5.5.dev75/tests/network/test_endpoints__tvmaze.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/tests/network/test_providers__omdb.py` & `mnamer-2.5.5.dev75/tests/network/test_providers__omdb.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/tests/network/test_providers__tmdb.py` & `mnamer-2.5.5.dev75/tests/network/test_providers__tmdb.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/tests/network/test_providers__tvdb.py` & `mnamer-2.5.5.dev75/tests/network/test_providers__tvdb.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev69/tests/network/test_providers__tvmaze.py` & `mnamer-2.5.5.dev75/tests/network/test_providers__tvmaze.py`

 * *Files identical despite different names*

