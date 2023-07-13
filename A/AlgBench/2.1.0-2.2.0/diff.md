# Comparing `tmp/AlgBench-2.1.0.tar.gz` & `tmp/AlgBench-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlgBench-2.1.0.tar", last modified: Fri Jul  7 17:00:06 2023, max compression
+gzip compressed data, was "AlgBench-2.2.0.tar", last modified: Thu Jul 13 16:47:13 2023, max compression
```

## Comparing `AlgBench-2.1.0.tar` & `AlgBench-2.2.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.888727 AlgBench-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-07 16:59:53.000000 AlgBench-2.1.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.876726 AlgBench-2.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.880726 AlgBench-2.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-07 16:59:53.000000 AlgBench-2.1.0/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-07 16:59:53.000000 AlgBench-2.1.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-07 16:59:53.000000 AlgBench-2.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-07 16:59:53.000000 AlgBench-2.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-07 16:59:53.000000 AlgBench-2.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-07 16:59:53.000000 AlgBench-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24547 2023-07-07 17:00:06.888727 AlgBench-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24004 2023-07-07 16:59:53.000000 AlgBench-2.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.880726 AlgBench-2.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-07 16:59:53.000000 AlgBench-2.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-07 16:59:53.000000 AlgBench-2.1.0/docs/algbench.db.rst
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-07 16:59:53.000000 AlgBench-2.1.0/docs/algbench.rst
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-07 16:59:53.000000 AlgBench-2.1.0/docs/algbench.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-07 16:59:53.000000 AlgBench-2.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-07 16:59:53.000000 AlgBench-2.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-07 16:59:53.000000 AlgBench-2.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-07 16:59:53.000000 AlgBench-2.1.0/docs/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.876726 AlgBench-2.1.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.884727 AlgBench-2.1.0/examples/graph_coloring/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/00_generate_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/01_instances.zip
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/02_run_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/02b_run_benchmark_with_slurminade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.884727 AlgBench-2.1.0/examples/graph_coloring/03_benchmark_data/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/03_benchmark_data/algbench.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.884727 AlgBench-2.1.0/examples/graph_coloring/03_benchmark_data/arg_fingerprints/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/03_benchmark_data/arg_fingerprints/_compressed.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.884727 AlgBench-2.1.0/examples/graph_coloring/03_benchmark_data/env_info/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/03_benchmark_data/env_info/_compressed.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.884727 AlgBench-2.1.0/examples/graph_coloring/03_benchmark_data/results/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/03_benchmark_data/results/_compressed.zip
--rw-r--r--   0 runner    (1001) docker     (123)    36424 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/04_check_results.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/05_process_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/06_simplified_results.json.zip
--rw-r--r--   0 runner    (1001) docker     (123)    15837 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/07_analyze_mean.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  1072992 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/08_analyze_runtime.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   397344 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/09_analyze_quality.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.884727 AlgBench-2.1.0/examples/graph_coloring/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-07 16:59:53.000000 AlgBench-2.1.0/examples/graph_coloring/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-07-07 16:59:53.000000 AlgBench-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-07 16:59:53.000000 AlgBench-2.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 17:00:06.888727 AlgBench-2.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.876726 AlgBench-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.884727 AlgBench-2.1.0/src/AlgBench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24547 2023-07-07 17:00:06.000000 AlgBench-2.1.0/src/AlgBench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-07 17:00:06.000000 AlgBench-2.1.0/src/AlgBench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 17:00:06.000000 AlgBench-2.1.0/src/AlgBench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-07 17:00:06.000000 AlgBench-2.1.0/src/AlgBench.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-07 17:00:06.000000 AlgBench-2.1.0/src/AlgBench.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.884727 AlgBench-2.1.0/src/algbench/
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-07 16:59:53.000000 AlgBench-2.1.0/src/algbench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-07 16:59:53.000000 AlgBench-2.1.0/src/algbench/_stream_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-07-07 16:59:53.000000 AlgBench-2.1.0/src/algbench/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-07 16:59:53.000000 AlgBench-2.1.0/src/algbench/benchmark_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.884727 AlgBench-2.1.0/src/algbench/db/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-07 16:59:53.000000 AlgBench-2.1.0/src/algbench/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-07 16:59:53.000000 AlgBench-2.1.0/src/algbench/db/json_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-07 16:59:53.000000 AlgBench-2.1.0/src/algbench/db/nfs_json_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-07-07 16:59:53.000000 AlgBench-2.1.0/src/algbench/db/nfs_json_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-07 16:59:53.000000 AlgBench-2.1.0/src/algbench/db/nfs_json_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-07 16:59:53.000000 AlgBench-2.1.0/src/algbench/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-07 16:59:53.000000 AlgBench-2.1.0/src/algbench/fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-07 16:59:53.000000 AlgBench-2.1.0/src/algbench/log_capture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-07 16:59:53.000000 AlgBench-2.1.0/src/algbench/pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.884727 AlgBench-2.1.0/src/algbench/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-07 16:59:53.000000 AlgBench-2.1.0/src/algbench/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-07 16:59:53.000000 AlgBench-2.1.0/src/algbench/utils/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 17:00:06.884727 AlgBench-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-07 16:59:53.000000 AlgBench-2.1.0/tests/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-07 16:59:53.000000 AlgBench-2.1.0/tests/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:47:13.527564 AlgBench-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-13 16:47:00.000000 AlgBench-2.2.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:47:13.503564 AlgBench-2.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:47:13.511564 AlgBench-2.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-13 16:47:00.000000 AlgBench-2.2.0/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-13 16:47:00.000000 AlgBench-2.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-13 16:47:00.000000 AlgBench-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-13 16:47:00.000000 AlgBench-2.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-13 16:47:00.000000 AlgBench-2.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-13 16:47:00.000000 AlgBench-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24636 2023-07-13 16:47:13.527564 AlgBench-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24093 2023-07-13 16:47:00.000000 AlgBench-2.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:47:13.515565 AlgBench-2.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-13 16:47:00.000000 AlgBench-2.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-13 16:47:00.000000 AlgBench-2.2.0/docs/algbench.db.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-13 16:47:00.000000 AlgBench-2.2.0/docs/algbench.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-13 16:47:00.000000 AlgBench-2.2.0/docs/algbench.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-13 16:47:00.000000 AlgBench-2.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-13 16:47:00.000000 AlgBench-2.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-13 16:47:00.000000 AlgBench-2.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-13 16:47:00.000000 AlgBench-2.2.0/docs/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:47:13.507564 AlgBench-2.2.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:47:13.519564 AlgBench-2.2.0/examples/graph_coloring/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-13 16:47:00.000000 AlgBench-2.2.0/examples/graph_coloring/00_generate_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-13 16:47:00.000000 AlgBench-2.2.0/examples/graph_coloring/01_instances.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-13 16:47:00.000000 AlgBench-2.2.0/examples/graph_coloring/02_run_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-13 16:47:00.000000 AlgBench-2.2.0/examples/graph_coloring/02b_run_benchmark_with_slurminade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:47:13.519564 AlgBench-2.2.0/examples/graph_coloring/03_benchmark_data/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-13 16:47:00.000000 AlgBench-2.2.0/examples/graph_coloring/03_benchmark_data/algbench.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:47:13.519564 AlgBench-2.2.0/examples/graph_coloring/03_benchmark_data/arg_fingerprints/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-13 16:47:00.000000 AlgBench-2.2.0/examples/graph_coloring/03_benchmark_data/arg_fingerprints/_compressed.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:47:13.519564 AlgBench-2.2.0/examples/graph_coloring/03_benchmark_data/env_info/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-13 16:47:00.000000 AlgBench-2.2.0/examples/graph_coloring/03_benchmark_data/env_info/_compressed.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:47:13.519564 AlgBench-2.2.0/examples/graph_coloring/03_benchmark_data/results/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-13 16:47:00.000000 AlgBench-2.2.0/examples/graph_coloring/03_benchmark_data/results/_compressed.zip
+-rw-r--r--   0 runner    (1001) docker     (123)    36424 2023-07-13 16:47:00.000000 AlgBench-2.2.0/examples/graph_coloring/04_check_results.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-13 16:47:00.000000 AlgBench-2.2.0/examples/graph_coloring/05_process_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-13 16:47:00.000000 AlgBench-2.2.0/examples/graph_coloring/06_simplified_results.json.zip
+-rw-r--r--   0 runner    (1001) docker     (123)    15837 2023-07-13 16:47:00.000000 AlgBench-2.2.0/examples/graph_coloring/07_analyze_mean.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1072992 2023-07-13 16:47:01.000000 AlgBench-2.2.0/examples/graph_coloring/08_analyze_runtime.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   397344 2023-07-13 16:47:01.000000 AlgBench-2.2.0/examples/graph_coloring/09_analyze_quality.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-13 16:47:01.000000 AlgBench-2.2.0/examples/graph_coloring/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:47:13.519564 AlgBench-2.2.0/examples/graph_coloring/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-13 16:47:01.000000 AlgBench-2.2.0/examples/graph_coloring/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-13 16:47:01.000000 AlgBench-2.2.0/examples/graph_coloring/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-07-13 16:47:01.000000 AlgBench-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-13 16:47:01.000000 AlgBench-2.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 16:47:13.527564 AlgBench-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:47:13.507564 AlgBench-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:47:13.523564 AlgBench-2.2.0/src/AlgBench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24636 2023-07-13 16:47:13.000000 AlgBench-2.2.0/src/AlgBench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-13 16:47:13.000000 AlgBench-2.2.0/src/AlgBench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:47:13.000000 AlgBench-2.2.0/src/AlgBench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-13 16:47:13.000000 AlgBench-2.2.0/src/AlgBench.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 16:47:13.000000 AlgBench-2.2.0/src/AlgBench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:47:13.523564 AlgBench-2.2.0/src/algbench/
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-13 16:47:01.000000 AlgBench-2.2.0/src/algbench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-13 16:47:01.000000 AlgBench-2.2.0/src/algbench/_stream_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11151 2023-07-13 16:47:01.000000 AlgBench-2.2.0/src/algbench/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-13 16:47:01.000000 AlgBench-2.2.0/src/algbench/benchmark_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:47:13.523564 AlgBench-2.2.0/src/algbench/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-13 16:47:01.000000 AlgBench-2.2.0/src/algbench/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-13 16:47:01.000000 AlgBench-2.2.0/src/algbench/db/json_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-13 16:47:01.000000 AlgBench-2.2.0/src/algbench/db/nfs_json_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-07-13 16:47:01.000000 AlgBench-2.2.0/src/algbench/db/nfs_json_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-13 16:47:01.000000 AlgBench-2.2.0/src/algbench/db/nfs_json_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-13 16:47:01.000000 AlgBench-2.2.0/src/algbench/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-13 16:47:01.000000 AlgBench-2.2.0/src/algbench/fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-13 16:47:01.000000 AlgBench-2.2.0/src/algbench/log_capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-13 16:47:01.000000 AlgBench-2.2.0/src/algbench/pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:47:13.527564 AlgBench-2.2.0/src/algbench/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-13 16:47:01.000000 AlgBench-2.2.0/src/algbench/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-13 16:47:01.000000 AlgBench-2.2.0/src/algbench/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:47:13.527564 AlgBench-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-13 16:47:01.000000 AlgBench-2.2.0/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-13 16:47:01.000000 AlgBench-2.2.0/tests/test_logger.py
```

### Comparing `AlgBench-2.1.0/.github/workflows/pytest.yml` & `AlgBench-2.2.0/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `AlgBench-2.1.0/.github/workflows/release.yml` & `AlgBench-2.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `AlgBench-2.1.0/.gitignore` & `AlgBench-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `AlgBench-2.1.0/.pre-commit-config.yaml` & `AlgBench-2.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `AlgBench-2.1.0/.readthedocs.yaml` & `AlgBench-2.2.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `AlgBench-2.1.0/LICENSE` & `AlgBench-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `AlgBench-2.1.0/PKG-INFO` & `AlgBench-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlgBench
-Version: 2.1.0
+Version: 2.2.0
 Summary: Util for benchmarking algorithms.
 Author-email: "TU Braunschweig, IBR, Algorithms Group (Dominik Krupke)" <krupke@ibr.cs.tu-bs.de>
 Project-URL: Homepage, https://github.com/d-krupke/AlgBench
 Project-URL: Issues, https://github.com/d-krupke/AlgBench/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
