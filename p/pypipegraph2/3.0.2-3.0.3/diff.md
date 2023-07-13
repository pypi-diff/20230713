# Comparing `tmp/pypipegraph2-3.0.2.tar.gz` & `tmp/pypipegraph2-3.0.3.tar.gz`

## Comparing `pypipegraph2-3.0.2.tar` & `pypipegraph2-3.0.3.tar`

### file list

```diff
@@ -1,122 +1,122 @@
--rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 pypipegraph2-3.0.2/Cargo.toml
--rw-r--r--   0     1001      123      595 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/.coveragerc
--rw-r--r--   0     1001      123     1231 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/.github/workflows/pytest.yml
--rw-r--r--   0     1001      123     1876 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/.github/workflows/release.yml
--rw-r--r--   0     1001      123      754 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/.gitignore
--rw-r--r--   0     1001      123      754 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/.gitignore.orig
--rw-r--r--   0     1001      123      106 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/.hgignore
--rw-r--r--   0     1001      123       30 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/.ppg/logs/runtimes.tsv
--rw-r--r--   0     1001      123       95 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/AUTHORS.rst
--rw-r--r--   0     1001      123      128 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/CHANGELOG.rst
--rw-r--r--   0     1001      123    13831 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/Cargo.lock
--rw-r--r--   0     1001      123     9569 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/README.md
--rwxr-xr-x   0     1001      123       55 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/bacon.sh
--rw-r--r--   0     1001      123      700 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/benches/bench1.rs
--rwxr-xr-x   0     1001      123      841 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/benchmarks/bench_disjoint.py
--rwxr-xr-x   0     1001      123      802 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/benchmarks/bench_kilo_jobs.py
--rwxr-xr-x   0     1001      123     1133 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/benchmarks/bench_simple.py
--rwxr-xr-x   0     1001      123      985 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/benchmarks/bench_tall.py
--rwxr-xr-x   0     1001      123      947 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/benchmarks/bench_wide.py
--rw-r--r--   0     1001      123     6315 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/designgoals.md
--rw-r--r--   0     1001      123     7618 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/docs/Makefile
--rw-r--r--   0     1001      123       18 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/docs/_static/.gitignore
--rw-r--r--   0     1001      123       41 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/docs/authors.rst
--rw-r--r--   0     1001      123       43 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/docs/changelog.rst
--rw-r--r--   0     1001      123     9264 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/docs/conf.py
--rw-r--r--   0     1001      123     2241 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/docs/index.rst
--rw-r--r--   0     1001      123       67 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/docs/license.rst
--rw-r--r--   0     1001      123    21307 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/examples/Basic_notebook.ipynb
--rw-r--r--   0     1001      123     1409 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/examples/abort_when_stalled.py
--rw-r--r--   0     1001      123     1120 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/examples/call_externals.py
--rw-r--r--   0     1001      123     1126 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/examples/long_for_interactive.py
--rw-r--r--   0     1001      123      260 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/examples/massive_exception.py
--rw-r--r--   0     1001      123      501 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/examples/nested_exception.py
--rw-r--r--   0     1001      123      563 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/examples/pandas_exception.py
--rw-r--r--   0     1001      123      506 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/examples/runtimes.py
--rw-r--r--   0     1001      123     5790 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/examples/simplest/simplest.py
--rw-r--r--   0     1001      123     1148 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/examples/slow_for_interactive.py
--rw-r--r--   0     1001      123     1241 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/examples/stall.py
--rw-r--r--   0     1001      123     1458 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/examples/stop_then_abort_when_stalled.py
--rw-r--r--   0     1001      123     1554 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/examples/stop_when_stalled.py
--rw-r--r--   0     1001      123     2533 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/flake.lock
--rw-r--r--   0     1001      123     6109 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/flake.nix
--rw-r--r--   0     1001      123  1650094 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/flame.svg
--rwxr-xr-x   0     1001      123      121 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/loop_cargo_test.sh
--rwxr-xr-x   0     1001      123      151 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/loop_main.sh
--rwxr-xr-x   0     1001      123      162 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/loop_ppg2_iterations_with_fail.sh
--rwxr-xr-x   0     1001      123      165 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/loop_ppg2_iterations_without_fail.sh
--rwxr-xr-x   0     1001      123       64 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/loop_pytest.sh
--rwxr-xr-x   0     1001      123      171 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/prep_for_tests.sh
--rw-r--r--   0     1001      123     1972 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/pyproject.toml
--rwxr-xr-x   0     1001      123     6124 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/__init__.py
--rw-r--r--   0     1001      123     3224 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/entry_points.py
--rw-r--r--   0     1001      123     1831 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/enums.py
--rw-r--r--   0     1001      123     1899 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/exceptions.py
--rwxr-xr-x   0     1001      123    28025 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/graph.py
--rw-r--r--   0     1001      123     1528 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/hashers.py
--rwxr-xr-x   0     1001      123     1466 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/history_comparisons.py
--rw-r--r--   0     1001      123    10730 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/interactive.py
--rwxr-xr-x   0     1001      123      843 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/job_status.py
--rwxr-xr-x   0     1001      123   112223 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/jobs.py
--rw-r--r--   0     1001      123     3408 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/parallel.py
--rw-r--r--   0     1001      123    18439 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/ppg1_compatibility.py
--rw-r--r--   0     1001      123     8513 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/ppg_traceback.py
--rwxr-xr-x   0     1001      123    40775 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/runner.py
--rw-r--r--   0     1001      123     2551 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/testing/__init__.py
--rw-r--r--   0     1001      123     9557 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/testing/fixtures.py
--rw-r--r--   0     1001      123     5217 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/python/pypipegraph2/util.py
--rwxr-xr-x   0     1001      123      806 2023-07-05 09:25:40.000000 pypipegraph2-3.0.2/run-maturin-action.sh
--rwxr-xr-x   0     1001      123      167 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/run_pytest.sh
--rw-r--r--   0     1001      123     1645 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/setup.cfg
--rw-r--r--   0     1001      123      557 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/setup.py
--rwxr-xr-x   0     1001      123    97038 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/src/engine.rs
--rwxr-xr-x   0     1001      123    19910 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/src/lib.rs
--rw-r--r--   0     1001      123     1009 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/src/main.rs
--rw-r--r--   0     1001      123    15543 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/src/main_iterations_with_fail.rs
--rw-r--r--   0     1001      123    10553 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/src/main_iterations_without_fail.rs
--rwxr-xr-x   0     1001      123    79221 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/src/tests.rs
--rw-r--r--   0     1001      123      209 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/t.py
--rw-r--r--   0     1001      123        0 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/__init__.py
--rw-r--r--   0     1001      123      282 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/_import_does_not_hang.py
--rw-r--r--   0     1001      123     4975 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/conftest.py
--rw-r--r--   0     1001      123      677 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/old_history_for_conversion_test.gz
--rw-r--r--   0     1001      123        0 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/__init__.py
--rw-r--r--   0     1001      123      965 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/shared.py
--rw-r--r--   0     1001      123    27757 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_cache_jobs.py
--rw-r--r--   0     1001      123     5840 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_compatibility_layer.py
--rw-r--r--   0     1001      123     3050 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_cycles.py
--rw-r--r--   0     1001      123    75082 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_invariants_and_depedencies.py
--rw-r--r--   0     1001      123    23004 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_job_gen_jobs.py
--rw-r--r--   0     1001      123    17831 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_other.py
--rw-r--r--   0     1001      123    21651 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_plotjobs.py
--rw-r--r--   0     1001      123     4365 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_prune.py
--rw-r--r--   0     1001      123     3196 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_simple.py
--rw-r--r--   0     1001      123     4792 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_util.py
--rw-r--r--   0     1001      123      927 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/shared.py
--rw-r--r--   0     1001      123    69648 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_basics.py
--rw-r--r--   0     1001      123     7374 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_bootstrap.py
--rw-r--r--   0     1001      123    14235 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_cache_jobs.py
--rw-r--r--   0     1001      123     1636 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_cycles.py
--rw-r--r--   0     1001      123      558 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_flake8.py
--rw-r--r--   0     1001      123     3366 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_function_invariants.py
--rw-r--r--   0     1001      123     2499 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_interactive.py
--rw-r--r--   0     1001      123    47281 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_invariants_and_dependencies.py
--rw-r--r--   0     1001      123    11292 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_job_generating_jobs.py
--rwxr-xr-x   0     1001      123    67423 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_jobs.py
--rw-r--r--   0     1001      123    21959 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_other.py
--rw-r--r--   0     1001      123     2616 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_parallel.py
--rw-r--r--   0     1001      123        2 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_parent_termination_kills_children/A
--rw-r--r--   0     1001      123      759 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_parent_termination_kills_children/manual.py
--rwxr-xr-x   0     1001      123       52 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_parent_termination_kills_children/sleeper.sh
--rw-r--r--   0     1001      123      977 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_parent_termination_kills_children/stage2.py
--rw-r--r--   0     1001      123    16239 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_plotjobs.py
--rw-r--r--   0     1001      123     2736 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_prune.py
--rw-r--r--   0     1001      123     1914 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_rust_conversion.py
--rw-r--r--   0     1001      123    23688 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_shared_jobs.py
--rw-r--r--   0     1001      123     1846 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_simple.py
--rw-r--r--   0     1001      123     3691 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_util.py
--rw-r--r--   0     1001      123      508 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/test_version.py
--rw-r--r--   0     1001      123    61338 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tests/tests_from_the_field.py
--rw-r--r--   0     1001      123     5453 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/todo.md
--rw-r--r--   0     1001      123      154 2023-07-05 09:25:10.000000 pypipegraph2-3.0.2/tox.ini
--rw-r--r--   0        0        0    11398 1970-01-01 00:00:00.000000 pypipegraph2-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 pypipegraph2-3.0.3/Cargo.toml
+-rw-r--r--   0     1001      123      595 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/.coveragerc
+-rw-r--r--   0     1001      123     1231 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/.github/workflows/pytest.yml
+-rw-r--r--   0     1001      123     1876 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/.github/workflows/release.yml
+-rw-r--r--   0     1001      123      754 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/.gitignore
+-rw-r--r--   0     1001      123      754 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/.gitignore.orig
+-rw-r--r--   0     1001      123      106 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/.hgignore
+-rw-r--r--   0     1001      123       30 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/.ppg/logs/runtimes.tsv
+-rw-r--r--   0     1001      123       95 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/AUTHORS.rst
+-rw-r--r--   0     1001      123      128 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/CHANGELOG.rst
+-rw-r--r--   0     1001      123    13831 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/Cargo.lock
+-rw-r--r--   0     1001      123     9569 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/README.md
+-rw-r--r--   0     1001      123     1363 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/Session.vim
+-rwxr-xr-x   0     1001      123       55 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/bacon.sh
+-rw-r--r--   0     1001      123      700 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/benches/bench1.rs
+-rwxr-xr-x   0     1001      123      841 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/benchmarks/bench_disjoint.py
+-rwxr-xr-x   0     1001      123      802 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/benchmarks/bench_kilo_jobs.py
+-rwxr-xr-x   0     1001      123     1133 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/benchmarks/bench_simple.py
+-rwxr-xr-x   0     1001      123      985 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/benchmarks/bench_tall.py
+-rwxr-xr-x   0     1001      123      947 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/benchmarks/bench_wide.py
+-rw-r--r--   0     1001      123     6315 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/designgoals.md
+-rw-r--r--   0     1001      123     7618 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/docs/Makefile
+-rw-r--r--   0     1001      123       18 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/docs/_static/.gitignore
+-rw-r--r--   0     1001      123       41 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/docs/authors.rst
+-rw-r--r--   0     1001      123       43 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/docs/changelog.rst
+-rw-r--r--   0     1001      123     9264 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/docs/conf.py
+-rw-r--r--   0     1001      123     2241 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/docs/index.rst
+-rw-r--r--   0     1001      123       67 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/docs/license.rst
+-rw-r--r--   0     1001      123    21307 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/examples/Basic_notebook.ipynb
+-rw-r--r--   0     1001      123     1409 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/examples/abort_when_stalled.py
+-rw-r--r--   0     1001      123     1120 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/examples/call_externals.py
+-rw-r--r--   0     1001      123     1126 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/examples/long_for_interactive.py
+-rw-r--r--   0     1001      123      260 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/examples/massive_exception.py
+-rw-r--r--   0     1001      123      501 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/examples/nested_exception.py
+-rw-r--r--   0     1001      123      563 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/examples/pandas_exception.py
+-rw-r--r--   0     1001      123      506 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/examples/runtimes.py
+-rw-r--r--   0     1001      123     5790 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/examples/simplest/simplest.py
+-rw-r--r--   0     1001      123     1148 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/examples/slow_for_interactive.py
+-rw-r--r--   0     1001      123     1241 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/examples/stall.py
+-rw-r--r--   0     1001      123     1458 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/examples/stop_then_abort_when_stalled.py
+-rw-r--r--   0     1001      123     1554 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/examples/stop_when_stalled.py
+-rw-r--r--   0     1001      123     2533 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/flake.lock
+-rw-r--r--   0     1001      123     6109 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/flake.nix
+-rw-r--r--   0     1001      123  1650094 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/flame.svg
+-rwxr-xr-x   0     1001      123      121 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/loop_cargo_test.sh
+-rwxr-xr-x   0     1001      123      151 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/loop_main.sh
+-rwxr-xr-x   0     1001      123      162 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/loop_ppg2_iterations_with_fail.sh
+-rwxr-xr-x   0     1001      123      165 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/loop_ppg2_iterations_without_fail.sh
+-rwxr-xr-x   0     1001      123       64 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/loop_pytest.sh
+-rwxr-xr-x   0     1001      123      171 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/prep_for_tests.sh
+-rw-r--r--   0     1001      123     1972 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/pyproject.toml
+-rwxr-xr-x   0     1001      123     6124 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/__init__.py
+-rw-r--r--   0     1001      123     3224 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/entry_points.py
+-rw-r--r--   0     1001      123     1831 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/enums.py
+-rw-r--r--   0     1001      123     1899 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/exceptions.py
+-rwxr-xr-x   0     1001      123    28025 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/graph.py
+-rw-r--r--   0     1001      123     1528 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/hashers.py
+-rwxr-xr-x   0     1001      123     2063 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/history_comparisons.py
+-rw-r--r--   0     1001      123    10730 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/interactive.py
+-rwxr-xr-x   0     1001      123      843 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/job_status.py
+-rwxr-xr-x   0     1001      123   112223 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/jobs.py
+-rw-r--r--   0     1001      123     3408 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/parallel.py
+-rw-r--r--   0     1001      123    18439 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/ppg1_compatibility.py
+-rw-r--r--   0     1001      123     8513 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/ppg_traceback.py
+-rwxr-xr-x   0     1001      123    40841 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/runner.py
+-rw-r--r--   0     1001      123     2551 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/testing/__init__.py
+-rw-r--r--   0     1001      123     9557 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/testing/fixtures.py
+-rw-r--r--   0     1001      123     5217 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/python/pypipegraph2/util.py
+-rwxr-xr-x   0     1001      123      167 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/run_pytest.sh
+-rw-r--r--   0     1001      123     1645 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/setup.cfg
+-rw-r--r--   0     1001      123      557 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/setup.py
+-rwxr-xr-x   0     1001      123   106720 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/src/engine.rs
+-rwxr-xr-x   0     1001      123    20032 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/src/lib.rs
+-rw-r--r--   0     1001      123     1009 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/src/main.rs
+-rw-r--r--   0     1001      123    15543 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/src/main_iterations_with_fail.rs
+-rw-r--r--   0     1001      123    10553 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/src/main_iterations_without_fail.rs
+-rwxr-xr-x   0     1001      123    91028 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/src/tests.rs
+-rw-r--r--   0     1001      123      209 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/t.py
+-rw-r--r--   0     1001      123        0 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/__init__.py
+-rw-r--r--   0     1001      123      282 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/_import_does_not_hang.py
+-rw-r--r--   0     1001      123     4975 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/conftest.py
+-rw-r--r--   0     1001      123      677 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/old_history_for_conversion_test.gz
+-rw-r--r--   0     1001      123        0 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/__init__.py
+-rw-r--r--   0     1001      123      965 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/shared.py
+-rw-r--r--   0     1001      123    27757 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_cache_jobs.py
+-rw-r--r--   0     1001      123     5840 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_compatibility_layer.py
+-rw-r--r--   0     1001      123     3050 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_cycles.py
+-rw-r--r--   0     1001      123    75082 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_invariants_and_depedencies.py
+-rw-r--r--   0     1001      123    23004 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_job_gen_jobs.py
+-rw-r--r--   0     1001      123    17831 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_other.py
+-rw-r--r--   0     1001      123    21651 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_plotjobs.py
+-rw-r--r--   0     1001      123     4365 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_prune.py
+-rw-r--r--   0     1001      123     3196 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_simple.py
+-rw-r--r--   0     1001      123     4792 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_util.py
+-rw-r--r--   0     1001      123      927 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/shared.py
+-rw-r--r--   0     1001      123    69648 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_basics.py
+-rw-r--r--   0     1001      123     7374 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_bootstrap.py
+-rw-r--r--   0     1001      123    14235 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_cache_jobs.py
+-rw-r--r--   0     1001      123     1636 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_cycles.py
+-rw-r--r--   0     1001      123      558 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_flake8.py
+-rw-r--r--   0     1001      123     3366 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_function_invariants.py
+-rw-r--r--   0     1001      123     2499 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_interactive.py
+-rw-r--r--   0     1001      123    47281 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_invariants_and_dependencies.py
+-rw-r--r--   0     1001      123    11292 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_job_generating_jobs.py
+-rwxr-xr-x   0     1001      123    67423 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_jobs.py
+-rw-r--r--   0     1001      123    22839 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_other.py
+-rw-r--r--   0     1001      123     2616 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_parallel.py
+-rw-r--r--   0     1001      123        2 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_parent_termination_kills_children/A
+-rw-r--r--   0     1001      123      759 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_parent_termination_kills_children/manual.py
+-rwxr-xr-x   0     1001      123       52 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_parent_termination_kills_children/sleeper.sh
+-rw-r--r--   0     1001      123      977 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_parent_termination_kills_children/stage2.py
+-rw-r--r--   0     1001      123    16239 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_plotjobs.py
+-rw-r--r--   0     1001      123     2736 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_prune.py
+-rw-r--r--   0     1001      123     1914 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_rust_conversion.py
+-rw-r--r--   0     1001      123    23688 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_shared_jobs.py
+-rw-r--r--   0     1001      123     1846 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_simple.py
+-rw-r--r--   0     1001      123     3691 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_util.py
+-rw-r--r--   0     1001      123      507 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/test_version.py
+-rw-r--r--   0     1001      123    61338 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tests/tests_from_the_field.py
+-rw-r--r--   0     1001      123     5453 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/todo.md
+-rw-r--r--   0     1001      123      154 2023-07-13 14:05:11.000000 pypipegraph2-3.0.3/tox.ini
+-rw-r--r--   0        0        0    11398 1970-01-01 00:00:00.000000 pypipegraph2-3.0.3/PKG-INFO
```

