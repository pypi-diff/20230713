# Comparing `tmp/vivarium_cluster_tools-1.3.8.tar.gz` & `tmp/vivarium_cluster_tools-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vivarium_cluster_tools-1.3.8.tar", last modified: Tue Dec 27 22:43:06 2022, max compression
+gzip compressed data, was "vivarium_cluster_tools-1.3.9.tar", last modified: Thu Jun  1 20:46:20 2023, max compression
```

## Comparing `vivarium_cluster_tools-1.3.8.tar` & `vivarium_cluster_tools-1.3.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 22:43:06.050036 vivarium_cluster_tools-1.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      111 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2022-12-27 22:43:06.050036 vivarium_cluster_tools-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      152 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-27 22:43:06.050036 vivarium_cluster_tools-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 22:43:06.034036 vivarium_cluster_tools-1.3.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 22:43:06.038036 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/cli_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 22:43:06.042036 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9762 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/branches.py
--rw-r--r--   0 runner    (1001) docker     (123)     8205 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 22:43:06.046036 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/cluster/cli_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/cluster/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/model_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/pip_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 22:43:06.046036 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/redis_dbs/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/redis_dbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/redis_dbs/cli_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/redis_dbs/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    10977 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/redis_dbs/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 22:43:06.046036 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/results/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/results/cli_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/results/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9797 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 22:43:06.050036 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/worker/
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/worker/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/worker/load_test_work_horse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6089 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/worker/vivarium_work_horse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 22:43:06.050036 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/vipin/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/vipin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/vipin/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/vipin/perf_counters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7996 2022-12-27 22:42:57.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/vipin/perf_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 22:43:06.042036 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2022-12-27 22:43:05.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2022-12-27 22:43:05.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-27 22:43:05.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2022-12-27 22:43:05.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-27 22:43:05.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      275 2022-12-27 22:43:05.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-27 22:43:05.000000 vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:46:20.590841 vivarium_cluster_tools-1.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-01 20:46:20.590841 vivarium_cluster_tools-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 20:46:20.590841 vivarium_cluster_tools-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:46:20.582841 vivarium_cluster_tools-1.3.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:46:20.586841 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/cli_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:46:20.586841 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:46:20.586841 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/cluster/cli_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/cluster/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/model_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/pip_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:46:20.586841 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/redis_dbs/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/redis_dbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/redis_dbs/cli_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/redis_dbs/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/redis_dbs/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:46:20.586841 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/results/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/results/cli_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/results/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:46:20.586841 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/worker/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/worker/load_test_work_horse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/worker/vivarium_work_horse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:46:20.586841 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/vipin/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/vipin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/vipin/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/vipin/perf_counters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-06-01 20:46:10.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/vipin/perf_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:46:20.586841 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-01 20:46:20.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-01 20:46:20.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:46:20.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-01 20:46:20.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:46:20.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-01 20:46:20.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 20:46:20.000000 vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools.egg-info/top_level.txt
```

### Comparing `vivarium_cluster_tools-1.3.8/CHANGELOG.rst` & `vivarium_cluster_tools-1.3.9/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+**1.3.9 - 06/01/23**
+
+ - Increments version of Vivarium required 
+
 **1.3.8 - 12/27/22**
 
  - Updates CI and setup to build python 3.7-3.10
  - Updates codeowners
 
 **1.3.7 - 10/28/22**
```

### Comparing `vivarium_cluster_tools-1.3.8/LICENSE` & `vivarium_cluster_tools-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vivarium_cluster_tools-1.3.8/PKG-INFO` & `vivarium_cluster_tools-1.3.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,121 +1,120 @@
 Metadata-Version: 2.1
 Name: vivarium_cluster_tools
-Version: 1.3.8
+Version: 1.3.9
 Summary: A set of tools for running simulation using vivarium on cluster.
 Home-page: https://github.com/ihmeuw/vivarium_cluster_tools
 Author: The vivarium developers
 Author-email: vivarium.dev@gmail.com