@@ -571,15 +571,15 @@
    my_alg()
 
 A further advantage of the logging framework is that you can separate
 the message structure from the data. This allows you to easily query
 for specific events and directly extract the data you want to analyze.
 
 .. code:: python
-   
+
    logger.info("Submodule X needed %d iterations", 42)
 
 Will be saved as a dictionary with a separate field for the message and
 the data:
 
 ::
 
@@ -635,14 +635,15 @@
 .. code:: bash
 
    git add .gitattributes
 
 Version History
 ===============
 
+- **2.2.0** Allowing to skip entries in ``read_as_pandas`` by returning a None for the row.
 - **2.1.0** More flexible stream handling. You can now disable the output saving and hidding. The default behavior still is to save the output with time stamps and hide it from the console.
 - **2.0.0** Extensive change of stdout/stderr handling and new logging functionality.
    By default, stdout and stderr will now be saved with the runtime of the function.
    Additionally, you can now capture loggers of the Python logging framework and save them to the database.
    This is especially useful if you use a library that uses the logging framework. Prefere ``logging`` over ``print`` for logging information.
 -  **1.1.0** Some changes for efficiency turned out to be less robust in
    case of, e.g., keyboard interrupt. Fixed that.
```

### Comparing `AlgBench-2.1.0/README.rst` & `AlgBench-2.2.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -557,15 +557,15 @@
    my_alg()
 
 A further advantage of the logging framework is that you can separate
 the message structure from the data. This allows you to easily query
 for specific events and directly extract the data you want to analyze.
 
 .. code:: python
