# Comparing `tmp/mnamer-2.5.5.dev77.tar.gz` & `tmp/mnamer-2.5.5.dev79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnamer-2.5.5.dev77.tar", last modified: Thu Jul 13 17:12:18 2023, max compression
+gzip compressed data, was "mnamer-2.5.5.dev79.tar", last modified: Thu Jul 13 17:11:45 2023, max compression
```

## Comparing `mnamer-2.5.5.dev77.tar` & `mnamer-2.5.5.dev79.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:12:18.325663 mnamer-2.5.5.dev77/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:12:18.297663 mnamer-2.5.5.dev77/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:12:18.297663 mnamer-2.5.5.dev77/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:12:18.301663 mnamer-2.5.5.dev77/.github/actions/init/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/.github/actions/init/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:12:18.301663 mnamer-2.5.5.dev77/.github/actions/lint/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/.github/actions/lint/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:12:18.301663 mnamer-2.5.5.dev77/.github/actions/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/.github/actions/test/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:12:18.301663 mnamer-2.5.5.dev77/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/.github/workflows/pull_request.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/.python-version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:12:18.301663 mnamer-2.5.5.dev77/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-07-13 17:12:18.325663 mnamer-2.5.5.dev77/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:12:18.313663 mnamer-2.5.5.dev77/assets/
--rw-r--r--   0 runner    (1001) docker     (123)  1074066 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/assets/design.eps
--rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/assets/logo-2.png
--rw-r--r--   0 runner    (1001) docker     (123)    11154 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/assets/logo-3.png
--rw-r--r--   0 runner    (1001) docker     (123)    15178 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/assets/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)  4765533 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/assets/recording.mov
--rw-r--r--   0 runner    (1001) docker     (123)  3269286 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/assets/screenshot.eps
--rw-r--r--   0 runner    (1001) docker     (123)    42324 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/assets/screenshot.png
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:12:18.317663 mnamer-2.5.5.dev77/mnamer/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/mnamer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/mnamer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-13 17:12:17.000000 mnamer-2.5.5.dev77/mnamer/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/mnamer/argument.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/mnamer/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    19376 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/mnamer/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/mnamer/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/mnamer/frontends.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/mnamer/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/mnamer/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    17416 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/mnamer/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/mnamer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/mnamer/setting_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    16022 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/mnamer/setting_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     9206 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/mnamer/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/mnamer/tty.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/mnamer/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    14824 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/mnamer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:12:18.321663 mnamer-2.5.5.dev77/mnamer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-07-13 17:12:18.000000 mnamer-2.5.5.dev77/mnamer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-13 17:12:18.000000 mnamer-2.5.5.dev77/mnamer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:12:18.000000 mnamer-2.5.5.dev77/mnamer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-13 17:12:18.000000 mnamer-2.5.5.dev77/mnamer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-13 17:12:18.000000 mnamer-2.5.5.dev77/mnamer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-13 17:12:18.000000 mnamer-2.5.5.dev77/mnamer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 17:12:18.325663 mnamer-2.5.5.dev77/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:12:18.321663 mnamer-2.5.5.dev77/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:12:18.321663 mnamer-2.5.5.dev77/tests/e2e/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/tests/e2e/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/tests/e2e/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/tests/e2e/test_directives.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/tests/e2e/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/tests/e2e/test_moving.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:12:18.325663 mnamer-2.5.5.dev77/tests/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/tests/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/tests/local/test_argument.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/tests/local/test_language.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/tests/local/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/tests/local/test_setting_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/tests/local/test_setting_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/tests/local/test_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/tests/local/test_tty.py
--rw-r--r--   0 runner    (1001) docker     (123)    25741 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/tests/local/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:12:18.325663 mnamer-2.5.5.dev77/tests/network/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/tests/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/tests/network/test_endpoints__omdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/tests/network/test_endpoints__tmdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/tests/network/test_endpoints__tvdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/tests/network/test_endpoints__tvmaze.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/tests/network/test_providers__omdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/tests/network/test_providers__tmdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/tests/network/test_providers__tvdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-07-13 17:11:47.000000 mnamer-2.5.5.dev77/tests/network/test_providers__tvmaze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:45.257692 mnamer-2.5.5.dev79/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:45.241692 mnamer-2.5.5.dev79/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:45.237692 mnamer-2.5.5.dev79/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:45.241692 mnamer-2.5.5.dev79/.github/actions/init/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/.github/actions/init/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:45.241692 mnamer-2.5.5.dev79/.github/actions/lint/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/.github/actions/lint/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:45.241692 mnamer-2.5.5.dev79/.github/actions/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/.github/actions/test/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:45.241692 mnamer-2.5.5.dev79/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/.github/workflows/pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/.python-version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:45.241692 mnamer-2.5.5.dev79/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-07-13 17:11:45.257692 mnamer-2.5.5.dev79/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:45.253692 mnamer-2.5.5.dev79/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)  1074066 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/assets/design.eps
+-rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/assets/logo-2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11154 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/assets/logo-3.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15178 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/assets/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)  4765533 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/assets/recording.mov
+-rw-r--r--   0 runner    (1001) docker     (123)  3269286 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/assets/screenshot.eps
+-rw-r--r--   0 runner    (1001) docker     (123)    42324 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/assets/screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:45.253692 mnamer-2.5.5.dev79/mnamer/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/mnamer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/mnamer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-13 17:11:44.000000 mnamer-2.5.5.dev79/mnamer/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/mnamer/argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/mnamer/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19376 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/mnamer/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/mnamer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/mnamer/frontends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/mnamer/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/mnamer/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17416 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/mnamer/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/mnamer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/mnamer/setting_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16022 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/mnamer/setting_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9206 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/mnamer/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/mnamer/tty.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/mnamer/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14824 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/mnamer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:45.253692 mnamer-2.5.5.dev79/mnamer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-07-13 17:11:45.000000 mnamer-2.5.5.dev79/mnamer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-13 17:11:45.000000 mnamer-2.5.5.dev79/mnamer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:11:45.000000 mnamer-2.5.5.dev79/mnamer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-13 17:11:45.000000 mnamer-2.5.5.dev79/mnamer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-13 17:11:45.000000 mnamer-2.5.5.dev79/mnamer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-13 17:11:45.000000 mnamer-2.5.5.dev79/mnamer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 17:11:45.257692 mnamer-2.5.5.dev79/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:45.253692 mnamer-2.5.5.dev79/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:45.253692 mnamer-2.5.5.dev79/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/tests/e2e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/tests/e2e/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/tests/e2e/test_directives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/tests/e2e/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/tests/e2e/test_moving.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:45.257692 mnamer-2.5.5.dev79/tests/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/tests/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/tests/local/test_argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/tests/local/test_language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/tests/local/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/tests/local/test_setting_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/tests/local/test_setting_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/tests/local/test_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/tests/local/test_tty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25741 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/tests/local/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:45.257692 mnamer-2.5.5.dev79/tests/network/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/tests/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/tests/network/test_endpoints__omdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/tests/network/test_endpoints__tmdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/tests/network/test_endpoints__tvdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/tests/network/test_endpoints__tvmaze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/tests/network/test_providers__omdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/tests/network/test_providers__tmdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/tests/network/test_providers__tvdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-07-13 17:11:23.000000 mnamer-2.5.5.dev79/tests/network/test_providers__tvmaze.py
```

### Comparing `mnamer-2.5.5.dev77/.github/actions/lint/action.yml` & `mnamer-2.5.5.dev79/.github/actions/lint/action.yml`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/.github/actions/test/action.yml` & `mnamer-2.5.5.dev79/.github/actions/test/action.yml`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/.github/workflows/pull_request.yml` & `mnamer-2.5.5.dev79/.github/workflows/pull_request.yml`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/.github/workflows/push.yml` & `mnamer-2.5.5.dev79/.github/workflows/push.yml`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/LICENSE.txt` & `mnamer-2.5.5.dev79/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/PKG-INFO` & `mnamer-2.5.5.dev79/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnamer
-Version: 2.5.5.dev77
+Version: 2.5.5.dev79
 Summary: A command-line utility for organizing media files.
 Author-email: Jessy Williams <jessy@jessywilliams.com>
 Maintainer-email: Jessy Williams <jessy@jessywilliams.com>
 License: MIT License
         
         Copyright (c) 2017 Jessy Williams