### Comparing `pypipegraph2-3.0.2/Cargo.toml` & `pypipegraph2-3.0.3/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pypipegraph2"
-version = "3.0.2"
+version = "3.0.3"
 edition = "2018"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pypipegraph2"
 crate-type = ["cdylib", "rlib"]
```

### Comparing `pypipegraph2-3.0.2/.coveragerc` & `pypipegraph2-3.0.3/.coveragerc`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/.github/workflows/pytest.yml` & `pypipegraph2-3.0.3/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/.github/workflows/release.yml` & `pypipegraph2-3.0.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/.gitignore` & `pypipegraph2-3.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/.gitignore.orig` & `pypipegraph2-3.0.3/.gitignore.orig`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/Cargo.lock` & `pypipegraph2-3.0.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -385,15 +385,15 @@
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pypipegraph2"
-version = "3.0.2"
+version = "3.0.3"
 dependencies = [
  "backtrace",
  "colored",
  "env_logger",
  "itertools",
  "log",
  "num_cpus",
```

### Comparing `pypipegraph2-3.0.2/README.md` & `pypipegraph2-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/benches/bench1.rs` & `pypipegraph2-3.0.3/benches/bench1.rs`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/benchmarks/bench_disjoint.py` & `pypipegraph2-3.0.3/benchmarks/bench_disjoint.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/benchmarks/bench_kilo_jobs.py` & `pypipegraph2-3.0.3/benchmarks/bench_kilo_jobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/benchmarks/bench_simple.py` & `pypipegraph2-3.0.3/benchmarks/bench_simple.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/benchmarks/bench_tall.py` & `pypipegraph2-3.0.3/benchmarks/bench_tall.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/benchmarks/bench_wide.py` & `pypipegraph2-3.0.3/benchmarks/bench_wide.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/designgoals.md` & `pypipegraph2-3.0.3/designgoals.md`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/docs/Makefile` & `pypipegraph2-3.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/docs/conf.py` & `pypipegraph2-3.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/docs/index.rst` & `pypipegraph2-3.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/examples/Basic_notebook.ipynb` & `pypipegraph2-3.0.3/examples/Basic_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/examples/abort_when_stalled.py` & `pypipegraph2-3.0.3/examples/abort_when_stalled.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/examples/call_externals.py` & `pypipegraph2-3.0.3/examples/call_externals.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/examples/long_for_interactive.py` & `pypipegraph2-3.0.3/examples/long_for_interactive.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/examples/pandas_exception.py` & `pypipegraph2-3.0.3/examples/pandas_exception.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/examples/simplest/simplest.py` & `pypipegraph2-3.0.3/examples/simplest/simplest.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/examples/slow_for_interactive.py` & `pypipegraph2-3.0.3/examples/slow_for_interactive.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/examples/stall.py` & `pypipegraph2-3.0.3/examples/stall.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/examples/stop_then_abort_when_stalled.py` & `pypipegraph2-3.0.3/examples/stop_then_abort_when_stalled.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/examples/stop_when_stalled.py` & `pypipegraph2-3.0.3/examples/stop_when_stalled.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/flake.lock` & `pypipegraph2-3.0.3/flake.lock`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/flake.nix` & `pypipegraph2-3.0.3/flake.nix`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/flame.svg` & `pypipegraph2-3.0.3/flame.svg`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/pyproject.toml` & `pypipegraph2-3.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.12,<0.13"]
 build-backend = "maturin"
 
 [project]
 name = "pypipegraph2"
-version = "3.0.2"
+version = "3.0.3"
 description = "Advanced python 'what changed and what do we need to do' tracking"
 long-description = "README.md"
 authors = [
  {"name" = "Florian Finkernagel", "email" = "finkernagel@imt.uni-marburg.de"}
 ]
 classifiers = [
 	"Development Status :: 4 - Beta",
```

### Comparing `pypipegraph2-3.0.2/python/pypipegraph2/__init__.py` & `pypipegraph2-3.0.3/python/pypipegraph2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "3.0.2"
+__version__ = "3.0.3"
 
 from pathlib import Path
 import logging
 import contextlib
 from .graph import PyPipeGraph, ALL_CORES
 from .jobs import (
     FileGeneratingJob,
```

### Comparing `pypipegraph2-3.0.2/python/pypipegraph2/entry_points.py` & `pypipegraph2-3.0.3/python/pypipegraph2/entry_points.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/python/pypipegraph2/enums.py` & `pypipegraph2-3.0.3/python/pypipegraph2/enums.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/python/pypipegraph2/exceptions.py` & `pypipegraph2-3.0.3/python/pypipegraph2/exceptions.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/python/pypipegraph2/graph.py` & `pypipegraph2-3.0.3/python/pypipegraph2/graph.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/python/pypipegraph2/hashers.py` & `pypipegraph2-3.0.3/python/pypipegraph2/hashers.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/python/pypipegraph2/history_comparisons.py` & `pypipegraph2-3.0.3/python/pypipegraph2/history_comparisons.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,28 +12,39 @@
 def history_is_different(runner, job_upstream_id, job_downstream_id, str_last, str_now):
     # note that at this point, we already know str_last != str_now,
     # that was tested in rust
     # log_error(f"history is maybe different {job_upstream_id} {job_downstream_id} {str_last == str_now}")
     job_upstream = runner.jobs[job_upstream_id]
     obj_last = json.loads(str_last)
     obj_now = json.loads(str_now)
-    try:
+    if job_downstream_id == "!!!":
+        # special case where we compare a job to itself, not to the input it delivered into another job.
+        # Has to do with ephemeral jobs not changing output when validated-but-rerun.
         outputs = job_upstream.outputs
-        inputs = runner.job_inputs[job_downstream_id]
-        for ip in inputs:
-            if ip in outputs:
-                altered = not job_upstream.compare_hashes(obj_last[ip], obj_now[ip])
-                if altered:
-                    log_error(
-                        f"history is actually different {obj_last[ip]} {obj_now[ip]}"
-                    )
-                    return True
-    except:  # noqa: E722 yes we really want to capture and reraise *everything*
-        exception_type, exception_value, tb = sys.exc_info()
-        captured_tb = ppg_traceback.Trace(exception_type, exception_value, tb)
-        log_error(f"old was {str_last}")
-        log_error(f"now was {str_now}")
-        log_error(f"{captured_tb}")
-        raise
+        for ip in outputs:
+            altered = not job_upstream.compare_hashes(obj_last[ip], obj_now[ip])
+            if altered:
+                log_error(f"history is actually different {obj_last[ip]} {obj_now[ip]}")
+                return True
+
+    else:
+        try:
+            outputs = job_upstream.outputs
+            inputs = runner.job_inputs[job_downstream_id]
+            for ip in inputs:
+                if ip in outputs:
+                    altered = not job_upstream.compare_hashes(obj_last[ip], obj_now[ip])
+                    if altered:
+                        log_error(
+                            f"history is actually different {obj_last[ip]} {obj_now[ip]}"
+                        )
+                        return True
+        except:  # noqa: E722 yes we really want to capture and reraise *everything*
+            exception_type, exception_value, tb = sys.exc_info()
+            captured_tb = ppg_traceback.Trace(exception_type, exception_value, tb)
+            log_error(f"old was {str_last}")
+            log_error(f"now was {str_now}")
+            log_error(f"{captured_tb}")
+            raise
 
     # log_error(f"history the same {job_upstream_id} {job_downstream_id}")
     return False
```

### Comparing `pypipegraph2-3.0.2/python/pypipegraph2/interactive.py` & `pypipegraph2-3.0.3/python/pypipegraph2/interactive.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/python/pypipegraph2/job_status.py` & `pypipegraph2-3.0.3/python/pypipegraph2/job_status.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/python/pypipegraph2/jobs.py` & `pypipegraph2-3.0.3/python/pypipegraph2/jobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/python/pypipegraph2/parallel.py` & `pypipegraph2-3.0.3/python/pypipegraph2/parallel.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/python/pypipegraph2/ppg1_compatibility.py` & `pypipegraph2-3.0.3/python/pypipegraph2/ppg1_compatibility.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/python/pypipegraph2/ppg_traceback.py` & `pypipegraph2-3.0.3/python/pypipegraph2/ppg_traceback.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/python/pypipegraph2/runner.py` & `pypipegraph2-3.0.3/python/pypipegraph2/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -463,14 +463,16 @@
             for job_id in global_pipegraph.jobs:
                 if job_id not in self.jobs:
                     log_job_trace(f"new job {job_id}")
             raise _RunAgain(
                 (self.job_outcomes, self.evaluator.new_history())
             )  # self.job_states)
         log_trace("Left runner.run()")
+        if self.aborted:
+            self.evaluator.event_abort()
 
         return self.job_outcomes, self.evaluator.new_history()
 
     def _interactive_start(self):
         """Activate the interactive thread"""
         if self.job_graph.run_mode is RunMode.CONSOLE:
             self.interactive = ConsoleInteractive()
```

### Comparing `pypipegraph2-3.0.2/python/pypipegraph2/testing/__init__.py` & `pypipegraph2-3.0.3/python/pypipegraph2/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/python/pypipegraph2/testing/fixtures.py` & `pypipegraph2-3.0.3/python/pypipegraph2/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/python/pypipegraph2/util.py` & `pypipegraph2-3.0.3/python/pypipegraph2/util.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/setup.cfg` & `pypipegraph2-3.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 [metadata]
 name = pypipegraph2
 description = Advanced python 'what changed and what do we need to do' tracking
-version = 3.0.2
+version = 3.0.3
 author = Florian Finkernagel
 author-email = finkernagel@imt.uni-marburg.de
 license = mit
 long-description = file: README.md
 long-description-content-type = text/markdown; charset=UTF-8
 url = https://github.com/pyscaffold/pyscaffold/
 project-urls =
```

### Comparing `pypipegraph2-3.0.2/setup.py` & `pypipegraph2-3.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/src/engine.rs` & `pypipegraph2-3.0.3/src/engine.rs`

 * *Files 3% similar despite different names*

```diff
@@ -45,25 +45,27 @@
 pub enum JobStateAlways {
     Undetermined,
     ReadyToRun, // ie. upstreams done.
     Running,
     FinishedSuccess,
     FinishedFailure,
     FinishedUpstreamFailure,
+    FinishedAborted,
 }
 
 #[derive(Copy, Clone, Debug, PartialEq, Eq)]
 pub enum JobStateOutput {
     NotReady(ValidationStatus),
     ReadyToRun,
     Running,
     FinishedSuccess,
     FinishedFailure,
     FinishedUpstreamFailure,
     FinishedSkipped,
+    FinishedAborted,
 }
 
 #[derive(Copy, Clone, Debug, PartialEq, Eq)]
 pub enum JobStateEphemeral {
     NotReady(ValidationStatus),
     ReadyButDelayed, //ie. we have not made a decision on whether this is a go or not.
     ReadyToRun(ValidationStatus),
@@ -71,14 +73,15 @@
     FinishedSuccessNotReadyForCleanup,
     FinishedSuccessReadyForCleanup,
     FinishedSuccessCleanedUp,
     FinishedSuccessSkipCleanup,
     FinishedFailure,
     FinishedUpstreamFailure,
     FinishedSkipped,
+    FinishedAborted,
 }
 
 #[derive(Copy, Clone, Debug, PartialEq, Eq)]
 pub enum JobState {
     Always(JobStateAlways),
     Output(JobStateOutput),
     Ephemeral(JobStateEphemeral),
@@ -115,21 +118,24 @@
         match self {
             JobStateAlways::Undetermined => false,
             JobStateAlways::ReadyToRun => false,
             JobStateAlways::Running => false,
             JobStateAlways::FinishedSuccess => true,
             JobStateAlways::FinishedFailure => true,
             JobStateAlways::FinishedUpstreamFailure => true,
+            JobStateAlways::FinishedAborted => true,
         }
     }
 
     fn is_failed(&self) -> bool {
         matches!(
             self,
-            JobStateAlways::FinishedFailure | JobStateAlways::FinishedUpstreamFailure
+            JobStateAlways::FinishedFailure
+                | JobStateAlways::FinishedUpstreamFailure
+                | JobStateAlways::FinishedAborted
         )
     }
 
     fn is_skipped(&self) -> bool {
         false
     }
 }
@@ -139,21 +145,24 @@
             JobStateOutput::NotReady(_) => false,
             JobStateOutput::ReadyToRun => false,
             JobStateOutput::Running => false,
             JobStateOutput::FinishedSuccess => true,
             JobStateOutput::FinishedFailure => true,
             JobStateOutput::FinishedUpstreamFailure => true,
             JobStateOutput::FinishedSkipped => true,
+            JobStateOutput::FinishedAborted => true,
         }
     }
 
     fn is_failed(&self) -> bool {
         matches!(
             self,
-            JobStateOutput::FinishedFailure | JobStateOutput::FinishedUpstreamFailure
+            JobStateOutput::FinishedFailure
+                | JobStateOutput::FinishedUpstreamFailure
+                | JobStateOutput::FinishedAborted
         )
     }
 
     fn is_skipped(&self) -> bool {
         matches!(self, JobStateOutput::FinishedSkipped)
     }
 }