-   
+
    logger.info("Submodule X needed %d iterations", 42)
 
 Will be saved as a dictionary with a separate field for the message and
 the data:
 
 ::
 
@@ -621,14 +621,15 @@
 .. code:: bash
 
    git add .gitattributes
 
 Version History
 ===============
 
+- **2.2.0** Allowing to skip entries in ``read_as_pandas`` by returning a None for the row.
 - **2.1.0** More flexible stream handling. You can now disable the output saving and hidding. The default behavior still is to save the output with time stamps and hide it from the console.
 - **2.0.0** Extensive change of stdout/stderr handling and new logging functionality.
    By default, stdout and stderr will now be saved with the runtime of the function.
    Additionally, you can now capture loggers of the Python logging framework and save them to the database.
    This is especially useful if you use a library that uses the logging framework. Prefere ``logging`` over ``print`` for logging information.
 -  **1.1.0** Some changes for efficiency turned out to be less robust in
    case of, e.g., keyboard interrupt. Fixed that.
```

### Comparing `AlgBench-2.1.0/docs/Makefile` & `AlgBench-2.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `AlgBench-2.1.0/docs/algbench.db.rst` & `AlgBench-2.2.0/docs/algbench.db.rst`

 * *Files identical despite different names*

### Comparing `AlgBench-2.1.0/docs/algbench.rst` & `AlgBench-2.2.0/docs/algbench.rst`

 * *Files identical despite different names*