-License: UNKNOWN
-Description: Vivarium Cluster Tools
-        =======================
-        
-        .. image:: https://badge.fury.io/py/vivarium-cluster-tools.svg
-            :target: https://badge.fury.io/py/vivarium-cluster-tools
-        
-        .. image:: https://travis-ci.org/ihmeuw/vivarium_cluster_tools.svg?branch=main
-            :target: https://travis-ci.org/ihmeuw/vivarium_cluster_tools
-            :alt: Latest Version
-        
-        .. image:: https://readthedocs.org/projects/vivarium-cluster-tools/badge/?version=latest
-            :target: https://vivarium-cluster-tools.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        Vivarium cluster tools is a python package that makes running ``vivarium``
-        simulations at scale on a Univa Grid Engine cluster easy.
-        
-        Installation
-        ------------
-        
-        You can install this package with
-        
-        .. code-block:: console
-        
-            pip install vivarium-cluster-tools
-        
-        In addition, this tool needs the redis client. This must be installed using conda.
-        
-        .. code-block:: console
-        
-            conda install redis
-        
-        A simple example
-        ----------------
-        
-        If you have a ``vivarium`` model specifcation file defining a particular model,
-        you can use that along side a **branches file** to launch a run of many
-        simulations at once with variations in the input data, random seed, or with
-        different parameter settings.
-        
-        .. code-block:: console
-        
-            psimulate run /path/to/model_specification.yaml /path/to/branches_file.yaml
-        
-        The simplest branches file defines a count of input data draws and random seeds
-        to launch.
-        
-        .. code-block:: yaml
-        
-            input_draw_count: 25
-            random_seed_count: 10
-        
-        
-        This branches file defines a set of simulations for all combinations of 25
-        input draws and 10 random seeds and so would run, in total, 250 simulations.
-        
-        You can also define a set of parameter variations to run your model over. Say
-        your original model specification looked something like
-        
-        .. code-block:: yaml
-        
-            plugins:
-              optional: ...
-        
-            components:
-              vivarium_public_health:
-                population:
-                  - BasePopulation()
-                  - Mortality()
-                disease.models:
-                  - SIS('lower_respiratory_infections')
-              my_lri_intervention:
-                components:
-                  - GiveKidsVaccines()
-        
-            configuration:
-              population:
-                population_size: 1000
-                age_start: 0
-                age_end: 5
-              lri_vaccine:
-                coverage: 0.2
-                efficacy: 0.8
-        
-        Defining a simple model of lower respiratory infections and a vaccine
-        intervention. You could then write a branches file that varied over both
-        input data draws and random seeds, but also over different levels of coverage
-        and efficacy for the vaccine.  That file would look like
-        
-        .. code-block:: yaml
-        
-            input_draw_count: 25
-            random_seed_count: 10
-        
-            branches:
-              lri_vaccine:
-                coverage: [0.0, 0.2, 0.4, 0.8, 1.0]
-                efficacy: [0.4, 0.6, 0.8]
-        
-        The branches file would overwrite your original ``lri_vaccine`` configuration
-        with each combination of coverage and efficacy in the branches file and launch
-        a simulation. More, it would run each coverage-efficacy pair in the branches
-        for each combination of input draw and random seed to produce 25 * 10 * 5 * 3 =
-        3750 unique simulations.
-        
-        To read about more of the available features and get a better understanding
-        of how to correctly write your own branches files, check out the
-        `vivarium cluster tools documentation <https://vivarium-cluster-tools.readthedocs.io/en/latest/?badge=latest>`_.
-        
-Platform: UNKNOWN
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: dev
+License-File: LICENSE
+
+Vivarium Cluster Tools
+=======================
+
+.. image:: https://badge.fury.io/py/vivarium-cluster-tools.svg
+    :target: https://badge.fury.io/py/vivarium-cluster-tools
+
+.. image:: https://travis-ci.org/ihmeuw/vivarium_cluster_tools.svg?branch=main
+    :target: https://travis-ci.org/ihmeuw/vivarium_cluster_tools
+    :alt: Latest Version
+
+.. image:: https://readthedocs.org/projects/vivarium-cluster-tools/badge/?version=latest
+    :target: https://vivarium-cluster-tools.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+Vivarium cluster tools is a python package that makes running ``vivarium``
+simulations at scale on a Univa Grid Engine cluster easy.
+
+Installation
+------------
+
+You can install this package with
+
+.. code-block:: console
+
+    pip install vivarium-cluster-tools
+
+In addition, this tool needs the redis client. This must be installed using conda.
+
+.. code-block:: console
+
+    conda install redis
+
+A simple example
+----------------
+
+If you have a ``vivarium`` model specifcation file defining a particular model,
+you can use that along side a **branches file** to launch a run of many
+simulations at once with variations in the input data, random seed, or with
+different parameter settings.
+
+.. code-block:: console
+
+    psimulate run /path/to/model_specification.yaml /path/to/branches_file.yaml
+
+The simplest branches file defines a count of input data draws and random seeds
+to launch.
+
+.. code-block:: yaml
+
+    input_draw_count: 25
+    random_seed_count: 10
+
+
+This branches file defines a set of simulations for all combinations of 25
+input draws and 10 random seeds and so would run, in total, 250 simulations.
+
+You can also define a set of parameter variations to run your model over. Say
+your original model specification looked something like
+
+.. code-block:: yaml
+
+    plugins:
+      optional: ...
+
+    components:
+      vivarium_public_health:
+        population:
+          - BasePopulation()
+          - Mortality()
+        disease.models:
+          - SIS('lower_respiratory_infections')
+      my_lri_intervention:
+        components:
+          - GiveKidsVaccines()
+
+    configuration:
+      population:
+        population_size: 1000
+        age_start: 0
+        age_end: 5
+      lri_vaccine:
+        coverage: 0.2
+        efficacy: 0.8
+
+Defining a simple model of lower respiratory infections and a vaccine
+intervention. You could then write a branches file that varied over both
+input data draws and random seeds, but also over different levels of coverage
+and efficacy for the vaccine.  That file would look like
+
+.. code-block:: yaml
+
+    input_draw_count: 25
+    random_seed_count: 10
+
+    branches:
+      lri_vaccine:
+        coverage: [0.0, 0.2, 0.4, 0.8, 1.0]
+        efficacy: [0.4, 0.6, 0.8]
+
+The branches file would overwrite your original ``lri_vaccine`` configuration
+with each combination of coverage and efficacy in the branches file and launch
+a simulation. More, it would run each coverage-efficacy pair in the branches
+for each combination of input draw and random seed to produce 25 * 10 * 5 * 3 =
+3750 unique simulations.
+
+To read about more of the available features and get a better understanding
+of how to correctly write your own branches files, check out the
+`vivarium cluster tools documentation <https://vivarium-cluster-tools.readthedocs.io/en/latest/?badge=latest>`_.
```

### Comparing `vivarium_cluster_tools-1.3.8/README.rst` & `vivarium_cluster_tools-1.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `vivarium_cluster_tools-1.3.8/setup.py` & `vivarium_cluster_tools-1.3.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         "numpy",
         "tables",
         "loguru",
         "pyyaml>=5.1",
         "drmaa",
         "redis",
         "rq",
-        "vivarium>=1.0.2",
+        "vivarium>=1.2.0",
         "click",
         "psutil",
         "requests",
     ]
 
     test_requirements = [
         "pytest",
```