@@ -168,21 +177,24 @@
             JobStateEphemeral::FinishedSuccessNotReadyForCleanup => true,
             JobStateEphemeral::FinishedSuccessReadyForCleanup => true,
             JobStateEphemeral::FinishedSuccessCleanedUp => true,
             JobStateEphemeral::FinishedSuccessSkipCleanup => true,
             JobStateEphemeral::FinishedFailure => true,
             JobStateEphemeral::FinishedUpstreamFailure => true,
             JobStateEphemeral::FinishedSkipped => true,
+            JobStateEphemeral::FinishedAborted => true,
         }
     }
 
     fn is_failed(&self) -> bool {
         matches!(
             self,
-            JobStateEphemeral::FinishedFailure | JobStateEphemeral::FinishedUpstreamFailure
+            JobStateEphemeral::FinishedFailure
+                | JobStateEphemeral::FinishedUpstreamFailure
+                | JobStateEphemeral::FinishedAborted
         )
     }
 
     fn is_skipped(&self) -> bool {
         matches!(self, JobStateEphemeral::FinishedSkipped,)
     }
 }
@@ -250,14 +262,15 @@
     JobFinishedSkip,
     JobDone,
     JobFinishedSuccess,
     JobFinishedFailure,
     JobUpstreamFailure,
     ConsiderJob,
     JobCleanedUp,