### Comparing `AlgBench-2.1.0/docs/conf.py` & `AlgBench-2.2.0/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.viewcode",
 ]
 # For including __iniit__ docstrings
 autodoc_default_options = {
-    'members': True,
-    'member-order': 'bysource',
-    'special-members': '__init__',
-    'undoc-members': True,
-    'exclude-members': '__weakref__'
+    "members": True,
+    "member-order": "bysource",
+    "special-members": "__init__",
+    "undoc-members": True,
+    "exclude-members": "__weakref__",
 }
 
 
 templates_path = ["_templates"]
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
```

### Comparing `AlgBench-2.1.0/docs/make.bat` & `AlgBench-2.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `AlgBench-2.1.0/examples/graph_coloring/00_generate_instances.py` & `AlgBench-2.2.0/examples/graph_coloring/00_generate_instances.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.1.0/examples/graph_coloring/02_run_benchmark.py` & `AlgBench-2.2.0/examples/graph_coloring/02_run_benchmark.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.1.0/examples/graph_coloring/02b_run_benchmark_with_slurminade.py` & `AlgBench-2.2.0/examples/graph_coloring/02b_run_benchmark_with_slurminade.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.1.0/examples/graph_coloring/04_check_results.ipynb` & `AlgBench-2.2.0/examples/graph_coloring/04_check_results.ipynb`

 * *Files identical despite different names*