```

### Comparing `mnamer-2.5.5.dev77/README.md` & `mnamer-2.5.5.dev79/README.md`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/assets/design.eps` & `mnamer-2.5.5.dev79/assets/design.eps`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/assets/logo-2.png` & `mnamer-2.5.5.dev79/assets/logo-2.png`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/assets/logo-3.png` & `mnamer-2.5.5.dev79/assets/logo-3.png`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/assets/logo.png` & `mnamer-2.5.5.dev79/assets/logo.png`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/assets/recording.mov` & `mnamer-2.5.5.dev79/assets/recording.mov`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/assets/screenshot.eps` & `mnamer-2.5.5.dev79/assets/screenshot.eps`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/assets/screenshot.png` & `mnamer-2.5.5.dev79/assets/screenshot.png`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/makefile` & `mnamer-2.5.5.dev79/makefile`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/mnamer/__main__.py` & `mnamer-2.5.5.dev79/mnamer/__main__.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/mnamer/argument.py` & `mnamer-2.5.5.dev79/mnamer/argument.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/mnamer/const.py` & `mnamer-2.5.5.dev79/mnamer/const.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/mnamer/endpoints.py` & `mnamer-2.5.5.dev79/mnamer/endpoints.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/mnamer/exceptions.py` & `mnamer-2.5.5.dev79/mnamer/exceptions.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/mnamer/frontends.py` & `mnamer-2.5.5.dev79/mnamer/frontends.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/mnamer/language.py` & `mnamer-2.5.5.dev79/mnamer/language.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/mnamer/metadata.py` & `mnamer-2.5.5.dev79/mnamer/metadata.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/mnamer/providers.py` & `mnamer-2.5.5.dev79/mnamer/providers.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/mnamer/setting_spec.py` & `mnamer-2.5.5.dev79/mnamer/setting_spec.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/mnamer/setting_store.py` & `mnamer-2.5.5.dev79/mnamer/setting_store.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/mnamer/target.py` & `mnamer-2.5.5.dev79/mnamer/target.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/mnamer/tty.py` & `mnamer-2.5.5.dev79/mnamer/tty.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/mnamer/types.py` & `mnamer-2.5.5.dev79/mnamer/types.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/mnamer/utils.py` & `mnamer-2.5.5.dev79/mnamer/utils.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/mnamer.egg-info/PKG-INFO` & `mnamer-2.5.5.dev79/mnamer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnamer
-Version: 2.5.5.dev77
+Version: 2.5.5.dev79
 Summary: A command-line utility for organizing media files.
 Author-email: Jessy Williams <jessy@jessywilliams.com>
 Maintainer-email: Jessy Williams <jessy@jessywilliams.com>
 License: MIT License
         
         Copyright (c) 2017 Jessy Williams
```