+    JobAborted,
 }
 
 impl Signal {
     fn job_id<'a>(&self, jobs: &'a [NodeInfo]) -> &'a str {
         &jobs[self.node_idx as usize].job_id
     }
 }
@@ -423,14 +436,35 @@
             EdgeInfo {
                 required: Required::Unknown,
                 invalidated: Required::Unknown,
             },
         );
     }
 
+    pub fn abort_remaining(&mut self) -> Result<(), PPGEvaluatorError> {
+        let mut signal_failure = Vec::new();
+
+        let mut new_signals: Vec<Signal> = Vec::new();
+
+        for (job_idx, job) in self.jobs.iter_mut().enumerate() {
+            if !job.state.is_finished() {
+                dbg!("Declaring upstream failure", job);
+                signal_failure.push(job_idx);
+            }
+        }
+
+        for job_idx in signal_failure {
+            new_signals.push(NewSignal!(SignalKind::JobAborted, job_idx, self.jobs));
+        }
+        self.signals.extend(new_signals);
+        self.process_signals(0)?;
+        self.is_finished();
+        Ok(())
+    }
+
     pub fn is_finished(&mut self) -> bool {
         match self.already_started {
             StartStatus::NotStarted => false,
             StartStatus::Finished => true,
             StartStatus::Running => {
                 for job in self.jobs.iter() {
                     if !job.state.is_finished() {
@@ -617,18 +651,21 @@
             if !Self::_job_and_downstreams_are_ephemeral(dag, jobs, ds_id) {
                 return false;
             }
         }
         true
     }
     pub fn new_history(&self) -> Result<HashMap<String, String>, PPGEvaluatorError> {
-        /* if !self.is_finished() {
-            debug!("{}", Self::debug(&self.dag, &self.jobs));
-            panic!("Graph wasn't finished, not handing out history..."); // todo: actually, why not, we could save history occasionally?
-        } */
+        match self.already_started {
+            StartStatus::Finished => {}
+            _ => {
+                debug!("{}", Self::debug(&self.dag, &self.jobs));
+                panic!("Graph wasn't finished, not handing out history..."); // todo: actually, why not, we could save history occasionally?
+            }
+        }
         //our history 'keys'
         //(we can't do tuple indices because of json dumping)
         //no !!! -> job output.
         //ends with !!! -> the list of named inputs
         //x!!!y -> input x for job y.
         //todo: consider splitting into multiple functions?
         let mut multi_output_job_filtered_outputs = HashSet::new();
@@ -692,14 +729,16 @@
             .collect();
 
         for (idx, job) in self.jobs.iter().enumerate() {
             //step 1: record what jobs when into this one
 
             //step 2: record the actual output of this job
             // (are we using this anywhere?)
+            // We're not for checking-the-ephemeral-invariant-upholding,
+            // for that we use the ones stored on the downstream jobs.
 
             let key = job.job_id.to_string();
             let job_was_success = job.history_output.is_some();
             let input_name_key = format!("{}!!!", job.job_id);
             if job_was_success {
                 // if the job did not succeed, we want it to rerun!
                 out.insert(
@@ -735,16 +774,21 @@
             } else {
                 // the job did not finish.
                 // and by throwing away the history, we make sure it's
                 // rerun on the next round.
                 //
                 // but if it failed because of upstream failure,
                 // we need to *keep* the history.
+                //
+                //
+                // is this not a problem on abort?
+                // no abort fails the currently running jobs (external, python does that)
 
                 // paranoia...
+                dbg!(&job);
                 assert!(
                     job.state.is_failed()
                         || Self::_job_and_downstreams_are_ephemeral(&self.dag, &self.jobs, idx)
                 );
                 if !job.state.is_upstream_failure() {
                     out.remove(&job.job_id);
                     out.remove(&input_name_key);
@@ -944,16 +988,90 @@
                 return Err(PPGEvaluatorError::APIError(format!(
                     "Reported a job as finished that was not running ! {:?}",
                     j
                 )))
             }
         }
         if j.state == JobState::Ephemeral(JobStateEphemeral::Running(ValidationStatus::Validated)) {
+            // changing your output when you were Validated is not allowed.
+            // We the the job-output history, not the one on the downstreams
+            // because those might be actually different, if the upstream epehemeral had run
+            // and we had aborted/failed the downstreams in a previous run,
+            // and this turn it's then obvs validated, but the downstreams do no longer match.
+            //
+            // We have to query the  downstream jobs though if it is really different
+            // for history_is_different on the python side only considers those outputs
+            // that are then again inputs for the downstream jobs.
+            // (side-effect: if it changes in an output that's not used by any downstream,
+            // this would not trigger.
+            // It's an unlikely problem, and I currently don't see how to work around it.
+            // witohut turning the downstream_job_id into a magic value that means 'check all the
+            // outputs (we need the upstream job to know what comparison to use)
+            //
+            let hist_key = &j.job_id;
+            if let Some(job_history) = self.history.get(hist_key) {
+                // we have to check for actually altered history.
+                // the timestamp may change, but the hash not...
+                // any would do
+                if self
+                    .strategy
+                    .is_history_altered(job_id, "!!!", job_history, &history_to_store)
+                {
+                    self.signals.push_back(NewSignal!(
+                        SignalKind::JobFinishedFailure,
+                        node_idx,
+                        self.jobs
+                    ));
+                    let my_err = PPGEvaluatorError::EphemeralChangedOutput {
+                        job_id: j.job_id.clone(),
+                        last_history: job_history.to_string(),
+                        new_history: history_to_store,
+                    };
+                    self.process_signals(0)?;
+                    return Err(my_err);
+                }
+            }
+
+            /*
             let downstreams = self.dag.neighbors_directed(node_idx, Direction::Outgoing);
             for downstream_idx in downstreams {
+                debug!(
+                    "Ephemeral {} finished, downstream {} is now ready to run. Downstream state was {:?}",
+                    job_id, self.jobs[downstream_idx as usize].job_id
+                    , self.jobs[downstream_idx as usize].state
+                );
+                match self.jobs[downstream_idx].state {
+                    JobState::Always(_) => {}
+                    JobState::Output(jo) => match jo {
+                        JobStateOutput::NotReady(v) => match v {
+                            ValidationStatus::Unknown => {}, //
+                            ValidationStatus::Validated => {} // to the chekc.
+                            ValidationStatus::Invalidated => continue,
+                        },
+                        JobStateOutput::FinishedSkipped => continue,
+                        JobStateOutput::FinishedUpstreamFailure => continue,
+                        x => panic!("Should not happen: {:?}", x),
+                    },
+                    JobState::Ephemeral(je) => match je {
+                        JobStateEphemeral::NotReady(v) => match v {
+                            ValidationStatus::Unknown => {},
+                            ValidationStatus::Validated => {}
+                            ValidationStatus::Invalidated => continue,
+                        },
+                        JobStateEphemeral::ReadyButDelayed => continue,
+                        JobStateEphemeral::ReadyToRun(v) => match v {
+                            ValidationStatus::Unknown => panic!("Should not happen"),
+                            ValidationStatus::Validated => {}
+                            ValidationStatus::Invalidated => continue,
+                        },
+                        JobStateEphemeral::FinishedSkipped => continue,
+                        JobStateEphemeral::FinishedUpstreamFailure => continue,
+                        _ => panic!("Should not happen"),
+                    },
+                }
                 let hist_key = format!(
                     "{}!!!{}",
                     j.job_id, &self.jobs[downstream_idx as usize].job_id
                 );
                 if let Some(downstream_history) = self.history.get(&hist_key) {
                     // we have to check for actually altered history.
                     // the timestamp may change, but the hash not...
@@ -974,14 +1092,15 @@
                             new_history: history_to_store,
                         };
                         self.process_signals(0)?;
                         return Err(my_err);
                     }
                 }
             }
+            */
         }
 
         let j = &mut self.jobs[node_idx as usize];
         j.history_output = Some(history_to_store);
 
         self.signals.push_back(NewSignal!(
             SignalKind::JobFinishedSuccess,
@@ -1362,15 +1481,15 @@
                         &self.strategy,
                         &mut self.dag,
                         &mut self.jobs,
                         &self.history,
                         node_idx,
                         &mut new_signals,
                         &mut self.gen,
-                        &mut ignore_consider_signals
+                        &mut ignore_consider_signals,
                     )?;
                 }
                 SignalKind::JobCleanedUp => {
                     let j = &mut self.jobs[node_idx as usize];
                     match j.state {
                         JobState::Ephemeral(JobStateEphemeral::FinishedSuccessReadyForCleanup) => {
                             set_node_state!(
@@ -1384,14 +1503,42 @@
                             return Err(PPGEvaluatorError::InternalError(format!(
                                 "unexpected was 8 {:?}",
                                 j
                             )))
                         }
                     }
                 }
+                SignalKind::JobAborted => {
+                    let j = &mut self.jobs[node_idx as usize];
+                    if !j.state.is_finished() {
+                        match j.state {
+                            JobState::Ephemeral(_) => {
+                                set_node_state!(
+                                    j,
+                                    JobState::Ephemeral(JobStateEphemeral::FinishedAborted),
+                                    self.gen
+                                );
+                            }
+                            JobState::Output(_) => {
+                                set_node_state!(
+                                    j,
+                                    JobState::Output(JobStateOutput::FinishedAborted),
+                                    self.gen
+                                );
+                            }
+                            JobState::Always(_) => {
+                                set_node_state!(
+                                    j,
+                                    JobState::Always(JobStateAlways::FinishedAborted),
+                                    self.gen
+                                );
+                            }
+                        }
+                    }
+                }
             }
         }
         if !new_signals.is_empty() {
             debug!("New signals after process_signals - adding and processing");
             for s in new_signals.into_iter() {
                 debug!("\t {:?} {}", s, s.job_id(&self.jobs));
                 self.signals.push_back(s);
@@ -1679,14 +1826,53 @@
                         ValidationStatus::Validated,
                     )))
             {
                 // a validated ephemeral, can, even if it runs,
                 // not invalidate a downstream.
                 // If it produces a changed output,
                 // that's a job contract failure.
+                //
+                // But! If it ran previously, produced a different output,
+                // and we did not run the downstream job to completion (abort, possibly failure?)
+                // Then it can invalidate the downstream job!
+                //
+                //TODO
+                let upstream_historical_output =
+                    history.get(&jobs[upstream_idx].job_id).ok_or_else(|| {
+                        PPGEvaluatorError::InternalError(
+                            "Should have had history for it, if it was validated?!".to_string(),
+                        )
+                    })?;
+                let my_historical_input = history.get(&format!(
+                    "{}!!!{}",
+                    &jobs[upstream_idx].job_id, &jobs[node_idx].job_id
+                ));
+                match my_historical_input {
+                    None => {
+                        //no history, so certainly invalidated
+                        debug!(
+                            "edge invalidated: No history for {}->{}",
+                            &jobs[upstream_idx].job_id, &jobs[node_idx].job_id
+                        );
+                        invalidated = true;
+                    }
+                    Some(my_historical_input) => {
+                        if upstream_historical_output != my_historical_input {
+                            debug!("edge invalidated by epheremeral changed in prev run: History for {}->{} changed",
+                                   &jobs[upstream_idx].job_id,
+                                   &jobs[node_idx].job_id);
+                            invalidated = true;
+                            dag.edge_weight_mut(upstream_idx, node_idx)
+                                .unwrap()
+                                .required = Required::Yes;
+                        } else {
+                            continue;
+                        }
+                    }
+                }
             } else if jobs[upstream_idx as usize].state
                 == JobState::Output(JobStateOutput::NotReady(ValidationStatus::Validated))
             {
                 //neither can an output job that is validated
             } else {
                 debug!(
                     "\t\t edge Counted as not done {} {}",
@@ -1944,14 +2130,28 @@
                                 jobs[node_idx as usize],
                                 JobState::Ephemeral(JobStateEphemeral::NotReady(solid_vs),),
                                 gen
                             );
                             // not the most elegant control flow, but ok.
                             //
                             reconsider_job!(jobs, node_idx, new_signals, gen.get());
+                            if let ValidationStatus::Invalidated = solid_vs {
+                                //this happens when we did not run the ephemeral last time
+                                //(aborted),
+                                //but would have had to run it due to invalidation.
+                                //and now it's invalidated again, but we have to tell the upstream
+                                //ephemerals
+                                Self::reconsider_ephemeral_upstreams(
+                                    dag,
+                                    jobs,
+                                    node_idx,
+                                    new_signals,
+                                    gen,
+                                );
+                            }
                         }
                     }
                 }
                 _ => {}
             },
         }