### Comparing `AlgBench-2.1.0/examples/graph_coloring/05_process_results.py` & `AlgBench-2.2.0/examples/graph_coloring/05_process_results.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.1.0/examples/graph_coloring/07_analyze_mean.ipynb` & `AlgBench-2.2.0/examples/graph_coloring/07_analyze_mean.ipynb`

 * *Files identical despite different names*

### Comparing `AlgBench-2.1.0/examples/graph_coloring/08_analyze_runtime.ipynb` & `AlgBench-2.2.0/examples/graph_coloring/08_analyze_runtime.ipynb`

 * *Files identical despite different names*

### Comparing `AlgBench-2.1.0/examples/graph_coloring/09_analyze_quality.ipynb` & `AlgBench-2.2.0/examples/graph_coloring/09_analyze_quality.ipynb`

 * *Files identical despite different names*

### Comparing `AlgBench-2.1.0/examples/graph_coloring/README.md` & `AlgBench-2.2.0/examples/graph_coloring/README.md`

 * *Files identical despite different names*

### Comparing `AlgBench-2.1.0/examples/graph_coloring/_utils/__init__.py` & `AlgBench-2.2.0/examples/graph_coloring/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.1.0/pyproject.toml` & `AlgBench-2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `AlgBench-2.1.0/src/AlgBench.egg-info/PKG-INFO` & `AlgBench-2.2.0/src/AlgBench.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlgBench
-Version: 2.1.0
+Version: 2.2.0
 Summary: Util for benchmarking algorithms.
 Author-email: "TU Braunschweig, IBR, Algorithms Group (Dominik Krupke)" <krupke@ibr.cs.tu-bs.de>
 Project-URL: Homepage, https://github.com/d-krupke/AlgBench
 Project-URL: Issues, https://github.com/d-krupke/AlgBench/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
@@ -571,15 +571,15 @@
    my_alg()
 
 A further advantage of the logging framework is that you can separate
 the message structure from the data. This allows you to easily query
 for specific events and directly extract the data you want to analyze.
 
 .. code:: python
-   
+
    logger.info("Submodule X needed %d iterations", 42)
 
 Will be saved as a dictionary with a separate field for the message and
 the data:
 
 ::
 
@@ -635,14 +635,15 @@
 .. code:: bash
 
    git add .gitattributes
 
 Version History
 ===============
 
+- **2.2.0** Allowing to skip entries in ``read_as_pandas`` by returning a None for the row.
 - **2.1.0** More flexible stream handling. You can now disable the output saving and hidding. The default behavior still is to save the output with time stamps and hide it from the console.
 - **2.0.0** Extensive change of stdout/stderr handling and new logging functionality.
    By default, stdout and stderr will now be saved with the runtime of the function.
    Additionally, you can now capture loggers of the Python logging framework and save them to the database.
    This is especially useful if you use a library that uses the logging framework. Prefere ``logging`` over ``print`` for logging information.
 -  **1.1.0** Some changes for efficiency turned out to be less robust in
    case of, e.g., keyboard interrupt. Fixed that.