### Comparing `vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/cli_tools.py` & `vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/cli_tools.py`

 * *Files identical despite different names*

### Comparing `vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/logs.py` & `vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/logs.py`

 * *Files identical despite different names*

### Comparing `vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/branches.py` & `vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/branches.py`

 * *Files identical despite different names*

### Comparing `vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/cli.py` & `vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/cli.py`

 * *Files identical despite different names*

### Comparing `vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/cluster/cli_options.py` & `vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/cluster/cli_options.py`

 * *Files identical despite different names*

### Comparing `vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/cluster/interface.py` & `vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/cluster/interface.py`

 * *Files identical despite different names*

### Comparing `vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/environment.py` & `vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/environment.py`

 * *Files identical despite different names*

### Comparing `vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/jobs.py` & `vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/jobs.py`

 * *Files identical despite different names*

### Comparing `vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/model_specification.py` & `vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/model_specification.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,8 +81,10 @@
     return model_specification
 
 
 def persist(
     model_specification: ConfigTree,
     model_specification_path: Path,
 ) -> None:
-    model_specification_path.write_text(yaml.dump(model_specification.to_dict()))
+    model_specification_path.write_text(
+        yaml.dump(model_specification.to_dict(), sort_keys=False)
+    )
```

### Comparing `vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/paths.py` & `vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/paths.py`

 * *Files identical despite different names*

### Comparing `vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/pip_env.py` & `vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/pip_env.py`

 * *Files identical despite different names*

### Comparing `vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/redis_dbs/cli_options.py` & `vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/redis_dbs/cli_options.py`

 * *Files identical despite different names*

### Comparing `vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/redis_dbs/launcher.py` & `vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/redis_dbs/launcher.py`

 * *Files identical despite different names*

### Comparing `vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/redis_dbs/registry.py` & `vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/redis_dbs/registry.py`

 * *Files identical despite different names*

### Comparing `vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/results/cli_options.py` & `vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/results/cli_options.py`

 * *Files identical despite different names*

### Comparing `vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/results/processing.py` & `vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/results/processing.py`

 * *Files identical despite different names*

### Comparing `vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/runner.py` & `vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/runner.py`

 * *Files identical despite different names*

### Comparing `vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/worker/__init__.py` & `vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/worker/core.py` & `vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/worker/core.py`

 * *Files identical despite different names*

### Comparing `vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/worker/load_test_work_horse.py` & `vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/worker/load_test_work_horse.py`

 * *Files identical despite different names*

### Comparing `vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/psimulate/worker/vivarium_work_horse.py` & `vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/psimulate/worker/vivarium_work_horse.py`

 * *Files identical despite different names*

### Comparing `vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/utilities.py` & `vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/utilities.py`

 * *Files identical despite different names*

### Comparing `vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/vipin/cli.py` & `vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/vipin/cli.py`

 * *Files identical despite different names*

### Comparing `vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/vipin/perf_counters.py` & `vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/vipin/perf_counters.py`

 * *Files identical despite different names*

### Comparing `vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools/vipin/perf_report.py` & `vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools/vipin/perf_report.py`

 * *Files identical despite different names*

### Comparing `vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools.egg-info/PKG-INFO` & `vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,121 +1,120 @@
 Metadata-Version: 2.1
 Name: vivarium-cluster-tools