```

### Comparing `pypipegraph2-3.0.2/src/lib.rs` & `pypipegraph2-3.0.3/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -582,14 +582,19 @@
     }
 
     pub fn reconsider_all_jobs(&mut self) -> Result<(), PyErr> {
         error!("Reconsidering all jobs!");
         self.evaluator.reconsider_all_jobs()?;
         Ok(())
     }
+
+    pub fn event_abort(&mut self) -> Result<(), PyErr> {
+        self.evaluator.abort_remaining()?;
+        Ok(())
+    }
 }
 
 /// Formats the sum of two numbers as string.
 #[pyfunction]
 fn enable_logging() -> PyResult<()> {
     start_logging();
     error!("hello from rust");
```

### Comparing `pypipegraph2-3.0.2/src/main.rs` & `pypipegraph2-3.0.3/src/main.rs`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/src/main_iterations_with_fail.rs` & `pypipegraph2-3.0.3/src/main_iterations_with_fail.rs`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/src/main_iterations_without_fail.rs` & `pypipegraph2-3.0.3/src/main_iterations_without_fail.rs`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/src/tests.rs` & `pypipegraph2-3.0.3/src/tests.rs`

 * *Files 15% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 fn test_one_output() {
     fn create_graph(g: &mut PPGEvaluator<StrategyForTesting>) {
         g.add_node("A", JobKind::Output);
     }
     let mut ro = TestGraphRunner::new(Box::new(create_graph));
     let g = ro.run(&Vec::new()).unwrap();
     let new_history = g.new_history().unwrap();
-    dbg!(&new_history);
     assert!(new_history.contains_key("A"));
     assert!(ro.run_counters.get("A") == Some(&1));
     error!("Run again");
     let g = ro.run(&Vec::new()).unwrap();
     assert!(ro.run_counters.get("A") == Some(&1));
 }
 
@@ -445,14 +444,15 @@
         already_done.borrow_mut().insert("B".to_string());
         assert_eq!(g.query_ready_to_run(), set!["C"]);
         g.event_now_running("C").unwrap();
         assert!(g.query_ready_to_run().is_empty());
         g.event_job_finished_success("C", "histC".to_string())
             .unwrap();
         already_done.borrow_mut().insert("C".to_string());
+        g.abort_remaining().unwrap();
         g.new_history().unwrap()
     };
     error!("part 2");
 
     {
         let mut g2 = init(history.clone());
         g2.event_startup().unwrap();
@@ -1507,17 +1507,19 @@
         g.depends_on("C", "TA"); // so this retrigers
     }
 
     ro.setup_graph = Box::new(create_graph2);
     ro.outputs.insert("TA".to_string(), "changed".to_string());
 
     error!("part2");