```

### Comparing `AlgBench-2.1.0/src/AlgBench.egg-info/SOURCES.txt` & `AlgBench-2.2.0/src/AlgBench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AlgBench-2.1.0/src/algbench/__init__.py` & `AlgBench-2.2.0/src/algbench/__init__.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.1.0/src/algbench/_stream_utils.py` & `AlgBench-2.2.0/src/algbench/_stream_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 This files are wrapper for the output streams.
 They are used to capture the output of the functions
 and store it in the database.
 """
 
 
-from typing import Iterable, List, Tuple
 import io
+from typing import List, Tuple
+
 from .utils import Timer
 
 
 class PrintingStringIO(io.StringIO):
     """
     A StringIO that additionally prints to a stream.
     """
```

### Comparing `AlgBench-2.1.0/src/algbench/benchmark.py` & `AlgBench-2.2.0/src/algbench/benchmark.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import datetime
 import inspect
-import io
 import logging
+import sys
 import traceback
 import typing
-import sys
 from contextlib import ExitStack, redirect_stderr, redirect_stdout
 
 import yaml
 
+from ._stream_utils import NotSavingIO, PrintingStringIO, StreamWithTime
 from .benchmark_db import BenchmarkDb
 from .db.json_serializer import to_json
 from .fingerprint import fingerprint
 from .log_capture import JsonLogCapture, JsonLogHandler
-from ._stream_utils import StreamWithTime, PrintingStringIO, NotSavingIO
 from .utils import Timer
 
 
 class Benchmark:
     """
     This is the heart of the library. It allows to run, save, and load
     a benchmark.
@@ -37,15 +36,21 @@
     - unlink_logger
     - __iter__
 
     Don't call any of the other functions while the benchmark is
     running. It could lead to data loss.
     """
 
-    def __init__(self, path: str, save_output: bool = True, hide_output: bool = True, save_output_with_time: bool = True) -> None:
+    def __init__(
+        self,
+        path: str,
+        save_output: bool = True,
+        hide_output: bool = True,
+        save_output_with_time: bool = True,
+    ) -> None:
         """
         Just specify the path of where to put the
         database and everything else happens magically.
         Make sure not to use the same path for different
         databases, as they will get mixed.
 
         :param path: The path to the database.
@@ -179,24 +184,24 @@
                             "timestamp": timestamp,
                             "runtime": runtime,
                             "stdout": stdout.getvalue(),
                             "stderr": stderr.getvalue(),
                             "logging": log_handler.get_entries(),
                         },
                     )
-            print(".", end="")
+            print(".", end="")  # flake8: noqa T201
         except Exception as e:
-            print()
-            print("Exception while running benchmark.")
-            print("=====================================")
-            print(yaml.dump(arg_data))
-            print("-------------------------------------")
-            print("ERROR:", e, f"({type(e)})")
-            print(traceback.format_exc())
-            print("-------------------------------------")
+            print()  # flake8: noqa T201
+            print("Exception while running benchmark.")  # flake8: noqa T201
+            print("=====================================")  # flake8: noqa T201
+            print(yaml.dump(arg_data))  # flake8: noqa T201
+            print("-------------------------------------")  # flake8: noqa T201
+            print("ERROR:", e, f"({type(e)})")  # flake8: noqa T201
+            print(traceback.format_exc())  # flake8: noqa T201
+            print("-------------------------------------")  # flake8: noqa T201
             raise
 
     def add(self, func: typing.Callable, *args, **kwargs):
         """
         Will add the function call with the arguments
         to the benchmark if not yet contained.
```

### Comparing `AlgBench-2.1.0/src/algbench/benchmark_db.py` & `AlgBench-2.2.0/src/algbench/benchmark_db.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.1.0/src/algbench/db/json_serializer.py` & `AlgBench-2.2.0/src/algbench/db/json_serializer.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.1.0/src/algbench/db/nfs_json_dict.py` & `AlgBench-2.2.0/src/algbench/db/nfs_json_dict.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.1.0/src/algbench/db/nfs_json_list.py` & `AlgBench-2.2.0/src/algbench/db/nfs_json_list.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.1.0/src/algbench/db/nfs_json_set.py` & `AlgBench-2.2.0/src/algbench/db/nfs_json_set.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.1.0/src/algbench/environment.py` & `AlgBench-2.2.0/src/algbench/environment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Gathering information of the environment the
 code is running.
 """