-Version: 1.3.8
+Version: 1.3.9
 Summary: A set of tools for running simulation using vivarium on cluster.
 Home-page: https://github.com/ihmeuw/vivarium_cluster_tools
 Author: The vivarium developers
 Author-email: vivarium.dev@gmail.com
-License: UNKNOWN
-Description: Vivarium Cluster Tools
-        =======================
-        
-        .. image:: https://badge.fury.io/py/vivarium-cluster-tools.svg
-            :target: https://badge.fury.io/py/vivarium-cluster-tools
-        
-        .. image:: https://travis-ci.org/ihmeuw/vivarium_cluster_tools.svg?branch=main
-            :target: https://travis-ci.org/ihmeuw/vivarium_cluster_tools
-            :alt: Latest Version
-        
-        .. image:: https://readthedocs.org/projects/vivarium-cluster-tools/badge/?version=latest
-            :target: https://vivarium-cluster-tools.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        Vivarium cluster tools is a python package that makes running ``vivarium``
-        simulations at scale on a Univa Grid Engine cluster easy.
-        
-        Installation
-        ------------
-        
-        You can install this package with
-        
-        .. code-block:: console
-        
-            pip install vivarium-cluster-tools
-        
-        In addition, this tool needs the redis client. This must be installed using conda.
-        
-        .. code-block:: console
-        
-            conda install redis
-        
-        A simple example
-        ----------------
-        
-        If you have a ``vivarium`` model specifcation file defining a particular model,
-        you can use that along side a **branches file** to launch a run of many
-        simulations at once with variations in the input data, random seed, or with
-        different parameter settings.
-        
-        .. code-block:: console
-        
-            psimulate run /path/to/model_specification.yaml /path/to/branches_file.yaml
-        
-        The simplest branches file defines a count of input data draws and random seeds
-        to launch.
-        
-        .. code-block:: yaml
-        
-            input_draw_count: 25
-            random_seed_count: 10
-        
-        
-        This branches file defines a set of simulations for all combinations of 25
-        input draws and 10 random seeds and so would run, in total, 250 simulations.
-        
-        You can also define a set of parameter variations to run your model over. Say
-        your original model specification looked something like
-        
-        .. code-block:: yaml
-        
-            plugins:
-              optional: ...
-        
-            components:
-              vivarium_public_health:
-                population:
-                  - BasePopulation()
-                  - Mortality()
-                disease.models:
-                  - SIS('lower_respiratory_infections')
-              my_lri_intervention:
-                components:
-                  - GiveKidsVaccines()
-        
-            configuration:
-              population:
-                population_size: 1000
-                age_start: 0
-                age_end: 5
-              lri_vaccine:
-                coverage: 0.2
-                efficacy: 0.8
-        
-        Defining a simple model of lower respiratory infections and a vaccine
-        intervention. You could then write a branches file that varied over both
-        input data draws and random seeds, but also over different levels of coverage
-        and efficacy for the vaccine.  That file would look like
-        
-        .. code-block:: yaml
-        
-            input_draw_count: 25
-            random_seed_count: 10
-        
-            branches:
-              lri_vaccine:
-                coverage: [0.0, 0.2, 0.4, 0.8, 1.0]
-                efficacy: [0.4, 0.6, 0.8]
-        
-        The branches file would overwrite your original ``lri_vaccine`` configuration
-        with each combination of coverage and efficacy in the branches file and launch
-        a simulation. More, it would run each coverage-efficacy pair in the branches
-        for each combination of input draw and random seed to produce 25 * 10 * 5 * 3 =
-        3750 unique simulations.
-        
-        To read about more of the available features and get a better understanding
-        of how to correctly write your own branches files, check out the
-        `vivarium cluster tools documentation <https://vivarium-cluster-tools.readthedocs.io/en/latest/?badge=latest>`_.
-        
-Platform: UNKNOWN
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: dev
+License-File: LICENSE
+
+Vivarium Cluster Tools
+=======================
+
+.. image:: https://badge.fury.io/py/vivarium-cluster-tools.svg
+    :target: https://badge.fury.io/py/vivarium-cluster-tools
+
+.. image:: https://travis-ci.org/ihmeuw/vivarium_cluster_tools.svg?branch=main
+    :target: https://travis-ci.org/ihmeuw/vivarium_cluster_tools
+    :alt: Latest Version
+
+.. image:: https://readthedocs.org/projects/vivarium-cluster-tools/badge/?version=latest
+    :target: https://vivarium-cluster-tools.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+Vivarium cluster tools is a python package that makes running ``vivarium``
+simulations at scale on a Univa Grid Engine cluster easy.
+
+Installation
+------------
+
+You can install this package with
+
+.. code-block:: console
+
+    pip install vivarium-cluster-tools
+
+In addition, this tool needs the redis client. This must be installed using conda.
+
+.. code-block:: console
+
+    conda install redis
+
+A simple example
+----------------
+
+If you have a ``vivarium`` model specifcation file defining a particular model,
+you can use that along side a **branches file** to launch a run of many
+simulations at once with variations in the input data, random seed, or with
+different parameter settings.
+
+.. code-block:: console
+
+    psimulate run /path/to/model_specification.yaml /path/to/branches_file.yaml
+
+The simplest branches file defines a count of input data draws and random seeds
+to launch.
+
+.. code-block:: yaml
+
+    input_draw_count: 25
+    random_seed_count: 10
+
+
+This branches file defines a set of simulations for all combinations of 25
+input draws and 10 random seeds and so would run, in total, 250 simulations.
+
+You can also define a set of parameter variations to run your model over. Say
+your original model specification looked something like
+
+.. code-block:: yaml
+
+    plugins:
+      optional: ...
+
+    components:
+      vivarium_public_health:
+        population:
+          - BasePopulation()
+          - Mortality()
+        disease.models:
+          - SIS('lower_respiratory_infections')
+      my_lri_intervention:
+        components:
+          - GiveKidsVaccines()
+
+    configuration:
+      population:
+        population_size: 1000
+        age_start: 0
+        age_end: 5
+      lri_vaccine:
+        coverage: 0.2
+        efficacy: 0.8
+
+Defining a simple model of lower respiratory infections and a vaccine
+intervention. You could then write a branches file that varied over both
+input data draws and random seeds, but also over different levels of coverage
+and efficacy for the vaccine.  That file would look like
+
+.. code-block:: yaml
+
+    input_draw_count: 25
+    random_seed_count: 10
+
+    branches:
+      lri_vaccine:
+        coverage: [0.0, 0.2, 0.4, 0.8, 1.0]
+        efficacy: [0.4, 0.6, 0.8]
+
+The branches file would overwrite your original ``lri_vaccine`` configuration
+with each combination of coverage and efficacy in the branches file and launch
+a simulation. More, it would run each coverage-efficacy pair in the branches
+for each combination of input draw and random seed to produce 25 * 10 * 5 * 3 =
+3750 unique simulations.
+
+To read about more of the available features and get a better understanding
+of how to correctly write your own branches files, check out the
+`vivarium cluster tools documentation <https://vivarium-cluster-tools.readthedocs.io/en/latest/?badge=latest>`_.
```

### Comparing `vivarium_cluster_tools-1.3.8/src/vivarium_cluster_tools.egg-info/SOURCES.txt` & `vivarium_cluster_tools-1.3.9/src/vivarium_cluster_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