+    start_logging();
     let g = ro.run(&Vec::new()).unwrap();
     assert!(ro.run_counters.get("TA") == Some(&2));
     let failed = g.query_failed();
+    dbg!(&failed);
     assert!(failed.contains("TA"));
     assert!(failed.len() == 1);
     let upstream_failed = g.query_upstream_failed();
     assert!(upstream_failed.contains("B"));
     assert!(upstream_failed.contains("C"));
     assert!(upstream_failed.len() == 2);
     // an ephemeral must not change it's output
@@ -1781,15 +1783,14 @@
     let g = ro.run(&[]).unwrap();
     let history = g.new_history().unwrap();
     assert!(history.contains_key("A"));
     assert!(history.contains_key("B"));
     assert!(history.contains_key("C"));
     assert!(history.contains_key("D:E:F"));
 
-    //start_logging_to_file("shu.txt");
     ro.already_done.remove("A");
     let g = ro.run(&["A"]).unwrap();
     assert!(g.query_failed().len() == 1);
     let history = g.new_history().unwrap();
     assert!(history.contains_key("B"));
     assert!(history.contains_key("C"));
 
@@ -1919,15 +1920,14 @@
         g.depends_on("N3", "N1");
         g.depends_on("N4", "N1");
         g.depends_on("N3", "N2");
         g.depends_on("N4", "N3");
     }
     let mut ro = TestGraphRunner::new(Box::new(create_graph));
     let g = ro.run(&[]).unwrap();
-    start_logging_to_file("debug.log");
     let g = ro.run(&[]).unwrap();
 }
 
 #[test]
 fn test_fuzz_4() {
     //always can go from undetermined to ready to run when it's getting validated
     fn create_graph(g: &mut PPGEvaluator<StrategyForTesting>) {
@@ -1985,15 +1985,14 @@
         }
     }
     let mut ro = TestGraphRunner::new(Box::new(create_graph));
     let g = ro.run(&[]).unwrap();
     ro.setup_graph = Box::new(create_graph2);
 
     let fails = ["N0"];
-    start_logging();
     let g = ro
         .run(&fails)
         .map_err(|x| {
             dbg!(&x);
             x
         })
         .unwrap();
@@ -2064,15 +2063,14 @@
                 g.depends_on(a, b);
             }
         }
     }
 
     let mut ro = TestGraphRunner::new(Box::new(create_graph));
     let g = ro.run(&[]).unwrap();
-    start_logging();
     let g = ro.run(&[]).unwrap();
 }
 
 #[test]
 fn test_fuzz_8() {
     fn create_graph(g: &mut PPGEvaluator<StrategyForTesting>) {
         g.add_node("N0", JobKind::Ephemeral);
@@ -2229,15 +2227,14 @@
         ];
         for (a, b) in edges {
             if g.contains_node(a) && g.contains_node(b) {
                 g.depends_on(a, b);
             }
         }
     }
-    start_logging();
 
     ro.setup_graph = Box::new(create_graph2);
     let g = ro.run(&["N1"]).unwrap();
 }
 
 #[test]
 fn test_fuzz_11() {
@@ -2290,14 +2287,283 @@
             }
         }
     }
 
     ro.setup_graph = Box::new(create_graph2);
     let g = ro.run(&["N0"]).unwrap();
 }