-import os
 import socket
 import subprocess
 import sys
 import typing
+from pathlib import Path
 
 import __main__
 import pkg_resources
 
 __cached = None
 
 
@@ -38,15 +38,15 @@
     global __cached
     if cached and __cached:
         return __cached
     __cached = {
         "hostname": socket.gethostname(),
         "python_version": sys.version,
         "python": sys.executable,
-        "cwd": os.getcwd(),
+        "cwd": Path.cwd(),
         "environment": [
             {
                 "name": str(pkg.project_name),
                 "path": str(pkg.location),
                 "version": str(pkg.parsed_version),
             }
             for pkg in pkg_resources.working_set
```

### Comparing `AlgBench-2.1.0/src/algbench/log_capture.py` & `AlgBench-2.2.0/src/algbench/log_capture.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,50 +2,58 @@
 Code for capturing logs and returning them as a list of JSON compatible
 dictionaries. You don't need to use this code directly. Use the
 ``Benchmark.capture_logger`` method instead.
 """
 
 import logging
 from typing import Optional
+
 from .db.json_serializer import to_json
 from .utils import Timer
 
+
 class JsonLogHandler(logging.Handler):
     """
     A logging handler that stores log entries in a list of JSON compatible
     dictionaries.
     """
 
-    def __init__(self, level = logging.NOTSET) -> None:
+    def __init__(self, level=logging.NOTSET) -> None:
         """
         :param level: The level of the logger to catch.
         """
         super().__init__(level)
         self._log = []
-        self._timer= Timer()
+        self._timer = Timer()
 
     def emit(self, record: logging.LogRecord) -> None:
-        data = dict()
+        data = {}
         data.update(record.__dict__)
         data["runtime"] = self._timer.time()
         self._log.append(to_json(data))
 
     def reset(self):
         self._timer.reset()
         self._log = []
 
     def get_entries(self) -> list:
         return self._log
 
+
 class JsonLogCapture:
     """
     A context manager that captures logs and returns them as a list of JSON
     """
 
-    def __init__(self, logger_name: str, level = logging.NOTSET, handler: Optional[JsonLogHandler]=None) -> None:
+    def __init__(
+        self,
+        logger_name: str,
+        level=logging.NOTSET,
+        handler: Optional[JsonLogHandler] = None,
+    ) -> None:
         """
         :param logger_name: The name of the logger to catch.
         :param level: The level of the logger to catch.
         """
         self._logger = logging.getLogger(logger_name)
         self._level = level
         self._prior_level = self._logger.getEffectiveLevel()
@@ -66,9 +74,7 @@
             self._logger.setLevel(self._prior_level)
 
     def get_entries(self) -> list:
         """
         Returns the log entries as a list of JSON compatible dictionaries.
         """
         return self._json_log.get_entries()
-    
-
```

### Comparing `AlgBench-2.1.0/src/algbench/pandas.py` & `AlgBench-2.2.0/src/algbench/pandas.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,54 +9,54 @@
     data: typing.Dict, indentation: int, max_length: int, max_depth: int
 ):
     if max_depth == 0:
         return
     for i, (key, val) in enumerate(data.items()):
         if i >= max_length:
             if i < len(data) - 1:
-                print(indentation * "|", "...")
+                print(indentation * "|", "...")  # flake8: noqa T201
             return
         if isinstance(val, dict):
             if max_depth == 1:
-                print(indentation * "|", f"{key}: ...")
+                print(indentation * "|", f"{key}: ...")  # flake8: noqa T201
             else:
-                print(indentation * "|", f"{key}:")
+                print(indentation * "|", f"{key}:")  # flake8: noqa T201
                 _describe_data(val, indentation + 1, max_length, max_depth - 1)
         else:
             val_text = str(val)
             if len(val_text) > 80:
                 val_text = val_text[:77] + "..."
-            print(indentation * "|", f"{key}: {val_text}")
+            print(indentation * "|", f"{key}: {val_text}")  # flake8: noqa T201
 
 
 def describe(path: str):
     """
     Describe the benchmark by printing the first entry.
     """
 
-    print("An entry in the database can look like this:")
-    print("_____________________________________________")
+    print("An entry in the database can look like this:")  # flake8: noqa T201
+    print("_____________________________________________")  # flake8: noqa T201
     entry = Benchmark(path).front()
     if not entry:
         return
     _describe_data(entry, 0, 20, 5)
-    print("______________________________________________")
-    print(
+    print("______________________________________________")  # flake8: noqa T201
+    print(  # flake8: noqa T201
         "Note that this is only based on the first entry,"
         " other entries could differ."
     )
 
 
 def read_as_pandas(
-    path: str, row_creator: typing.Callable[[typing.Dict], typing.Dict]
+    path: str, row_creator: typing.Callable[[typing.Dict], typing.Optional[typing.Dict]]
 ) -> pd.DataFrame:
     """
     Read the benchmark as pandas table.
     For this, you have to tell the function, which data should
-    go into which column.
+    go into which column. If you want to skip an entry, return None (or an empty dict) in the row_creator.
 
     An example could look like this:
 
     .. code-block:: python
 
         t = read_as_pandas(
             "./03_benchmark_data/",
@@ -69,20 +69,26 @@
                 "colors": result["result"]["n_colors"],
                 "runtime": result["runtime"],
                 "num_vertices": result["result"]["num_vertices"],
                 "num_edges": result["result"]["num_edges"],
             },
         )
 
+    :param path: Path to the benchmark
+    :param row_creator: Function that creates a row from an entry
+    :return: Pandas DataFrame
     """
     data: typing.Dict[str, list] = {}
     n = 0
     benchmark = Benchmark(path)
     for entry in benchmark:
         row = row_creator(entry)
+        if not row:
+            # Skip entry
+            continue
         for key, value in row.items():
             if key not in data:
                 data[key] = n * []
             data[key].append(value)
             n += 1
         # Fill up missing entries with None
         for column in data:
```

### Comparing `AlgBench-2.1.0/src/algbench/utils/timer.py` & `AlgBench-2.2.0/src/algbench/utils/timer.py`

 * *Files identical despite different names*

### Comparing `AlgBench-2.1.0/tests/test_basics.py` & `AlgBench-2.2.0/tests/test_basics.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-from algbench import Benchmark, describe
 import logging
 
+from algbench import Benchmark, describe
+
+
 def test_simple():
     benchmark = Benchmark("./test_benchmark")
 
     def f(x, _test=2, default="default"):
         print(x)
         logging.getLogger("test").info("f(%d)", x)
         return {"r1": x, "r2": "test"}
```

### Comparing `AlgBench-2.1.0/tests/test_logger.py` & `AlgBench-2.2.0/tests/test_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-
 import logging
-from algbench import JsonLogHandler, JsonLogCapture
+
+from algbench import JsonLogCapture, JsonLogHandler
+
 
 def test_logger_basics():
     logger = logging.getLogger("test_logger")
     logger.setLevel(logging.DEBUG)
     json_log = JsonLogHandler()
     logger.addHandler(json_log)
     logger.info("test")
     assert len(json_log.get_entries()) == 1
     print(json_log.get_entries())
 
+
 def test_log_catcher():
     logger = logging.getLogger("test_logger")
     logger.setLevel(logging.ERROR)
     # The following case should catch the log, as we set the level to INFO
     with JsonLogCapture("test_logger", logging.INFO) as catcher:
         logger.info("test")
     assert len(catcher.get_entries()) == 1
     # The following case should not catch anything
     with JsonLogCapture("test_logger", logging.CRITICAL) as catcher:
         logger.info("test")
-    assert len(catcher.get_entries()) == 0
+    assert len(catcher.get_entries()) == 0
```