### Comparing `mnamer-2.5.5.dev77/mnamer.egg-info/SOURCES.txt` & `mnamer-2.5.5.dev79/mnamer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/pyproject.toml` & `mnamer-2.5.5.dev79/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/tests/__init__.py` & `mnamer-2.5.5.dev79/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/tests/conftest.py` & `mnamer-2.5.5.dev79/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/tests/e2e/conftest.py` & `mnamer-2.5.5.dev79/tests/e2e/conftest.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/tests/e2e/test_directives.py` & `mnamer-2.5.5.dev79/tests/e2e/test_directives.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/tests/e2e/test_errors.py` & `mnamer-2.5.5.dev79/tests/e2e/test_errors.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/tests/e2e/test_moving.py` & `mnamer-2.5.5.dev79/tests/e2e/test_moving.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/tests/local/test_argument.py` & `mnamer-2.5.5.dev79/tests/local/test_argument.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/tests/local/test_language.py` & `mnamer-2.5.5.dev79/tests/local/test_language.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/tests/local/test_metadata.py` & `mnamer-2.5.5.dev79/tests/local/test_metadata.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/tests/local/test_setting_spec.py` & `mnamer-2.5.5.dev79/tests/local/test_setting_spec.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/tests/local/test_setting_store.py` & `mnamer-2.5.5.dev79/tests/local/test_setting_store.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/tests/local/test_target.py` & `mnamer-2.5.5.dev79/tests/local/test_target.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/tests/local/test_tty.py` & `mnamer-2.5.5.dev79/tests/local/test_tty.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/tests/local/test_utils.py` & `mnamer-2.5.5.dev79/tests/local/test_utils.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/tests/network/test_endpoints__omdb.py` & `mnamer-2.5.5.dev79/tests/network/test_endpoints__omdb.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/tests/network/test_endpoints__tmdb.py` & `mnamer-2.5.5.dev79/tests/network/test_endpoints__tmdb.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/tests/network/test_endpoints__tvdb.py` & `mnamer-2.5.5.dev79/tests/network/test_endpoints__tvdb.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/tests/network/test_endpoints__tvmaze.py` & `mnamer-2.5.5.dev79/tests/network/test_endpoints__tvmaze.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/tests/network/test_providers__omdb.py` & `mnamer-2.5.5.dev79/tests/network/test_providers__omdb.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/tests/network/test_providers__tmdb.py` & `mnamer-2.5.5.dev79/tests/network/test_providers__tmdb.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/tests/network/test_providers__tvdb.py` & `mnamer-2.5.5.dev79/tests/network/test_providers__tvdb.py`

 * *Files identical despite different names*

### Comparing `mnamer-2.5.5.dev77/tests/network/test_providers__tvmaze.py` & `mnamer-2.5.5.dev79/tests/network/test_providers__tvmaze.py`

 * *Files identical despite different names*