+#[test]
+fn test_aborting_inbetween_jobs() {
+    fn create_graph(g: &mut PPGEvaluator<StrategyForTesting>) {
+        g.add_node("N1", JobKind::Output);
+        g.add_node("N2", JobKind::Ephemeral);
+        g.add_node("N3", JobKind::Output);
+        g.depends_on("N2", "N1");
+        g.depends_on("N3", "N2");
+    }
+    let strat = StrategyForTesting::new();
+    let mut g = PPGEvaluator::new(strat);
+    let strat = StrategyForTesting::new();
+    create_graph(&mut g);
+    g.event_startup().unwrap();
+    assert_eq!(g.query_ready_to_run(), set!["N1"]);
+    g.event_now_running("N1").unwrap();
+    assert!(g.query_ready_to_run().is_empty());
+    g.event_job_finished_success("N1", "out1output".to_string())
+        .unwrap();
+    strat.already_done.borrow_mut().insert("N1".to_string());
+    assert_eq!(g.query_ready_to_run(), set!["N2"]);
+    assert!(!g.is_finished());
+    g.event_now_running("N2").unwrap();
+    assert!(!g.is_finished());
+    g.event_job_finished_success("N2", "out2output".to_string())
+        .unwrap();
+    strat.already_done.borrow_mut().insert("N2".to_string());
+    assert_eq!(g.query_ready_to_run(), set!["N3"]);
+    g.event_now_running("N3").unwrap();
+    assert!(!g.is_finished());
+    g.event_job_finished_success("N3", "out3output".to_string())
+        .unwrap();
+    assert!(g.is_finished());
+    strat.already_done.borrow_mut().insert("N3".to_string());
+    let history = g.new_history().unwrap();
+    assert!(history.get(&("N1!!!N2".to_string())).unwrap() == "out1output");
+    assert!(history.get(&("N2!!!N3".to_string())).unwrap() == "out2output");
+    assert!(history.len() == 2 + 3 + 3);
+
+    let mut g = PPGEvaluator::new_with_history(history.clone(), strat);
+    create_graph(&mut g);
+    g.add_node("A", JobKind::Always);
+    g.add_node("B", JobKind::Output);
+    g.depends_on("N1", "A");
+    g.event_startup().unwrap();
+    assert_eq!(g.query_ready_to_run(), set!["A", "B"]);
+    g.event_now_running("A").unwrap();
+    assert_eq!(g.query_ready_to_run(), set!["B"]);
+    g.event_job_finished_success("A", "outA".to_string())
+        .unwrap();
+    assert_eq!(g.query_ready_to_run(), set!["N1", "B"]);
+    g.event_now_running("N1").unwrap();
+    g.event_job_finished_success("N1", "out1output_changed".to_string())
+        .unwrap();
+    assert_eq!(g.query_ready_to_run(), set!["N2", "B"]);
+    g.event_now_running("N2").unwrap();
+    g.event_job_finished_failure("N2").unwrap();
+    assert_eq!(g.query_ready_to_run(), set!["B"]);
+    g.abort_remaining().unwrap();
+
+    let history2 = g.new_history().unwrap();
+}
+#[test]
+fn test_aborting_while_ephemeral_is_running() {
+    fn create_graph(g: &mut PPGEvaluator<StrategyForTesting>) {
+        g.add_node("N1", JobKind::Output);
+        g.add_node("N2", JobKind::Ephemeral);
+        g.add_node("N3", JobKind::Output);
+        g.depends_on("N2", "N1");
+        g.depends_on("N3", "N2");
+    }
+    let strat = StrategyForTesting::new();
+    let mut g = PPGEvaluator::new(strat.clone());
+    create_graph(&mut g);
+    g.event_startup().unwrap();
+    assert_eq!(g.query_ready_to_run(), set!["N1"]);
+    g.event_now_running("N1").unwrap();
+    assert!(g.query_ready_to_run().is_empty());
+    g.event_job_finished_success("N1", "out1output".to_string())
+        .unwrap();
+    strat.already_done.borrow_mut().insert("N1".to_string());
+    assert_eq!(g.query_ready_to_run(), set!["N2"]);
+    assert!(!g.is_finished());
+    g.event_now_running("N2").unwrap();
+    assert!(!g.is_finished());
+    g.event_job_finished_success("N2", "out2output".to_string())
+        .unwrap();
+    strat.already_done.borrow_mut().insert("N2".to_string());
+    assert_eq!(g.query_ready_to_run(), set!["N3"]);
+    g.event_now_running("N3").unwrap();
+    assert!(!g.is_finished());
+    g.event_job_finished_success("N3", "out3output".to_string())
+        .unwrap();
+    strat.already_done.borrow_mut().insert("N3".to_string());
+    assert!(g.is_finished());
+    let history = g.new_history().unwrap();
+    assert!(history.get(&("N1!!!N2".to_string())).unwrap() == "out1output");
+    assert!(history.get(&("N2!!!N3".to_string())).unwrap() == "out2output");
+    assert!(history.len() == 2 + 3 + 3);
+    assert!(strat.already_done.borrow_mut().contains("N1"));
+
+    let mut g = PPGEvaluator::new_with_history(history.clone(), strat.clone());
+    create_graph(&mut g);
+    g.add_node("A", JobKind::Always);
+    g.add_node("B", JobKind::Output);
+    g.depends_on("N1", "A");
+    g.event_startup().unwrap();
+    assert_eq!(g.query_ready_to_run(), set!["A", "B"]);
+    g.event_now_running("A").unwrap();
+    assert_eq!(g.query_ready_to_run(), set!["B"]);
+    g.event_job_finished_success("A", "outA".to_string())
+        .unwrap();
+    assert_eq!(g.query_ready_to_run(), set!["N1", "B"]);
+    g.event_now_running("N1").unwrap();
+    g.event_job_finished_success("N1", "out1output_changed".to_string())
+        .unwrap();
+    assert_eq!(g.query_ready_to_run(), set!["N2", "B"]);
+    g.event_now_running("N2").unwrap();
+    g.event_job_finished_failure("N2").unwrap();
+    assert_eq!(g.query_ready_to_run(), set!["B"]);
+
+    g.abort_remaining().unwrap();
+
+    let history2 = g.new_history().unwrap();
+
+    assert!(history2.get(&("N1".to_string())).unwrap() == "out1output_changed");
+    assert!(history2.get(&("N1!!!".to_string())).unwrap() == "A");
+    assert!(history2.get(&("N1!!!N2".to_string())).unwrap() == "out1output"); //we did not filter
+                                                                              //this.
+    assert!(history2.get(&("N2!!!".to_string())).is_none());
+    assert!(history2.get(&("N2".to_string())).is_none());
+
+    let strat = StrategyForTesting::new();
+    strat.already_done.borrow_mut().insert("N1".to_string());
+    strat.already_done.borrow_mut().insert("N3".to_string());
+    let mut g = PPGEvaluator::new_with_history(history2.clone(), strat);
+    create_graph(&mut g);
+    g.add_node("A", JobKind::Always);
+    g.add_node("B", JobKind::Output);
+    g.depends_on("N1", "A");
+    g.depends_on("B", "N2");
+    g.event_startup().unwrap();
+    assert_eq!(g.query_ready_to_run(), set!["A"]);
+    g.event_now_running("A").unwrap();
+    assert!(g.query_ready_to_run().is_empty());
+    g.event_job_finished_success("A", "outA".to_string())
+        .unwrap();
+
+    assert_eq!(g.query_ready_to_run(), set!["N2"]);
+    g.event_now_running("N2").unwrap();
+    g.event_job_finished_success("N2", "out2output_changed".to_string())
+        .unwrap();
+    assert_eq!(g.query_ready_to_run(), set!["N3", "B"]);
+}
+
+#[test]
+fn test_aborting_between_ephemerals_1() {
+    fn create_graph(g: &mut PPGEvaluator<StrategyForTesting>) {
+        g.add_node("N1", JobKind::Ephemeral);
+        g.add_node("N2a", JobKind::Ephemeral);
+        g.add_node("N2b", JobKind::Ephemeral);
+        g.add_node("N2c", JobKind::Ephemeral);
+        g.add_node("N3", JobKind::Output);
+        g.depends_on("N2a", "N1");
+        g.depends_on("N2b", "N1");
+        g.depends_on("N2c", "N1");
+        g.depends_on("N3", "N2a");
+        g.depends_on("N3", "N2b");
+        g.depends_on("N3", "N2c");
+    }
+    //so the idea is that everything had run. Then it was rerun, and N1 was rebuild
+    // (because it was missing, or perhaps because it was invalidated),
+    // and then N2a was run, but before N2b could be run (and update it's inputs), the abort
+    // happend
+    // so we have diverging history.
+    // and we need a third job go the ephemeral to rebuild.
+    // but we should not need a third job, the fact taht N2b is invalidated by the (stored) N1 
+    // output should already retrigger N1.
+    // So We might Have Two Bugs: Not triggering N1 thouh N2b is invalidated
+    // and then 'comparing with stored on "N1!!N2b" instead of "N2b"
+    let strat = StrategyForTesting::new();
+    strat.already_done.borrow_mut().insert("N1".to_string());
+    strat.already_done.borrow_mut().insert("N3".to_string());
+    let mut history = HashMap::new();
+    history.insert("N1".to_string(), "1_changed".to_string());
+    history.insert("N1!!!".to_string(), "".to_string());
+
+    history.insert("N2a".to_string(), "2a".to_string());
+    history.insert("N2a!!!".to_string(), "N1".to_string());
+    history.insert("N1!!!N2a".to_string(), "1_changed".to_string());
+
+    history.insert("N2b".to_string(), "2b".to_string());
+    history.insert("N2b!!!".to_string(), "N1".to_string());
+    history.insert("N1!!!N2b".to_string(), "1".to_string()); // that's the one that did not update.
+
+    history.insert("N3".to_string(), "3".to_string());
+    history.insert("N3!!!".to_string(), "N2a\nN2b".to_string());
+    history.insert("N2a!!!N3".to_string(), "2a".to_string()); // that's the one that did not update.
+    history.insert("N2b!!!N3".to_string(), "2b".to_string()); // that's the one that did not update.
+
+    let mut g = PPGEvaluator::new_with_history(history, strat);
+    start_logging();
+    create_graph(&mut g);
+    g.event_startup().unwrap();
+    assert_eq!(g.query_ready_to_run(), set!["N1"]);
+    g.event_now_running("N1").unwrap();
+    g.event_job_finished_success("N1", "1_changed".to_string()) .unwrap();
+    assert_eq!(g.query_ready_to_run(), set!["N2a", "N2b", "N2c"]); // N3 needs all three.
+    g.event_now_running("N2a").unwrap();
+    g.event_now_running("N2b").unwrap();
+    g.event_now_running("N2c").unwrap();
+    g.event_job_finished_success("N2a", "2a".to_string()) .unwrap();
+    g.event_job_finished_success("N2b", "2b".to_string()) .unwrap();
+    g.event_job_finished_success("N2c", "2c".to_string()) .unwrap();
+    assert_eq!(g.query_ready_to_run(), set!["N3"]);
+    g.event_now_running("N3").unwrap();
+    g.event_job_finished_success("N3", "3".to_string()) .unwrap();
+                                                                   //
+    assert!(g.query_ready_to_run().is_empty());
+    assert!(g.is_finished());
+}
+
+#[test]
+fn test_aborting_between_ephemerals_invalidation_triggers() {
+    //same as above, but forcing us to actually have the N2b invalidation because N1 changed.
+    fn create_graph(g: &mut PPGEvaluator<StrategyForTesting>) {
+        g.add_node("N1", JobKind::Ephemeral);
+        g.add_node("N2a", JobKind::Ephemeral);
+        g.add_node("N2b", JobKind::Ephemeral);
+        g.add_node("N3", JobKind::Output);
+        g.depends_on("N2a", "N1");
+        g.depends_on("N2b", "N1");
+        g.depends_on("N3", "N2a");
+        g.depends_on("N3", "N2b");
+    }
+    let strat = StrategyForTesting::new();
+    strat.already_done.borrow_mut().insert("N1".to_string());
+    strat.already_done.borrow_mut().insert("N3".to_string());
+    let mut history = HashMap::new();
+    history.insert("N1".to_string(), "1_changed".to_string());
+    history.insert("N1!!!".to_string(), "".to_string());
+
+    history.insert("N2a".to_string(), "2a".to_string());
+    history.insert("N2a!!!".to_string(), "N1".to_string());
+    history.insert("N1!!!N2a".to_string(), "1_changed".to_string());
+
+    history.insert("N2b".to_string(), "2b".to_string());
+    history.insert("N2b!!!".to_string(), "N1".to_string());
+    history.insert("N1!!!N2b".to_string(), "1".to_string()); // that's the one that did not update.
+
+    history.insert("N3".to_string(), "3".to_string());
+    history.insert("N3!!!".to_string(), "N2a\nN2b".to_string());
+    history.insert("N2a!!!N3".to_string(), "2a".to_string()); // that's the one that did not update.
+    history.insert("N2b!!!N3".to_string(), "2b".to_string()); // that's the one that did not update.
+
+    let mut g = PPGEvaluator::new_with_history(history, strat);
+    create_graph(&mut g);
+    g.event_startup().unwrap();
+    assert_eq!(g.query_ready_to_run(), set!["N1"]);
+    g.event_now_running("N1").unwrap();
+    g.event_job_finished_success("N1", "1_changed".to_string())
+        .unwrap();
+    assert_eq!(g.query_ready_to_run(), set!["N2b"]);
+    g.event_now_running("N2b").unwrap();
+    g.event_job_finished_success("N2b", "2b".to_string()).unwrap();
+
+    assert!(g.is_finished());
+}
+
 /*
 #[test]
 fn test_multi_file_job_gaining_output() {
     // the rust engine does not know anything about filenames or jobs with 'multiple'
     // outputs
     // we fake that by delegating to is_history_altered on the python side.
     // but adding/removing an output will retrigger the downstreams
```

### Comparing `pypipegraph2-3.0.2/tests/conftest.py` & `pypipegraph2-3.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/old_history_for_conversion_test.gz` & `pypipegraph2-3.0.3/tests/old_history_for_conversion_test.gz`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/shared.py` & `pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/shared.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_cache_jobs.py` & `pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_cache_jobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_compatibility_layer.py` & `pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_compatibility_layer.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_cycles.py` & `pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_cycles.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_invariants_and_depedencies.py` & `pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_invariants_and_depedencies.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_job_gen_jobs.py` & `pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_job_gen_jobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_other.py` & `pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_other.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_plotjobs.py` & `pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_plotjobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_prune.py` & `pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_prune.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_simple.py` & `pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_simple.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/ppg1_compatibility_layer/test_util.py` & `pypipegraph2-3.0.3/tests/ppg1_compatibility_layer/test_util.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/shared.py` & `pypipegraph2-3.0.3/tests/shared.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/test_basics.py` & `pypipegraph2-3.0.3/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/test_bootstrap.py` & `pypipegraph2-3.0.3/tests/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/test_cache_jobs.py` & `pypipegraph2-3.0.3/tests/test_cache_jobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/test_cycles.py` & `pypipegraph2-3.0.3/tests/test_cycles.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/test_flake8.py` & `pypipegraph2-3.0.3/tests/test_flake8.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/test_function_invariants.py` & `pypipegraph2-3.0.3/tests/test_function_invariants.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/test_interactive.py` & `pypipegraph2-3.0.3/tests/test_interactive.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/test_invariants_and_dependencies.py` & `pypipegraph2-3.0.3/tests/test_invariants_and_dependencies.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/test_job_generating_jobs.py` & `pypipegraph2-3.0.3/tests/test_job_generating_jobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/test_jobs.py` & `pypipegraph2-3.0.3/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/test_other.py` & `pypipegraph2-3.0.3/tests/test_other.py`

 * *Files 3% similar despite different names*

```diff
@@ -672,7 +672,30 @@
             raise ValueError(
                 "children not killed, found a sleep",
                 "pid",
                 proc.pid,
                 "ppid",
                 proc.ppid(),
             )
+
+
+def test_tempmultifilegen_changing_output_but_had_been_validated(ppg2_per_test):
+    import random
+
+    def bad(files):
+        files[0].write_text("hello")
+        files[1].write_text("world" + str(random.random()))
+
+    tmfg = ppg.MultiTempFileGeneratingJob(["a", "b"], bad)
+    c = ppg.FileGeneratingJob("c", lambda of: of.write_text(Path("a").read_text()))
+    c.depends_on("a")
+    ppg.run()
+    ppg.new()
+    tmfg = ppg.MultiTempFileGeneratingJob(["a", "b"], bad)
+    c = ppg.FileGeneratingJob("c", lambda of: of.write_text(Path("a").read_text()))
+    c.depends_on("a")
+    d = ppg.FileGeneratingJob("d", lambda of: of.write_text(Path("a").read_text()))
+    d.depends_on("a")
+    with pytest.raises(ppg.JobsFailed):
+        ppg.run()
+    error = ppg.global_pipegraph.last_run_result[tmfg.job_id].error
+    assert "changed output" in error and "ephemeral" in error.lower()
```

### Comparing `pypipegraph2-3.0.2/tests/test_parallel.py` & `pypipegraph2-3.0.3/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/test_parent_termination_kills_children/manual.py` & `pypipegraph2-3.0.3/tests/test_parent_termination_kills_children/manual.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/test_parent_termination_kills_children/stage2.py` & `pypipegraph2-3.0.3/tests/test_parent_termination_kills_children/stage2.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/test_plotjobs.py` & `pypipegraph2-3.0.3/tests/test_plotjobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/test_prune.py` & `pypipegraph2-3.0.3/tests/test_prune.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/test_rust_conversion.py` & `pypipegraph2-3.0.3/tests/test_rust_conversion.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/test_shared_jobs.py` & `pypipegraph2-3.0.3/tests/test_shared_jobs.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/test_simple.py` & `pypipegraph2-3.0.3/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/test_util.py` & `pypipegraph2-3.0.3/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/tests/tests_from_the_field.py` & `pypipegraph2-3.0.3/tests/tests_from_the_field.py`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/todo.md` & `pypipegraph2-3.0.3/todo.md`

 * *Files identical despite different names*

### Comparing `pypipegraph2-3.0.2/PKG-INFO` & `pypipegraph2-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypipegraph2
-Version: 3.0.2
+Version: 3.0.3
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Rust
 Requires-Dist: loguru
 Requires-Dist: rich
 Requires-Dist: xxhash
 Requires-Dist: wrapt
```

